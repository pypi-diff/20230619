# Comparing `tmp/omars_analysis-1.0.8.tar.gz` & `tmp/omars_analysis-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omars_analysis-1.0.8.tar", max compression
+gzip compressed data, was "omars_analysis-2.0.0.tar", max compression
```

## Comparing `omars_analysis-1.0.8.tar` & `omars_analysis-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4801 2022-12-25 21:25:41.010645 omars_analysis-1.0.8/README.md
--rw-r--r--   0        0        0        5 2022-12-15 12:47:13.568014 omars_analysis-1.0.8/omars_analysis/.gitignore
--rw-r--r--   0        0        0       61 2022-12-25 21:25:37.185857 omars_analysis-1.0.8/omars_analysis/__init__.py
--rw-r--r--   0        0        0      277 2022-12-13 12:37:02.164382 omars_analysis-1.0.8/omars_analysis/data/Laser_data.txt
--rw-r--r--   0        0        0      447 2022-12-14 09:55:19.309044 omars_analysis-1.0.8/omars_analysis/data/jn_data.txt
--rw-r--r--   0        0        0     5348 2022-12-14 16:09:06.169078 omars_analysis-1.0.8/omars_analysis/generate_model_matrix_heredity.py
--rw-r--r--   0        0        0    10958 2023-01-24 16:11:14.954841 omars_analysis-1.0.8/omars_analysis/main.py
--rw-r--r--   0        0        0     3933 2022-12-27 12:55:01.888057 omars_analysis-1.0.8/omars_analysis/subset_selection.py
--rw-r--r--   0        0        0      486 2023-01-24 16:13:17.855630 omars_analysis-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     5660 1970-01-01 00:00:00.000000 omars_analysis-1.0.8/setup.py
--rw-r--r--   0        0        0     5468 1970-01-01 00:00:00.000000 omars_analysis-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     4801 2022-12-25 21:25:41.010645 omars_analysis-2.0.0/README.md
+-rw-r--r--   0        0        0        5 2022-12-15 12:47:13.568014 omars_analysis-2.0.0/omars_analysis/.gitignore
+-rw-r--r--   0        0        0       61 2022-12-25 21:25:37.185857 omars_analysis-2.0.0/omars_analysis/__init__.py
+-rw-r--r--   0        0        0      277 2022-12-13 12:37:02.164382 omars_analysis-2.0.0/omars_analysis/data/Laser_data.txt
+-rw-r--r--   0        0        0      447 2022-12-14 09:55:19.309044 omars_analysis-2.0.0/omars_analysis/data/jn_data.txt
+-rw-r--r--   0        0        0     5348 2022-12-14 16:09:06.169078 omars_analysis-2.0.0/omars_analysis/generate_model_matrix_heredity.py
+-rw-r--r--   0        0        0    10937 2023-06-19 12:30:46.401659 omars_analysis-2.0.0/omars_analysis/main.py
+-rw-r--r--   0        0        0     2325 2023-06-19 12:29:25.591655 omars_analysis-2.0.0/omars_analysis/omars_analysis_oop.py
+-rw-r--r--   0        0        0     3933 2022-12-27 12:55:01.888057 omars_analysis-2.0.0/omars_analysis/subset_selection.py
+-rw-r--r--   0        0        0      486 2023-06-19 12:33:49.178888 omars_analysis-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5660 1970-01-01 00:00:00.000000 omars_analysis-2.0.0/setup.py
+-rw-r--r--   0        0        0     5468 1970-01-01 00:00:00.000000 omars_analysis-2.0.0/PKG-INFO
```

### Comparing `omars_analysis-1.0.8/README.md` & `omars_analysis-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `omars_analysis-1.0.8/omars_analysis/generate_model_matrix_heredity.py` & `omars_analysis-2.0.0/omars_analysis/generate_model_matrix_heredity.py`

 * *Files identical despite different names*

### Comparing `omars_analysis-1.0.8/omars_analysis/main.py` & `omars_analysis-2.0.0/omars_analysis/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,234 +1,245 @@
-import numpy as np
-import itertools
-import datetime
-import sys
-from scipy.stats import t
-from scipy.stats import f
-
-from omars_analysis.subset_selection import get_soe
-from omars_analysis.generate_model_matrix_heredity import create_model_matrix_heredity
-
-# from subset_selection import get_soe
-# from generate_model_matrix_heredity import create_model_matrix_heredity
-
-def hat_matrix(smat):
-    hat = smat @ np.linalg.pinv(smat.T @ smat) @ smat.T
-    return hat
-
-def create_quadratic_interactions(smat):
-    no_runs, nf = smat.shape[0], smat.shape[1]
-    quad_ix = [i for i,x in enumerate(smat.T) if (abs(x)!=1).any()]
-    
-    # Quadratic
-    if len(quad_ix) > 0:
-        quadratic = np.absolute(smat[:,quad_ix])
-        soe_mat = np.hstack((np.ones((no_runs,1)),quadratic))
-    else:
-        soe_mat = np.ones((no_runs,1))
-
-    # Interactions
-    for combi in itertools.combinations(range(nf), 2):
-        col = (smat[:,combi[0]]*smat[:,combi[1]]).reshape((no_runs,1))
-        soe_mat = np.hstack((soe_mat, col))
-
-    #centering (important for later functions)
-    soe_mat = soe_mat - soe_mat.mean(axis=0)
-
-    return soe_mat[:,1:], quad_ix
-
-def code(smat):
-    a = np.ones((smat.shape[0],1))
-    for i in smat.T:
-        maxi = max(i)
-        mini = min(i)
-        avg = (maxi + mini)/2
-        diff = (maxi - mini)/2
-        temp = (i - avg)/diff
-        temp = temp.reshape((smat.shape[0],1))
-        a = np.hstack((a,temp))
-       
-    return a[:,1:]
-
-def get_omars_analysis(smat: np.ndarray, cy: np.ndarray, alpha: list = [0.05, 0.2, 0.2], qheredity: str='n', iheredity: str='n', effects_to_drop: list=[], full: str='y', force_me: list=[], user_limit_for_step_two=None):
-    
-    web_statements=[]
-
-    i_start = datetime.datetime.now()
-    mat = code(smat)
-    no_runs, nf = mat.shape[0], mat.shape[1]
-
-    # Centering response in case not centered already
-    cy = (cy - cy.mean(axis=0)).reshape(no_runs,1)
-
-    # Calculate error variance
-    intercept = np.ones((no_runs, 1))
-    mat_qi, quad_ix = create_quadratic_interactions(mat)
-    total_mat = np.hstack((np.hstack((intercept, mat)),mat_qi))
-    
-    new_error_variance_projection = np.identity(no_runs) - (total_mat @ np.linalg.pinv(total_mat))
-    denominator = no_runs - np.linalg.matrix_rank(total_mat)
-    print('\nInitial error degrees of freedom available - {}'.format(denominator))
-    web_statements.append('\nInitial error degrees of freedom available - {}'.format(denominator))
-
-    if denominator == 0:
-        print('Analysis cannot continue due to lack of available degrees of freedom to estimate error variance')
-        web_statements.append('Analysis cannot continue due to lack of available degrees of freedom to estimate error variance')
-        return web_statements
-
-    new_variance = (cy.T @ new_error_variance_projection @ cy)/denominator
-    print('\nInitial estimate of error variance - {}'.format(round(float(new_variance),3)))
-    web_statements.append('\nInitial estimate of error variance - {}'.format(round(float(new_variance),3)))
-    
-    s = np.sqrt(new_variance)
-    
-    '''
-    ANALYSIS OF ME (STEP 1)
-    '''
-    mebeta = (np.linalg.inv(mat.T @ mat) @ mat.T @ cy).reshape(1,nf)
-    vdiags = np.matrix.diagonal(np.linalg.inv(mat.T @ mat))
-    svdiags = np.sqrt(vdiags).reshape(1,nf)
-    tvalue = np.absolute(mebeta/(s*svdiags))
-    ttest = t.ppf(1 - (alpha[0]/2), df=denominator)
-    tcomp = tvalue/ttest
-    
-    indexrme = [i for i,x in enumerate(tcomp[0]) if (abs(x)>=1)] # index of active main effects    
-    indexfme = [i for i,x in enumerate(tcomp[0]) if (abs(x)<1)] # index of inactive main effects
-    
-    new_me = [g+1 for g in indexrme]
-    print('\nActive main effects - {}'.format(new_me))
-    web_statements.append('\nActive main effects - {}'.format(new_me))
-    # p_values_ttest = [t.cdf(ttest,denominator)]
-    p_value_ttest = 1-t.cdf(tvalue,denominator)
-    print('\nThe p-values for double sided t-tests for main effects - {} (threshold alpha/2 = {})'.format(p_value_ttest[0], alpha[0]/2))
-    web_statements.append(list(np.round(p_value_ttest[0]*2,5)))
-
-    if full == 'n':
-        return web_statements
-    
-    '''
-    END OF STEP 1
-    '''
-
-    # Force main effects in step two:
-    if len(force_me)>0:
-        print('\nForced main effect - {}'.format(force_me))
-        web_statements.append('\nForced main effect - {}'.format(force_me))
-        ix = [int(x) for x in force_me]
-        for x in ix:
-            if x-1 in indexrme:
-                pass
-            elif x-1 in indexfme:
-                indexrme.append(x-1)
-
-    indexrme.sort()
-    indexfme = [x for x in range(nf) if x not in indexrme]
-    inactive = mat[:, indexfme]
-
-    # Update error variance
-    if len(indexfme)>0:
-        inactive_proj = hat_matrix(inactive)
-    else:
-        inactive_proj = np.zeros((no_runs, no_runs))
-    new_variance_projection_updated = new_error_variance_projection + inactive_proj
-    numerator = cy.T @ new_variance_projection_updated @ cy
-    new_denominator = denominator + len(indexfme)
-    new_variance = numerator/new_denominator
-    print('\nUpdated estimate of error variance taking into account inactive main effects- {}'.format(round(float(new_variance),3)))
-    web_statements.append('\nUpdated estimate of error variance taking into account inactive main effects- {}'.format(round(float(new_variance),3)))
-    '''
-    ANALYSIS OF SOE (STEP 2)
-    '''
-    # Second order proection matrix (make sure to only multiply with centered response since intercept is ignored)
-    y_second_projection = np.identity(no_runs) - hat_matrix(mat) - new_error_variance_projection
-    cy_second = (y_second_projection @ cy).reshape(no_runs,1)
-    TSS = cy_second.T @ cy_second # Total sum of squares (for second order space)
-    
-    ####        F Test for second order effects
-    o_dfleft = np.linalg.matrix_rank(mat_qi) # quadratics need to be centered in mat_qi
-    ftest = f.ppf(q= 1-alpha[1], dfn=o_dfleft, dfd=new_denominator)
-    F1 = (TSS/o_dfleft)/new_variance
-    fcomp = F1/ftest
-    p_value_intial = 1-f.cdf(F1, o_dfleft, new_denominator)
-    print('\nThe p-value for the first F-test is {} (threshold alpha value - {})'.format(round(float(p_value_intial),3),alpha[1]))
-    web_statements.append('\nThe p-value for the first F-test is {} (threshold alpha value - {})'.format(round(float(p_value_intial),3),alpha[1]))
-    '''
-    CREATE SECOND ORDER MATRIX WITH HEREDITY FOR ANALYSIS (WITHOUT INTERCEPT)
-    '''
-    if fcomp >= 1:
-        # standardize columns
-        std = 'n'
-        soe_mat2, my_dictionary_soe_single  = create_model_matrix_heredity(std, mat, quad_ix, indexrme, indexfme, qheredity, iheredity)
-        
-        ix_del = [my_dictionary_soe_single[x] for x in effects_to_drop]
-        soe_mat2 = np.delete(soe_mat2, ix_del, axis=1)
-        new_names = [x for x in my_dictionary_soe_single.keys() if x not in effects_to_drop]
-        my_dictionary_soe_single = {new_names[i]:i for i in range(len(new_names))}
-        
-        # if quadratic_special_coding == 'y':
-        #     relevant_q = []
-        #     for dumzy in my_dictionary_soe_single:
-        #         if dumzy.split('_')[0] == dumzy.split('_')[1]:
-        #             relevant_q.append(int(dumzy.split('_')[0])-1)
-                    
-        #     if len(relevant_q)>0:
-        #         temp_mat = mat[:,relevant_q]
-        #         temp_mat = temp_mat - temp_mat.mean(axis=0) # center
-        #         temp_mat = np.square(temp_mat) # square
-        #         temp_mat = code(temp_mat) # normalize
-        #         soe_mat2[:,0:len(relevant_q)] = temp_mat.copy()
-        active_soe, p_value_omars, actual_soe_df, concluding_statement = get_soe(mat, o_dfleft, soe_mat2, cy_second, new_denominator, new_variance, my_dictionary_soe_single, alpha_val=alpha[2], limit_for_step_two=user_limit_for_step_two)
-
-        print('\nThe p-value for the final F-test is \n {} (threshold alpha value - {})'.format(round(p_value_omars,3), alpha[2]))
-        web_statements.append('\nThe p-value for the final F-test is \n {} (threshold alpha value - {})'.format(round(p_value_omars,3), alpha[2]))
-    else:
-        active_soe = []
-        p_value_omars = np.nan
-    
-    new_qe = []
-    new_ie = []
-    for d in active_soe:
-        x = d.split('_')
-        if x[0] == x[1]:
-            new_qe.append(d)
-        else:
-            new_ie.append(d)
-
-    if len(new_ie+new_qe) >= 1:
-        print('\nActive interaction effects - {}'.format(new_ie))
-        print('\nActive quadratic effects - {}'.format(new_qe))
-        web_statements.append('\nActive interaction effects - {}'.format(new_ie))
-        web_statements.append('\nActive quadratic effects - {}'.format(new_qe))
-    else:
-        print('\nNo active second order effects detected')
-        web_statements.append('\nNo active second order effects detected')
-
-    i_finish = datetime.datetime.now()
-    timing = (i_finish - i_start).total_seconds()
-    print('\nAnalysis performed in {} seconds'.format(round(timing,3)))
-
-    web_statements.append('\nAnalysis performed in {} seconds'.format(round(timing,3)))
-
-    if fcomp >= 1:
-        print('\n=============================================================')
-        print('\nInformation on the limit of second order terms allowed to enter the model:')
-        print(concluding_statement)
-        print('Number of second order effects considered - {}'.format(soe_mat2.shape[1]))
-        print('Maximum number of second order terms jointly estimable of all the second order effects considered - {}'.format(actual_soe_df))
-        print('\nRank of matrix with all {} possible second order terms is {} (in case the rank is less than the number of total second order terms, it is advisable to set a limit that is less than half of the rank)\n'.format(mat_qi.shape[1], o_dfleft))
-        
-        web_statements.append('\n=============================================================')
-        web_statements.append('Number of second order effects considered - {}'.format(soe_mat2.shape[1]))
-        web_statements.append(concluding_statement)
-        web_statements.append('Maximum number of second order terms jointly estimable of all the second order effects considered - {}'.format(actual_soe_df))
-        web_statements.append('\nRank of matrix with all {} possible second order terms is {} (in case the rank is less than the number of total second order terms, it is advisable to set a limit that is less than half of the rank)\n'.format(mat_qi.shape[1], o_dfleft))
-
-    return web_statements
-
-# if __name__ == '__main__':
-#     file = np.loadtxt('omars_analysis/data/Laser_data.txt')
-
-#     matz = file[:,:-1]
-#     resp = file[:,[-1]]
-
-#     # output = get_omars_analysis(smat=matz, cy=resp, qheredity='y', iheredity='n', effects_to_drop=[], force_me=['4'])
+import numpy as np
+import itertools
+import datetime
+import sys
+from scipy.stats import t
+from scipy.stats import f
+
+from omars_analysis.subset_selection import get_soe
+from omars_analysis.generate_model_matrix_heredity import create_model_matrix_heredity
+
+# from subset_selection import get_soe
+# from generate_model_matrix_heredity import create_model_matrix_heredity
+
+def hat_matrix(smat):
+    hat = smat @ np.linalg.pinv(smat.T @ smat) @ smat.T
+    return hat
+
+def create_quadratic_interactions(smat):
+    no_runs, nf = smat.shape[0], smat.shape[1]
+    quad_ix = [i for i,x in enumerate(smat.T) if (abs(x)!=1).any()]
+    
+    # Quadratic
+    if len(quad_ix) > 0:
+        quadratic = np.absolute(smat[:,quad_ix])
+        soe_mat = np.hstack((np.ones((no_runs,1)),quadratic))
+    else:
+        soe_mat = np.ones((no_runs,1))
+
+    # Interactions
+    for combi in itertools.combinations(range(nf), 2):
+        col = (smat[:,combi[0]]*smat[:,combi[1]]).reshape((no_runs,1))
+        soe_mat = np.hstack((soe_mat, col))
+
+    #centering (important for later functions)
+    soe_mat = soe_mat - soe_mat.mean(axis=0)
+
+    return soe_mat[:,1:], quad_ix
+
+def code(smat):
+    a = np.ones((smat.shape[0],1))
+    for i in smat.T:
+        maxi = max(i)
+        mini = min(i)
+        avg = (maxi + mini)/2
+        diff = (maxi - mini)/2
+        temp = (i - avg)/diff
+        temp = temp.reshape((smat.shape[0],1))
+        a = np.hstack((a,temp))
+       
+    return a[:,1:]
+
+def get_omars_analysis(smat: np.ndarray, cy: np.ndarray, alpha: list = [0.05, 0.2, 0.2], qheredity: str='n', iheredity: str='n', effects_to_drop: list=[], full: str='y', force_me: list=[], user_limit_for_step_two=None):
+    
+    collect_outputs = {}
+
+    i_start = datetime.datetime.now()
+    mat = code(smat)
+    no_runs, nf = mat.shape[0], mat.shape[1]
+
+    # Centering response in case not centered already
+    cy = (cy - cy.mean(axis=0)).reshape(no_runs,1)
+
+    # Calculate error variance
+    intercept = np.ones((no_runs, 1))
+    mat_qi, quad_ix = create_quadratic_interactions(mat)
+    total_mat = np.hstack((np.hstack((intercept, mat)),mat_qi))
+    
+    new_error_variance_projection = np.identity(no_runs) - (total_mat @ np.linalg.pinv(total_mat))
+    denominator = no_runs - np.linalg.matrix_rank(total_mat)
+    
+    # print('\nInitial error degrees of freedom available - {}'.format(denominator))
+    # web_statements.append('\nInitial error degrees of freedom available - {}'.format(denominator))
+
+    if denominator == 0:
+        collect_outputs['success'] = False
+        return collect_outputs
+
+    collect_outputs['success'] = True
+    collect_outputs['initial_df'] = denominator.copy()
+
+    new_variance = (cy.T @ new_error_variance_projection @ cy)/denominator
+    s = np.sqrt(new_variance)
+    collect_outputs['initial_rmse'] = round(float(s),3)
+    
+    '''
+    ANALYSIS OF ME (STEP 1)
+    '''
+    mebeta = (np.linalg.inv(mat.T @ mat) @ mat.T @ cy).reshape(1,nf)
+    vdiags = np.matrix.diagonal(np.linalg.inv(mat.T @ mat))
+    svdiags = np.sqrt(vdiags).reshape(1,nf)
+    tvalue = np.absolute(mebeta/(s*svdiags))
+    ttest = t.ppf(1 - (alpha[0]/2), df=denominator)
+    tcomp = tvalue/ttest
+    
+    indexrme = [i for i,x in enumerate(tcomp[0]) if (abs(x)>=1)] # index of active main effects    
+    indexfme = [i for i,x in enumerate(tcomp[0]) if (abs(x)<1)] # index of inactive main effects
+    
+    new_me = [g+1 for g in indexrme]
+
+    collect_outputs['active_me'] = new_me
+
+    # p_values_ttest = [t.cdf(ttest,denominator)]
+    p_value_ttest = 1-t.cdf(tvalue,denominator)
+
+    collect_outputs['me_p_values'] = list(np.round(p_value_ttest[0]*2,5))
+
+    if full == 'n':
+        return collect_outputs
+    
+    '''
+    END OF STEP 1
+    '''
+
+    # Force main effects in step two:
+    if len(force_me)>0:
+        ix = [int(x) for x in force_me]
+        for x in ix:
+            if x-1 in indexrme:
+                pass
+            elif x-1 in indexfme:
+                indexrme.append(x-1)
+
+    indexrme.sort()
+    indexfme = [x for x in range(nf) if x not in indexrme]
+    inactive = mat[:, indexfme]
+
+    # Update error variance
+    if len(indexfme)>0:
+        inactive_proj = hat_matrix(inactive)
+    else:
+        inactive_proj = np.zeros((no_runs, no_runs))
+    new_variance_projection_updated = new_error_variance_projection + inactive_proj
+    numerator = cy.T @ new_variance_projection_updated @ cy
+    new_denominator = denominator + len(indexfme)
+    new_variance = numerator/new_denominator
+
+    collect_outputs['updated_rmse'] = round(float(np.sqrt(new_variance)),3)
+    '''
+    ANALYSIS OF SOE (STEP 2)
+    '''
+    # Second order proection matrix (make sure to only multiply with centered response since intercept is ignored)
+    y_second_projection = np.identity(no_runs) - hat_matrix(mat) - new_error_variance_projection
+    cy_second = (y_second_projection @ cy).reshape(no_runs,1)
+    TSS = cy_second.T @ cy_second # Total sum of squares (for second order space)
+    
+    ####        F Test for second order effects
+    o_dfleft = np.linalg.matrix_rank(mat_qi) # quadratics need to be centered in mat_qi
+    ftest = f.ppf(q= 1-alpha[1], dfn=o_dfleft, dfd=new_denominator)
+    F1 = (TSS/o_dfleft)/new_variance
+    fcomp = F1/ftest
+    p_value_intial = 1-f.cdf(F1, o_dfleft, new_denominator)
+
+    collect_outputs['p_value_initial_f_test'] = round(float(p_value_intial),3)
+    # print('\nThe p-value for the first F-test is {} (threshold alpha value - {})'.format(round(float(p_value_intial),3),alpha[1]))
+    # web_statements.append('\nThe p-value for the first F-test is {} (threshold alpha value - {})'.format(round(float(p_value_intial),3),alpha[1]))
+    '''
+    CREATE SECOND ORDER MATRIX WITH HEREDITY FOR ANALYSIS (WITHOUT INTERCEPT)
+    '''
+    if fcomp >= 1:
+        collect_outputs['active_soe'] = True
+        # standardize columns
+        std = 'n'
+        soe_mat2, my_dictionary_soe_single  = create_model_matrix_heredity(std, mat, quad_ix, indexrme, indexfme, qheredity, iheredity)
+        
+        ix_del = [my_dictionary_soe_single[x] for x in effects_to_drop]
+        soe_mat2 = np.delete(soe_mat2, ix_del, axis=1)
+        new_names = [x for x in my_dictionary_soe_single.keys() if x not in effects_to_drop]
+        my_dictionary_soe_single = {new_names[i]:i for i in range(len(new_names))}
+        
+        # if quadratic_special_coding == 'y':
+        #     relevant_q = []
+        #     for dumzy in my_dictionary_soe_single:
+        #         if dumzy.split('_')[0] == dumzy.split('_')[1]:
+        #             relevant_q.append(int(dumzy.split('_')[0])-1)
+                    
+        #     if len(relevant_q)>0:
+        #         temp_mat = mat[:,relevant_q]
+        #         temp_mat = temp_mat - temp_mat.mean(axis=0) # center
+        #         temp_mat = np.square(temp_mat) # square
+        #         temp_mat = code(temp_mat) # normalize
+        #         soe_mat2[:,0:len(relevant_q)] = temp_mat.copy()
+        active_soe, p_value_omars, actual_soe_df, concluding_statement = get_soe(mat, o_dfleft, soe_mat2, cy_second, new_denominator, new_variance, my_dictionary_soe_single, alpha_val=alpha[2], limit_for_step_two=user_limit_for_step_two)
+
+        collect_outputs['p_value_final_f_test'] = round(p_value_omars,3)
+        # print('\nThe p-value for the final F-test is \n {} (threshold alpha value - {})'.format(round(p_value_omars,3), alpha[2]))
+        # web_statements.append('\nThe p-value for the final F-test is \n {} (threshold alpha value - {})'.format(round(p_value_omars,3), alpha[2]))
+    else:
+        active_soe = []
+        p_value_omars = np.nan
+    
+    new_qe = []
+    new_ie = []
+    for d in active_soe:
+        x = d.split('_')
+        if x[0] == x[1]:
+            new_qe.append(d)
+        else:
+            new_ie.append(d)
+
+    if len(new_ie+new_qe) >= 1:
+        collect_outputs['active_ie'] = new_ie
+        collect_outputs['active_qe'] = new_qe
+        # print('\nActive interaction effects - {}'.format(new_ie))
+        # print('\nActive quadratic effects - {}'.format(new_qe))
+        # web_statements.append('\nActive interaction effects - {}'.format(new_ie))
+        # web_statements.append('\nActive quadratic effects - {}'.format(new_qe))
+    else:
+        collect_outputs['active_soe'] = False
+        # print('\nNo active second order effects detected')
+        # web_statements.append('\nNo active second order effects detected')
+
+    i_finish = datetime.datetime.now()
+    timing = (i_finish - i_start).total_seconds()
+
+    collect_outputs['analysis_time'] = round(timing,3)
+    # print('\nAnalysis performed in {} seconds'.format(round(timing,3)))
+    # web_statements.append('\nAnalysis performed in {} seconds'.format(round(timing,3)))
+
+    if fcomp >= 1:
+        rank_statements = []
+        # print('\n=============================================================')
+        # print('\nInformation on the limit of second order terms allowed to enter the model:')
+        # print(concluding_statement)
+        # print('Number of second order effects considered - {}'.format(soe_mat2.shape[1]))
+        # print('Maximum number of second order terms jointly estimable of all the second order effects considered - {}'.format(actual_soe_df))
+        # print('\nRank of matrix with all {} possible second order terms is {} (in case the rank is less than the number of total second order terms, it is advisable to set a limit that is less than half of the rank)\n'.format(mat_qi.shape[1], o_dfleft))
+        
+        rank_statements.append('\n=============================================================')
+        rank_statements.append('Number of second order effects considered - {}'.format(soe_mat2.shape[1]))
+        rank_statements.append(concluding_statement)
+        rank_statements.append('Maximum number of second order terms jointly estimable of all the second order effects considered - {}'.format(actual_soe_df))
+        rank_statements.append('\nRank of matrix with all {} possible second order terms is {} (in case the rank is less than the number of total second order terms, it is advisable to set a limit that is less than half of the rank)\n'.format(mat_qi.shape[1], o_dfleft))
+
+        collect_outputs['rank_statements'] = rank_statements
+
+    return collect_outputs
+
+# if __name__ == '__main__':
+#     file = np.loadtxt('omars_analysis/data/Laser_data.txt')
+
+#     matz = file[:,:-1]
+#     resp = file[:,[-1]]
+
+#     # output = get_omars_analysis(smat=matz, cy=resp, qheredity='y', iheredity='n', effects_to_drop=[], force_me=['4'])
 #     output = get_omars_analysis(smat=matz, cy=resp, alpha=[0.05, 0.2, 0.2], qheredity='n', iheredity='n', effects_to_drop=[], full='y', force_me=['4'], user_limit_for_step_two=None)
```

### Comparing `omars_analysis-1.0.8/omars_analysis/subset_selection.py` & `omars_analysis-2.0.0/omars_analysis/subset_selection.py`

 * *Files identical despite different names*

### Comparing `omars_analysis-1.0.8/setup.py` & `omars_analysis-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'omars_analysis': ['data/*']}
 
 install_requires = \
 ['numpy>=1.23.5,<2.0.0', 'scipy>=1.9.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'omars-analysis',
-    'version': '1.0.8',
+    'version': '2.0.0',
     'description': '',
     'long_description': '# Documentation for package omars-analysis\n\nThis package has one function \'get_omars_analysis\'\n\nFirst run the following:\n\n```python\nfrom omars_analysis.main import get_omars_analysis\n```\n\nRunning the above command will make the function \'get_omars_analysis\' available for use.\n\n## Function usage\n\nThe function can be used with nine inputs (only the first two are required):\n\n- smat\n  \n  the first input is the design matrix. This should be a numpy array. The design matrix need not be coded, however it must only consist of continuous variables. The function is meant to be used with designs that have all factors either with two levels or three levels per factor column. The design should **NOT** consist of headers. The design matrix should not consist of second order effects since this will be built internally in the function.\n\n- cy\n  \n  This is the response. This should be a one dimensional column vector (1-D numpy).\n\n- qheredity\n  \n  This is to specify heredity constraints for quadratic effects. The accepted inputs are \'y\' or \'n\' (\'y\'- strong heredity, \'n\'- no heredity, \'n\'- No heredity). The input must be a string in lowercase. The default is \'n\'.\n\n- iheredity\n  \n  This is to specify heredity constraints for two-factor interaction effects. The accepted inputs are \'s\', \'w\' or \'n\' (\'s\'- strong heredity, \'w\'- weak heredity, \'n\'- no heredity). The input must be a string in lowercase. The default is \'n\'.\n\n- alpha\n  Here the three different alpha values can be specified (refer paper for mor information). The input must be a list of alpha values in float format. The default value for this parameter is [0.05, 0.2, 0.2].\n\n- effects_to_drop\n  \n  This is to specify second order effects that must be excluded from the analysis. The input must be a list of strings. For example: [\'1_1\', \'2_3\']. This input specifies that the quadratic effect of the first factor and the interaction effect between factor two and three must be excluded from the second step of the analysis (subset selection). The default value for this parameter is an empty list.\n\n  Note: Entering interaction between factor one and two should be represented as \'1_2\' and not as \'2_1\'. The smaller factor number should always come first.\n\n- full\n  \n  \'n\' -  analysis is performed on the main effects only\n  \n  \'y\' - analysis is performed on the main effects and second order effects.\n\n  The default is set to \'y\'\n\n- force_me\n  \n  Here certain main effects can be forced into the model. This can be used in cases where a main effect is statistically insignificant but by only a small margin. Forcing such main effects into the model can have an impact in reducing the updated estimate of the error.\n  \n  The input can be defined as a list of string values corresponding to the factor number that is to be forced. eg: [\'3\', \'4\']. The default value for this parameter is an empty list.\n\n- user_limit_for_step_two\n  \n  The max limit on the number of second order effects to be fit can be specified using this parameter. The input should be an integer. The default value for this parameter is "None". If the user has specified a limit, then this limit will be considered, otherwise the limit on the terms is case dependent. More information is given below:\n  - No limit is set if all second order terms for all factors are jointly estimable.\n  - The limit is set to the number of second order terms specified using the heredity parameters (qheredity and iheredity), if this number is less than the maximum number of jointly estimable terms for all second order effects.\n  - Otherwise, the limit will be always set to run size divided by four (refer paper).\n\n## Output\n\nThe function will auttomatically print out the following:\n\n- Initial error degrees of freedom available\n- Initial estimate of the error variance\n- Main effects that are declared active\n- p-values for the different main effects tested during main effects selection\n- Main effects that are forced into the model (if any)\n- Updated estimate of the error variance taking into account inactive main effects\n- p-value for the initial F-test (Step 4a from paper)\n- Limit on the number of terms for subset selection (Step 4b from paper)\n- Rank of matrix with only second order terms (this gives the possible maximum number of second order terms that can be fit during subset selection)\n- p-value for the final F-test (Step 4b from paper)\n- Active interaction effects\n- Active quadratic effects\n\nThe function outputs one return value. This value is the p-value from the last failed F-test during the second order effects selection.\n\n## Example code\n\n```python\noutput = get_omars_analysis(smat=design_matrix, cy=response, alpha=[0.05, 0.2, 0.2], qheredity=\'n\', iheredity=\'n\', effects_to_drop=[\'1_3\', \'2_6\'], full=\'y\', force_me=[\'4\'], user_limit_for_step_two=None)\n```\n',
     'author': 'Mohammed Saif Ismail Hameed',
     'author_email': 'saifismailh@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/saif-ismail/omars_analysis/',
```

### Comparing `omars_analysis-1.0.8/PKG-INFO` & `omars_analysis-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omars-analysis
-Version: 1.0.8
+Version: 2.0.0
 Summary: 
 Home-page: https://github.com/saif-ismail/omars_analysis/
 Author: Mohammed Saif Ismail Hameed
 Author-email: saifismailh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


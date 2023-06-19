# Comparing `tmp/current_events_magnifier-0.0.3.7.tar.gz` & `tmp/current_events_magnifier-0.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.3.7.tar", last modified: Fri Jun 16 09:52:54 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.0.3.8.tar", last modified: Mon Jun 19 07:00:54 2023, max compression
```

## Comparing `current_events_magnifier-0.0.3.7.tar` & `current_events_magnifier-0.0.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.7/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5972 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5354 2023-06-16 09:02:40.000000 current_events_magnifier-0.0.3.7/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6317 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6737 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2969 2023-06-16 09:52:24.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7625 2023-06-16 08:56:20.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5972 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1157 2023-06-16 09:52:49.000000 current_events_magnifier-0.0.3.7/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.8/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8295 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7677 2023-06-19 07:00:52.000000 current_events_magnifier-0.0.3.8/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6370 2023-06-19 06:06:59.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6737 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3813 2023-06-19 06:18:39.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7625 2023-06-16 08:56:20.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8295 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1157 2023-06-19 07:00:52.000000 current_events_magnifier-0.0.3.8/setup.py
```

### Comparing `current_events_magnifier-0.0.3.7/LICENSE` & `current_events_magnifier-0.0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/README.md` & `current_events_magnifier-0.0.3.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 # Current_Magnifier
 `Current_Magnifier` is a sample tool designed to visualize the features(Mean,Median,Dwell_time,STD) that distinguish between two groups of ONT data from the same species at the site level.
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
+
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 ## Still developing
 ### TO do list
 1. More normalization methods (finished)
 2. Test on minus strand or reversed strand (finished)
 3. Subsample coverage (finished)
 4. single mode(finished)
 5. merge images together(finished)
 6. test data to github(finished)
-## What is re-squiggle
+## Before start, you should know
+### What is re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
+### Data format
+Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
+![alt text](example/data_format.png)
+In our program, we assume that the input provided by the user is in the **multi-fast5** format by default.
+### Reference and alignment
+For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 
 ## Installation
 Requirement : Python >=3.7, <3.10
 
 ```sh
-pip install current_events_magnifier==0.0.3.5
+pip install current_events_magnifier==0.0.3.8
+pip install ont-fast5-api
 conda install -c bioconda ont_vbz_hdf_plugin f5c slow5tools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 CE_magnifier.py tombo -h
 optional arguments:
@@ -68,47 +77,76 @@
   --strand STRAND       Strand of your interest (default:+)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
 
 ```
 ## Quick start
-### Preprocessing
-If you used R10 or want to use the last resquiggle program(f5c v1.2.0),
+### Run Basecaller on your ONT data
 ```sh
-# if fast5 is single format 
-# single is fast5s-base-directory
-#single_to_multi_fast5 -i single/ -s multi -n 500 --recursive
-#slow5tools f2s multi/ -d blow5_dir
-
-slow5tools f2s single -d blow5_dir
+# assumed your fast5 file folder name is fast5/
+guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
+cat guppy_out/*/*.fastq > all.fastq
+```
+Option ```-c``` means config file ,which will depend on your data
+### Decide the chrom or transcript name and region of your interest
+In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
+So for the following command , I used ```--chrom NR_103073.1  --pos A2030 --strand +```
+### 1. F5c resquiggle (v1.2)
+Step 1 and 2 should run on your two sample respectively, before the step 3.
+1. Data format conversion.
+```sh
+slow5tools f2s fast5/ -d blow5_dir
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
-
-minimap2 -ax map-ont -t 16 --MD <reference-fasta> <reads.fastq> | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
+```
+2. Run f5c resquiggle
+```sh
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
-
 f5c resquiggle -c final.fastq file.blow5 -o file.paf
-
+```
+3. Run current_events_magnifier to plot
+```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-python CE_magnifier.py f5c -i wt/file -c control/file -o f5c_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --ref reference.fa
+python CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+--chrom NR_103073.1 --strand + \
+--pos 3929 --len 10 \
+--ref reference.fasta 
+```
+### 2. Tombo resquiggle (v1.5.0)
+Step 1 and 3 should run on your two sample respectively, before the step 4.
+1. Data format conversion.
+```sh
+# assumed your fast5 file folder name is fast5/
+multi_to_single_fast5 -i fast5/ -o single/ --recursive -t 16
+```
+2. Subsample (Optional)
 
+Because Tombo resquiggle runs very slowly, it heavily relies on the read and write speed of SSD hard drives. Therefore, it is recommended to extract the aligned reads in advance.
+After obtaining the single-format fast5 files and bam files , we provide a script that can assist you with this.
+```sh
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
+samtools index file.bam
+extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ --chrom NR_103073.1 --pos 2030 
 ```
-If you used Tombo(v1.5.0),
+3. Run tombo resquiggle
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
-tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames <reads.fastq> --processes 16 
-tombo resquiggle single/ <reference-fasta> --processes 16 --num-most-common-errors 5
+tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
+tombo resquiggle single/ reference.fasta --processes 16 --num-most-common-errors 5
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
-
-python CE_magnifier.py tombo -i wt/single -c control/single -o tombo_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --cpu 4 --ref reference.fa
-
+# If you ran step2, run the tombo command on subsample_single but single
+```
+4. Run current_events_magnifier to plot
+```sh
+python CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
 ```
```

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/CE_magnifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,16 @@
             title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
         except:
             args.control = None
         if args.control is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
+    else:
+        raise Exception("Wrong work flow")
 
     category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
```

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier_test.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/extract_sub_fast5_from_bam.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/extract_sub_fast5_from_bam.py`

 * *Files 21% similar despite different names*

```diff
@@ -59,16 +59,20 @@
     print("Loading bam files ... ")
     if sam_file.split(".")[-1] == 'bam':
         sam_file=pysam.AlignmentFile(sam_file,'rb')
     else:
         sam_file=pysam.AlignmentFile(sam_file,'r')
 
     read_list=[]
-    for read in sam_file.fetch():
-        read_list.append(read.qname)
+    if args.chrom is None or args.pos is None:
+        for read in sam_file.fetch():
+            read_list.append(read.qname)
+    else:
+        for read in sam_file.fetch(args.chrom, args.pos - 10, args.pos + 10):
+            read_list.append(read.qname)
     df = pd.DataFrame(read_list)
     df.columns=['readname']
 
     #READ FAST5 FILE LIST
     print("Collecting fast5 files ... ")
     os.system("find " + fast5_path + " -name \"*.fast5\" >" + results_path+"/files.txt")
     fast5_file =  results_path+"/files.txt"
@@ -80,14 +84,23 @@
         total_fl.append(i.rstrip())
     total_fl = pd.DataFrame(np.array(total_fl))
     total_fl[1] = total_fl.apply(select_sub_reads, axis=1)
     transfer_fast5(total_fl, df,results_path)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-f","--fast5", default='/data/Ecoli_23s/data/L_rep2/single/',
+    parser.add_argument("-f","--fast5", required=True,
                         help="fast5_path")
-    parser.add_argument('-b',"--bam", default="/data/Ecoli_23s/data/L_rep2/file.bam",
+    parser.add_argument('-b',"--bam", required=True,
                         help="bam_path")
-    parser.add_argument('-o',"--output", default='/data/Ecoli_23s/data/L_rep2/subsample1', help="output_file")
+    parser.add_argument('-o',"--output", default='subsample_single', help="output_file")
+    parser.add_argument("--chrom",help="Gene or chromosome name(head of your fasta file)")
+    parser.add_argument("--pos", type=int, help="site of your interest")
+    # parser.add_argument("-f","--fast5", default='/data/Ecoli_23s/data/L_rep2/single/',
+    #                     help="fast5_path")
+    # parser.add_argument('-b',"--bam", default="/data/Ecoli_23s/data/L_rep2/file.bam",
+    #                     help="bam_path")
+    # parser.add_argument('-o',"--output", default='/data/Ecoli_23s/data/L_rep2/subsample2', help="output_file")
+    # parser.add_argument("--chrom", default='NR_103073.1',help="Gene or chromosome name(head of your fasta file)")
+    # parser.add_argument("--pos", default=2029, type=int, help="site of your interest")
     args = parser.parse_args()
     main(args)
```

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.3.8/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.7/setup.py` & `current_events_magnifier-0.0.3.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.3.7",
+    version="0.0.3.8",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```


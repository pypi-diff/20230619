# Comparing `tmp/pandoc-latex-admonition-1.3.2.tar.gz` & `tmp/pandoc_latex_admonition-1.3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pandoc-latex-admonition-1.3.2.tar", last modified: Mon Feb 22 16:29:52 2021, max compression
+gzip compressed data, was "pandoc_latex_admonition-1.3.3.0.tar", max compression
```

## Comparing `pandoc-latex-admonition-1.3.2.tar` & `pandoc_latex_admonition-1.3.3.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxrwxr-x   0 chdemko   (1000) chdemko   (1000)        0 2021-02-22 16:29:52.761727 pandoc-latex-admonition-1.3.2/
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)     1521 2019-02-19 22:23:40.000000 pandoc-latex-admonition-1.3.2/LICENSE
--rw-rw-r--   0 chdemko   (1000) chdemko   (1000)       55 2017-12-11 09:56:32.000000 pandoc-latex-admonition-1.3.2/MANIFEST.in
--rw-rw-r--   0 chdemko   (1000) chdemko   (1000)    11114 2021-02-22 16:29:52.761727 pandoc-latex-admonition-1.3.2/PKG-INFO
--rw-rw-r--   0 chdemko   (1000) chdemko   (1000)     9424 2021-02-22 16:29:33.000000 pandoc-latex-admonition-1.3.2/README.md
-drwxrwxr-x   0 chdemko   (1000) chdemko   (1000)        0 2021-02-22 16:29:52.761727 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.egg-info/
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)    11114 2021-02-22 16:29:52.000000 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.egg-info/PKG-INFO
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)      359 2021-02-22 16:29:52.000000 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.egg-info/SOURCES.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)        1 2021-02-22 16:29:52.000000 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.egg-info/dependency_links.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)       74 2021-02-22 16:29:52.000000 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.egg-info/entry_points.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)       68 2021-02-22 16:29:52.000000 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.egg-info/requires.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)       24 2021-02-22 16:29:52.000000 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.egg-info/top_level.txt
--rw-rw-r--   0 chdemko   (1000) chdemko   (1000)    19337 2021-02-22 16:28:30.000000 pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.py
--rw-rw-r--   0 chdemko   (1000) chdemko   (1000)      133 2021-02-22 16:29:52.761727 pandoc-latex-admonition-1.3.2/setup.cfg
--rw-rw-r--   0 chdemko   (1000) chdemko   (1000)     3450 2021-02-22 16:28:30.000000 pandoc-latex-admonition-1.3.2/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-19 11:46:05.671285 pandoc_latex_admonition-1.3.3.0/LICENSE
+-rw-r--r--   0        0        0     9499 2023-06-19 11:46:05.671285 pandoc_latex_admonition-1.3.3.0/README.md
+-rw-r--r--   0        0        0    18795 2023-06-19 11:46:05.675285 pandoc_latex_admonition-1.3.3.0/pandoc_latex_admonition.py
+-rw-r--r--   0        0        0     2933 2023-06-19 11:46:05.675285 pandoc_latex_admonition-1.3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10606 1970-01-01 00:00:00.000000 pandoc_latex_admonition-1.3.3.0/PKG-INFO
```

### Comparing `pandoc-latex-admonition-1.3.2/LICENSE` & `pandoc_latex_admonition-1.3.3.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2017-2019, Christophe Demko
+Copyright (c) 2017-2023, Christophe Demko
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pandoc-latex-admonition-1.3.2/PKG-INFO` & `pandoc_latex_admonition-1.3.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,107 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-admonition
-Version: 1.3.2
+Version: 1.3.3.0
 Summary: A pandoc filter for adding admonition in LaTeX
 Home-page: https://github.com/chdemko/pandoc-latex-admonition
+License: BSD-3-Clause
+Keywords: pandoc,filters,latex,admonition
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
-Maintainer: Christophe Demko
-Maintainer-email: chdemko@gmail.com
-License: BSD-3-Clause
-Download-URL: https://github.com/chdemko/pandoc-latex-admonition/archive/master.zip
-Description: # pandoc-latex-admonition
-        [![Build Status](https://img.shields.io/travis/chdemko/pandoc-latex-admonition/1.3.2.svg?logo=travis)](https://travis-ci.org/chdemko/pandoc-latex-admonition/branches)
-        [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-admonition/1.3.2.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-latex-admonition?branch=1.3.2)
-        [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-latex-admonition/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-latex-admonition/)
-        [![Code Beat](https://codebeat.co/badges/8430d731-6b3d-401a-a26f-1172904e8e5b)](https://codebeat.co/projects/github-com-chdemko-pandoc-latex-admonition-develop/)
-        [![Codacy](https://img.shields.io/codacy/grade/443f4a26698a4ba0be5064fe9323f2a0.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-latex-admonition)
-        [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-latex-admonition/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-latex-admonition)
-        [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-admonition.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-admonition/)
-        [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-admonition/)
-        [![License](https://img.shields.io/pypi/l/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-latex-admonition/1.3.2/LICENSE)
-        [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-admonition.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-admonition/)
-        [![Downloads](https://pepy.tech/badge/pandoc-latex-admonition)](https://pepy.tech/project/pandoc-latex-admonition)
-        [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-admonition/)
-        [![Docs](https://img.shields.io/readthedocs/pandoc-latex-admonition.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-admonition.readthedocs.io/en/latest/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
-        
-        *pandoc-latex-admonition* is a [pandoc] filter for adding admonition to `div`s or `codeblock`s elements.
-        
-        It uses the *tcolorbox* LaTeX package to generate admonitions and the *footnote* LaTeX package to handle correctly footnotes in admonition.
-        
-        [pandoc]: http://pandoc.org/
-        
-        Documentation
-        -------------
-        
-        See the [Read the docs pages](http://pandoc-latex-admonition.readthedocs.io/en/latest/).
-        
-        Usage
-        -----
-        
-        To apply the filter, use the following option with pandoc:
-        
-            --filter pandoc-latex-admonition
-        
-        Installation
-        ------------
-        
-        *pandoc-latex-admonition* requires [python 3.6], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
-        
-        Install *pandoc-latex-admonition* as root using the bash command
-        
-            pip install pandoc-latex-admonition
-        
-        To upgrade to the most recent release, use
-        
-            pip install --upgrade pandoc-latex-admonition
-        
-        To upgrade to the current code, use
-        
-            pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-admonition
-        
-        `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
-        
-            apt-get update
-            apt-get install python-pip
-        
-        Make sure you have the
-        
-        * *tcolorbox*
-        * *footnote*
-        * *xcolor*
-        * *ifthen*
-        
-        LaTeX packages. On linux you have to install some extra libraries **before** *pandoc-latex-admonition*. On a Debian-based system (including Ubuntu), you can install it as root using
-        
-        	apt-get install texlive-latex-extra
-        
-        [python 3.6]: https://www.python.org
-        [on Windows]: https://www.python.org/downloads/windows
-        [PyPI]: https://pypi.org
-        
-        
-        Getting Help
-        ------------
-        
-        If you have any difficulties with pandoc-latex-admonition, please feel welcome to [file an issue] on github so that we can help.
-        
-        [file an issue]: https://github.com/chdemko/pandoc-latex-admonition/issues
-        
-        
-Keywords: pandoc filters latex admonition
-Platform: UNKNOWN
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Text Processing :: Filters
+Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
+
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-latex-admonition/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-admonition/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-admonition/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-latex-admonition?branch=develop)
+[![Code Climate](https://codeclimate.com/github/chdemko/pandoc-latex-admonition/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-latex-admonition/)
+[![Code Beat](https://codebeat.co/badges/6ce21bdf-71da-4409-a74a-575987461a72)](https://codebeat.co/projects/github-com-chdemko-pandoc-latex-admonition-develop/)
+[![Codacy](https://img.shields.io/codacy/grade/443f4a26698a4ba0be5064fe9323f2a0.svg?logo=codacy&logoColor=white)](https://app.codacy.com/gh/chdemko/pandoc-latex-admonition/)
+[![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-latex-admonition/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-latex-admonition)
+[![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-admonition.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-admonition/)
+[![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-admonition/)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-latex-admonition/develop/LICENSE)
+[![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-admonition.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-admonition/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-3.0%20|%203.1-blue.svg)](https://pandoc.org/)
+[![Downloads](https://pepy.tech/badge/pandoc-latex-admonition)](https://pepy.tech/project/pandoc-latex-admonition)
+[![Development Status](https://img.shields.io/pypi/status/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-admonition/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-latex-admonition.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-admonition.readthedocs.io/en/latest/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
+
+*pandoc-latex-admonition* is a [pandoc] filter for adding admonition to `div`s or `codeblock`s elements.
+
+It uses the *tcolorbox* LaTeX package to generate admonitions and the *footnote* LaTeX package to handle correctly footnotes in admonition.
+
+[pandoc]: http://pandoc.org/
+
+Instructions
+------------
+
+*pandoc-latex-admonition* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+
+Install *pandoc-latex-admonition* using the bash command
+
+~~~shell
+$ pip install pandoc-latex-admonition
+~~~
+
+To upgrade to the most recent release, use
+
+~~~shell
+$ pip install --upgrade pandoc-latex-admonition
+~~~
+
+To upgrade to the current code, use
+
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-admonition
+~~~
+
+`pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
+
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
+
+Make sure you have the
+
+* *tcolorbox*
+* *footnote*
+* *xcolor*
+* *ifthen*
+
+LaTeX packages. On linux you have to install some extra libraries **before** *pandoc-latex-admonition*. On a Debian-based system (including Ubuntu), you can install it as root using
+
+~~~shell
+$ sudo apt-get install texlive-latex-extra
+~~~
+
+[python]: https://www.python.org
+[on Windows]: https://www.python.org/downloads/windows
+[PyPI]: https://pypi.org
+
+
+Getting Help
+------------
+
+If you have any difficulties with pandoc-latex-admonition, please feel welcome to [file an issue] on github so that we can help.
+
+[file an issue]: https://github.com/chdemko/pandoc-latex-admonition/issues
+
+
```

### Comparing `pandoc-latex-admonition-1.3.2/README.md` & `pandoc_latex_admonition-1.3.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-# pandoc-latex-admonition
-[![Build Status](https://img.shields.io/travis/chdemko/pandoc-latex-admonition/1.3.2.svg?logo=travis)](https://travis-ci.org/chdemko/pandoc-latex-admonition/branches)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-admonition/1.3.2.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-latex-admonition?branch=1.3.2)
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-latex-admonition/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-admonition/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-admonition/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-latex-admonition?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-latex-admonition/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-latex-admonition/)
-[![Code Beat](https://codebeat.co/badges/8430d731-6b3d-401a-a26f-1172904e8e5b)](https://codebeat.co/projects/github-com-chdemko-pandoc-latex-admonition-develop/)
-[![Codacy](https://img.shields.io/codacy/grade/443f4a26698a4ba0be5064fe9323f2a0.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-latex-admonition)
+[![Code Beat](https://codebeat.co/badges/6ce21bdf-71da-4409-a74a-575987461a72)](https://codebeat.co/projects/github-com-chdemko-pandoc-latex-admonition-develop/)
+[![Codacy](https://img.shields.io/codacy/grade/443f4a26698a4ba0be5064fe9323f2a0.svg?logo=codacy&logoColor=white)](https://app.codacy.com/gh/chdemko/pandoc-latex-admonition/)
 [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-latex-admonition/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-latex-admonition)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-admonition.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-admonition/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-admonition/)
-[![License](https://img.shields.io/pypi/l/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-latex-admonition/1.3.2/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-latex-admonition/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-admonition.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-admonition/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-3.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Downloads](https://pepy.tech/badge/pandoc-latex-admonition)](https://pepy.tech/project/pandoc-latex-admonition)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-admonition.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-admonition/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-latex-admonition.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-admonition.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 *pandoc-latex-admonition* is a [pandoc] filter for adding admonition to `div`s or `codeblock`s elements.
 
 It uses the *tcolorbox* LaTeX package to generate admonitions and the *footnote* LaTeX package to handle correctly footnotes in admonition.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [Read the docs pages](http://pandoc-latex-admonition.readthedocs.io/en/latest/).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-latex-admonition
-
-Installation
+Instructions
 ------------
 
-*pandoc-latex-admonition* requires [python 3.6], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+*pandoc-latex-admonition* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-latex-admonition* as root using the bash command
+Install *pandoc-latex-admonition* using the bash command
 
-    pip install pandoc-latex-admonition
+~~~shell
+$ pip install pandoc-latex-admonition
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-latex-admonition
+~~~shell
+$ pip install --upgrade pandoc-latex-admonition
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-admonition
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-admonition
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
 
 Make sure you have the
 
 * *tcolorbox*
 * *footnote*
 * *xcolor*
 * *ifthen*
 
 LaTeX packages. On linux you have to install some extra libraries **before** *pandoc-latex-admonition*. On a Debian-based system (including Ubuntu), you can install it as root using
 
-	apt-get install texlive-latex-extra
+~~~shell
+$ sudo apt-get install texlive-latex-extra
+~~~
 
-[python 3.6]: https://www.python.org
+[python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
 
 
 Getting Help
 ------------
```

### Comparing `pandoc-latex-admonition-1.3.2/pandoc_latex_admonition.py` & `pandoc_latex_admonition-1.3.3.0/pandoc_latex_admonition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for adding admonition in LaTeX
+Pandoc filter for adding admonition in LaTeX.
 """
 
 import uuid
 
-from panflute import (
-    convert_text,
-    run_filter,
-    debug,
+from panflute import (  # type: ignore
+    Figure,
+    MetaBool,
+    MetaInlines,
+    MetaList,
     Note,
-    RawInline,
     RawBlock,
-    Para,
-    Image,
-    MetaList,
-    MetaInlines,
-    MetaBool,
+    RawInline,
+    convert_text,
+    debug,
+    run_filter,
 )
 
 
 def default_environment():
     """
-    Defines the default environment
+    Get the default environment.
 
     Returns
     -------
         The default environment
     """
     return {
         "env": "env-" + str(uuid.uuid4()),
@@ -39,15 +38,15 @@
         "localfootnotes": False,
         "nobreak": False,
     }
 
 
 def x11colors():
     """
-    Get the x11 colors
+    Get the x11 colors.
 
     Returns
     -------
         The x11 colors
     """
     # See https://www.w3.org/TR/css-color-3/#svg-color
     return {
@@ -200,30 +199,29 @@
         "yellowgreen": "9ACD32",
     }
 
 
 # pylint: disable=inconsistent-return-statements
 def admonition(elem, doc):
     """
-    Add admonition to elem
+    Add admonition to elem.
 
     Arguments
     ---------
-        elem:
-            The current element
-        doc:
-            The pandoc document
+    elem
+        The current element
+    doc
+        The pandoc document
 
     Returns
     -------
-        The modified element
+        The modified element or None
     """
     # Is it in the right format and is it Div or a CodeBlock?
-    if doc.format in ["latex", "beamer"] and elem.tag in ["Div", "CodeBlock"]:
-
+    if doc.format in ("latex", "beamer") and elem.tag in ("Div", "CodeBlock"):
         # Is there a latex-admonition-color attribute?
         if "latex-admonition-color" in elem.attributes:
             environment = define_environment(
                 doc,
                 elem.attributes,
                 "latex-admonition-color",
                 "latex-admonition-position",
@@ -236,31 +234,31 @@
             doc.added.append(environment)
             return add_latex(elem, environment)
         # Get the classes
         classes = set(elem.classes)
 
         # Loop on all fontsize definition
         for environment in doc.defined:
-
             # Are the classes correct?
             if classes >= environment["classes"]:
                 return add_latex(elem, environment)
+    return None
 
 
 def add_latex(elem, environment):
     """
     Add LaTeX code to the element.
 
     Arguments
     ---------
-        elem:
-            The current element
+    elem
+        The current element
 
-        environment:
-            The environment to add
+    environment
+        The environment to add
 
     Returns
     -------
         The modified element
     """
 
     def note(element, doc):
@@ -279,59 +277,54 @@
                             output_format="latex",
                         ),
                         "}",
                     ]
                 ),
                 "tex",
             )
+        return None
 
     images = []
 
     def extract_images(element, _doc):
         # Extract image which is alone with a title
-        if (
-            isinstance(element, Para)
-            and len(element.content) == 1
-            and isinstance(element.content[0], Image)
-            and bool(element.content[0].content)
-        ):
+        if isinstance(element, Figure) and len(element.content) == 1:
             images.append(element)
             return []
+        return None
 
     # The images need to be placed after the framed environment
     return [
         RawBlock("\\begin{" + environment["env"] + "}", "tex"),
         elem.walk(extract_images).walk(note),
         RawBlock("\\end{" + environment["env"] + "}", "tex"),
     ] + images
 
 
 def prepare(doc):
     """
-    Prepare the document
+    Prepare the document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
     """
     doc.x11colors = x11colors()
 
     # Prepare the definitions
     doc.defined = []
     doc.added = []
 
     # Get the meta data
     meta = doc.get_metadata("pandoc-latex-admonition")
 
     if isinstance(meta, list):
-
         # Loop on all definitions
         for definition in meta:
-
             # Verify the definition
             if (
                 isinstance(definition, dict)
                 and "classes" in definition
                 and isinstance(definition["classes"], list)
             ):
                 environment = define_environment(
@@ -358,44 +351,44 @@
     key_linewidth,
     key_margin,
     key_innermargin,
     key_localfootnotes,
     key_nobreak,
 ):
     """
-    Define a new environment
+    Define a new environment.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_color:
-            The color key
+    key_color
+        The color key
 
-        key_position:
-            The position key
+    key_position
+        The position key
 
-        key_linewidth:
-            The linewidth key
+    key_linewidth
+        The linewidth key
 
-        key_margin:
-            The margin key
+    key_margin
+        The margin key
 
-        key_innermargin:
-            The innermargin key
+    key_innermargin
+        The innermargin key
 
-        key_localfootnotes:
-            The localfootnotes key
+    key_localfootnotes
+        The localfootnotes key
 
-        key_nobreak:
-            The nobreak key
+    key_nobreak
+        The nobreak key
 
     Returns
     -------
         A new environment
     """
     # Get the default environment
     environment = default_environment()
@@ -407,30 +400,29 @@
     define_localfootnotes(environment, definition, key_localfootnotes)
     define_nobreak(environment, definition, key_nobreak)
     return environment
 
 
 def define_color(environment, definition, key_color, doc=None):
     """
-    Get the color
+    Define the color.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_color:
-            The color key
-
-        doc:
-            The pandoc document
+    key_color
+        The color key
 
+    doc
+        The pandoc document
     """
     if key_color in definition:
         color = str(definition[key_color]).lower()
         if color in doc.x11colors:
             environment["color"] = color
         else:
             # color must be a valid x11 color
@@ -441,45 +433,45 @@
                 + " is not a valid x11 color; using "
                 + environment["color"]
             )
 
 
 def define_position(environment, definition, key_position):
     """
-    Get the position
+    Define the position.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_position:
-            The position key
+    key_position
+        The position key
     """
     if key_position in definition:
         environment["position"] = str(definition[key_position])
 
 
 def define_linewidth(environment, definition, key_linewidth):
     """
-    Get the line width
+    Define the line width.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_linewidth:
-            The linewidth key
+    key_linewidth
+        The linewidth key
     """
     if key_linewidth in definition:
         try:
             linewidth = int(str(definition[key_linewidth]))
             if linewidth <= 0:
                 debug(
                     "[WARNING] pandoc-latex-admonition: "
@@ -493,113 +485,113 @@
                 "[WARNING] pandoc-latex-admonition: linewidth is not a valid; using "
                 + str(environment["linewidth"])
             )
 
 
 def define_margin(environment, definition, key_margin):
     """
-    Get the margin
+    Define the margin.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_margin:
-            The margin key
+    key_margin
+        The margin key
     """
     if key_margin in definition:
         try:
             environment["margin"] = int(str(definition[key_margin]))
         except ValueError:
             debug(
                 "[WARNING] pandoc-latex-admonition: margin is not a valid; using "
                 + str(environment["margin"])
             )
 
 
 def define_innermargin(environment, definition, key_innermargin):
     """
-    Get the inner margin
+    Define the inner margin.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_innermargin:
-            The inner margin key
+    key_innermargin
+        The inner margin key
     """
     if key_innermargin in definition:
         try:
             environment["innermargin"] = int(str(definition[key_innermargin]))
         except ValueError:
             debug(
                 "[WARNING] pandoc-latex-admonition: innermargin is not a valid; using "
                 + str(environment["innermargin"])
             )
 
 
 def define_localfootnotes(environment, definition, key_localfootnotes):
     """
-    Get the local footnotes
+    Define the local footnotes.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_localfootnotes:
-            The localfootnotes key
+    key_localfootnotes
+        The localfootnotes key
     """
     if key_localfootnotes in definition:
         environment["localfootnotes"] = (
             str(definition[key_localfootnotes]).lower() == "true"
         )
 
 
 def define_nobreak(environment, definition, key_nobreak):
     """
-    Get the nobreak
+    Define the nobreak.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        definition:
-            The definition
+    definition
+        The definition
 
-        key_nobreak:
-            The nobreak key
+    key_nobreak
+        The nobreak key
     """
     if key_nobreak in definition:
         environment["nobreak"] = str(definition[key_nobreak]).lower() == "true"
 
 
 def new_environment(doc, environment):
     """
-    Create a new environment
+    Create a new environment.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
 
-        environment:
-            The environment
+    environment
+        The environment
 
     Returns
     -------
         The LaTeX environment
     """
     options = ["blanker"]
 
@@ -607,141 +599,133 @@
         options.append("breakable")
     if environment["position"] == "left":
         options.append(left_bar(environment))
     elif environment["position"] == "right":
         options.append(right_bar(environment))
     elif environment["position"] == "inner":
         options.append(
-            "if odd page={%s}{%s}" % (left_bar(environment), right_bar(environment))
+            f"if odd page={{{left_bar(environment)}}}{{{right_bar(environment)}}}"
         )
     elif environment["position"] == "outer":
         options.append(
-            "if odd page={%s}{%s}" % (right_bar(environment), left_bar(environment))
+            f"if odd page={{{right_bar(environment)}}}{{{left_bar(environment)}}}"
         )
     else:
         options.append(left_bar(environment))
 
     if environment["localfootnotes"] or doc.format == "beamer":
-        return r"""
-\newenvironment{%s}
-{
-    \tcolorbox[%s]
-}
-{
-    \endtcolorbox
-}
-        """ % (
-            environment["env"],
-            ",".join(options),
-        )
-    return r"""
-\newenvironment{%s}
-{
-    \savenotes\tcolorbox[%s]
-}
-{
-    \endtcolorbox\spewnotes
-}
-                """ % (
-        environment["env"],
-        ",".join(options),
-    )
+        return f"""
+\\newenvironment{{{environment['env']}}}
+{{
+    \\tcolorbox[{','.join(options)}]
+}}
+{{
+    \\endtcolorbox
+}}
+        """
+    return f"""
+\\newenvironment{{{environment['env']}}}
+{{
+    \\savenotes\\tcolorbox[{','.join(options)}]
+}}
+{{
+    \\endtcolorbox\\spewnotes
+}}
+        """
 
 
 def left_bar(environment):
     """
-    Generates a left bar
+    Generate a left bar.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
     Returns
     -------
         The left bar options
     """
     return bar(environment, "left", "west")
 
 
 def right_bar(environment):
     """
-    Generates a right bar
+    Generate a right bar.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
     Returns
     -------
         The right bar options
     """
     return bar(environment, "right", "east")
 
 
 # pylint: disable=blacklisted-name
 def bar(environment, position, localization):
     """
-    Generates a bar
+    Generate a bar.
 
     Arguments
     ---------
-        environment:
-            The environment
+    environment
+        The environment
 
-        position:
-            left or right
+    position
+        left or right
 
-        localization:
-            east or west
+    localization
+        east or west
 
     Returns
     -------
         The bar options
     """
-    return "%s=%gpt,borderline %s={%gpt}{%gpt}{%s}" % (
-        position,
-        environment["innermargin"],
-        localization,
-        environment["linewidth"],
-        environment["margin"],
-        environment["color"],
+    return (
+        f"{position}={environment['innermargin']:g}pt,borderline "
+        f"{localization}={{{environment['linewidth']:g}pt}}"
+        f"{{{environment['margin']:g}pt}}{{{environment['color']}}}"
     )
 
 
 def finalize(doc):
     """
-    Finalize the pandoc document
+    Finalize the pandoc document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
     """
     # load footnote or footnotehyper package
     if doc.format == "latex":
         doc.metadata["tables"] = MetaBool(True)
 
     # Add header-includes if necessary
     if "header-includes" not in doc.metadata:
         doc.metadata["header-includes"] = MetaList()
     # Convert header-includes to MetaList if necessary
     elif not isinstance(doc.metadata["header-includes"], MetaList):
         doc.metadata["header-includes"] = MetaList(doc.metadata["header-includes"])
 
-    # Add usefull LaTexPackage
+    # Add useful LaTexPackage
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\\usepackage{xcolor}", "tex"))
     )
 
     # Define x11 colors
-    tex = []
-    for name, color in doc.x11colors.items():
-        tex.append("\\definecolor{" + name.lower() + "}{HTML}{" + color + "}")
+    tex = [
+        f"\\definecolor{{{name.lower()}}}{{HTML}}{{{color}}}"
+        for name, color in doc.x11colors.items()
+    ]
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\n".join(tex), "tex"))
     )
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\\usepackage[most]{tcolorbox}", "tex"))
     )
     doc.metadata["header-includes"].append(
@@ -767,20 +751,20 @@
         doc.metadata["header-includes"].append(
             MetaInlines(RawInline(new_environment(doc, environment), "tex"))
         )
 
 
 def main(doc=None):
     """
-    Main function called by the script.
+    Convert the pandoc document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
 
     Returns
     -------
         The modified pandoc document
     """
     return run_filter(admonition, prepare=prepare, finalize=finalize, doc=doc)
```


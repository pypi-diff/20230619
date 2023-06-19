# Comparing `tmp/pandoc-beamer-multigraphics-0.1.1.tar.gz` & `tmp/pandoc_beamer_multigraphics-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-beamer-multigraphics-0.1.1.tar", last modified: Mon Feb 22 20:16:53 2021, max compression
+gzip compressed data, was "pandoc_beamer_multigraphics-1.0.0.0.tar", max compression
```

## Comparing `pandoc-beamer-multigraphics-0.1.1.tar` & `pandoc_beamer_multigraphics-1.0.0.0.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-22 20:16:53.883468 pandoc-beamer-multigraphics-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-02-22 20:16:44.000000 pandoc-beamer-multigraphics-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10831 2021-02-22 20:16:53.887467 pandoc-beamer-multigraphics-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9064 2021-02-22 20:16:44.000000 pandoc-beamer-multigraphics-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-22 20:16:53.883468 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10831 2021-02-22 20:16:53.000000 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-02-22 20:16:53.000000 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-22 20:16:53.000000 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-02-22 20:16:53.000000 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-02-22 20:16:53.000000 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-02-22 20:16:53.000000 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2021-02-22 20:16:44.000000 pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-02-22 20:16:53.887467 pandoc-beamer-multigraphics-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4052 2021-02-22 20:16:44.000000 pandoc-beamer-multigraphics-0.1.1/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-19 13:10:44.878840 pandoc_beamer_multigraphics-1.0.0.0/LICENSE
+-rw-r--r--   0        0        0     9260 2023-06-19 13:10:44.882840 pandoc_beamer_multigraphics-1.0.0.0/README.md
+-rw-r--r--   0        0        0     4182 2023-06-19 13:10:44.886840 pandoc_beamer_multigraphics-1.0.0.0/pandoc_beamer_multigraphics.py
+-rw-r--r--   0        0        0     2954 2023-06-19 13:10:44.886840 pandoc_beamer_multigraphics-1.0.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10373 1970-01-01 00:00:00.000000 pandoc_beamer_multigraphics-1.0.0.0/PKG-INFO
```

### Comparing `pandoc-beamer-multigraphics-0.1.1/PKG-INFO` & `pandoc_beamer_multigraphics-1.0.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,92 @@
 Metadata-Version: 2.1
 Name: pandoc-beamer-multigraphics
-Version: 0.1.1
-Summary: A pandoc filter for adding beamer multigraphics ability
-Home-page: https://github.com/chdemko/pandoc-beamer-multigraphics
-Author: Christophe Demko
-Author-email: chdemko@gmail.com
-Maintainer: Christophe Demko
-Maintainer-email: chdemko@gmail.com
+Version: 1.0.0.0
+Summary: A pandoc filter for adding admonition in LaTeX
+Home-page: https://github.com/chdemko/beamer-multigraphics
 License: BSD-3-Clause
-Download-URL: https://github.com/chdemko/pandoc-beamer-multigraphics/archive/master.zip
-Description: # pandoc-beamer-multigraphics
-        ![Python package](https://github.com/chdemko/pandoc-beamer-multigraphics/workflows/Python%20package/badge.svg?branch=0.1.1)
-        [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-multigraphics/0.1.1.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-multigraphics?branch=0.1.1)
-        [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-multigraphics/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-multigraphics/)
-        [![Code Beat](https://codebeat.co/badges/cb5538dc-f30b-4ac4-abf6-3c213682c54d)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-multigraphics-develop/)
-        [![Codacy](https://img.shields.io/codacy/grade/af5a670790264990811713280a8f8dcf.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-multigraphics)
-        [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-multigraphics/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-multigraphics)
-        [![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-multigraphics.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-multigraphics/)
-        [![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-multigraphics/)
-        [![License](https://img.shields.io/pypi/l/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-multigraphics/0.1.1/LICENSE)
-        [![Python version](https://img.shields.io/pypi/pyversions/pandoc-beamer-multigraphics.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-multigraphics/)
-        [![Downloads](https://pepy.tech/badge/pandoc-beamer-multigraphics)](https://pepy.tech/project/pandoc-beamer-multigraphics)
-        [![Development Status](https://img.shields.io/pypi/status/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-multigraphics/)
-        [![Docs](https://img.shields.io/readthedocs/pandoc-beamer-multigraphics.svg?logo=read-the-docs&logoColor=white)](http://pandoc-beamer-multigraphics.readthedocs.io/en/0.1.1/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
-        
-        *pandoc-beamer-multigraphics* is a [pandoc] filter for adding beamer ability to use multi-images.
-        
-        [pandoc]: http://pandoc.org/
-        
-        Documentation
-        -------------
-        
-        See the [Read the docs pages](http://pandoc-beamer-multigraphics.readthedocs.io/en/0.1.1/).
-        
-        Usage
-        -----
-        
-        To apply the filter, use the following option with pandoc:
-        
-            --filter pandoc-beamer-multigraphics
-        
-        Installation
-        ------------
-        
-        *pandoc-beamer-multigraphics* requires [python 3.6], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
-        
-        Install *pandoc-beamer-multigraphics* as root using the bash command
-        
-            pip install pandoc-beamer-multigraphics
-        
-        To upgrade to the most recent release, use
-        
-            pip install --upgrade pandoc-beamer-multigraphics
-        
-        To upgrade to the current code, use
-        
-            pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-multigraphics
-        
-        `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
-        
-            apt-get update
-            apt-get install python-pip
-        
-        [python 3.6]: https://www.python.org
-        [on Windows]: https://www.python.org/downloads/windows
-        [PyPI]: https://pypi.org
-        
-        
-        Getting Help
-        ------------
-        
-        If you have any difficulties with pandoc-beamer-multigraphics, please feel welcome to [file an issue] on github so that we can help.
-        
-        [file an issue]: https://github.com/chdemko/pandoc-beamer-multigraphics/issues
-        
-        
 Keywords: pandoc,filters,graphics,latex,beamer
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
+Author: Christophe Demko
+Author-email: chdemko@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Natural Language :: English
+Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: test
+
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-beamer-multigraphics/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-beamer-multigraphics/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-multigraphics/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-multigraphics?branch=develop)
+[![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-multigraphics/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-multigraphics/)
+[![Code Beat](https://codebeat.co/badges/cb5538dc-f30b-4ac4-abf6-3c213682c54d)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-multigraphics-develop/)
+[![Codacy](https://img.shields.io/codacy/grade/af5a670790264990811713280a8f8dcf.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-multigraphics)
+[![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-multigraphics/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-multigraphics)
+[![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-multigraphics.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-multigraphics/)
+[![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-multigraphics/)
+[![License](https://img.shields.io/pypi/l/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-multigraphics/develop/LICENSE)
+[![Python version](https://img.shields.io/pypi/pyversions/pandoc-beamer-multigraphics.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-multigraphics/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
+[![Downloads](https://pepy.tech/badge/pandoc-beamer-multigraphics)](https://pepy.tech/project/pandoc-beamer-multigraphics)
+[![Development Status](https://img.shields.io/pypi/status/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-multigraphics/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-beamer-multigraphics.svg?logo=read-the-docs&logoColor=white)](http://pandoc-beamer-multigraphics.readthedocs.io/en/latest/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
+
+*pandoc-beamer-multigraphics* is a [pandoc] filter for adding beamer ability to use multi-images.
+
+[pandoc]: http://pandoc.org/
+
+Instructions
+------------
+
+*pandoc-beamer-multigraphics* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+
+Install *pandoc-beamer-multigraphics* using the bash command
+
+~~~shell
+$ pip install pandoc-beamer-multigraphics
+~~~
+
+To upgrade to the most recent release, use
+
+~~~shell
+$ pip install --upgrade pandoc-beamer-multigraphics
+~~~
+
+To upgrade to the current code, use
+
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-multigraphics
+~~~
+
+`pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
+
+~~~shell
+$ sudo apt-get install python3-pip
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
+If you have any difficulties with pandoc-beamer-multigraphics, please feel welcome to [file an issue] on github so that we can help.
+
+[file an issue]: https://github.com/chdemko/pandoc-beamer-multigraphics/issues
+
+
```

### Comparing `pandoc-beamer-multigraphics-0.1.1/README.md` & `pandoc_beamer_multigraphics-1.0.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-# pandoc-beamer-multigraphics
-![Python package](https://github.com/chdemko/pandoc-beamer-multigraphics/workflows/Python%20package/badge.svg?branch=0.1.1)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-multigraphics/0.1.1.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-multigraphics?branch=0.1.1)
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-beamer-multigraphics/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-beamer-multigraphics/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-multigraphics/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-multigraphics?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-multigraphics/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-multigraphics/)
 [![Code Beat](https://codebeat.co/badges/cb5538dc-f30b-4ac4-abf6-3c213682c54d)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-multigraphics-develop/)
 [![Codacy](https://img.shields.io/codacy/grade/af5a670790264990811713280a8f8dcf.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-multigraphics)
 [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-multigraphics/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-multigraphics)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-multigraphics.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-multigraphics/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-multigraphics/)
-[![License](https://img.shields.io/pypi/l/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-multigraphics/0.1.1/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-multigraphics/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-beamer-multigraphics.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-multigraphics/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Downloads](https://pepy.tech/badge/pandoc-beamer-multigraphics)](https://pepy.tech/project/pandoc-beamer-multigraphics)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-beamer-multigraphics.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-multigraphics/)
-[![Docs](https://img.shields.io/readthedocs/pandoc-beamer-multigraphics.svg?logo=read-the-docs&logoColor=white)](http://pandoc-beamer-multigraphics.readthedocs.io/en/0.1.1/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-beamer-multigraphics.svg?logo=read-the-docs&logoColor=white)](http://pandoc-beamer-multigraphics.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 *pandoc-beamer-multigraphics* is a [pandoc] filter for adding beamer ability to use multi-images.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [Read the docs pages](http://pandoc-beamer-multigraphics.readthedocs.io/en/0.1.1/).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-beamer-multigraphics
-
-Installation
+Instructions
 ------------
 
-*pandoc-beamer-multigraphics* requires [python 3.6], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+*pandoc-beamer-multigraphics* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-beamer-multigraphics* as root using the bash command
+Install *pandoc-beamer-multigraphics* using the bash command
 
-    pip install pandoc-beamer-multigraphics
+~~~shell
+$ pip install pandoc-beamer-multigraphics
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-beamer-multigraphics
+~~~shell
+$ pip install --upgrade pandoc-beamer-multigraphics
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-multigraphics
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-multigraphics
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
 
-[python 3.6]: https://www.python.org
+[python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
 
 
 Getting Help
 ------------
```

### Comparing `pandoc-beamer-multigraphics-0.1.1/pandoc_beamer_multigraphics.py` & `pandoc_beamer_multigraphics-1.0.0.0/pandoc_beamer_multigraphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for using beamer multi-graphics ability
+Pandoc filter for using beamer multi-graphics ability.
 """
 
-from panflute import run_filter, Image, RawInline, MetaList, MetaInlines
+from panflute import (  # type: ignore
+    Image,
+    MetaInlines,
+    MetaList,
+    RawInline,
+    run_filter,
+)
 
 
 def image(elem, doc):
     """
     Transform image element.
 
     Arguments
     ---------
-        elem:
-            current element
-        doc:
-            pandoc document
+    elem
+        current element
+    doc
+        pandoc document
+
+    Returns
+    -------
+        RawInline or None
     """
     if doc.format == "beamer" and isinstance(elem, Image):
         classes = frozenset(elem.classes)
 
-        # Loop on all multigraphics definition
+        # Loop on all multi-graphics definition
         for definition in doc.defined:
-
             # Are the classes correct?
             if classes >= definition["classes"]:
-
                 graphics = []
 
                 if (
                     "height" in elem.attributes
                     or "width" in elem.attributes
                     or "height" in definition
                     or "width" in definition
@@ -51,54 +59,53 @@
                             )
                         )
                     )
 
                 options = []
 
                 if "start" in elem.attributes:
-                    options.append("start=%d" % int(elem.attributes["start"]))
+                    options.append(f"start={int(elem.attributes['start']):d}")
 
                 if "end" in elem.attributes:
-                    options.append("end=%d" % int(elem.attributes["end"]))
+                    options.append(f"end={int(elem.attributes['end']):d}")
 
                 options.append(
-                    "format=%s"
-                    % str(elem.attributes.get("format", definition["format"]))
+                    f"format={elem.attributes.get('format', definition['format'])}"
                 )
 
                 return RawInline(
-                    "\\multiinclude[graphics={%s},%s]{%s}"
-                    % (",".join(graphics), ",".join(options), elem.url),
+                    (
+                        f"\\multiinclude"
+                        f"[graphics={{{','.join(graphics)}}},{','.join(options)}]"
+                        f"{{{elem.url}}}"
+                    ),
                     "tex",
                 )
 
     return None
 
 
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
-
     # Prepare the definitions
     doc.defined = []
 
     # Get the meta data
     meta = doc.get_metadata("pandoc-beamer-multigraphics")
 
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
                 definition["classes"] = frozenset(definition["classes"])
@@ -109,20 +116,20 @@
                     definition["height"] = str(definition["height"])
 
                 doc.defined.append(definition)
 
 
 def finalize(doc):
     """
-    Finalize the document
+    Finalize the document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
     """
     # Add header-includes if necessary
     if "header-includes" not in doc.metadata:
         doc.metadata["header-includes"] = MetaList()
     # Convert header-includes to MetaList if necessary
     elif not isinstance(doc.metadata["header-includes"], MetaList):
         doc.metadata["header-includes"] = MetaList(doc.metadata["header-includes"])
@@ -130,19 +137,23 @@
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\\usepackage{xmpmulti}", "tex"))
     )
 
 
 def main(doc=None):
     """
-    main function.
+    Transform the document.
 
     Arguments
     ---------
-        doc:
-            pandoc document
+    doc
+        pandoc document
+
+    Returns
+    -------
+        The transformed document.
     """
     return run_filter(image, doc=doc, prepare=prepare, finalize=finalize)
 
 
 if __name__ == "__main__":
     main()
```


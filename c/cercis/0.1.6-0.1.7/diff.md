# Comparing `tmp/cercis-0.1.6.tar.gz` & `tmp/cercis-0.1.7.tar.gz`

## Comparing `cercis-0.1.6.tar` & `cercis-0.1.7.tar`

### file list

```diff
@@ -1,373 +1,377 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.6/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.6/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.6/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.6/.gitattributes
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.6/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.6/.prettierrc.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.6/.readthedocs.yaml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 cercis-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0    49716 2020-02-02 00:00:00.000000 cercis-0.1.6/CHANGES.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.6/Dockerfile
--rw-r--r--   0        0        0    23227 2020-02-02 00:00:00.000000 cercis-0.1.6/README.md
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 cercis-0.1.6/action.yml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.6/mypy.ini
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.6/test_requirements.txt
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.6/tox.ini
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/dependabot.yml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/docs-issue.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/style_issue.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/check-changelog.yml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/diff_shades_comment.yml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/lint.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/test.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/upload_binary.yml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/version-check.yml
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 cercis-0.1.6/action/main.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.6/autoload/black.vim
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.6/gallery/Dockerfile
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.6/gallery/README.md
--rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.6/gallery/gallery.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.6/plugin/black.vim
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/check_version_and_changelog.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/diff_shades_gha_helper.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/fuzz.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/make_width_table.py
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/migrate-black.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.6/src/_cercis_version.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blackd/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blackd/__main__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blackd/middlewares.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/Grammar.txt
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/PatternGrammar.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/README
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/__init__.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pygram.py
--rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pytree.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/__init__.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/conv.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/driver.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/grammar.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/literals.py
--rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/parse.py
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/pgen.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/token.py
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/tokenize.py
--rw-r--r--   0        0        0    52483 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/__main__.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/_width_table.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/brackets.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/cache.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/comments.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/concurrency.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/const.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/debug.py
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/files.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/handle_ipynb_magics.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/indent.py
--rw-r--r--   0        0        0    64165 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/linegen.py
--rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/lines.py
--rw-r--r--   0        0        0     8468 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/mode.py
--rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/numerics.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/output.py
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/py.typed
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/rusty.py
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/strings.py
--rw-r--r--   0        0        0    91890 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/trans.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/utils_line_wrapping.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/utils_linegen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/optional.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test.toml
--rw-r--r--   0        0        0   101263 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_black.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_blackd.py
--rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_format.py
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_ipynb.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_trans.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_utils_line_wrapping.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_False_False.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_False_True.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_True_False.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_True_True.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/edge_cases.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
--rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Black_default.py
--rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Black_default_2.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Cercis_default.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring_preview.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/more_quotes.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/torture.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/no_blank_line_before_docstring.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.6/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.6/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.6/LICENSE_ORIGINAL
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 cercis-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    27277 2020-02-02 00:00:00.000000 cercis-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.7/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.7/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.7/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.7/.gitattributes
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.7/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.7/.prettierrc.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.7/.readthedocs.yaml
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 cercis-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0    50085 2020-02-02 00:00:00.000000 cercis-0.1.7/CHANGES.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.7/Dockerfile
+-rw-r--r--   0        0        0    23227 2020-02-02 00:00:00.000000 cercis-0.1.7/README.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 cercis-0.1.7/action.yml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.7/mypy.ini
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.7/test_requirements.txt
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.7/tox.ini
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/ISSUE_TEMPLATE/docs-issue.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/ISSUE_TEMPLATE/style_issue.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/check-changelog.yml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/diff_shades_comment.yml
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/upload_binary.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.7/.github/workflows/version-check.yml
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 cercis-0.1.7/action/main.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.7/autoload/black.vim
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.7/gallery/Dockerfile
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.7/gallery/README.md
+-rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.7/gallery/gallery.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.7/plugin/black.vim
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/check_version_and_changelog.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/check_version_in_basics_example.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/fuzz.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.7/scripts/migrate-black.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.7/src/_cercis_version.py
+-rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blackd/middlewares.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/Grammar.txt
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/PatternGrammar.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/README
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.7/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0    52612 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/__main__.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/_width_table.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/brackets.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/cache.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/comments.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/concurrency.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/const.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/debug.py
+-rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/files.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/handle_ipynb_magics.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/indent.py
+-rw-r--r--   0        0        0    64924 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/linegen.py
+-rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/lines.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/mode.py
+-rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/numerics.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/output.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/py.typed
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/rusty.py
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/strings.py
+-rw-r--r--   0        0        0    91890 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/trans.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/utils_line_wrapping.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.7/src/cercis/utils_linegen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/optional.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test.toml
+-rw-r--r--   0        0        0   102069 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test_black.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test_blackd.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test_format.py
+-rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test_trans.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/test_utils_line_wrapping.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_comments/case_False_False.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_comments/case_False_True.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_comments/case_True_False.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_comments/case_True_True.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/edge_cases.py
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
+-rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Black_default.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Black_default_2.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Cercis_default.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/single_quote/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/single_quote/docstring_preview.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/single_quote/more_quotes.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/single_quote/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/configurable_cases/single_quote/torture.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/no_blank_line_before_docstring.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_312/type_aliases.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_312/type_params.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/pep_604.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.7/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.7/LICENSE_ORIGINAL
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 cercis-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    27417 2020-02-02 00:00:00.000000 cercis-0.1.7/PKG-INFO
```

### Comparing `cercis-0.1.6/.pre-commit-config.yaml` & `cercis-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.pre-commit-hooks.yaml` & `cercis-0.1.7/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/CHANGELOG.md` & `cercis-0.1.7/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## [0.1.7] - 2023-06-19
+
+- Changed
+  - Pulled in the latest changes from psf/black (code diff:
+    https://github.com/jsh9/cercis/pull/27)
+
 ## [0.1.6] - 2023-05-23
 
 - Added
   - A new option `--wrap-comments` to not wrap any comments (not just pragma comments)
   - A new option `--keep-blank-lines-in-brackets`
 - Changed
   - Improved the CLI output text colors because the current colors are confusing or not
```

### Comparing `cercis-0.1.6/CHANGES.md` & `cercis-0.1.7/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 <!-- Include any especially major or disruptive changes here -->
 
 ### Stable style
 
 <!-- Changes that affect Black's stable style -->
 
+- Fix a bug where an illegal trailing comma was added to return type annotations using
+  PEP 604 unions (#3735)
+
 ### Preview style
 
 <!-- Changes that affect Black's preview style -->
 
 - Implicitly concatenated strings used as function args are no longer wrapped inside
   parentheses (#3640)
 - Remove blank lines between a class definition and its docstring (#3692)
@@ -28,26 +31,33 @@
 
 <!-- Changes to how Black is packaged, such as dependency requirements -->
 
 ### Parser
 
 <!-- Changes to the parser or to version autodetection -->
 
+- Add support for the new PEP 695 syntax in Python 3.12 (#3703)
+
 ### Performance
 
 <!-- Changes that improve Black's performance. -->
 
 ### Output
 
 <!-- Changes to Black's terminal output and error messages -->
 
+- Use aware UTC datetimes internally, avoids deprecation warning on Python 3.12 (#3728)
+
 ### _Blackd_
 
 <!-- Changes to blackd -->
 
+- The `blackd` argument parser now shows the default values for options in their help
+  text (#3712)
+
 ### Integrations
 
 <!-- For example, Docker, GitHub Actions, pre-commit, editors -->
 
 - Update GitHub Action to display black output in the job summary (#3688)
 
 ### Documentation
```

### Comparing `cercis-0.1.6/Dockerfile` & `cercis-0.1.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/README.md` & `cercis-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/action.yml` & `cercis-0.1.7/action.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/mypy.ini` & `cercis-0.1.7/mypy.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tox.ini` & `cercis-0.1.7/tox.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/PULL_REQUEST_TEMPLATE.md` & `cercis-0.1.7/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/dependabot.yml` & `cercis-0.1.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md` & `cercis-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/ISSUE_TEMPLATE/config.yml` & `cercis-0.1.7/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/ISSUE_TEMPLATE/docs-issue.md` & `cercis-0.1.7/.github/ISSUE_TEMPLATE/docs-issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `cercis-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/ISSUE_TEMPLATE/style_issue.md` & `cercis-0.1.7/.github/ISSUE_TEMPLATE/style_issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/check-changelog.yml` & `cercis-0.1.7/.github/workflows/check-changelog.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/diff_shades_comment.yml` & `cercis-0.1.7/.github/workflows/diff_shades_comment.yml`

 * *Files 5% similar despite different names*

```diff
@@ -37,13 +37,13 @@
         with:
           issue-number: ${{ steps.metadata.outputs.pr-number }}
           comment-author: "github-actions[bot]"
           body-includes: "diff-shades"
 
       - name: Create or update PR comment
         if: steps.metadata.outputs.needs-comment == 'true'
-        uses: peter-evans/create-or-update-comment@ca08ebd5dc95aa0cd97021e9708fcd6b87138c9b
+        uses: peter-evans/create-or-update-comment@c6c9a1a66007646a28c153e2a8580a5bad27bcfa
         with:
           comment-id: ${{ steps.find-comment.outputs.comment-id }}
           issue-number: ${{ steps.metadata.outputs.pr-number }}
           body: ${{ steps.metadata.outputs.comment-body }}
           edit-mode: replace
```

### Comparing `cercis-0.1.6/.github/workflows/docker.yml` & `cercis-0.1.7/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/fuzz.yml` & `cercis-0.1.7/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/lint.yml` & `cercis-0.1.7/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/python-package.yml` & `cercis-0.1.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/python-publish.yml` & `cercis-0.1.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/test.yml` & `cercis-0.1.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/upload_binary.yml` & `cercis-0.1.7/.github/workflows/upload_binary.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/.github/workflows/version-check.yml` & `cercis-0.1.7/.github/workflows/version-check.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/action/main.py` & `cercis-0.1.7/action/main.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/autoload/black.vim` & `cercis-0.1.7/autoload/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/gallery/README.md` & `cercis-0.1.7/gallery/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/gallery/gallery.py` & `cercis-0.1.7/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/plugin/black.vim` & `cercis-0.1.7/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/scripts/check_version_and_changelog.py` & `cercis-0.1.7/scripts/check_version_and_changelog.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/scripts/diff_shades_gha_helper.py` & `cercis-0.1.7/scripts/diff_shades_gha_helper.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/scripts/fuzz.py` & `cercis-0.1.7/scripts/fuzz.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/scripts/make_width_table.py` & `cercis-0.1.7/scripts/make_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/scripts/migrate-black.py` & `cercis-0.1.7/scripts/migrate-black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blackd/__init__.py` & `cercis-0.1.7/src/blackd/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import logging
 from concurrent.futures import Executor, ProcessPoolExecutor
-from datetime import datetime
+from datetime import datetime, timezone
 from functools import partial
 from multiprocessing import freeze_support
 from typing import Set, Tuple
 
 try:
     from aiohttp import web
 
@@ -55,17 +55,23 @@
 
 class InvalidVariantHeader(Exception):
     pass
 
 
 @click.command(context_settings={"help_option_names": ["-h", "--help"]})
 @click.option(
-    "--bind-host", type=str, help="Address to bind the server to.", default="localhost"
+    "--bind-host",
+    type=str,
+    help="Address to bind the server to.",
+    default="localhost",
+    show_default=True,
+)
+@click.option(
+    "--bind-port", type=int, help="Port to listen on", default=45484, show_default=True
 )
-@click.option("--bind-port", type=int, help="Port to listen on", default=45484)
 @click.version_option(version=cercis.__version__)
 def main(bind_host: str, bind_port: int) -> None:
     logging.basicConfig(level=logging.INFO)
     app = make_app()
     ver = cercis.__version__
     cercis.out(f"blackd version {ver} listening on {bind_host} port {bind_port}")
     web.run_app(app, host=bind_host, port=bind_port, handle_signals=True, print=None)
@@ -128,15 +134,15 @@
             string_normalization=not skip_string_normalization,
             magic_trailing_comma=not skip_magic_trailing_comma,
             preview=preview,
         )
         req_bytes = await request.content.read()
         charset = request.charset if request.charset is not None else "utf8"
         req_str = req_bytes.decode(charset)
-        then = datetime.utcnow()
+        then = datetime.now(timezone.utc)
 
         header = ""
         if skip_source_first_line:
             first_newline_position: int = req_str.find("\n") + 1
             header = req_str[:first_newline_position]
             req_str = req_str[first_newline_position:]
 
@@ -156,17 +162,17 @@
         # Put the source first line back
         req_str = header + req_str
         formatted_str = header + formatted_str
 
         # Only output the diff in the HTTP response
         only_diff = bool(request.headers.get(DIFF_HEADER, False))
         if only_diff:
-            now = datetime.utcnow()
-            src_name = f"In\t{then} +0000"
-            dst_name = f"Out\t{now} +0000"
+            now = datetime.now(timezone.utc)
+            src_name = f"In\t{then}"
+            dst_name = f"Out\t{now}"
             loop = asyncio.get_event_loop()
             formatted_str = await loop.run_in_executor(
                 executor,
                 partial(cercis.diff, req_str, formatted_str, src_name, dst_name),
             )
 
         return web.Response(
```

### Comparing `cercis-0.1.6/src/blackd/middlewares.py` & `cercis-0.1.7/src/blackd/middlewares.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/Grammar.txt` & `cercis-0.1.7/src/blib2to3/Grammar.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,25 @@
 #	single_input is a single interactive statement;
 #	eval_input is the input for the eval() and input() functions.
 # NB: compound_stmt in single_input is followed by extra NEWLINE!
 file_input: (NEWLINE | stmt)* ENDMARKER
 single_input: NEWLINE | simple_stmt | compound_stmt NEWLINE
 eval_input: testlist NEWLINE* ENDMARKER
 
+typevar: NAME [':' expr]
+paramspec: '**' NAME
+typevartuple: '*' NAME
+typeparam: typevar | paramspec | typevartuple
+typeparams: '[' typeparam (',' typeparam)* [','] ']'
+
 decorator: '@' namedexpr_test NEWLINE
 decorators: decorator+
 decorated: decorators (classdef | funcdef | async_funcdef)
 async_funcdef: ASYNC funcdef
-funcdef: 'def' NAME parameters ['->' test] ':' suite
+funcdef: 'def' NAME [typeparams] parameters ['->' test] ':' suite
 parameters: '(' [typedargslist] ')'
 
 # The following definition for typedarglist is equivalent to this set of rules:
 #
 #     arguments = argument (',' argument)*
 #     argument = tfpdef ['=' test]
 #     kwargs = '**' tname [',']
@@ -70,15 +76,15 @@
 
 vname: NAME
 vfpdef: vname | '(' vfplist ')'
 vfplist: vfpdef (',' vfpdef)* [',']
 
 stmt: simple_stmt | compound_stmt
 simple_stmt: small_stmt (';' small_stmt)* [';'] NEWLINE
-small_stmt: (expr_stmt | print_stmt  | del_stmt | pass_stmt | flow_stmt |
+small_stmt: (type_stmt | expr_stmt | print_stmt  | del_stmt | pass_stmt | flow_stmt |
              import_stmt | global_stmt | exec_stmt | assert_stmt)
 expr_stmt: testlist_star_expr (annassign | augassign (yield_expr|testlist) |
                      ('=' (yield_expr|testlist_star_expr))*)
 annassign: ':' test ['=' (yield_expr|testlist_star_expr)]
 testlist_star_expr: (test|star_expr) (',' (test|star_expr))* [',']
 augassign: ('+=' | '-=' | '*=' | '@=' | '/=' | '%=' | '&=' | '|=' | '^=' |
             '<<=' | '>>=' | '**=' | '//=')
@@ -101,14 +107,15 @@
 dotted_as_name: dotted_name ['as' NAME]
 import_as_names: import_as_name (',' import_as_name)* [',']
 dotted_as_names: dotted_as_name (',' dotted_as_name)*
 dotted_name: NAME ('.' NAME)*
 global_stmt: ('global' | 'nonlocal') NAME (',' NAME)*
 exec_stmt: 'exec' expr ['in' test [',' test]]
 assert_stmt: 'assert' test [',' test]
+type_stmt: "type" NAME [typeparams] '=' expr
 
 compound_stmt: if_stmt | while_stmt | for_stmt | try_stmt | with_stmt | funcdef | classdef | decorated | async_stmt | match_stmt
 async_stmt: ASYNC (funcdef | with_stmt | for_stmt)
 if_stmt: 'if' namedexpr_test ':' suite ('elif' namedexpr_test ':' suite)* ['else' ':' suite]
 while_stmt: 'while' namedexpr_test ':' suite ['else' ':' suite]
 for_stmt: 'for' exprlist 'in' testlist_star_expr ':' suite ['else' ':' suite]
 try_stmt: ('try' ':' suite
@@ -170,15 +177,15 @@
 exprlist: (expr|star_expr) (',' (expr|star_expr))* [',']
 testlist: test (',' test)* [',']
 dictsetmaker: ( ((test ':' asexpr_test | '**' expr)
                  (comp_for | (',' (test ':' asexpr_test | '**' expr))* [','])) |
                 ((test [':=' test] | star_expr)
 		 (comp_for | (',' (test [':=' test] | star_expr))* [','])) )
 
-classdef: 'class' NAME ['(' [arglist] ')'] ':' suite
+classdef: 'class' NAME [typeparams] ['(' [arglist] ')'] ':' suite
 
 arglist: argument (',' argument)* [',']
 
 # "test '=' test" is really "keyword '=' test", but we have no such token.
 # These need to be in a single rule to avoid grammar that is ambiguous
 # to our LL(1) parser. Even though 'test' includes '*expr' in star_expr,
 # we explicitly match '*' here, too, to give it proper precedence.
```

### Comparing `cercis-0.1.6/src/blib2to3/LICENSE` & `cercis-0.1.7/src/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/PatternGrammar.txt` & `cercis-0.1.7/src/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/README` & `cercis-0.1.7/src/blib2to3/README`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pygram.py` & `cercis-0.1.7/src/blib2to3/pygram.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     old_comp_for: int
     old_comp_if: int
     old_comp_iter: int
     old_lambdef: int
     old_test: int
     or_test: int
     parameters: int
+    paramspec: int
     pass_stmt: int
     pattern: int
     patterns: int
     power: int
     print_stmt: int
     raise_stmt: int
     return_stmt: int
@@ -122,15 +123,20 @@
     testlist_star_expr: int
     tfpdef: int
     tfplist: int
     tname: int
     tname_star: int
     trailer: int
     try_stmt: int
+    type_stmt: int
     typedargslist: int
+    typeparam: int
+    typeparams: int
+    typevar: int
+    typevartuple: int
     varargslist: int
     vfpdef: int
     vfplist: int
     vname: int
     while_stmt: int
     with_stmt: int
     xor_expr: int
```

### Comparing `cercis-0.1.6/src/blib2to3/pytree.py` & `cercis-0.1.7/src/blib2to3/pytree.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/conv.py` & `cercis-0.1.7/src/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/driver.py` & `cercis-0.1.7/src/blib2to3/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/grammar.py` & `cercis-0.1.7/src/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/literals.py` & `cercis-0.1.7/src/blib2to3/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/parse.py` & `cercis-0.1.7/src/blib2to3/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/pgen.py` & `cercis-0.1.7/src/blib2to3/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/token.py` & `cercis-0.1.7/src/blib2to3/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/blib2to3/pgen2/tokenize.py` & `cercis-0.1.7/src/blib2to3/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/__init__.py` & `cercis-0.1.7/src/cercis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import platform
 import re
 import sys
 import tokenize
 import traceback
 from contextlib import contextmanager
 from dataclasses import replace
-from datetime import datetime
+from datetime import datetime, timezone
 from enum import Enum
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import (
     Any,
     Dict,
     Generator,
@@ -986,15 +986,15 @@
     `mode` and `fast` options are passed to :func:`format_file_contents`.
     """
     if src.suffix == ".pyi":
         mode = replace(mode, is_pyi=True)
     elif src.suffix == ".ipynb":
         mode = replace(mode, is_ipynb=True)
 
-    then = datetime.utcfromtimestamp(src.stat().st_mtime)
+    then = datetime.fromtimestamp(src.stat().st_mtime, timezone.utc)
     header = b""
     with open(src, "rb") as buf:
         if mode.skip_source_first_line:
             header = buf.readline()
         src_contents, encoding, newline = decode_bytes(buf.read())
     try:
         dst_contents = format_file_contents(src_contents, fast=fast, mode=mode)
@@ -1007,17 +1007,17 @@
     src_contents = header.decode(encoding) + src_contents
     dst_contents = header.decode(encoding) + dst_contents
 
     if write_back == WriteBack.YES:
         with open(src, "w", encoding=encoding, newline=newline) as f:
             f.write(dst_contents)
     elif write_back in (WriteBack.DIFF, WriteBack.COLOR_DIFF):
-        now = datetime.utcnow()
-        src_name = f"{src}\t{then} +0000"
-        dst_name = f"{src}\t{now} +0000"
+        now = datetime.now(timezone.utc)
+        src_name = f"{src}\t{then}"
+        dst_name = f"{src}\t{now}"
         if mode.is_ipynb:
             diff_contents = ipynb_diff(src_contents, dst_contents, src_name, dst_name)
         else:
             diff_contents = diff(src_contents, dst_contents, src_name, dst_name)
 
         if write_back == WriteBack.COLOR_DIFF:
             diff_contents = color_diff(diff_contents)
@@ -1047,15 +1047,15 @@
 
     If content is None, it's read from sys.stdin.
 
     If `write_back` is YES, write reformatted code back to stdout. If it is DIFF,
     write a diff to stdout. The `mode` argument is passed to
     :func:`format_file_contents`.
     """
-    then = datetime.utcnow()
+    then = datetime.now(timezone.utc)
 
     if content is None:
         src, encoding, newline = decode_bytes(sys.stdin.buffer.read())
     else:
         src, encoding, newline = content, "utf-8", ""
 
     dst = src
@@ -1072,17 +1072,17 @@
         )
         if write_back == WriteBack.YES:
             # Make sure there's a newline after the content
             if dst and dst[-1] != "\n":
                 dst += "\n"
             f.write(dst)
         elif write_back in (WriteBack.DIFF, WriteBack.COLOR_DIFF):
-            now = datetime.utcnow()
-            src_name = f"STDIN\t{then} +0000"
-            dst_name = f"STDOUT\t{now} +0000"
+            now = datetime.now(timezone.utc)
+            src_name = f"STDIN\t{then}"
+            dst_name = f"STDOUT\t{now}"
             d = diff(src, dst, src_name, dst_name)
             if write_back == WriteBack.COLOR_DIFF:
                 d = color_diff(d)
                 f = wrap_stream_for_windows(f)
             f.write(d)
         f.detach()
 
@@ -1454,14 +1454,17 @@
         elif (
             n.type == syms.tname_star
             and len(n.children) == 3
             and n.children[2].type == syms.star_expr
         ):
             features.add(Feature.VARIADIC_GENERICS)
 
+        elif n.type in (syms.type_stmt, syms.typeparams):
+            features.add(Feature.TYPE_PARAMS)
+
     return features
 
 
 def detect_target_versions(
         node: Node, *, future_imports: Optional[Set[str]] = None
 ) -> Set[TargetVersion]:
     """Detect the version to target based on the nodes used."""
```

### Comparing `cercis-0.1.6/src/cercis/_width_table.py` & `cercis-0.1.7/src/cercis/_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/brackets.py` & `cercis-0.1.7/src/cercis/brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/cache.py` & `cercis-0.1.7/src/cercis/cache.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/comments.py` & `cercis-0.1.7/src/cercis/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/concurrency.py` & `cercis-0.1.7/src/cercis/concurrency.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/const.py` & `cercis-0.1.7/src/cercis/const.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/debug.py` & `cercis-0.1.7/src/cercis/debug.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/files.py` & `cercis-0.1.7/src/cercis/files.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/handle_ipynb_magics.py` & `cercis-0.1.7/src/cercis/handle_ipynb_magics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/indent.py` & `cercis-0.1.7/src/cercis/indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/linegen.py` & `cercis-0.1.7/src/cercis/linegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,14 +267,26 @@
         )
         for child in node.children:
             if is_name_token(child) and child.value in keywords:
                 yield from self.line()
 
             yield from self.visit(child)
 
+    def visit_typeparams(self, node: Node) -> Iterator[Line]:
+        yield from self.visit_default(node)
+        node.children[0].prefix = ""
+
+    def visit_typevartuple(self, node: Node) -> Iterator[Line]:
+        yield from self.visit_default(node)
+        node.children[1].prefix = ""
+
+    def visit_paramspec(self, node: Node) -> Iterator[Line]:
+        yield from self.visit_default(node)
+        node.children[1].prefix = ""
+
     def visit_dictsetmaker(self, node: Node) -> Iterator[Line]:
         if Preview.wrap_long_dict_values_in_parens in self.mode:
             for i, child in enumerate(node.children):
                 if i == 0:
                     continue
                 if node.children[i - 1].type == token.COLON:
                     if child.type == syms.atom and child.children[0].type == token.LPAR:
@@ -1026,14 +1038,21 @@
                     node.prev_sibling.type == RARROW
                     for node in (
                         leaves[0].parent,
                         getattr(leaves[0].parent, "parent", None),
                     )
                     if isinstance(node, Node) and isinstance(node.prev_sibling, Leaf)
                 )
+                # Except the false negatives above for PEP 604 unions where we
+                # can't add the comma.
+                and not (
+                    leaves[0].parent
+                    and leaves[0].parent.next_sibling
+                    and leaves[0].parent.next_sibling.type == token.VBAR
+                )
             )
 
             if original.is_import or no_commas:
                 for i in range(len(leaves) - 1, -1, -1):
                     if leaves[i].type == STANDALONE_COMMENT:
                         continue
```

### Comparing `cercis-0.1.6/src/cercis/lines.py` & `cercis-0.1.7/src/cercis/lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/mode.py` & `cercis-0.1.7/src/cercis/mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     PY35 = 5
     PY36 = 6
     PY37 = 7
     PY38 = 8
     PY39 = 9
     PY310 = 10
     PY311 = 11
+    PY312 = 12
 
 
 class Feature(Enum):
     F_STRINGS = 2
     NUMERIC_UNDERSCORES = 3
     TRAILING_COMMA_IN_CALL = 4
     TRAILING_COMMA_IN_DEF = 5
@@ -61,14 +62,15 @@
     PATTERN_MATCHING = 11
     UNPACKING_ON_FLOW = 12
     ANN_ASSIGN_EXTENDED_RHS = 13
     EXCEPT_STAR = 14
     VARIADIC_GENERICS = 15
     DEBUG_F_STRINGS = 16
     PARENTHESIZED_CONTEXT_MANAGERS = 17
+    TYPE_PARAMS = 18
     FORCE_OPTIONAL_PARENTHESES = 50
 
     # __future__ flags
     FUTURE_ANNOTATIONS = 51
 
 
 FUTURE_FLAG_TO_FEATURE: Final = {
@@ -153,14 +155,33 @@
         Feature.UNPACKING_ON_FLOW,
         Feature.ANN_ASSIGN_EXTENDED_RHS,
         Feature.PARENTHESIZED_CONTEXT_MANAGERS,
         Feature.PATTERN_MATCHING,
         Feature.EXCEPT_STAR,
         Feature.VARIADIC_GENERICS,
     },
+    TargetVersion.PY312: {
+        Feature.F_STRINGS,
+        Feature.DEBUG_F_STRINGS,
+        Feature.NUMERIC_UNDERSCORES,
+        Feature.TRAILING_COMMA_IN_CALL,
+        Feature.TRAILING_COMMA_IN_DEF,
+        Feature.ASYNC_KEYWORDS,
+        Feature.FUTURE_ANNOTATIONS,
+        Feature.ASSIGNMENT_EXPRESSIONS,
+        Feature.RELAXED_DECORATORS,
+        Feature.POS_ONLY_ARGUMENTS,
+        Feature.UNPACKING_ON_FLOW,
+        Feature.ANN_ASSIGN_EXTENDED_RHS,
+        Feature.PARENTHESIZED_CONTEXT_MANAGERS,
+        Feature.PATTERN_MATCHING,
+        Feature.EXCEPT_STAR,
+        Feature.VARIADIC_GENERICS,
+        Feature.TYPE_PARAMS,
+    },
 }
 
 
 def supports_feature(target_versions: Set[TargetVersion], feature: Feature) -> bool:
     return all(feature in VERSION_TO_FEATURES[version] for version in target_versions)
```

### Comparing `cercis-0.1.6/src/cercis/nodes.py` & `cercis-0.1.7/src/cercis/nodes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/numerics.py` & `cercis-0.1.7/src/cercis/numerics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/output.py` & `cercis-0.1.7/src/cercis/output.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/parsing.py` & `cercis-0.1.7/src/cercis/parsing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/report.py` & `cercis-0.1.7/src/cercis/report.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/rusty.py` & `cercis-0.1.7/src/cercis/rusty.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/strings.py` & `cercis-0.1.7/src/cercis/strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/trans.py` & `cercis-0.1.7/src/cercis/trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/utils_line_wrapping.py` & `cercis-0.1.7/src/cercis/utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/src/cercis/utils_linegen.py` & `cercis-0.1.7/src/cercis/utils_linegen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/optional.py` & `cercis-0.1.7/tests/optional.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/test_black.py` & `cercis-0.1.7/tests/test_black.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,16 +390,16 @@
 00001850: 653a 0a20 2020 2020 2020 2064 6966 665f  e:.        diff_
 00001860: 6865 6164 6572 203d 2072 652e 636f 6d70  header = re.comp
 00001870: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
 00001880: 2072 2228 5354 4449 4e7c 5354 444f 5554   r"(STDIN|STDOUT
 00001890: 295c 745c 645c 645c 645c 642d 5c64 5c64  )\t\d\d\d\d-\d\d
 000018a0: 2d5c 645c 6420 5c64 5c64 3a5c 645c 643a  -\d\d \d\d:\d\d:
 000018b0: 5c64 5c64 5c2e 5c64 5c64 5c64 5c64 5c64  \d\d\.\d\d\d\d\d
-000018c0: 5c64 2022 0a20 2020 2020 2020 2020 2020  \d ".           
-000018d0: 2072 225c 2b5c 645c 645c 645c 6422 0a20   r"\+\d\d\d\d". 
+000018c0: 5c64 220a 2020 2020 2020 2020 2020 2020  \d".            
+000018d0: 7222 5c2b 5c64 5c64 3a5c 645c 6422 0a20  r"\+\d\d:\d\d". 
 000018e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 000018f0: 2073 6f75 7263 652c 205f 203d 2072 6561   source, _ = rea
 00001900: 645f 6461 7461 2822 7369 6d70 6c65 5f63  d_data("simple_c
 00001910: 6173 6573 222c 2022 6578 7072 6573 7369  ases", "expressi
 00001920: 6f6e 2e70 7922 290a 2020 2020 2020 2020  on.py").        
 00001930: 6578 7065 6374 6564 2c20 5f20 3d20 7265  expected, _ = re
 00001940: 6164 5f64 6174 6128 2273 696d 706c 655f  ad_data("simple_
@@ -539,5791 +539,5842 @@
 000021a0: 2020 2020 2020 2076 6572 7369 6f6e 7320         versions 
 000021b0: 3d20 6365 7263 6973 2e64 6574 6563 745f  = cercis.detect_
 000021c0: 7461 7267 6574 5f76 6572 7369 6f6e 7328  target_versions(
 000021d0: 726f 6f74 290a 2020 2020 2020 2020 7365  root).        se
 000021e0: 6c66 2e61 7373 6572 7449 6e28 6365 7263  lf.assertIn(cerc
 000021f0: 6973 2e54 6172 6765 7456 6572 7369 6f6e  is.TargetVersion
 00002200: 2e50 5933 382c 2076 6572 7369 6f6e 7329  .PY38, versions)
-00002210: 0a0a 2020 2020 6465 6620 7465 7374 5f65  ..    def test_e
-00002220: 7870 7265 7373 696f 6e5f 6666 2873 656c  xpression_ff(sel
-00002230: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00002240: 2020 2020 736f 7572 6365 2c20 6578 7065      source, expe
-00002250: 6374 6564 203d 2072 6561 645f 6461 7461  cted = read_data
-00002260: 2822 7369 6d70 6c65 5f63 6173 6573 222c  ("simple_cases",
-00002270: 2022 6578 7072 6573 7369 6f6e 2e70 7922   "expression.py"
-00002280: 290a 2020 2020 2020 2020 746d 705f 6669  ).        tmp_fi
-00002290: 6c65 203d 2050 6174 6828 6365 7263 6973  le = Path(cercis
-000022a0: 2e64 756d 705f 746f 5f66 696c 6528 736f  .dump_to_file(so
-000022b0: 7572 6365 2929 0a20 2020 2020 2020 206d  urce)).        m
-000022c0: 6f64 6520 3d20 7265 706c 6163 6528 4445  ode = replace(DE
-000022d0: 4641 554c 545f 4d4f 4445 2c20 6c69 6e65  FAULT_MODE, line
-000022e0: 5f6c 656e 6774 683d 3838 290a 2020 2020  _length=88).    
-000022f0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00002300: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00002310: 5472 7565 2866 6628 746d 705f 6669 6c65  True(ff(tmp_file
-00002320: 2c20 7772 6974 655f 6261 636b 3d63 6572  , write_back=cer
-00002330: 6369 732e 5772 6974 6542 6163 6b2e 5945  cis.WriteBack.YE
-00002340: 532c 206d 6f64 653d 6d6f 6465 2929 0a20  S, mode=mode)). 
-00002350: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00002360: 6f70 656e 2874 6d70 5f66 696c 652c 2065  open(tmp_file, e
-00002370: 6e63 6f64 696e 673d 2275 7466 3822 2920  ncoding="utf8") 
-00002380: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
-00002390: 2020 2020 2020 6163 7475 616c 203d 2066        actual = f
-000023a0: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
-000023b0: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
-000023c0: 2020 2020 206f 732e 756e 6c69 6e6b 2874       os.unlink(t
-000023d0: 6d70 5f66 696c 6529 0a20 2020 2020 2020  mp_file).       
-000023e0: 2073 656c 662e 6173 7365 7274 466f 726d   self.assertForm
-000023f0: 6174 4571 7561 6c28 6578 7065 6374 6564  atEqual(expected
-00002400: 2c20 6163 7475 616c 290a 2020 2020 2020  , actual).      
-00002410: 2020 7769 7468 2070 6174 6368 2822 6365    with patch("ce
-00002420: 7263 6973 2e64 756d 705f 746f 5f66 696c  rcis.dump_to_fil
-00002430: 6522 2c20 6475 6d70 5f74 6f5f 7374 6465  e", dump_to_stde
-00002440: 7272 293a 0a20 2020 2020 2020 2020 2020  rr):.           
-00002450: 2063 6572 6369 732e 6173 7365 7274 5f65   cercis.assert_e
-00002460: 7175 6976 616c 656e 7428 736f 7572 6365  quivalent(source
-00002470: 2c20 6163 7475 616c 290a 2020 2020 2020  , actual).      
-00002480: 2020 2020 2020 6365 7263 6973 2e61 7373        cercis.ass
-00002490: 6572 745f 7374 6162 6c65 2873 6f75 7263  ert_stable(sourc
-000024a0: 652c 2061 6374 7561 6c2c 206d 6f64 6529  e, actual, mode)
-000024b0: 0a0a 2020 2020 6465 6620 7465 7374 5f65  ..    def test_e
-000024c0: 7870 7265 7373 696f 6e5f 6469 6666 2873  xpression_diff(s
-000024d0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-000024e0: 2020 2020 2020 736f 7572 6365 2c20 5f20        source, _ 
-000024f0: 3d20 7265 6164 5f64 6174 6128 2273 696d  = read_data("sim
-00002500: 706c 655f 6361 7365 7322 2c20 2265 7870  ple_cases", "exp
-00002510: 7265 7373 696f 6e2e 7079 2229 0a20 2020  ression.py").   
-00002520: 2020 2020 2065 7870 6563 7465 642c 205f       expected, _
-00002530: 203d 2072 6561 645f 6461 7461 2822 7369   = read_data("si
-00002540: 6d70 6c65 5f63 6173 6573 222c 2022 6578  mple_cases", "ex
-00002550: 7072 6573 7369 6f6e 2e64 6966 6622 290a  pression.diff").
-00002560: 2020 2020 2020 2020 746d 705f 6669 6c65          tmp_file
-00002570: 203d 2050 6174 6828 6365 7263 6973 2e64   = Path(cercis.d
-00002580: 756d 705f 746f 5f66 696c 6528 736f 7572  ump_to_file(sour
-00002590: 6365 2929 0a20 2020 2020 2020 2064 6966  ce)).        dif
-000025a0: 665f 6865 6164 6572 203d 2072 652e 636f  f_header = re.co
-000025b0: 6d70 696c 6528 0a20 2020 2020 2020 2020  mpile(.         
-000025c0: 2020 2072 6622 7b72 652e 6573 6361 7065     rf"{re.escape
-000025d0: 2873 7472 2874 6d70 5f66 696c 6529 297d  (str(tmp_file))}
-000025e0: 5c74 5c64 5c64 5c64 5c64 2d5c 645c 642d  \t\d\d\d\d-\d\d-
-000025f0: 5c64 5c64 2022 0a20 2020 2020 2020 2020  \d\d ".         
-00002600: 2020 2072 225c 645c 643a 5c64 5c64 3a5c     r"\d\d:\d\d:\
-00002610: 645c 645c 2e5c 645c 645c 645c 645c 645c  d\d\.\d\d\d\d\d\
-00002620: 6420 5c2b 5c64 5c64 5c64 5c64 220a 2020  d \+\d\d\d\d".  
-00002630: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002640: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00002650: 2072 6573 756c 7420 3d20 426c 6163 6b52   result = BlackR
-00002660: 756e 6e65 7228 292e 696e 766f 6b65 280a  unner().invoke(.
-00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002680: 6365 7263 6973 2e6d 6169 6e2c 0a20 2020  cercis.main,.   
-00002690: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
-000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026b0: 2020 2022 2d2d 6469 6666 222c 0a20 2020     "--diff",.   
-000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026d0: 2073 7472 2874 6d70 5f66 696c 6529 2c0a   str(tmp_file),.
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 6622 2d2d 636f 6e66 6967 3d7b      f"--config={
-00002700: 454d 5054 595f 434f 4e46 4947 7d22 2c0a  EMPTY_CONFIG}",.
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2020 222d 2d6c 696e 652d 6c65 6e67      "--line-leng
-00002730: 7468 3d38 3822 2c0a 2020 2020 2020 2020  th=88",.        
-00002740: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00002750: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00002760: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00002770: 4571 7561 6c28 7265 7375 6c74 2e65 7869  Equal(result.exi
-00002780: 745f 636f 6465 2c20 3029 0a20 2020 2020  t_code, 0).     
-00002790: 2020 2066 696e 616c 6c79 3a0a 2020 2020     finally:.    
-000027a0: 2020 2020 2020 2020 6f73 2e75 6e6c 696e          os.unlin
-000027b0: 6b28 746d 705f 6669 6c65 290a 2020 2020  k(tmp_file).    
-000027c0: 2020 2020 6163 7475 616c 203d 2072 6573      actual = res
-000027d0: 756c 742e 6f75 7470 7574 0a20 2020 2020  ult.output.     
-000027e0: 2020 2061 6374 7561 6c20 3d20 6469 6666     actual = diff
-000027f0: 5f68 6561 6465 722e 7375 6228 4445 5445  _header.sub(DETE
-00002800: 524d 494e 4953 5449 435f 4845 4144 4552  RMINISTIC_HEADER
-00002810: 2c20 6163 7475 616c 290a 2020 2020 2020  , actual).      
-00002820: 2020 6966 2065 7870 6563 7465 6420 213d    if expected !=
-00002830: 2061 6374 7561 6c3a 0a20 2020 2020 2020   actual:.       
-00002840: 2020 2020 2064 756d 7020 3d20 6365 7263       dump = cerc
-00002850: 6973 2e64 756d 705f 746f 5f66 696c 6528  is.dump_to_file(
-00002860: 6163 7475 616c 290a 2020 2020 2020 2020  actual).        
-00002870: 2020 2020 6d73 6720 3d20 280a 2020 2020      msg = (.    
-00002880: 2020 2020 2020 2020 2020 2020 2245 7870              "Exp
-00002890: 6563 7465 6420 6469 6666 2069 736e 2774  ected diff isn't
-000028a0: 2065 7175 616c 2074 6f20 7468 6520 6163   equal to the ac
-000028b0: 7475 616c 2e20 4966 2079 6f75 206d 6164  tual. If you mad
-000028c0: 6520 6368 616e 6765 7320 746f 220a 2020  e changes to".  
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2220                " 
-000028e0: 6578 7072 6573 7369 6f6e 2e70 7920 616e  expression.py an
-000028f0: 6420 7468 6973 2069 7320 616e 2061 6e74  d this is an ant
-00002900: 6963 6970 6174 6564 2064 6966 6665 7265  icipated differe
-00002910: 6e63 652c 206f 7665 7277 7269 7465 220a  nce, overwrite".
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 6622 2074 6573 7473 2f64 6174 612f 6578  f" tests/data/ex
-00002940: 7072 6573 7369 6f6e 2e64 6966 6620 7769  pression.diff wi
-00002950: 7468 207b 6475 6d70 7d22 0a20 2020 2020  th {dump}".     
-00002960: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00002970: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00002980: 4571 7561 6c28 6578 7065 6374 6564 2c20  Equal(expected, 
-00002990: 6163 7475 616c 2c20 6d73 6729 0a0a 2020  actual, msg)..  
-000029a0: 2020 6465 6620 7465 7374 5f65 7870 7265    def test_expre
-000029b0: 7373 696f 6e5f 6469 6666 5f77 6974 685f  ssion_diff_with_
-000029c0: 636f 6c6f 7228 7365 6c66 2920 2d3e 204e  color(self) -> N
-000029d0: 6f6e 653a 0a20 2020 2020 2020 2073 6f75  one:.        sou
-000029e0: 7263 652c 205f 203d 2072 6561 645f 6461  rce, _ = read_da
-000029f0: 7461 2822 7369 6d70 6c65 5f63 6173 6573  ta("simple_cases
-00002a00: 222c 2022 6578 7072 6573 7369 6f6e 2e70  ", "expression.p
-00002a10: 7922 290a 2020 2020 2020 2020 6578 7065  y").        expe
-00002a20: 6374 6564 2c20 5f20 3d20 7265 6164 5f64  cted, _ = read_d
-00002a30: 6174 6128 2273 696d 706c 655f 6361 7365  ata("simple_case
-00002a40: 7322 2c20 2265 7870 7265 7373 696f 6e2e  s", "expression.
-00002a50: 6469 6666 2229 0a20 2020 2020 2020 2074  diff").        t
-00002a60: 6d70 5f66 696c 6520 3d20 5061 7468 2863  mp_file = Path(c
-00002a70: 6572 6369 732e 6475 6d70 5f74 6f5f 6669  ercis.dump_to_fi
-00002a80: 6c65 2873 6f75 7263 6529 290a 2020 2020  le(source)).    
-00002a90: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00002aa0: 2020 2020 2072 6573 756c 7420 3d20 426c       result = Bl
-00002ab0: 6163 6b52 756e 6e65 7228 292e 696e 766f  ackRunner().invo
-00002ac0: 6b65 280a 2020 2020 2020 2020 2020 2020  ke(.            
-00002ad0: 2020 2020 6365 7263 6973 2e6d 6169 6e2c      cercis.main,
-00002ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002af0: 205b 222d 2d64 6966 6622 2c20 222d 2d63   ["--diff", "--c
-00002b00: 6f6c 6f72 222c 2073 7472 2874 6d70 5f66  olor", str(tmp_f
-00002b10: 696c 6529 2c20 6622 2d2d 636f 6e66 6967  ile), f"--config
-00002b20: 3d7b 454d 5054 595f 434f 4e46 4947 7d22  ={EMPTY_CONFIG}"
-00002b30: 5d2c 0a20 2020 2020 2020 2020 2020 2029  ],.            )
-00002b40: 0a20 2020 2020 2020 2066 696e 616c 6c79  .        finally
-00002b50: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
-00002b60: 2e75 6e6c 696e 6b28 746d 705f 6669 6c65  .unlink(tmp_file
-00002b70: 290a 2020 2020 2020 2020 6163 7475 616c  ).        actual
-00002b80: 203d 2072 6573 756c 742e 6f75 7470 7574   = result.output
-00002b90: 0a20 2020 2020 2020 2023 2057 6520 6368  .        # We ch
-00002ba0: 6563 6b20 7468 6520 636f 6e74 656e 7473  eck the contents
-00002bb0: 206f 6620 7468 6520 6469 6666 2069 6e20   of the diff in 
-00002bc0: 6074 6573 745f 6578 7072 6573 7369 6f6e  `test_expression
-00002bd0: 5f64 6966 6660 2e20 416c 6c0a 2020 2020  _diff`. All.    
-00002be0: 2020 2020 2320 7765 206e 6565 6420 746f      # we need to
-00002bf0: 2063 6865 636b 2068 6572 6520 6973 2074   check here is t
-00002c00: 6861 7420 636f 6c6f 7220 636f 6465 7320  hat color codes 
-00002c10: 6578 6973 7420 696e 2074 6865 2072 6573  exist in the res
-00002c20: 756c 742e 0a20 2020 2020 2020 2073 656c  ult..        sel
-00002c30: 662e 6173 7365 7274 496e 2822 5c30 3333  f.assertIn("\033
-00002c40: 5b31 6d22 2c20 6163 7475 616c 290a 2020  [1m", actual).  
-00002c50: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00002c60: 7449 6e28 225c 3033 335b 3336 6d22 2c20  tIn("\033[36m", 
-00002c70: 6163 7475 616c 290a 2020 2020 2020 2020  actual).        
-00002c80: 7365 6c66 2e61 7373 6572 7449 6e28 225c  self.assertIn("\
-00002c90: 3033 335b 3332 6d22 2c20 6163 7475 616c  033[32m", actual
-00002ca0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00002cb0: 7373 6572 7449 6e28 225c 3033 335b 3331  ssertIn("\033[31
-00002cc0: 6d22 2c20 6163 7475 616c 290a 2020 2020  m", actual).    
-00002cd0: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
-00002ce0: 6e28 225c 3033 335b 306d 222c 2061 6374  n("\033[0m", act
-00002cf0: 7561 6c29 0a0a 2020 2020 6465 6620 7465  ual)..    def te
-00002d00: 7374 5f64 6574 6563 745f 706f 735f 6f6e  st_detect_pos_on
-00002d10: 6c79 5f61 7267 756d 656e 7473 2873 656c  ly_arguments(sel
-00002d20: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00002d30: 2020 2020 736f 7572 6365 2c20 5f20 3d20      source, _ = 
-00002d40: 7265 6164 5f64 6174 6128 2270 795f 3338  read_data("py_38
-00002d50: 222c 2022 7065 705f 3537 3022 290a 2020  ", "pep_570").  
-00002d60: 2020 2020 2020 726f 6f74 203d 2063 6572        root = cer
-00002d70: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
-00002d80: 6528 736f 7572 6365 290a 2020 2020 2020  e(source).      
-00002d90: 2020 6665 6174 7572 6573 203d 2063 6572    features = cer
-00002da0: 6369 732e 6765 745f 6665 6174 7572 6573  cis.get_features
-00002db0: 5f75 7365 6428 726f 6f74 290a 2020 2020  _used(root).    
-00002dc0: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
-00002dd0: 6e28 6365 7263 6973 2e46 6561 7475 7265  n(cercis.Feature
-00002de0: 2e50 4f53 5f4f 4e4c 595f 4152 4755 4d45  .POS_ONLY_ARGUME
-00002df0: 4e54 532c 2066 6561 7475 7265 7329 0a20  NTS, features). 
-00002e00: 2020 2020 2020 2076 6572 7369 6f6e 7320         versions 
-00002e10: 3d20 6365 7263 6973 2e64 6574 6563 745f  = cercis.detect_
-00002e20: 7461 7267 6574 5f76 6572 7369 6f6e 7328  target_versions(
-00002e30: 726f 6f74 290a 2020 2020 2020 2020 7365  root).        se
-00002e40: 6c66 2e61 7373 6572 7449 6e28 6365 7263  lf.assertIn(cerc
-00002e50: 6973 2e54 6172 6765 7456 6572 7369 6f6e  is.TargetVersion
-00002e60: 2e50 5933 382c 2076 6572 7369 6f6e 7329  .PY38, versions)
-00002e70: 0a0a 2020 2020 6465 6620 7465 7374 5f64  ..    def test_d
-00002e80: 6574 6563 745f 6465 6275 675f 665f 7374  etect_debug_f_st
-00002e90: 7269 6e67 7328 7365 6c66 2920 2d3e 204e  rings(self) -> N
-00002ea0: 6f6e 653a 0a20 2020 2020 2020 2072 6f6f  one:.        roo
-00002eb0: 7420 3d20 6365 7263 6973 2e6c 6962 3274  t = cercis.lib2t
-00002ec0: 6f33 5f70 6172 7365 2822 2222 6622 7b78  o3_parse("""f"{x
-00002ed0: 3d7d 2220 2222 2229 0a20 2020 2020 2020  =}" """).       
-00002ee0: 2066 6561 7475 7265 7320 3d20 6365 7263   features = cerc
-00002ef0: 6973 2e67 6574 5f66 6561 7475 7265 735f  is.get_features_
-00002f00: 7573 6564 2872 6f6f 7429 0a20 2020 2020  used(root).     
-00002f10: 2020 2073 656c 662e 6173 7365 7274 496e     self.assertIn
-00002f20: 2863 6572 6369 732e 4665 6174 7572 652e  (cercis.Feature.
-00002f30: 4445 4255 475f 465f 5354 5249 4e47 532c  DEBUG_F_STRINGS,
-00002f40: 2066 6561 7475 7265 7329 0a20 2020 2020   features).     
-00002f50: 2020 2076 6572 7369 6f6e 7320 3d20 6365     versions = ce
-00002f60: 7263 6973 2e64 6574 6563 745f 7461 7267  rcis.detect_targ
-00002f70: 6574 5f76 6572 7369 6f6e 7328 726f 6f74  et_versions(root
-00002f80: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00002f90: 7373 6572 7449 6e28 6365 7263 6973 2e54  ssertIn(cercis.T
-00002fa0: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
-00002fb0: 382c 2076 6572 7369 6f6e 7329 0a0a 2020  8, versions)..  
-00002fc0: 2020 2020 2020 726f 6f74 203d 2063 6572        root = cer
-00002fd0: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
-00002fe0: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00002ff0: 2222 6622 7b78 7d22 5c6e 6627 7b22 3d22  ""f"{x}"\nf'{"="
-00003000: 7d27 5c6e 6627 7b28 783a 3d35 297d 275c  }'\nf'{(x:=5)}'\
-00003010: 6e66 277b 6628 613d 2233 3d22 297d 275c  nf'{f(a="3=")}'\
-00003020: 6e66 277b 783a 3d31 307d 275c 6e22 2222  nf'{x:=10}'\n"""
-00003030: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00003040: 2020 2066 6561 7475 7265 7320 3d20 6365     features = ce
-00003050: 7263 6973 2e67 6574 5f66 6561 7475 7265  rcis.get_feature
-00003060: 735f 7573 6564 2872 6f6f 7429 0a20 2020  s_used(root).   
-00003070: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00003080: 4e6f 7449 6e28 6365 7263 6973 2e46 6561  NotIn(cercis.Fea
-00003090: 7475 7265 2e44 4542 5547 5f46 5f53 5452  ture.DEBUG_F_STR
-000030a0: 494e 4753 2c20 6665 6174 7572 6573 290a  INGS, features).
-000030b0: 0a20 2020 2020 2020 2023 2057 6520 646f  .        # We do
-000030c0: 6e27 7420 7965 7420 7375 7070 6f72 7420  n't yet support 
-000030d0: 6665 6174 7572 6520 7665 7273 696f 6e20  feature version 
-000030e0: 6465 7465 6374 696f 6e20 696e 206e 6573  detection in nes
-000030f0: 7465 6420 662d 7374 7269 6e67 730a 2020  ted f-strings.  
-00003100: 2020 2020 2020 726f 6f74 203d 2063 6572        root = cer
-00003110: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
-00003120: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00003130: 2222 6622 6865 6172 6420 6120 7275 6d6f  ""f"heard a rumo
-00003140: 7572 2074 6861 7420 7b20 6627 7b31 2b31  ur that { f'{1+1
-00003150: 3d7d 2720 7d20 2e2e 2e20 7365 656d 7320  =}' } ... seems 
-00003160: 6c69 6b65 2069 7420 636f 756c 6420 6265  like it could be
-00003170: 2074 7275 6522 2022 2222 0a20 2020 2020   true" """.     
-00003180: 2020 2029 0a20 2020 2020 2020 2066 6561     ).        fea
-00003190: 7475 7265 7320 3d20 6365 7263 6973 2e67  tures = cercis.g
-000031a0: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
-000031b0: 2872 6f6f 7429 0a20 2020 2020 2020 2073  (root).        s
-000031c0: 656c 662e 6173 7365 7274 4e6f 7449 6e28  elf.assertNotIn(
-000031d0: 6365 7263 6973 2e46 6561 7475 7265 2e44  cercis.Feature.D
-000031e0: 4542 5547 5f46 5f53 5452 494e 4753 2c20  EBUG_F_STRINGS, 
-000031f0: 6665 6174 7572 6573 290a 0a20 2020 2040  features)..    @
-00003200: 7061 7463 6828 2263 6572 6369 732e 6475  patch("cercis.du
-00003210: 6d70 5f74 6f5f 6669 6c65 222c 2064 756d  mp_to_file", dum
-00003220: 705f 746f 5f73 7464 6572 7229 0a20 2020  p_to_stderr).   
-00003230: 2064 6566 2074 6573 745f 7374 7269 6e67   def test_string
-00003240: 5f71 756f 7465 7328 7365 6c66 2920 2d3e  _quotes(self) ->
-00003250: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-00003260: 6f75 7263 652c 2065 7870 6563 7465 6420  ource, expected 
-00003270: 3d20 7265 6164 5f64 6174 6128 226d 6973  = read_data("mis
-00003280: 6365 6c6c 616e 656f 7573 222c 2022 7374  cellaneous", "st
-00003290: 7269 6e67 5f71 756f 7465 7322 290a 2020  ring_quotes").  
-000032a0: 2020 2020 2020 6d6f 6465 203d 2063 6572        mode = cer
-000032b0: 6369 732e 4d6f 6465 2870 7265 7669 6577  cis.Mode(preview
-000032c0: 3d54 7275 652c 2073 696e 676c 655f 7175  =True, single_qu
-000032d0: 6f74 653d 4661 6c73 6529 0a20 2020 2020  ote=False).     
-000032e0: 2020 2061 7373 6572 745f 666f 726d 6174     assert_format
-000032f0: 2873 6f75 7263 652c 2065 7870 6563 7465  (source, expecte
-00003300: 642c 206d 6f64 6529 0a20 2020 2020 2020  d, mode).       
-00003310: 206d 6f64 6520 3d20 7265 706c 6163 6528   mode = replace(
-00003320: 6d6f 6465 2c20 7374 7269 6e67 5f6e 6f72  mode, string_nor
-00003330: 6d61 6c69 7a61 7469 6f6e 3d46 616c 7365  malization=False
-00003340: 290a 2020 2020 2020 2020 6e6f 745f 6e6f  ).        not_no
-00003350: 726d 616c 697a 6564 203d 2066 7328 736f  rmalized = fs(so
-00003360: 7572 6365 2c20 6d6f 6465 3d6d 6f64 6529  urce, mode=mode)
-00003370: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00003380: 7365 7274 466f 726d 6174 4571 7561 6c28  sertFormatEqual(
-00003390: 736f 7572 6365 2e72 6570 6c61 6365 2822  source.replace("
-000033a0: 5c5c 5c6e 222c 2022 2229 2c20 6e6f 745f  \\\n", ""), not_
-000033b0: 6e6f 726d 616c 697a 6564 290a 2020 2020  normalized).    
-000033c0: 2020 2020 6365 7263 6973 2e61 7373 6572      cercis.asser
-000033d0: 745f 6571 7569 7661 6c65 6e74 2873 6f75  t_equivalent(sou
-000033e0: 7263 652c 206e 6f74 5f6e 6f72 6d61 6c69  rce, not_normali
-000033f0: 7a65 6429 0a20 2020 2020 2020 2063 6572  zed).        cer
-00003400: 6369 732e 6173 7365 7274 5f73 7461 626c  cis.assert_stabl
-00003410: 6528 736f 7572 6365 2c20 6e6f 745f 6e6f  e(source, not_no
-00003420: 726d 616c 697a 6564 2c20 6d6f 6465 3d6d  rmalized, mode=m
-00003430: 6f64 6529 0a0a 2020 2020 6465 6620 7465  ode)..    def te
-00003440: 7374 5f73 6b69 705f 736f 7572 6365 5f66  st_skip_source_f
-00003450: 6972 7374 5f6c 696e 6528 7365 6c66 2920  irst_line(self) 
-00003460: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00003470: 2073 6f75 7263 652c 205f 203d 2072 6561   source, _ = rea
-00003480: 645f 6461 7461 2822 6d69 7363 656c 6c61  d_data("miscella
-00003490: 6e65 6f75 7322 2c20 2269 6e76 616c 6964  neous", "invalid
-000034a0: 5f68 6561 6465 7222 290a 2020 2020 2020  _header").      
-000034b0: 2020 746d 705f 6669 6c65 203d 2050 6174    tmp_file = Pat
-000034c0: 6828 6365 7263 6973 2e64 756d 705f 746f  h(cercis.dump_to
-000034d0: 5f66 696c 6528 736f 7572 6365 2929 0a20  _file(source)). 
-000034e0: 2020 2020 2020 2023 2046 756c 6c20 736f         # Full so
-000034f0: 7572 6365 2073 686f 756c 6420 6661 696c  urce should fail
-00003500: 2028 696e 7661 6c69 6420 7379 6e74 6178   (invalid syntax
-00003510: 2061 7420 6865 6164 6572 290a 2020 2020   at header).    
-00003520: 2020 2020 7365 6c66 2e69 6e76 6f6b 6542      self.invokeB
-00003530: 6c61 636b 285b 7374 7228 746d 705f 6669  lack([str(tmp_fi
-00003540: 6c65 292c 2022 2d2d 6469 6666 222c 2022  le), "--diff", "
-00003550: 2d2d 6368 6563 6b22 5d2c 2065 7869 745f  --check"], exit_
-00003560: 636f 6465 3d31 3233 290a 2020 2020 2020  code=123).      
-00003570: 2020 2320 536f 2c20 736b 6970 7069 6e67    # So, skipping
-00003580: 2074 6865 2066 6972 7374 206c 696e 6520   the first line 
-00003590: 7368 6f75 6c64 2077 6f72 6b0a 2020 2020  should work.    
-000035a0: 2020 2020 7265 7375 6c74 203d 2042 6c61      result = Bla
-000035b0: 636b 5275 6e6e 6572 2829 2e69 6e76 6f6b  ckRunner().invok
-000035c0: 6528 0a20 2020 2020 2020 2020 2020 2063  e(.            c
-000035d0: 6572 6369 732e 6d61 696e 2c20 5b73 7472  ercis.main, [str
-000035e0: 2874 6d70 5f66 696c 6529 2c20 222d 7822  (tmp_file), "-x"
-000035f0: 2c20 6622 2d2d 636f 6e66 6967 3d7b 454d  , f"--config={EM
-00003600: 5054 595f 434f 4e46 4947 7d22 5d0a 2020  PTY_CONFIG}"].  
-00003610: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003620: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00003630: 2872 6573 756c 742e 6578 6974 5f63 6f64  (result.exit_cod
-00003640: 652c 2030 290a 2020 2020 2020 2020 7769  e, 0).        wi
-00003650: 7468 206f 7065 6e28 746d 705f 6669 6c65  th open(tmp_file
-00003660: 2c20 656e 636f 6469 6e67 3d22 7574 6638  , encoding="utf8
-00003670: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
-00003680: 2020 2020 2061 6374 7561 6c20 3d20 662e       actual = f.
-00003690: 7265 6164 2829 0a20 2020 2020 2020 2073  read().        s
-000036a0: 656c 662e 6173 7365 7274 466f 726d 6174  elf.assertFormat
-000036b0: 4571 7561 6c28 736f 7572 6365 2c20 6163  Equal(source, ac
-000036c0: 7475 616c 290a 0a20 2020 2064 6566 2074  tual)..    def t
-000036d0: 6573 745f 736b 6970 5f73 6f75 7263 655f  est_skip_source_
-000036e0: 6669 7273 745f 6c69 6e65 5f77 6865 6e5f  first_line_when_
-000036f0: 6d69 7869 6e67 5f6e 6577 6c69 6e65 7328  mixing_newlines(
-00003700: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00003710: 2020 2020 2020 2063 6f64 655f 6d69 7869         code_mixi
-00003720: 6e67 5f6e 6577 6c69 6e65 7320 3d20 6222  ng_newlines = b"
-00003730: 4865 6164 6572 2077 696c 6c20 6265 2073  Header will be s
-00003740: 6b69 7070 6564 5c72 5c6e 6920 3d20 5b31  kipped\r\ni = [1
-00003750: 2c32 2c33 5d5c 6e6a 203d 205b 312c 322c  ,2,3]\nj = [1,2,
-00003760: 335d 5c6e 220a 2020 2020 2020 2020 6578  3]\n".        ex
-00003770: 7065 6374 6564 203d 2062 2248 6561 6465  pected = b"Heade
-00003780: 7220 7769 6c6c 2062 6520 736b 6970 7065  r will be skippe
-00003790: 645c 725c 6e69 203d 205b 312c 2032 2c20  d\r\ni = [1, 2, 
-000037a0: 335d 5c6e 6a20 3d20 5b31 2c20 322c 2033  3]\nj = [1, 2, 3
-000037b0: 5d5c 6e22 0a20 2020 2020 2020 2077 6974  ]\n".        wit
-000037c0: 6820 5465 6d70 6f72 6172 7944 6972 6563  h TemporaryDirec
-000037d0: 746f 7279 2829 2061 7320 776f 726b 7370  tory() as worksp
-000037e0: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
-000037f0: 2074 6573 745f 6669 6c65 203d 2050 6174   test_file = Pat
-00003800: 6828 776f 726b 7370 6163 6529 202f 2022  h(workspace) / "
-00003810: 736b 6970 5f68 6561 6465 722e 7079 220a  skip_header.py".
-00003820: 2020 2020 2020 2020 2020 2020 7465 7374              test
-00003830: 5f66 696c 652e 7772 6974 655f 6279 7465  _file.write_byte
-00003840: 7328 636f 6465 5f6d 6978 696e 675f 6e65  s(code_mixing_ne
-00003850: 776c 696e 6573 290a 2020 2020 2020 2020  wlines).        
-00003860: 2020 2020 6d6f 6465 203d 2072 6570 6c61      mode = repla
-00003870: 6365 2844 4546 4155 4c54 5f4d 4f44 452c  ce(DEFAULT_MODE,
-00003880: 2073 6b69 705f 736f 7572 6365 5f66 6972   skip_source_fir
-00003890: 7374 5f6c 696e 653d 5472 7565 290a 2020  st_line=True).  
-000038a0: 2020 2020 2020 2020 2020 6666 2874 6573            ff(tes
-000038b0: 745f 6669 6c65 2c20 6d6f 6465 3d6d 6f64  t_file, mode=mod
-000038c0: 652c 2077 7269 7465 5f62 6163 6b3d 6365  e, write_back=ce
-000038d0: 7263 6973 2e57 7269 7465 4261 636b 2e59  rcis.WriteBack.Y
-000038e0: 4553 290a 2020 2020 2020 2020 2020 2020  ES).            
-000038f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00003900: 2874 6573 745f 6669 6c65 2e72 6561 645f  (test_file.read_
-00003910: 6279 7465 7328 292c 2065 7870 6563 7465  bytes(), expecte
-00003920: 6429 0a0a 2020 2020 6465 6620 7465 7374  d)..    def test
-00003930: 5f73 6b69 705f 6d61 6769 635f 7472 6169  _skip_magic_trai
-00003940: 6c69 6e67 5f63 6f6d 6d61 2873 656c 6629  ling_comma(self)
-00003950: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00003960: 2020 736f 7572 6365 2c20 5f20 3d20 7265    source, _ = re
-00003970: 6164 5f64 6174 6128 2273 696d 706c 655f  ad_data("simple_
-00003980: 6361 7365 7322 2c20 2265 7870 7265 7373  cases", "express
-00003990: 696f 6e22 290a 2020 2020 2020 2020 6578  ion").        ex
-000039a0: 7065 6374 6564 2c20 5f20 3d20 7265 6164  pected, _ = read
-000039b0: 5f64 6174 6128 0a20 2020 2020 2020 2020  _data(.         
-000039c0: 2020 2022 6d69 7363 656c 6c61 6e65 6f75     "miscellaneou
-000039d0: 7322 2c20 2265 7870 7265 7373 696f 6e5f  s", "expression_
-000039e0: 736b 6970 5f6d 6167 6963 5f74 7261 696c  skip_magic_trail
-000039f0: 696e 675f 636f 6d6d 612e 6469 6666 220a  ing_comma.diff".
-00003a00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00003a10: 2020 746d 705f 6669 6c65 203d 2050 6174    tmp_file = Pat
-00003a20: 6828 6365 7263 6973 2e64 756d 705f 746f  h(cercis.dump_to
-00003a30: 5f66 696c 6528 736f 7572 6365 2929 0a20  _file(source)). 
-00003a40: 2020 2020 2020 2064 6966 665f 6865 6164         diff_head
-00003a50: 6572 203d 2072 652e 636f 6d70 696c 6528  er = re.compile(
-00003a60: 0a20 2020 2020 2020 2020 2020 2072 6622  .            rf"
-00003a70: 7b72 652e 6573 6361 7065 2873 7472 2874  {re.escape(str(t
-00003a80: 6d70 5f66 696c 6529 297d 5c74 5c64 5c64  mp_file))}\t\d\d
-00003a90: 5c64 5c64 2d5c 645c 642d 5c64 5c64 2022  \d\d-\d\d-\d\d "
-00003aa0: 0a20 2020 2020 2020 2020 2020 2072 225c  .            r"\
-00003ab0: 645c 643a 5c64 5c64 3a5c 645c 645c 2e5c  d\d:\d\d:\d\d\.\
-00003ac0: 645c 645c 645c 645c 645c 6420 5c2b 5c64  d\d\d\d\d\d \+\d
-00003ad0: 5c64 5c64 5c64 220a 2020 2020 2020 2020  \d\d\d".        
-00003ae0: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-00003af0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00003b00: 7420 3d20 426c 6163 6b52 756e 6e65 7228  t = BlackRunner(
-00003b10: 292e 696e 766f 6b65 280a 2020 2020 2020  ).invoke(.      
-00003b20: 2020 2020 2020 2020 2020 6365 7263 6973            cercis
-00003b30: 2e6d 6169 6e2c 0a20 2020 2020 2020 2020  .main,.         
-00003b40: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00003b50: 2020 2020 2020 2020 2020 2020 2022 2d43               "-C
-00003b60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003b70: 2020 2020 2020 2022 2d2d 6469 6666 222c         "--diff",
-00003b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b90: 2020 2020 2073 7472 2874 6d70 5f66 696c       str(tmp_fil
-00003ba0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00003bb0: 2020 2020 2020 2020 6622 2d2d 636f 6e66          f"--conf
-00003bc0: 6967 3d7b 454d 5054 595f 434f 4e46 4947  ig={EMPTY_CONFIG
-00003bd0: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-00003be0: 2020 2020 2020 2020 222d 2d6c 696e 652d          "--line-
-00003bf0: 6c65 6e67 7468 3d38 3822 2c0a 2020 2020  length=88",.    
-00003c00: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-00003c10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00003c20: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00003c30: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
-00003c40: 2e65 7869 745f 636f 6465 2c20 3029 0a20  .exit_code, 0). 
-00003c50: 2020 2020 2020 2066 696e 616c 6c79 3a0a         finally:.
-00003c60: 2020 2020 2020 2020 2020 2020 6f73 2e75              os.u
-00003c70: 6e6c 696e 6b28 746d 705f 6669 6c65 290a  nlink(tmp_file).
-00003c80: 2020 2020 2020 2020 6163 7475 616c 203d          actual =
-00003c90: 2072 6573 756c 742e 6f75 7470 7574 0a20   result.output. 
-00003ca0: 2020 2020 2020 2061 6374 7561 6c20 3d20         actual = 
-00003cb0: 6469 6666 5f68 6561 6465 722e 7375 6228  diff_header.sub(
-00003cc0: 4445 5445 524d 494e 4953 5449 435f 4845  DETERMINISTIC_HE
-00003cd0: 4144 4552 2c20 6163 7475 616c 290a 2020  ADER, actual).  
-00003ce0: 2020 2020 2020 6163 7475 616c 203d 2061        actual = a
-00003cf0: 6374 7561 6c2e 7273 7472 6970 2829 202b  ctual.rstrip() +
-00003d00: 2022 5c6e 2220 2023 2074 6865 2064 6966   "\n"  # the dif
-00003d10: 6620 6f75 7470 7574 2068 6173 2061 2074  f output has a t
-00003d20: 7261 696c 696e 6720 7370 6163 650a 2020  railing space.  
-00003d30: 2020 2020 2020 6966 2065 7870 6563 7465        if expecte
-00003d40: 6420 213d 2061 6374 7561 6c3a 0a20 2020  d != actual:.   
-00003d50: 2020 2020 2020 2020 2064 756d 7020 3d20           dump = 
-00003d60: 6365 7263 6973 2e64 756d 705f 746f 5f66  cercis.dump_to_f
-00003d70: 696c 6528 6163 7475 616c 290a 2020 2020  ile(actual).    
-00003d80: 2020 2020 2020 2020 6d73 6720 3d20 280a          msg = (.
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2245 7870 6563 7465 6420 6469 6666 2069  "Expected diff i
-00003db0: 736e 2774 2065 7175 616c 2074 6f20 7468  sn't equal to th
-00003dc0: 6520 6163 7475 616c 2e20 4966 2079 6f75  e actual. If you
-00003dd0: 206d 6164 6520 6368 616e 6765 7320 746f   made changes to
-00003de0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003df0: 2020 2220 6578 7072 6573 7369 6f6e 2e70    " expression.p
-00003e00: 7920 616e 6420 7468 6973 2069 7320 616e  y and this is an
-00003e10: 2061 6e74 6963 6970 6174 6564 2064 6966   anticipated dif
-00003e20: 6665 7265 6e63 652c 206f 7665 7277 7269  ference, overwri
-00003e30: 7465 220a 2020 2020 2020 2020 2020 2020  te".            
-00003e40: 2020 2020 2220 7465 7374 732f 6461 7461      " tests/data
-00003e50: 2f6d 6973 6365 6c6c 616e 656f 7573 2f65  /miscellaneous/e
-00003e60: 7870 7265 7373 696f 6e5f 736b 6970 5f6d  xpression_skip_m
-00003e70: 6167 6963 5f74 7261 696c 696e 675f 636f  agic_trailing_co
-00003e80: 6d6d 612e 6469 6666 220a 2020 2020 2020  mma.diff".      
-00003e90: 2020 2020 2020 2020 2020 6622 2077 6974            f" wit
-00003ea0: 6820 7b64 756d 707d 220a 2020 2020 2020  h {dump}".      
-00003eb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003ec0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00003ed0: 7175 616c 2865 7870 6563 7465 642c 2061  qual(expected, a
-00003ee0: 6374 7561 6c2c 206d 7367 290a 0a20 2020  ctual, msg)..   
-00003ef0: 2040 7061 7463 6828 2263 6572 6369 732e   @patch("cercis.
-00003f00: 6475 6d70 5f74 6f5f 6669 6c65 222c 2064  dump_to_file", d
-00003f10: 756d 705f 746f 5f73 7464 6572 7229 0a20  ump_to_stderr). 
-00003f20: 2020 2064 6566 2074 6573 745f 6173 796e     def test_asyn
-00003f30: 635f 6173 5f69 6465 6e74 6966 6965 7228  c_as_identifier(
-00003f40: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00003f50: 2020 2020 2020 2073 6f75 7263 655f 7061         source_pa
-00003f60: 7468 203d 2067 6574 5f63 6173 655f 7061  th = get_case_pa
-00003f70: 7468 2822 6d69 7363 656c 6c61 6e65 6f75  th("miscellaneou
-00003f80: 7322 2c20 2261 7379 6e63 5f61 735f 6964  s", "async_as_id
-00003f90: 656e 7469 6669 6572 2229 0a20 2020 2020  entifier").     
-00003fa0: 2020 2073 6f75 7263 652c 2065 7870 6563     source, expec
-00003fb0: 7465 6420 3d20 7265 6164 5f64 6174 615f  ted = read_data_
-00003fc0: 6672 6f6d 5f66 696c 6528 736f 7572 6365  from_file(source
-00003fd0: 5f70 6174 6829 0a20 2020 2020 2020 2061  _path).        a
-00003fe0: 6374 7561 6c20 3d20 6673 2873 6f75 7263  ctual = fs(sourc
-00003ff0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00004000: 6173 7365 7274 466f 726d 6174 4571 7561  assertFormatEqua
-00004010: 6c28 6578 7065 6374 6564 2c20 6163 7475  l(expected, actu
-00004020: 616c 290a 2020 2020 2020 2020 6d61 6a6f  al).        majo
-00004030: 722c 206d 696e 6f72 203d 2073 7973 2e76  r, minor = sys.v
-00004040: 6572 7369 6f6e 5f69 6e66 6f5b 3a32 5d0a  ersion_info[:2].
-00004050: 2020 2020 2020 2020 6966 206d 616a 6f72          if major
-00004060: 203c 2033 206f 7220 286d 616a 6f72 203c   < 3 or (major <
-00004070: 3d20 3320 616e 6420 6d69 6e6f 7220 3c20  = 3 and minor < 
-00004080: 3729 3a0a 2020 2020 2020 2020 2020 2020  7):.            
-00004090: 6365 7263 6973 2e61 7373 6572 745f 6571  cercis.assert_eq
-000040a0: 7569 7661 6c65 6e74 2873 6f75 7263 652c  uivalent(source,
-000040b0: 2061 6374 7561 6c29 0a20 2020 2020 2020   actual).       
-000040c0: 2063 6572 6369 732e 6173 7365 7274 5f73   cercis.assert_s
-000040d0: 7461 626c 6528 736f 7572 6365 2c20 6163  table(source, ac
-000040e0: 7475 616c 2c20 4445 4641 554c 545f 4d4f  tual, DEFAULT_MO
-000040f0: 4445 290a 2020 2020 2020 2020 2320 656e  DE).        # en
-00004100: 7375 7265 2063 6572 6369 7320 6361 6e20  sure cercis can 
-00004110: 7061 7273 6520 7468 6973 2077 6865 6e20  parse this when 
-00004120: 7468 6520 7461 7267 6574 2069 7320 332e  the target is 3.
-00004130: 360a 2020 2020 2020 2020 7365 6c66 2e69  6.        self.i
-00004140: 6e76 6f6b 6542 6c61 636b 285b 7374 7228  nvokeBlack([str(
-00004150: 736f 7572 6365 5f70 6174 6829 2c20 222d  source_path), "-
-00004160: 2d74 6172 6765 742d 7665 7273 696f 6e22  -target-version"
-00004170: 2c20 2270 7933 3622 5d29 0a20 2020 2020  , "py36"]).     
-00004180: 2020 2023 2062 7574 206e 6f74 206f 6e20     # but not on 
-00004190: 332e 372c 2062 6563 6175 7365 2061 7379  3.7, because asy
-000041a0: 6e63 2f61 7761 6974 2069 7320 6e6f 206c  nc/await is no l
-000041b0: 6f6e 6765 7220 616e 2069 6465 6e74 6966  onger an identif
-000041c0: 6965 720a 2020 2020 2020 2020 7365 6c66  ier.        self
-000041d0: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
-000041e0: 7228 736f 7572 6365 5f70 6174 6829 2c20  r(source_path), 
-000041f0: 222d 2d74 6172 6765 742d 7665 7273 696f  "--target-versio
-00004200: 6e22 2c20 2270 7933 3722 5d2c 2065 7869  n", "py37"], exi
-00004210: 745f 636f 6465 3d31 3233 290a 0a20 2020  t_code=123)..   
-00004220: 2040 7061 7463 6828 2263 6572 6369 732e   @patch("cercis.
-00004230: 6475 6d70 5f74 6f5f 6669 6c65 222c 2064  dump_to_file", d
-00004240: 756d 705f 746f 5f73 7464 6572 7229 0a20  ump_to_stderr). 
-00004250: 2020 2064 6566 2074 6573 745f 7079 7468     def test_pyth
-00004260: 6f6e 3337 2873 656c 6629 202d 3e20 4e6f  on37(self) -> No
-00004270: 6e65 3a0a 2020 2020 2020 2020 736f 7572  ne:.        sour
-00004280: 6365 5f70 6174 6820 3d20 6765 745f 6361  ce_path = get_ca
-00004290: 7365 5f70 6174 6828 2270 795f 3337 222c  se_path("py_37",
-000042a0: 2022 7079 7468 6f6e 3337 2229 0a20 2020   "python37").   
-000042b0: 2020 2020 2073 6f75 7263 652c 2065 7870       source, exp
-000042c0: 6563 7465 6420 3d20 7265 6164 5f64 6174  ected = read_dat
-000042d0: 615f 6672 6f6d 5f66 696c 6528 736f 7572  a_from_file(sour
-000042e0: 6365 5f70 6174 6829 0a20 2020 2020 2020  ce_path).       
-000042f0: 2061 6374 7561 6c20 3d20 6673 2873 6f75   actual = fs(sou
-00004300: 7263 6529 0a20 2020 2020 2020 2073 656c  rce).        sel
-00004310: 662e 6173 7365 7274 466f 726d 6174 4571  f.assertFormatEq
-00004320: 7561 6c28 6578 7065 6374 6564 2c20 6163  ual(expected, ac
-00004330: 7475 616c 290a 2020 2020 2020 2020 6d61  tual).        ma
-00004340: 6a6f 722c 206d 696e 6f72 203d 2073 7973  jor, minor = sys
-00004350: 2e76 6572 7369 6f6e 5f69 6e66 6f5b 3a32  .version_info[:2
-00004360: 5d0a 2020 2020 2020 2020 6966 206d 616a  ].        if maj
-00004370: 6f72 203e 2033 206f 7220 286d 616a 6f72  or > 3 or (major
-00004380: 203d 3d20 3320 616e 6420 6d69 6e6f 7220   == 3 and minor 
-00004390: 3e3d 2037 293a 0a20 2020 2020 2020 2020  >= 7):.         
-000043a0: 2020 2063 6572 6369 732e 6173 7365 7274     cercis.assert
-000043b0: 5f65 7175 6976 616c 656e 7428 736f 7572  _equivalent(sour
-000043c0: 6365 2c20 6163 7475 616c 290a 2020 2020  ce, actual).    
-000043d0: 2020 2020 6365 7263 6973 2e61 7373 6572      cercis.asser
-000043e0: 745f 7374 6162 6c65 2873 6f75 7263 652c  t_stable(source,
-000043f0: 2061 6374 7561 6c2c 2044 4546 4155 4c54   actual, DEFAULT
-00004400: 5f4d 4f44 4529 0a20 2020 2020 2020 2023  _MODE).        #
-00004410: 2065 6e73 7572 6520 6365 7263 6973 2063   ensure cercis c
-00004420: 616e 2070 6172 7365 2074 6869 7320 7768  an parse this wh
-00004430: 656e 2074 6865 2074 6172 6765 7420 6973  en the target is
-00004440: 2033 2e37 0a20 2020 2020 2020 2073 656c   3.7.        sel
-00004450: 662e 696e 766f 6b65 426c 6163 6b28 5b73  f.invokeBlack([s
-00004460: 7472 2873 6f75 7263 655f 7061 7468 292c  tr(source_path),
-00004470: 2022 2d2d 7461 7267 6574 2d76 6572 7369   "--target-versi
-00004480: 6f6e 222c 2022 7079 3337 225d 290a 2020  on", "py37"]).  
-00004490: 2020 2020 2020 2320 6275 7420 6e6f 7420        # but not 
-000044a0: 6f6e 2033 2e36 2c20 6265 6361 7573 6520  on 3.6, because 
-000044b0: 7765 2075 7365 2061 7379 6e63 2061 7320  we use async as 
-000044c0: 6120 7265 7365 7276 6564 206b 6579 776f  a reserved keywo
-000044d0: 7264 0a20 2020 2020 2020 2073 656c 662e  rd.        self.
-000044e0: 696e 766f 6b65 426c 6163 6b28 5b73 7472  invokeBlack([str
-000044f0: 2873 6f75 7263 655f 7061 7468 292c 2022  (source_path), "
-00004500: 2d2d 7461 7267 6574 2d76 6572 7369 6f6e  --target-version
-00004510: 222c 2022 7079 3336 225d 2c20 6578 6974  ", "py36"], exit
-00004520: 5f63 6f64 653d 3132 3329 0a0a 2020 2020  _code=123)..    
-00004530: 6465 6620 7465 7374 5f74 6162 5f63 6f6d  def test_tab_com
-00004540: 6d65 6e74 5f69 6e64 656e 7461 7469 6f6e  ment_indentation
-00004550: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00004560: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-00004570: 5f74 6162 203d 2022 6966 2031 3a5c 6e5c  _tab = "if 1:\n\
-00004580: 7469 6620 323a 5c6e 5c74 5c74 7061 7373  tif 2:\n\t\tpass
-00004590: 5c6e 5c74 2320 636f 6d6d 656e 745c 6e5c  \n\t# comment\n\
-000045a0: 7470 6173 735c 6e22 0a20 2020 2020 2020  tpass\n".       
-000045b0: 2063 6f6e 7465 6e74 735f 7370 6320 3d20   contents_spc = 
-000045c0: 2269 6620 313a 5c6e 2020 2020 6966 2032  "if 1:\n    if 2
-000045d0: 3a5c 6e20 2020 2020 2020 2070 6173 735c  :\n        pass\
-000045e0: 6e20 2020 2023 2063 6f6d 6d65 6e74 5c6e  n    # comment\n
-000045f0: 2020 2020 7061 7373 5c6e 220a 2020 2020      pass\n".    
-00004600: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
-00004610: 6f72 6d61 7445 7175 616c 2863 6f6e 7465  ormatEqual(conte
-00004620: 6e74 735f 7370 632c 2066 7328 636f 6e74  nts_spc, fs(cont
-00004630: 656e 7473 5f73 7063 2929 0a20 2020 2020  ents_spc)).     
-00004640: 2020 2073 656c 662e 6173 7365 7274 466f     self.assertFo
-00004650: 726d 6174 4571 7561 6c28 636f 6e74 656e  rmatEqual(conten
-00004660: 7473 5f73 7063 2c20 6673 2863 6f6e 7465  ts_spc, fs(conte
-00004670: 6e74 735f 7461 6229 290a 0a20 2020 2020  nts_tab))..     
-00004680: 2020 2063 6f6e 7465 6e74 735f 7461 6220     contents_tab 
-00004690: 3d20 2269 6620 313a 5c6e 5c74 6966 2032  = "if 1:\n\tif 2
-000046a0: 3a5c 6e5c 745c 7470 6173 735c 6e5c 745c  :\n\t\tpass\n\t\
-000046b0: 7423 2063 6f6d 6d65 6e74 5c6e 5c74 7061  t# comment\n\tpa
-000046c0: 7373 5c6e 220a 2020 2020 2020 2020 636f  ss\n".        co
-000046d0: 6e74 656e 7473 5f73 7063 203d 2022 6966  ntents_spc = "if
-000046e0: 2031 3a5c 6e20 2020 2069 6620 323a 5c6e   1:\n    if 2:\n
-000046f0: 2020 2020 2020 2020 7061 7373 5c6e 2020          pass\n  
-00004700: 2020 2020 2020 2320 636f 6d6d 656e 745c        # comment\
-00004710: 6e20 2020 2070 6173 735c 6e22 0a20 2020  n    pass\n".   
-00004720: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00004730: 466f 726d 6174 4571 7561 6c28 636f 6e74  FormatEqual(cont
-00004740: 656e 7473 5f73 7063 2c20 6673 2863 6f6e  ents_spc, fs(con
-00004750: 7465 6e74 735f 7370 6329 290a 2020 2020  tents_spc)).    
-00004760: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
-00004770: 6f72 6d61 7445 7175 616c 2863 6f6e 7465  ormatEqual(conte
-00004780: 6e74 735f 7370 632c 2066 7328 636f 6e74  nts_spc, fs(cont
-00004790: 656e 7473 5f74 6162 2929 0a0a 2020 2020  ents_tab))..    
-000047a0: 2020 2020 2320 6d69 7865 6420 7461 6273      # mixed tabs
-000047b0: 2061 6e64 2073 7061 6365 7320 2876 616c   and spaces (val
-000047c0: 6964 2050 7974 686f 6e20 3220 636f 6465  id Python 2 code
-000047d0: 290a 2020 2020 2020 2020 636f 6e74 656e  ).        conten
-000047e0: 7473 5f74 6162 203d 2022 6966 2031 3a5c  ts_tab = "if 1:\
-000047f0: 6e20 2020 2020 2020 2069 6620 323a 5c6e  n        if 2:\n
-00004800: 5c74 5c74 7061 7373 5c6e 5c74 2320 636f  \t\tpass\n\t# co
-00004810: 6d6d 656e 745c 6e20 2020 2020 2020 2070  mment\n        p
-00004820: 6173 735c 6e22 0a20 2020 2020 2020 2063  ass\n".        c
-00004830: 6f6e 7465 6e74 735f 7370 6320 3d20 2269  ontents_spc = "i
-00004840: 6620 313a 5c6e 2020 2020 6966 2032 3a5c  f 1:\n    if 2:\
-00004850: 6e20 2020 2020 2020 2070 6173 735c 6e20  n        pass\n 
-00004860: 2020 2023 2063 6f6d 6d65 6e74 5c6e 2020     # comment\n  
-00004870: 2020 7061 7373 5c6e 220a 2020 2020 2020    pass\n".      
-00004880: 2020 7365 6c66 2e61 7373 6572 7446 6f72    self.assertFor
-00004890: 6d61 7445 7175 616c 2863 6f6e 7465 6e74  matEqual(content
-000048a0: 735f 7370 632c 2066 7328 636f 6e74 656e  s_spc, fs(conten
-000048b0: 7473 5f73 7063 2929 0a20 2020 2020 2020  ts_spc)).       
-000048c0: 2073 656c 662e 6173 7365 7274 466f 726d   self.assertForm
-000048d0: 6174 4571 7561 6c28 636f 6e74 656e 7473  atEqual(contents
-000048e0: 5f73 7063 2c20 6673 2863 6f6e 7465 6e74  _spc, fs(content
-000048f0: 735f 7461 6229 290a 0a20 2020 2020 2020  s_tab))..       
-00004900: 2063 6f6e 7465 6e74 735f 7461 6220 3d20   contents_tab = 
-00004910: 2269 6620 313a 5c6e 2020 2020 2020 2020  "if 1:\n        
-00004920: 6966 2032 3a5c 6e5c 745c 7470 6173 735c  if 2:\n\t\tpass\
-00004930: 6e5c 745c 7423 2063 6f6d 6d65 6e74 5c6e  n\t\t# comment\n
-00004940: 2020 2020 2020 2020 7061 7373 5c6e 220a          pass\n".
-00004950: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-00004960: 5f73 7063 203d 2022 6966 2031 3a5c 6e20  _spc = "if 1:\n 
-00004970: 2020 2069 6620 323a 5c6e 2020 2020 2020     if 2:\n      
-00004980: 2020 7061 7373 5c6e 2020 2020 2020 2020    pass\n        
-00004990: 2320 636f 6d6d 656e 745c 6e20 2020 2070  # comment\n    p
-000049a0: 6173 735c 6e22 0a20 2020 2020 2020 2073  ass\n".        s
-000049b0: 656c 662e 6173 7365 7274 466f 726d 6174  elf.assertFormat
-000049c0: 4571 7561 6c28 636f 6e74 656e 7473 5f73  Equal(contents_s
-000049d0: 7063 2c20 6673 2863 6f6e 7465 6e74 735f  pc, fs(contents_
-000049e0: 7370 6329 290a 2020 2020 2020 2020 7365  spc)).        se
-000049f0: 6c66 2e61 7373 6572 7446 6f72 6d61 7445  lf.assertFormatE
-00004a00: 7175 616c 2863 6f6e 7465 6e74 735f 7370  qual(contents_sp
-00004a10: 632c 2066 7328 636f 6e74 656e 7473 5f74  c, fs(contents_t
-00004a20: 6162 2929 0a0a 2020 2020 6465 6620 7465  ab))..    def te
-00004a30: 7374 5f66 616c 7365 5f70 6f73 6974 6976  st_false_positiv
-00004a40: 655f 7379 6d6c 696e 6b5f 6f75 7470 7574  e_symlink_output
-00004a50: 5f69 7373 7565 5f33 3338 3428 7365 6c66  _issue_3384(self
-00004a60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00004a70: 2020 2023 2045 6d75 6c61 7465 2074 6865     # Emulate the
-00004a80: 2062 6568 6176 696f 7220 7768 656e 2075   behavior when u
-00004a90: 7369 6e67 2074 6865 2043 4c49 2028 6063  sing the CLI (`c
-00004aa0: 6572 6369 7320 2e2f 6368 696c 6420 202d  ercis ./child  -
-00004ab0: 2d76 6572 626f 7365 6029 2c20 7768 6963  -verbose`), whic
-00004ac0: 680a 2020 2020 2020 2020 2320 696e 766f  h.        # invo
-00004ad0: 6c76 6573 2070 6174 6368 696e 6720 736f  lves patching so
-00004ae0: 6d65 2060 7061 7468 6c69 622e 5061 7468  me `pathlib.Path
-00004af0: 6020 6d65 7468 6f64 732e 2049 6e20 7061  ` methods. In pa
-00004b00: 7274 6963 756c 6172 2c20 6069 735f 6469  rticular, `is_di
-00004b10: 7260 2069 730a 2020 2020 2020 2020 2320  r` is.        # 
-00004b20: 7061 7463 6865 6420 6f6e 6c79 206f 6e20  patched only on 
-00004b30: 6974 7320 6669 7273 7420 6361 6c6c 3a20  its first call: 
-00004b40: 7768 656e 2063 6865 636b 696e 6720 6966  when checking if
-00004b50: 2022 2e2f 6368 696c 6422 2069 7320 6120   "./child" is a 
-00004b60: 6469 7265 6374 6f72 7920 6974 0a20 2020  directory it.   
-00004b70: 2020 2020 2023 2073 686f 756c 6420 7265       # should re
-00004b80: 7475 726e 2054 7275 652e 2054 6865 2022  turn True. The "
-00004b90: 2e2f 6368 696c 6422 2066 6f6c 6465 7220  ./child" folder 
-00004ba0: 6578 6973 7473 2072 656c 6174 6976 6520  exists relative 
-00004bb0: 746f 2074 6865 2063 7764 2077 6865 6e0a  to the cwd when.
-00004bc0: 2020 2020 2020 2020 2320 7275 6e6e 696e          # runnin
-00004bd0: 6720 6672 6f6d 2043 4c49 2c20 6275 7420  g from CLI, but 
-00004be0: 6661 696c 7320 7768 656e 2072 756e 6e69  fails when runni
-00004bf0: 6e67 2074 6865 2074 6573 7473 2062 6563  ng the tests bec
-00004c00: 6175 7365 2063 7764 2069 7320 6469 6666  ause cwd is diff
-00004c10: 6572 656e 740a 2020 2020 2020 2020 7072  erent.        pr
-00004c20: 6f6a 6563 745f 726f 6f74 203d 2050 6174  oject_root = Pat
-00004c30: 6828 5448 4953 5f44 4952 202f 2022 6461  h(THIS_DIR / "da
-00004c40: 7461 2220 2f20 226e 6573 7465 645f 6769  ta" / "nested_gi
-00004c50: 7469 676e 6f72 655f 7465 7374 7322 290a  tignore_tests").
-00004c60: 2020 2020 2020 2020 776f 726b 696e 675f          working_
-00004c70: 6469 7265 6374 6f72 7920 3d20 7072 6f6a  directory = proj
-00004c80: 6563 745f 726f 6f74 202f 2022 726f 6f74  ect_root / "root
-00004c90: 220a 2020 2020 2020 2020 7461 7267 6574  ".        target
-00004ca0: 5f61 6273 7061 7468 203d 2077 6f72 6b69  _abspath = worki
-00004cb0: 6e67 5f64 6972 6563 746f 7279 202f 2022  ng_directory / "
-00004cc0: 6368 696c 6422 0a20 2020 2020 2020 2074  child".        t
-00004cd0: 6172 6765 745f 636f 6e74 656e 7473 203d  arget_contents =
-00004ce0: 2028 0a20 2020 2020 2020 2020 2020 2073   (.            s
-00004cf0: 7263 2e72 656c 6174 6976 655f 746f 2877  rc.relative_to(w
-00004d00: 6f72 6b69 6e67 5f64 6972 6563 746f 7279  orking_directory
-00004d10: 2920 666f 7220 7372 6320 696e 2074 6172  ) for src in tar
-00004d20: 6765 745f 6162 7370 6174 682e 6974 6572  get_abspath.iter
-00004d30: 6469 7228 290a 2020 2020 2020 2020 290a  dir().        ).
-00004d40: 0a20 2020 2020 2020 2064 6566 206d 6f63  .        def moc
-00004d50: 6b5f 6e5f 6361 6c6c 7328 7265 7370 6f6e  k_n_calls(respon
-00004d60: 7365 733a 204c 6973 745b 626f 6f6c 5d29  ses: List[bool])
-00004d70: 202d 3e20 4361 6c6c 6162 6c65 5b5b 5d2c   -> Callable[[],
-00004d80: 2062 6f6f 6c5d 3a0a 2020 2020 2020 2020   bool]:.        
-00004d90: 2020 2020 6465 6620 5f6d 6f63 6b65 645f      def _mocked_
-00004da0: 6361 6c6c 7328 2920 2d3e 2062 6f6f 6c3a  calls() -> bool:
-00004db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004dc0: 2069 6620 7265 7370 6f6e 7365 733a 0a20   if responses:. 
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-00004df0: 7365 732e 706f 7028 3029 0a20 2020 2020  ses.pop(0).     
-00004e00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004e10: 6e20 4661 6c73 650a 0a20 2020 2020 2020  n False..       
-00004e20: 2020 2020 2072 6574 7572 6e20 5f6d 6f63       return _moc
-00004e30: 6b65 645f 6361 6c6c 730a 0a20 2020 2020  ked_calls..     
-00004e40: 2020 2077 6974 6820 7061 7463 6828 2270     with patch("p
-00004e50: 6174 686c 6962 2e50 6174 682e 6974 6572  athlib.Path.iter
-00004e60: 6469 7222 2c20 7265 7475 726e 5f76 616c  dir", return_val
-00004e70: 7565 3d74 6172 6765 745f 636f 6e74 656e  ue=target_conten
-00004e80: 7473 292c 2070 6174 6368 280a 2020 2020  ts), patch(.    
-00004e90: 2020 2020 2020 2020 2270 6174 686c 6962          "pathlib
-00004ea0: 2e50 6174 682e 6377 6422 2c20 7265 7475  .Path.cwd", retu
-00004eb0: 726e 5f76 616c 7565 3d77 6f72 6b69 6e67  rn_value=working
-00004ec0: 5f64 6972 6563 746f 7279 0a20 2020 2020  _directory.     
-00004ed0: 2020 2029 2c20 7061 7463 6828 2270 6174     ), patch("pat
-00004ee0: 686c 6962 2e50 6174 682e 6973 5f64 6972  hlib.Path.is_dir
-00004ef0: 222c 2073 6964 655f 6566 6665 6374 3d6d  ", side_effect=m
-00004f00: 6f63 6b5f 6e5f 6361 6c6c 7328 5b54 7275  ock_n_calls([Tru
-00004f10: 655d 2929 3a0a 2020 2020 2020 2020 2020  e])):.          
-00004f20: 2020 6374 7820 3d20 4661 6b65 436f 6e74    ctx = FakeCont
-00004f30: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
-00004f40: 2020 6374 782e 6f62 6a5b 2272 6f6f 7422    ctx.obj["root"
-00004f50: 5d20 3d20 7072 6f6a 6563 745f 726f 6f74  ] = project_root
-00004f60: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00004f70: 6f72 7420 3d20 4d61 6769 634d 6f63 6b28  ort = MagicMock(
-00004f80: 7665 7262 6f73 653d 5472 7565 290a 2020  verbose=True).  
-00004f90: 2020 2020 2020 2020 2020 6365 7263 6973            cercis
-00004fa0: 2e67 6574 5f73 6f75 7263 6573 280a 2020  .get_sources(.  
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-00004fc0: 783d 6374 782c 0a20 2020 2020 2020 2020  x=ctx,.         
-00004fd0: 2020 2020 2020 2073 7263 3d28 222e 2f63         src=("./c
-00004fe0: 6869 6c64 222c 292c 0a20 2020 2020 2020  hild",),.       
-00004ff0: 2020 2020 2020 2020 2071 7569 6574 3d46           quiet=F
-00005000: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00005010: 2020 2020 2020 7665 7262 6f73 653d 5472        verbose=Tr
-00005020: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00005030: 2020 2020 696e 636c 7564 653d 4445 4641      include=DEFA
-00005040: 554c 545f 494e 434c 5544 452c 0a20 2020  ULT_INCLUDE,.   
-00005050: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00005060: 6c75 6465 3d4e 6f6e 652c 0a20 2020 2020  lude=None,.     
-00005070: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-00005080: 743d 7265 706f 7274 2c0a 2020 2020 2020  t=report,.      
-00005090: 2020 2020 2020 2020 2020 6578 7465 6e64            extend
-000050a0: 5f65 7863 6c75 6465 3d4e 6f6e 652c 0a20  _exclude=None,. 
-000050b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000050c0: 6f72 6365 5f65 7863 6c75 6465 3d4e 6f6e  orce_exclude=Non
-000050d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000050e0: 2020 2073 7464 696e 5f66 696c 656e 616d     stdin_filenam
-000050f0: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
-00005100: 2020 2020 290a 2020 2020 2020 2020 6173      ).        as
-00005110: 7365 7274 206e 6f74 2061 6e79 280a 2020  sert not any(.  
-00005120: 2020 2020 2020 2020 2020 6d6f 636b 5f61            mock_a
-00005130: 7267 735b 315d 2e73 7461 7274 7377 6974  rgs[1].startswit
-00005140: 6828 2269 7320 6120 7379 6d62 6f6c 6963  h("is a symbolic
-00005150: 206c 696e 6b20 7468 6174 2070 6f69 6e74   link that point
-00005160: 7320 6f75 7473 6964 6522 290a 2020 2020  s outside").    
-00005170: 2020 2020 2020 2020 666f 7220 5f2c 206d          for _, m
-00005180: 6f63 6b5f 6172 6773 2c20 5f20 696e 2072  ock_args, _ in r
-00005190: 6570 6f72 742e 7061 7468 5f69 676e 6f72  eport.path_ignor
-000051a0: 6564 2e6d 6f63 6b5f 6361 6c6c 730a 2020  ed.mock_calls.  
-000051b0: 2020 2020 2020 292c 2022 4120 7379 6d62        ), "A symb
-000051c0: 6f6c 6963 206c 696e 6b20 7761 7320 7265  olic link was re
-000051d0: 706f 7274 6564 2e22 0a20 2020 2020 2020  ported.".       
-000051e0: 2072 6570 6f72 742e 7061 7468 5f69 676e   report.path_ign
-000051f0: 6f72 6564 2e61 7373 6572 745f 6361 6c6c  ored.assert_call
-00005200: 6564 5f6f 6e63 655f 7769 7468 280a 2020  ed_once_with(.  
-00005210: 2020 2020 2020 2020 2020 5061 7468 2822            Path("
-00005220: 6368 696c 6422 2c20 2262 2e70 7922 292c  child", "b.py"),
-00005230: 2022 6d61 7463 6865 7320 6120 2e67 6974   "matches a .git
-00005240: 6967 6e6f 7265 2066 696c 6520 636f 6e74  ignore file cont
-00005250: 656e 7422 0a20 2020 2020 2020 2029 0a0a  ent".        )..
-00005260: 2020 2020 6465 6620 7465 7374 5f72 6570      def test_rep
-00005270: 6f72 745f 7665 7262 6f73 6528 7365 6c66  ort_verbose(self
-00005280: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00005290: 2020 2072 6570 6f72 7420 3d20 5265 706f     report = Repo
-000052a0: 7274 2876 6572 626f 7365 3d54 7275 6529  rt(verbose=True)
-000052b0: 0a20 2020 2020 2020 206f 7574 5f6c 696e  .        out_lin
-000052c0: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
-000052d0: 6572 725f 6c69 6e65 7320 3d20 5b5d 0a0a  err_lines = []..
-000052e0: 2020 2020 2020 2020 6465 6620 6f75 7428          def out(
-000052f0: 6d73 673a 2073 7472 2c20 2a2a 6b77 6172  msg: str, **kwar
-00005300: 6773 3a20 416e 7929 202d 3e20 4e6f 6e65  gs: Any) -> None
-00005310: 3a0a 2020 2020 2020 2020 2020 2020 6f75  :.            ou
-00005320: 745f 6c69 6e65 732e 6170 7065 6e64 286d  t_lines.append(m
-00005330: 7367 290a 0a20 2020 2020 2020 2064 6566  sg)..        def
-00005340: 2065 7272 286d 7367 3a20 7374 722c 202a   err(msg: str, *
-00005350: 2a6b 7761 7267 733a 2041 6e79 2920 2d3e  *kwargs: Any) ->
-00005360: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00005370: 2020 2065 7272 5f6c 696e 6573 2e61 7070     err_lines.app
-00005380: 656e 6428 6d73 6729 0a0a 2020 2020 2020  end(msg)..      
-00005390: 2020 7769 7468 2070 6174 6368 2822 6365    with patch("ce
-000053a0: 7263 6973 2e6f 7574 7075 742e 5f6f 7574  rcis.output._out
-000053b0: 222c 206f 7574 292c 2070 6174 6368 2822  ", out), patch("
-000053c0: 6365 7263 6973 2e6f 7574 7075 742e 5f65  cercis.output._e
-000053d0: 7272 222c 2065 7272 293a 0a20 2020 2020  rr", err):.     
-000053e0: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
-000053f0: 6e65 2850 6174 6828 2266 3122 292c 2063  ne(Path("f1"), c
-00005400: 6572 6369 732e 4368 616e 6765 642e 4e4f  ercis.Changed.NO
-00005410: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00005420: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00005430: 656e 286f 7574 5f6c 696e 6573 292c 2031  en(out_lines), 1
-00005440: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00005450: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00005460: 656e 2865 7272 5f6c 696e 6573 292c 2030  en(err_lines), 0
-00005470: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00005480: 6c66 2e61 7373 6572 7445 7175 616c 286f  lf.assertEqual(o
-00005490: 7574 5f6c 696e 6573 5b2d 315d 2c20 2266  ut_lines[-1], "f
-000054a0: 3120 616c 7265 6164 7920 7765 6c6c 2066  1 already well f
-000054b0: 6f72 6d61 7474 6564 2c20 676f 6f64 206a  ormatted, good j
-000054c0: 6f62 2e22 290a 2020 2020 2020 2020 2020  ob.").          
-000054d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000054e0: 616c 2875 6e73 7479 6c65 2873 7472 2872  al(unstyle(str(r
-000054f0: 6570 6f72 7429 292c 2022 3120 6669 6c65  eport)), "1 file
-00005500: 206c 6566 7420 756e 6368 616e 6765 642e   left unchanged.
-00005510: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00005520: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00005530: 7265 706f 7274 2e72 6574 7572 6e5f 636f  report.return_co
-00005540: 6465 2c20 3029 0a20 2020 2020 2020 2020  de, 0).         
-00005550: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
-00005560: 6174 6828 2266 3222 292c 2063 6572 6369  ath("f2"), cerci
-00005570: 732e 4368 616e 6765 642e 5945 5329 0a20  s.Changed.YES). 
-00005580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005590: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-000055a0: 6f75 745f 6c69 6e65 7329 2c20 3229 0a20  out_lines), 2). 
-000055b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000055c0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-000055d0: 6572 725f 6c69 6e65 7329 2c20 3029 0a20  err_lines), 0). 
-000055e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000055f0: 6173 7365 7274 4571 7561 6c28 6f75 745f  assertEqual(out_
-00005600: 6c69 6e65 735b 2d31 5d2c 2022 7265 666f  lines[-1], "refo
-00005610: 726d 6174 7465 6420 6632 2229 0a20 2020  rmatted f2").   
-00005620: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00005630: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-00005640: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
-00005650: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
-00005660: 2022 3120 6669 6c65 2072 6566 6f72 6d61   "1 file reforma
-00005670: 7474 6564 2c20 3120 6669 6c65 206c 6566  tted, 1 file lef
-00005680: 7420 756e 6368 616e 6765 642e 220a 2020  t unchanged.".  
-00005690: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000056a0: 2020 2020 2020 2020 7265 706f 7274 2e64          report.d
-000056b0: 6f6e 6528 5061 7468 2822 6633 2229 2c20  one(Path("f3"), 
-000056c0: 6365 7263 6973 2e43 6861 6e67 6564 2e43  cercis.Changed.C
-000056d0: 4143 4845 4429 0a20 2020 2020 2020 2020  ACHED).         
-000056e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000056f0: 7561 6c28 6c65 6e28 6f75 745f 6c69 6e65  ual(len(out_line
-00005700: 7329 2c20 3329 0a20 2020 2020 2020 2020  s), 3).         
-00005710: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00005720: 7561 6c28 6c65 6e28 6572 725f 6c69 6e65  ual(len(err_line
-00005730: 7329 2c20 3029 0a20 2020 2020 2020 2020  s), 0).         
-00005740: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00005750: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
-00005760: 2020 2020 206f 7574 5f6c 696e 6573 5b2d       out_lines[-
-00005770: 315d 2c20 2266 3320 7761 736e 2774 206d  1], "f3 wasn't m
-00005780: 6f64 6966 6965 6420 6f6e 2064 6973 6b20  odified on disk 
-00005790: 7369 6e63 6520 6c61 7374 2072 756e 2e22  since last run."
-000057a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000057b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000057c0: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-000057d0: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
-000057e0: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
-000057f0: 292c 2022 3120 6669 6c65 2072 6566 6f72  ), "1 file refor
-00005800: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
-00005810: 6c65 6674 2075 6e63 6861 6e67 6564 2e22  left unchanged."
-00005820: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00005830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005840: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
-00005850: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
-00005860: 3029 0a20 2020 2020 2020 2020 2020 2072  0).            r
-00005870: 6570 6f72 742e 6368 6563 6b20 3d20 5472  eport.check = Tr
-00005880: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
-00005890: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000058a0: 7265 706f 7274 2e72 6574 7572 6e5f 636f  report.return_co
-000058b0: 6465 2c20 3129 0a20 2020 2020 2020 2020  de, 1).         
-000058c0: 2020 2072 6570 6f72 742e 6368 6563 6b20     report.check 
-000058d0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-000058e0: 2020 2020 7265 706f 7274 2e66 6169 6c65      report.faile
-000058f0: 6428 5061 7468 2822 6531 2229 2c20 2262  d(Path("e1"), "b
-00005900: 6f6f 6d22 290a 2020 2020 2020 2020 2020  oom").          
-00005910: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00005920: 616c 286c 656e 286f 7574 5f6c 696e 6573  al(len(out_lines
-00005930: 292c 2033 290a 2020 2020 2020 2020 2020  ), 3).          
-00005940: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00005950: 616c 286c 656e 2865 7272 5f6c 696e 6573  al(len(err_lines
-00005960: 292c 2031 290a 2020 2020 2020 2020 2020  ), 1).          
-00005970: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00005980: 616c 2865 7272 5f6c 696e 6573 5b2d 315d  al(err_lines[-1]
-00005990: 2c20 2265 7272 6f72 3a20 6361 6e6e 6f74  , "error: cannot
-000059a0: 2066 6f72 6d61 7420 6531 3a20 626f 6f6d   format e1: boom
-000059b0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-000059c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000059d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059e0: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
-000059f0: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
-00005a00: 2020 2020 2020 2022 3120 6669 6c65 2072         "1 file r
-00005a10: 6566 6f72 6d61 7474 6564 2c20 3220 6669  eformatted, 2 fi
-00005a20: 6c65 7320 6c65 6674 2075 6e63 6861 6e67  les left unchang
-00005a30: 6564 2c20 3120 6669 6c65 2066 6169 6c65  ed, 1 file faile
-00005a40: 6420 746f 220a 2020 2020 2020 2020 2020  d to".          
-00005a50: 2020 2020 2020 2220 7265 666f 726d 6174        " reformat
-00005a60: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00005a70: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00005a80: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00005a90: 6570 6f72 742e 7265 7475 726e 5f63 6f64  eport.return_cod
-00005aa0: 652c 2031 3233 290a 2020 2020 2020 2020  e, 123).        
-00005ab0: 2020 2020 7265 706f 7274 2e64 6f6e 6528      report.done(
-00005ac0: 5061 7468 2822 6633 2229 2c20 6365 7263  Path("f3"), cerc
-00005ad0: 6973 2e43 6861 6e67 6564 2e59 4553 290a  is.Changed.YES).
-00005ae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005af0: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00005b00: 286f 7574 5f6c 696e 6573 292c 2034 290a  (out_lines), 4).
-00005b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005b20: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00005b30: 2865 7272 5f6c 696e 6573 292c 2031 290a  (err_lines), 1).
-00005b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005b50: 2e61 7373 6572 7445 7175 616c 286f 7574  .assertEqual(out
-00005b60: 5f6c 696e 6573 5b2d 315d 2c20 2272 6566  _lines[-1], "ref
-00005b70: 6f72 6d61 7474 6564 2066 3322 290a 2020  ormatted f3").  
-00005b80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00005b90: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00005ba0: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-00005bb0: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00005bc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005bd0: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
-00005be0: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
-00005bf0: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
-00005c00: 3120 6669 6c65 2066 6169 6c65 6420 746f  1 file failed to
-00005c10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00005c20: 2020 2220 7265 666f 726d 6174 2e22 2c0a    " reformat.",.
-00005c30: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00005c40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00005c50: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
-00005c60: 742e 7265 7475 726e 5f63 6f64 652c 2031  t.return_code, 1
-00005c70: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
-00005c80: 7265 706f 7274 2e66 6169 6c65 6428 5061  report.failed(Pa
-00005c90: 7468 2822 6532 2229 2c20 2262 6f6f 6d22  th("e2"), "boom"
-00005ca0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00005cb0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00005cc0: 656e 286f 7574 5f6c 696e 6573 292c 2034  en(out_lines), 4
-00005cd0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00005ce0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00005cf0: 656e 2865 7272 5f6c 696e 6573 292c 2032  en(err_lines), 2
-00005d00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00005d10: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-00005d20: 7272 5f6c 696e 6573 5b2d 315d 2c20 2265  rr_lines[-1], "e
-00005d30: 7272 6f72 3a20 6361 6e6e 6f74 2066 6f72  rror: cannot for
-00005d40: 6d61 7420 6532 3a20 626f 6f6d 2229 0a20  mat e2: boom"). 
-00005d50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005d60: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00005d70: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
-00005d80: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
-00005d90: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00005da0: 2020 2022 3220 6669 6c65 7320 7265 666f     "2 files refo
-00005db0: 726d 6174 7465 642c 2032 2066 696c 6573  rmatted, 2 files
-00005dc0: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
-00005dd0: 2032 2066 696c 6573 2066 6169 6c65 6420   2 files failed 
-00005de0: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
-00005df0: 2020 2020 2220 7265 666f 726d 6174 2e22      " reformat."
-00005e00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00005e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005e20: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
-00005e30: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
-00005e40: 2031 3233 290a 2020 2020 2020 2020 2020   123).          
-00005e50: 2020 7265 706f 7274 2e70 6174 685f 6967    report.path_ig
-00005e60: 6e6f 7265 6428 5061 7468 2822 7761 7422  nored(Path("wat"
-00005e70: 292c 2022 6e6f 206d 6174 6368 2229 0a20  ), "no match"). 
-00005e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005e90: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-00005ea0: 6f75 745f 6c69 6e65 7329 2c20 3529 0a20  out_lines), 5). 
-00005eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005ec0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-00005ed0: 6572 725f 6c69 6e65 7329 2c20 3229 0a20  err_lines), 2). 
-00005ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005ef0: 6173 7365 7274 4571 7561 6c28 6f75 745f  assertEqual(out_
-00005f00: 6c69 6e65 735b 2d31 5d2c 2022 7761 7420  lines[-1], "wat 
-00005f10: 6967 6e6f 7265 643a 206e 6f20 6d61 7463  ignored: no matc
-00005f20: 6822 290a 2020 2020 2020 2020 2020 2020  h").            
-00005f30: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00005f40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00005f50: 2020 756e 7374 796c 6528 7374 7228 7265    unstyle(str(re
-00005f60: 706f 7274 2929 2c0a 2020 2020 2020 2020  port)),.        
-00005f70: 2020 2020 2020 2020 2232 2066 696c 6573          "2 files
-00005f80: 2072 6566 6f72 6d61 7474 6564 2c20 3220   reformatted, 2 
-00005f90: 6669 6c65 7320 6c65 6674 2075 6e63 6861  files left uncha
-00005fa0: 6e67 6564 2c20 3220 6669 6c65 7320 6661  nged, 2 files fa
-00005fb0: 696c 6564 2074 6f22 0a20 2020 2020 2020  iled to".       
-00005fc0: 2020 2020 2020 2020 2022 2072 6566 6f72           " refor
-00005fd0: 6d61 742e 222c 0a20 2020 2020 2020 2020  mat.",.         
-00005fe0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00005ff0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00006000: 6c28 7265 706f 7274 2e72 6574 7572 6e5f  l(report.return_
-00006010: 636f 6465 2c20 3132 3329 0a20 2020 2020  code, 123).     
-00006020: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
-00006030: 6e65 2850 6174 6828 2266 3422 292c 2063  ne(Path("f4"), c
-00006040: 6572 6369 732e 4368 616e 6765 642e 4e4f  ercis.Changed.NO
-00006050: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006060: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00006070: 656e 286f 7574 5f6c 696e 6573 292c 2036  en(out_lines), 6
-00006080: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006090: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-000060a0: 656e 2865 7272 5f6c 696e 6573 292c 2032  en(err_lines), 2
-000060b0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000060c0: 6c66 2e61 7373 6572 7445 7175 616c 286f  lf.assertEqual(o
-000060d0: 7574 5f6c 696e 6573 5b2d 315d 2c20 2266  ut_lines[-1], "f
-000060e0: 3420 616c 7265 6164 7920 7765 6c6c 2066  4 already well f
-000060f0: 6f72 6d61 7474 6564 2c20 676f 6f64 206a  ormatted, good j
-00006100: 6f62 2e22 290a 2020 2020 2020 2020 2020  ob.").          
-00006110: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00006120: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00006130: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
-00006140: 7265 706f 7274 2929 2c0a 2020 2020 2020  report)),.      
-00006150: 2020 2020 2020 2020 2020 2232 2066 696c            "2 fil
-00006160: 6573 2072 6566 6f72 6d61 7474 6564 2c20  es reformatted, 
-00006170: 3320 6669 6c65 7320 6c65 6674 2075 6e63  3 files left unc
-00006180: 6861 6e67 6564 2c20 3220 6669 6c65 7320  hanged, 2 files 
-00006190: 6661 696c 6564 2074 6f22 0a20 2020 2020  failed to".     
-000061a0: 2020 2020 2020 2020 2020 2022 2072 6566             " ref
-000061b0: 6f72 6d61 742e 222c 0a20 2020 2020 2020  ormat.",.       
-000061c0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000061d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000061e0: 7561 6c28 7265 706f 7274 2e72 6574 7572  ual(report.retur
-000061f0: 6e5f 636f 6465 2c20 3132 3329 0a20 2020  n_code, 123).   
-00006200: 2020 2020 2020 2020 2072 6570 6f72 742e           report.
-00006210: 6368 6563 6b20 3d20 5472 7565 0a20 2020  check = True.   
-00006220: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00006230: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-00006240: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
-00006250: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
-00006260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006270: 2022 3220 6669 6c65 7320 776f 756c 6420   "2 files would 
-00006280: 6265 2072 6566 6f72 6d61 7474 6564 2c20  be reformatted, 
-00006290: 3320 6669 6c65 7320 776f 756c 6420 6265  3 files would be
-000062a0: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
-000062b0: 2032 220a 2020 2020 2020 2020 2020 2020   2".            
-000062c0: 2020 2020 2220 6669 6c65 7320 776f 756c      " files woul
-000062d0: 6420 6661 696c 2074 6f20 7265 666f 726d  d fail to reform
-000062e0: 6174 2e22 2c0a 2020 2020 2020 2020 2020  at.",.          
-000062f0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00006300: 7265 706f 7274 2e63 6865 636b 203d 2046  report.check = F
-00006310: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00006320: 2072 6570 6f72 742e 6469 6666 203d 2054   report.diff = T
-00006330: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00006340: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00006350: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00006360: 2020 756e 7374 796c 6528 7374 7228 7265    unstyle(str(re
-00006370: 706f 7274 2929 2c0a 2020 2020 2020 2020  port)),.        
-00006380: 2020 2020 2020 2020 2232 2066 696c 6573          "2 files
-00006390: 2077 6f75 6c64 2062 6520 7265 666f 726d   would be reform
-000063a0: 6174 7465 642c 2033 2066 696c 6573 2077  atted, 3 files w
-000063b0: 6f75 6c64 2062 6520 6c65 6674 2075 6e63  ould be left unc
-000063c0: 6861 6e67 6564 2c20 3222 0a20 2020 2020  hanged, 2".     
-000063d0: 2020 2020 2020 2020 2020 2022 2066 696c             " fil
-000063e0: 6573 2077 6f75 6c64 2066 6169 6c20 746f  es would fail to
-000063f0: 2072 6566 6f72 6d61 742e 222c 0a20 2020   reformat.",.   
-00006400: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00006410: 6465 6620 7465 7374 5f72 6570 6f72 745f  def test_report_
-00006420: 7175 6965 7428 7365 6c66 2920 2d3e 204e  quiet(self) -> N
-00006430: 6f6e 653a 0a20 2020 2020 2020 2072 6570  one:.        rep
-00006440: 6f72 7420 3d20 5265 706f 7274 2871 7569  ort = Report(qui
-00006450: 6574 3d54 7275 6529 0a20 2020 2020 2020  et=True).       
-00006460: 206f 7574 5f6c 696e 6573 203d 205b 5d0a   out_lines = [].
-00006470: 2020 2020 2020 2020 6572 725f 6c69 6e65          err_line
-00006480: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
-00006490: 6465 6620 6f75 7428 6d73 673a 2073 7472  def out(msg: str
-000064a0: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
-000064b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000064c0: 2020 2020 2020 6f75 745f 6c69 6e65 732e        out_lines.
-000064d0: 6170 7065 6e64 286d 7367 290a 0a20 2020  append(msg)..   
-000064e0: 2020 2020 2064 6566 2065 7272 286d 7367       def err(msg
-000064f0: 3a20 7374 722c 202a 2a6b 7761 7267 733a  : str, **kwargs:
-00006500: 2041 6e79 2920 2d3e 204e 6f6e 653a 0a20   Any) -> None:. 
-00006510: 2020 2020 2020 2020 2020 2065 7272 5f6c             err_l
-00006520: 696e 6573 2e61 7070 656e 6428 6d73 6729  ines.append(msg)
-00006530: 0a0a 2020 2020 2020 2020 7769 7468 2070  ..        with p
-00006540: 6174 6368 2822 6365 7263 6973 2e6f 7574  atch("cercis.out
-00006550: 7075 742e 5f6f 7574 222c 206f 7574 292c  put._out", out),
-00006560: 2070 6174 6368 2822 6365 7263 6973 2e6f   patch("cercis.o
-00006570: 7574 7075 742e 5f65 7272 222c 2065 7272  utput._err", err
-00006580: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00006590: 6570 6f72 742e 646f 6e65 2850 6174 6828  eport.done(Path(
-000065a0: 2266 3122 292c 2063 6572 6369 732e 4368  "f1"), cercis.Ch
-000065b0: 616e 6765 642e 4e4f 290a 2020 2020 2020  anged.NO).      
-000065c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000065d0: 7445 7175 616c 286c 656e 286f 7574 5f6c  tEqual(len(out_l
-000065e0: 696e 6573 292c 2030 290a 2020 2020 2020  ines), 0).      
-000065f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00006600: 7445 7175 616c 286c 656e 2865 7272 5f6c  tEqual(len(err_l
-00006610: 696e 6573 292c 2030 290a 2020 2020 2020  ines), 0).      
-00006620: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00006630: 7445 7175 616c 2875 6e73 7479 6c65 2873  tEqual(unstyle(s
-00006640: 7472 2872 6570 6f72 7429 292c 2022 3120  tr(report)), "1 
-00006650: 6669 6c65 206c 6566 7420 756e 6368 616e  file left unchan
-00006660: 6765 642e 2229 0a20 2020 2020 2020 2020  ged.").         
-00006670: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00006680: 7561 6c28 7265 706f 7274 2e72 6574 7572  ual(report.retur
-00006690: 6e5f 636f 6465 2c20 3029 0a20 2020 2020  n_code, 0).     
-000066a0: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
-000066b0: 6e65 2850 6174 6828 2266 3222 292c 2063  ne(Path("f2"), c
-000066c0: 6572 6369 732e 4368 616e 6765 642e 5945  ercis.Changed.YE
-000066d0: 5329 0a20 2020 2020 2020 2020 2020 2073  S).            s
-000066e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000066f0: 6c65 6e28 6f75 745f 6c69 6e65 7329 2c20  len(out_lines), 
-00006700: 3029 0a20 2020 2020 2020 2020 2020 2073  0).            s
-00006710: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00006720: 6c65 6e28 6572 725f 6c69 6e65 7329 2c20  len(err_lines), 
-00006730: 3029 0a20 2020 2020 2020 2020 2020 2073  0).            s
-00006740: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00006750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006760: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
-00006770: 6f72 7429 292c 2022 3120 6669 6c65 2072  ort)), "1 file r
-00006780: 6566 6f72 6d61 7474 6564 2c20 3120 6669  eformatted, 1 fi
-00006790: 6c65 206c 6566 7420 756e 6368 616e 6765  le left unchange
-000067a0: 642e 220a 2020 2020 2020 2020 2020 2020  d.".            
-000067b0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000067c0: 706f 7274 2e64 6f6e 6528 5061 7468 2822  port.done(Path("
-000067d0: 6633 2229 2c20 6365 7263 6973 2e43 6861  f3"), cercis.Cha
-000067e0: 6e67 6564 2e43 4143 4845 4429 0a20 2020  nged.CACHED).   
-000067f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00006800: 7365 7274 4571 7561 6c28 6c65 6e28 6f75  sertEqual(len(ou
-00006810: 745f 6c69 6e65 7329 2c20 3029 0a20 2020  t_lines), 0).   
-00006820: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00006830: 7365 7274 4571 7561 6c28 6c65 6e28 6572  sertEqual(len(er
-00006840: 725f 6c69 6e65 7329 2c20 3029 0a20 2020  r_lines), 0).   
-00006850: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00006860: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-00006870: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
-00006880: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
-00006890: 2022 3120 6669 6c65 2072 6566 6f72 6d61   "1 file reforma
-000068a0: 7474 6564 2c20 3220 6669 6c65 7320 6c65  tted, 2 files le
-000068b0: 6674 2075 6e63 6861 6e67 6564 2e22 0a20  ft unchanged.". 
-000068c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000068d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000068e0: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
-000068f0: 2e72 6574 7572 6e5f 636f 6465 2c20 3029  .return_code, 0)
-00006900: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00006910: 6f72 742e 6368 6563 6b20 3d20 5472 7565  ort.check = True
-00006920: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006930: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-00006940: 706f 7274 2e72 6574 7572 6e5f 636f 6465  port.return_code
-00006950: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-00006960: 2072 6570 6f72 742e 6368 6563 6b20 3d20   report.check = 
-00006970: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00006980: 2020 7265 706f 7274 2e66 6169 6c65 6428    report.failed(
-00006990: 5061 7468 2822 6531 2229 2c20 2262 6f6f  Path("e1"), "boo
-000069a0: 6d22 290a 2020 2020 2020 2020 2020 2020  m").            
-000069b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000069c0: 286c 656e 286f 7574 5f6c 696e 6573 292c  (len(out_lines),
-000069d0: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
-000069e0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000069f0: 286c 656e 2865 7272 5f6c 696e 6573 292c  (len(err_lines),
-00006a00: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
-00006a10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00006a20: 2865 7272 5f6c 696e 6573 5b2d 315d 2c20  (err_lines[-1], 
-00006a30: 2265 7272 6f72 3a20 6361 6e6e 6f74 2066  "error: cannot f
-00006a40: 6f72 6d61 7420 6531 3a20 626f 6f6d 2229  ormat e1: boom")
-00006a50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006a60: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00006a80: 6e73 7479 6c65 2873 7472 2872 6570 6f72  nstyle(str(repor
-00006a90: 7429 292c 0a20 2020 2020 2020 2020 2020  t)),.           
-00006aa0: 2020 2020 2022 3120 6669 6c65 2072 6566       "1 file ref
-00006ab0: 6f72 6d61 7474 6564 2c20 3220 6669 6c65  ormatted, 2 file
-00006ac0: 7320 6c65 6674 2075 6e63 6861 6e67 6564  s left unchanged
-00006ad0: 2c20 3120 6669 6c65 2066 6169 6c65 6420  , 1 file failed 
-00006ae0: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
-00006af0: 2020 2020 2220 7265 666f 726d 6174 2e22      " reformat."
-00006b00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00006b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006b20: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
-00006b30: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
-00006b40: 2031 3233 290a 2020 2020 2020 2020 2020   123).          
-00006b50: 2020 7265 706f 7274 2e64 6f6e 6528 5061    report.done(Pa
-00006b60: 7468 2822 6633 2229 2c20 6365 7263 6973  th("f3"), cercis
-00006b70: 2e43 6861 6e67 6564 2e59 4553 290a 2020  .Changed.YES).  
-00006b80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006b90: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
-00006ba0: 7574 5f6c 696e 6573 292c 2030 290a 2020  ut_lines), 0).  
-00006bb0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006bc0: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
-00006bd0: 7272 5f6c 696e 6573 292c 2031 290a 2020  rr_lines), 1).  
-00006be0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006bf0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00006c00: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-00006c10: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00006c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006c30: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
-00006c40: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
-00006c50: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
-00006c60: 3120 6669 6c65 2066 6169 6c65 6420 746f  1 file failed to
-00006c70: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00006c80: 2020 2220 7265 666f 726d 6174 2e22 2c0a    " reformat.",.
-00006c90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00006ca0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006cb0: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
-00006cc0: 742e 7265 7475 726e 5f63 6f64 652c 2031  t.return_code, 1
-00006cd0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
-00006ce0: 7265 706f 7274 2e66 6169 6c65 6428 5061  report.failed(Pa
-00006cf0: 7468 2822 6532 2229 2c20 2262 6f6f 6d22  th("e2"), "boom"
-00006d00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006d10: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00006d20: 656e 286f 7574 5f6c 696e 6573 292c 2030  en(out_lines), 0
-00006d30: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006d40: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00006d50: 656e 2865 7272 5f6c 696e 6573 292c 2032  en(err_lines), 2
-00006d60: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006d70: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-00006d80: 7272 5f6c 696e 6573 5b2d 315d 2c20 2265  rr_lines[-1], "e
-00006d90: 7272 6f72 3a20 6361 6e6e 6f74 2066 6f72  rror: cannot for
-00006da0: 6d61 7420 6532 3a20 626f 6f6d 2229 0a20  mat e2: boom"). 
-00006db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006dc0: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00006dd0: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
-00006de0: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
-00006df0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00006e00: 2020 2022 3220 6669 6c65 7320 7265 666f     "2 files refo
-00006e10: 726d 6174 7465 642c 2032 2066 696c 6573  rmatted, 2 files
-00006e20: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
-00006e30: 2032 2066 696c 6573 2066 6169 6c65 6420   2 files failed 
-00006e40: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
-00006e50: 2020 2020 2220 7265 666f 726d 6174 2e22      " reformat."
-00006e60: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00006e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006e80: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
-00006e90: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
-00006ea0: 2031 3233 290a 2020 2020 2020 2020 2020   123).          
-00006eb0: 2020 7265 706f 7274 2e70 6174 685f 6967    report.path_ig
-00006ec0: 6e6f 7265 6428 5061 7468 2822 7761 7422  nored(Path("wat"
-00006ed0: 292c 2022 6e6f 206d 6174 6368 2229 0a20  ), "no match"). 
-00006ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006ef0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-00006f00: 6f75 745f 6c69 6e65 7329 2c20 3029 0a20  out_lines), 0). 
-00006f10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006f20: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-00006f30: 6572 725f 6c69 6e65 7329 2c20 3229 0a20  err_lines), 2). 
-00006f40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006f50: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00006f60: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
-00006f70: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
-00006f80: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00006f90: 2020 2022 3220 6669 6c65 7320 7265 666f     "2 files refo
-00006fa0: 726d 6174 7465 642c 2032 2066 696c 6573  rmatted, 2 files
-00006fb0: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
-00006fc0: 2032 2066 696c 6573 2066 6169 6c65 6420   2 files failed 
-00006fd0: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
-00006fe0: 2020 2020 2220 7265 666f 726d 6174 2e22      " reformat."
-00006ff0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00007000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007010: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
-00007020: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
-00007030: 2031 3233 290a 2020 2020 2020 2020 2020   123).          
-00007040: 2020 7265 706f 7274 2e64 6f6e 6528 5061    report.done(Pa
-00007050: 7468 2822 6634 2229 2c20 6365 7263 6973  th("f4"), cercis
-00007060: 2e43 6861 6e67 6564 2e4e 4f29 0a20 2020  .Changed.NO).   
-00007070: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00007080: 7365 7274 4571 7561 6c28 6c65 6e28 6f75  sertEqual(len(ou
-00007090: 745f 6c69 6e65 7329 2c20 3029 0a20 2020  t_lines), 0).   
-000070a0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000070b0: 7365 7274 4571 7561 6c28 6c65 6e28 6572  sertEqual(len(er
-000070c0: 725f 6c69 6e65 7329 2c20 3229 0a20 2020  r_lines), 2).   
-000070d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000070e0: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-000070f0: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
-00007100: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
-00007110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007120: 2022 3220 6669 6c65 7320 7265 666f 726d   "2 files reform
-00007130: 6174 7465 642c 2033 2066 696c 6573 206c  atted, 3 files l
-00007140: 6566 7420 756e 6368 616e 6765 642c 2032  eft unchanged, 2
-00007150: 2066 696c 6573 2066 6169 6c65 6420 746f   files failed to
-00007160: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00007170: 2020 2220 7265 666f 726d 6174 2e22 2c0a    " reformat.",.
-00007180: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007190: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000071a0: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
-000071b0: 742e 7265 7475 726e 5f63 6f64 652c 2031  t.return_code, 1
-000071c0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
-000071d0: 7265 706f 7274 2e63 6865 636b 203d 2054  report.check = T
-000071e0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-000071f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00007200: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00007210: 2020 756e 7374 796c 6528 7374 7228 7265    unstyle(str(re
-00007220: 706f 7274 2929 2c0a 2020 2020 2020 2020  port)),.        
-00007230: 2020 2020 2020 2020 2232 2066 696c 6573          "2 files
-00007240: 2077 6f75 6c64 2062 6520 7265 666f 726d   would be reform
-00007250: 6174 7465 642c 2033 2066 696c 6573 2077  atted, 3 files w
-00007260: 6f75 6c64 2062 6520 6c65 6674 2075 6e63  ould be left unc
-00007270: 6861 6e67 6564 2c20 3222 0a20 2020 2020  hanged, 2".     
-00007280: 2020 2020 2020 2020 2020 2022 2066 696c             " fil
-00007290: 6573 2077 6f75 6c64 2066 6169 6c20 746f  es would fail to
-000072a0: 2072 6566 6f72 6d61 742e 222c 0a20 2020   reformat.",.   
-000072b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000072c0: 2020 2020 2020 2072 6570 6f72 742e 6368         report.ch
-000072d0: 6563 6b20 3d20 4661 6c73 650a 2020 2020  eck = False.    
-000072e0: 2020 2020 2020 2020 7265 706f 7274 2e64          report.d
-000072f0: 6966 6620 3d20 5472 7565 0a20 2020 2020  iff = True.     
-00007300: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007310: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
-00007320: 2020 2020 2020 2020 2075 6e73 7479 6c65           unstyle
-00007330: 2873 7472 2872 6570 6f72 7429 292c 0a20  (str(report)),. 
-00007340: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007350: 3220 6669 6c65 7320 776f 756c 6420 6265  2 files would be
-00007360: 2072 6566 6f72 6d61 7474 6564 2c20 3320   reformatted, 3 
-00007370: 6669 6c65 7320 776f 756c 6420 6265 206c  files would be l
-00007380: 6566 7420 756e 6368 616e 6765 642c 2032  eft unchanged, 2
-00007390: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000073a0: 2020 2220 6669 6c65 7320 776f 756c 6420    " files would 
-000073b0: 6661 696c 2074 6f20 7265 666f 726d 6174  fail to reformat
-000073c0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-000073d0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-000073e0: 7265 706f 7274 5f6e 6f72 6d61 6c28 7365  report_normal(se
-000073f0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00007400: 2020 2020 2072 6570 6f72 7420 3d20 6365       report = ce
-00007410: 7263 6973 2e52 6570 6f72 7428 290a 2020  rcis.Report().  
-00007420: 2020 2020 2020 6f75 745f 6c69 6e65 7320        out_lines 
-00007430: 3d20 5b5d 0a20 2020 2020 2020 2065 7272  = [].        err
-00007440: 5f6c 696e 6573 203d 205b 5d0a 0a20 2020  _lines = []..   
-00007450: 2020 2020 2064 6566 206f 7574 286d 7367       def out(msg
-00007460: 3a20 7374 722c 202a 2a6b 7761 7267 733a  : str, **kwargs:
-00007470: 2041 6e79 2920 2d3e 204e 6f6e 653a 0a20   Any) -> None:. 
-00007480: 2020 2020 2020 2020 2020 206f 7574 5f6c             out_l
-00007490: 696e 6573 2e61 7070 656e 6428 6d73 6729  ines.append(msg)
-000074a0: 0a0a 2020 2020 2020 2020 6465 6620 6572  ..        def er
-000074b0: 7228 6d73 673a 2073 7472 2c20 2a2a 6b77  r(msg: str, **kw
-000074c0: 6172 6773 3a20 416e 7929 202d 3e20 4e6f  args: Any) -> No
-000074d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000074e0: 6572 725f 6c69 6e65 732e 6170 7065 6e64  err_lines.append
-000074f0: 286d 7367 290a 0a20 2020 2020 2020 2077  (msg)..        w
-00007500: 6974 6820 7061 7463 6828 2263 6572 6369  ith patch("cerci
-00007510: 732e 6f75 7470 7574 2e5f 6f75 7422 2c20  s.output._out", 
-00007520: 6f75 7429 2c20 7061 7463 6828 2263 6572  out), patch("cer
-00007530: 6369 732e 6f75 7470 7574 2e5f 6572 7222  cis.output._err"
-00007540: 2c20 6572 7229 3a0a 2020 2020 2020 2020  , err):.        
-00007550: 2020 2020 7265 706f 7274 2e64 6f6e 6528      report.done(
-00007560: 5061 7468 2822 6631 2229 2c20 6365 7263  Path("f1"), cerc
-00007570: 6973 2e43 6861 6e67 6564 2e4e 4f29 0a20  is.Changed.NO). 
-00007580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007590: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-000075a0: 6f75 745f 6c69 6e65 7329 2c20 3029 0a20  out_lines), 0). 
-000075b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000075c0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-000075d0: 6572 725f 6c69 6e65 7329 2c20 3029 0a20  err_lines), 0). 
-000075e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000075f0: 6173 7365 7274 4571 7561 6c28 756e 7374  assertEqual(unst
-00007600: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00007610: 2c20 2231 2066 696c 6520 6c65 6674 2075  , "1 file left u
-00007620: 6e63 6861 6e67 6564 2e22 290a 2020 2020  nchanged.").    
-00007630: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00007640: 6572 7445 7175 616c 2872 6570 6f72 742e  ertEqual(report.
-00007650: 7265 7475 726e 5f63 6f64 652c 2030 290a  return_code, 0).
-00007660: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00007670: 7274 2e64 6f6e 6528 5061 7468 2822 6632  rt.done(Path("f2
-00007680: 2229 2c20 6365 7263 6973 2e43 6861 6e67  "), cercis.Chang
-00007690: 6564 2e59 4553 290a 2020 2020 2020 2020  ed.YES).        
-000076a0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000076b0: 7175 616c 286c 656e 286f 7574 5f6c 696e  qual(len(out_lin
-000076c0: 6573 292c 2031 290a 2020 2020 2020 2020  es), 1).        
-000076d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000076e0: 7175 616c 286c 656e 2865 7272 5f6c 696e  qual(len(err_lin
-000076f0: 6573 292c 2030 290a 2020 2020 2020 2020  es), 0).        
-00007700: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00007710: 7175 616c 286f 7574 5f6c 696e 6573 5b2d  qual(out_lines[-
-00007720: 315d 2c20 2272 6566 6f72 6d61 7474 6564  1], "reformatted
-00007730: 2066 3222 290a 2020 2020 2020 2020 2020   f2").          
-00007740: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007750: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00007760: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
-00007770: 7265 706f 7274 2929 2c20 2231 2066 696c  report)), "1 fil
-00007780: 6520 7265 666f 726d 6174 7465 642c 2031  e reformatted, 1
-00007790: 2066 696c 6520 6c65 6674 2075 6e63 6861   file left uncha
-000077a0: 6e67 6564 2e22 0a20 2020 2020 2020 2020  nged.".         
-000077b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000077c0: 2072 6570 6f72 742e 646f 6e65 2850 6174   report.done(Pat
-000077d0: 6828 2266 3322 292c 2063 6572 6369 732e  h("f3"), cercis.
-000077e0: 4368 616e 6765 642e 4341 4348 4544 290a  Changed.CACHED).
-000077f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007800: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00007810: 286f 7574 5f6c 696e 6573 292c 2031 290a  (out_lines), 1).
-00007820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007830: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00007840: 2865 7272 5f6c 696e 6573 292c 2030 290a  (err_lines), 0).
-00007850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007860: 2e61 7373 6572 7445 7175 616c 286f 7574  .assertEqual(out
-00007870: 5f6c 696e 6573 5b2d 315d 2c20 2272 6566  _lines[-1], "ref
-00007880: 6f72 6d61 7474 6564 2066 3222 290a 2020  ormatted f2").  
-00007890: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000078a0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-000078b0: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-000078c0: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-000078d0: 2c20 2231 2066 696c 6520 7265 666f 726d  , "1 file reform
-000078e0: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
-000078f0: 6566 7420 756e 6368 616e 6765 642e 220a  eft unchanged.".
-00007900: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007910: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00007920: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
-00007930: 742e 7265 7475 726e 5f63 6f64 652c 2030  t.return_code, 0
-00007940: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00007950: 706f 7274 2e63 6865 636b 203d 2054 7275  port.check = Tru
-00007960: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-00007970: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00007980: 6570 6f72 742e 7265 7475 726e 5f63 6f64  eport.return_cod
-00007990: 652c 2031 290a 2020 2020 2020 2020 2020  e, 1).          
-000079a0: 2020 7265 706f 7274 2e63 6865 636b 203d    report.check =
-000079b0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-000079c0: 2020 2072 6570 6f72 742e 6661 696c 6564     report.failed
-000079d0: 2850 6174 6828 2265 3122 292c 2022 626f  (Path("e1"), "bo
-000079e0: 6f6d 2229 0a20 2020 2020 2020 2020 2020  om").           
-000079f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00007a00: 6c28 6c65 6e28 6f75 745f 6c69 6e65 7329  l(len(out_lines)
-00007a10: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-00007a20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00007a30: 6c28 6c65 6e28 6572 725f 6c69 6e65 7329  l(len(err_lines)
-00007a40: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-00007a50: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00007a60: 6c28 6572 725f 6c69 6e65 735b 2d31 5d2c  l(err_lines[-1],
-00007a70: 2022 6572 726f 723a 2063 616e 6e6f 7420   "error: cannot 
-00007a80: 666f 726d 6174 2065 313a 2062 6f6f 6d22  format e1: boom"
-00007a90: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00007aa0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
-00007ad0: 7274 2929 2c0a 2020 2020 2020 2020 2020  rt)),.          
-00007ae0: 2020 2020 2020 2231 2066 696c 6520 7265        "1 file re
-00007af0: 666f 726d 6174 7465 642c 2032 2066 696c  formatted, 2 fil
-00007b00: 6573 206c 6566 7420 756e 6368 616e 6765  es left unchange
-00007b10: 642c 2031 2066 696c 6520 6661 696c 6564  d, 1 file failed
-00007b20: 2074 6f22 0a20 2020 2020 2020 2020 2020   to".           
-00007b30: 2020 2020 2022 2072 6566 6f72 6d61 742e       " reformat.
-00007b40: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00007b50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007b60: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-00007b70: 706f 7274 2e72 6574 7572 6e5f 636f 6465  port.return_code
-00007b80: 2c20 3132 3329 0a20 2020 2020 2020 2020  , 123).         
-00007b90: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
-00007ba0: 6174 6828 2266 3322 292c 2063 6572 6369  ath("f3"), cerci
-00007bb0: 732e 4368 616e 6765 642e 5945 5329 0a20  s.Changed.YES). 
-00007bc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007bd0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-00007be0: 6f75 745f 6c69 6e65 7329 2c20 3229 0a20  out_lines), 2). 
-00007bf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007c00: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-00007c10: 6572 725f 6c69 6e65 7329 2c20 3129 0a20  err_lines), 1). 
-00007c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007c30: 6173 7365 7274 4571 7561 6c28 6f75 745f  assertEqual(out_
-00007c40: 6c69 6e65 735b 2d31 5d2c 2022 7265 666f  lines[-1], "refo
-00007c50: 726d 6174 7465 6420 6633 2229 0a20 2020  rmatted f3").   
-00007c60: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00007c70: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-00007c80: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
-00007c90: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
-00007ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007cb0: 2022 3220 6669 6c65 7320 7265 666f 726d   "2 files reform
-00007cc0: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
-00007cd0: 6566 7420 756e 6368 616e 6765 642c 2031  eft unchanged, 1
-00007ce0: 2066 696c 6520 6661 696c 6564 2074 6f22   file failed to"
-00007cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d00: 2022 2072 6566 6f72 6d61 742e 222c 0a20   " reformat.",. 
-00007d10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00007d20: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00007d30: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
-00007d40: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
-00007d50: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
-00007d60: 6570 6f72 742e 6661 696c 6564 2850 6174  eport.failed(Pat
-00007d70: 6828 2265 3222 292c 2022 626f 6f6d 2229  h("e2"), "boom")
-00007d80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007d90: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00007da0: 6e28 6f75 745f 6c69 6e65 7329 2c20 3229  n(out_lines), 2)
-00007db0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007dc0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00007dd0: 6e28 6572 725f 6c69 6e65 7329 2c20 3229  n(err_lines), 2)
-00007de0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007df0: 662e 6173 7365 7274 4571 7561 6c28 6572  f.assertEqual(er
-00007e00: 725f 6c69 6e65 735b 2d31 5d2c 2022 6572  r_lines[-1], "er
-00007e10: 726f 723a 2063 616e 6e6f 7420 666f 726d  ror: cannot form
-00007e20: 6174 2065 323a 2062 6f6f 6d22 290a 2020  at e2: boom").  
-00007e30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00007e40: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00007e50: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-00007e60: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00007e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007e80: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
-00007e90: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
-00007ea0: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
-00007eb0: 3220 6669 6c65 7320 6661 696c 6564 2074  2 files failed t
-00007ec0: 6f22 0a20 2020 2020 2020 2020 2020 2020  o".             
-00007ed0: 2020 2022 2072 6566 6f72 6d61 742e 222c     " reformat.",
-00007ee0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00007ef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007f00: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
-00007f10: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
-00007f20: 3132 3329 0a20 2020 2020 2020 2020 2020  123).           
-00007f30: 2072 6570 6f72 742e 7061 7468 5f69 676e   report.path_ign
-00007f40: 6f72 6564 2850 6174 6828 2277 6174 2229  ored(Path("wat")
-00007f50: 2c20 226e 6f20 6d61 7463 6822 290a 2020  , "no match").  
-00007f60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00007f70: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
-00007f80: 7574 5f6c 696e 6573 292c 2032 290a 2020  ut_lines), 2).  
-00007f90: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00007fa0: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
-00007fb0: 7272 5f6c 696e 6573 292c 2032 290a 2020  rr_lines), 2).  
-00007fc0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00007fd0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00007fe0: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-00007ff0: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00008000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008010: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
-00008020: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
-00008030: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
-00008040: 3220 6669 6c65 7320 6661 696c 6564 2074  2 files failed t
-00008050: 6f22 0a20 2020 2020 2020 2020 2020 2020  o".             
-00008060: 2020 2022 2072 6566 6f72 6d61 742e 222c     " reformat.",
-00008070: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00008080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008090: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
-000080a0: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
-000080b0: 3132 3329 0a20 2020 2020 2020 2020 2020  123).           
-000080c0: 2072 6570 6f72 742e 646f 6e65 2850 6174   report.done(Pat
-000080d0: 6828 2266 3422 292c 2063 6572 6369 732e  h("f4"), cercis.
-000080e0: 4368 616e 6765 642e 4e4f 290a 2020 2020  Changed.NO).    
-000080f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008100: 6572 7445 7175 616c 286c 656e 286f 7574  ertEqual(len(out
-00008110: 5f6c 696e 6573 292c 2032 290a 2020 2020  _lines), 2).    
-00008120: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008130: 6572 7445 7175 616c 286c 656e 2865 7272  ertEqual(len(err
-00008140: 5f6c 696e 6573 292c 2032 290a 2020 2020  _lines), 2).    
-00008150: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008160: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
-00008170: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
-00008180: 6528 7374 7228 7265 706f 7274 2929 2c0a  e(str(report)),.
-00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081a0: 2232 2066 696c 6573 2072 6566 6f72 6d61  "2 files reforma
-000081b0: 7474 6564 2c20 3320 6669 6c65 7320 6c65  tted, 3 files le
-000081c0: 6674 2075 6e63 6861 6e67 6564 2c20 3220  ft unchanged, 2 
-000081d0: 6669 6c65 7320 6661 696c 6564 2074 6f22  files failed to"
-000081e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081f0: 2022 2072 6566 6f72 6d61 742e 222c 0a20   " reformat.",. 
-00008200: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00008210: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00008220: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
-00008230: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
-00008240: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
-00008250: 6570 6f72 742e 6368 6563 6b20 3d20 5472  eport.check = Tr
-00008260: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
-00008270: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00008280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008290: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
-000082a0: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
-000082b0: 2020 2020 2020 2022 3220 6669 6c65 7320         "2 files 
-000082c0: 776f 756c 6420 6265 2072 6566 6f72 6d61  would be reforma
-000082d0: 7474 6564 2c20 3320 6669 6c65 7320 776f  tted, 3 files wo
-000082e0: 756c 6420 6265 206c 6566 7420 756e 6368  uld be left unch
-000082f0: 616e 6765 642c 2032 220a 2020 2020 2020  anged, 2".      
-00008300: 2020 2020 2020 2020 2020 2220 6669 6c65            " file
-00008310: 7320 776f 756c 6420 6661 696c 2074 6f20  s would fail to 
-00008320: 7265 666f 726d 6174 2e22 2c0a 2020 2020  reformat.",.    
-00008330: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00008340: 2020 2020 2020 7265 706f 7274 2e63 6865        report.che
-00008350: 636b 203d 2046 616c 7365 0a20 2020 2020  ck = False.     
-00008360: 2020 2020 2020 2072 6570 6f72 742e 6469         report.di
-00008370: 6666 203d 2054 7275 650a 2020 2020 2020  ff = True.      
-00008380: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00008390: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
-000083a0: 2020 2020 2020 2020 756e 7374 796c 6528          unstyle(
-000083b0: 7374 7228 7265 706f 7274 2929 2c0a 2020  str(report)),.  
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2232                "2
-000083d0: 2066 696c 6573 2077 6f75 6c64 2062 6520   files would be 
-000083e0: 7265 666f 726d 6174 7465 642c 2033 2066  reformatted, 3 f
-000083f0: 696c 6573 2077 6f75 6c64 2062 6520 6c65  iles would be le
-00008400: 6674 2075 6e63 6861 6e67 6564 2c20 3222  ft unchanged, 2"
-00008410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008420: 2022 2066 696c 6573 2077 6f75 6c64 2066   " files would f
-00008430: 6169 6c20 746f 2072 6566 6f72 6d61 742e  ail to reformat.
-00008440: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00008450: 0a0a 2020 2020 6465 6620 7465 7374 5f6c  ..    def test_l
-00008460: 6962 3274 6f33 5f70 6172 7365 2873 656c  ib2to3_parse(sel
-00008470: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00008480: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-00008490: 7365 7274 5261 6973 6573 2863 6572 6369  sertRaises(cerci
-000084a0: 732e 496e 7661 6c69 6449 6e70 7574 293a  s.InvalidInput):
-000084b0: 0a20 2020 2020 2020 2020 2020 2063 6572  .            cer
-000084c0: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
-000084d0: 6528 2269 6e76 616c 6964 2073 796e 7461  e("invalid synta
-000084e0: 7822 290a 0a20 2020 2020 2020 2073 7472  x")..        str
-000084f0: 6164 646c 696e 6720 3d20 2278 202b 2079  addling = "x + y
-00008500: 220a 2020 2020 2020 2020 6365 7263 6973  ".        cercis
-00008510: 2e6c 6962 3274 6f33 5f70 6172 7365 2873  .lib2to3_parse(s
-00008520: 7472 6164 646c 696e 6729 0a20 2020 2020  traddling).     
-00008530: 2020 2063 6572 6369 732e 6c69 6232 746f     cercis.lib2to
-00008540: 335f 7061 7273 6528 7374 7261 6464 6c69  3_parse(straddli
-00008550: 6e67 2c20 7b54 6172 6765 7456 6572 7369  ng, {TargetVersi
-00008560: 6f6e 2e50 5933 367d 290a 0a20 2020 2020  on.PY36})..     
-00008570: 2020 2070 7932 5f6f 6e6c 7920 3d20 2270     py2_only = "p
-00008580: 7269 6e74 2078 220a 2020 2020 2020 2020  rint x".        
-00008590: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-000085a0: 5261 6973 6573 2863 6572 6369 732e 496e  Raises(cercis.In
-000085b0: 7661 6c69 6449 6e70 7574 293a 0a20 2020  validInput):.   
-000085c0: 2020 2020 2020 2020 2063 6572 6369 732e           cercis.
-000085d0: 6c69 6232 746f 335f 7061 7273 6528 7079  lib2to3_parse(py
-000085e0: 325f 6f6e 6c79 2c20 7b54 6172 6765 7456  2_only, {TargetV
-000085f0: 6572 7369 6f6e 2e50 5933 367d 290a 0a20  ersion.PY36}).. 
-00008600: 2020 2020 2020 2070 7933 5f6f 6e6c 7920         py3_only 
-00008610: 3d20 2265 7865 6328 782c 2065 6e64 3d79  = "exec(x, end=y
-00008620: 2922 0a20 2020 2020 2020 2063 6572 6369  )".        cerci
-00008630: 732e 6c69 6232 746f 335f 7061 7273 6528  s.lib2to3_parse(
-00008640: 7079 335f 6f6e 6c79 290a 2020 2020 2020  py3_only).      
-00008650: 2020 6365 7263 6973 2e6c 6962 3274 6f33    cercis.lib2to3
-00008660: 5f70 6172 7365 2870 7933 5f6f 6e6c 792c  _parse(py3_only,
-00008670: 207b 5461 7267 6574 5665 7273 696f 6e2e   {TargetVersion.
-00008680: 5059 3336 7d29 0a0a 2020 2020 6465 6620  PY36})..    def 
-00008690: 7465 7374 5f67 6574 5f66 6561 7475 7265  test_get_feature
-000086a0: 735f 7573 6564 5f64 6563 6f72 6174 6f72  s_used_decorator
-000086b0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000086c0: 2020 2020 2020 2020 2320 5465 7374 2074          # Test t
-000086d0: 6865 2066 6561 7475 7265 2064 6574 6563  he feature detec
-000086e0: 7469 6f6e 206f 6620 6e65 7720 6465 636f  tion of new deco
-000086f0: 7261 746f 7220 7379 6e74 6178 0a20 2020  rator syntax.   
-00008700: 2020 2020 2023 2073 696e 6365 2074 6869       # since thi
-00008710: 7320 6d61 6b65 7320 736f 6d65 2074 6573  s makes some tes
-00008720: 7420 6361 7365 7320 6f66 2074 6573 745f  t cases of test_
-00008730: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
-00008740: 6428 290a 2020 2020 2020 2020 2320 6661  d().        # fa
-00008750: 696c 7320 6966 2069 7420 6661 696c 732c  ils if it fails,
-00008760: 2074 6869 7320 6973 2074 6573 7465 6420   this is tested 
-00008770: 6669 7273 7420 736f 2074 6861 7420 6120  first so that a 
-00008780: 7573 6566 756c 2063 6173 650a 2020 2020  useful case.    
-00008790: 2020 2020 2320 6973 2069 6465 6e74 6966      # is identif
-000087a0: 6965 640a 2020 2020 2020 2020 7369 6d70  ied.        simp
-000087b0: 6c65 732c 2072 656c 6178 6564 203d 2072  les, relaxed = r
-000087c0: 6561 645f 6461 7461 2822 6d69 7363 656c  ead_data("miscel
-000087d0: 6c61 6e65 6f75 7322 2c20 2264 6563 6f72  laneous", "decor
-000087e0: 6174 6f72 7322 290a 2020 2020 2020 2020  ators").        
-000087f0: 2320 736b 6970 2065 7870 6c61 6e61 7469  # skip explanati
-00008800: 6f6e 2063 6f6d 6d65 6e74 7320 6174 2074  on comments at t
-00008810: 6865 2074 6f70 206f 6620 7468 6520 6669  he top of the fi
-00008820: 6c65 0a20 2020 2020 2020 2066 6f72 2073  le.        for s
-00008830: 696d 706c 655f 7465 7374 2069 6e20 7369  imple_test in si
-00008840: 6d70 6c65 732e 7370 6c69 7428 2223 2322  mples.split("##"
-00008850: 295b 313a 5d3a 0a20 2020 2020 2020 2020  )[1:]:.         
-00008860: 2020 206e 6f64 6520 3d20 6365 7263 6973     node = cercis
-00008870: 2e6c 6962 3274 6f33 5f70 6172 7365 2873  .lib2to3_parse(s
-00008880: 696d 706c 655f 7465 7374 290a 2020 2020  imple_test).    
-00008890: 2020 2020 2020 2020 6465 636f 7261 746f          decorato
-000088a0: 7220 3d20 7374 7228 6e6f 6465 2e63 6869  r = str(node.chi
-000088b0: 6c64 7265 6e5b 305d 2e63 6869 6c64 7265  ldren[0].childre
-000088c0: 6e5b 305d 292e 7374 7269 7028 290a 2020  n[0]).strip().  
-000088d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000088e0: 7373 6572 744e 6f74 496e 280a 2020 2020  ssertNotIn(.    
-000088f0: 2020 2020 2020 2020 2020 2020 4665 6174              Feat
-00008900: 7572 652e 5245 4c41 5845 445f 4445 434f  ure.RELAXED_DECO
-00008910: 5241 544f 5253 2c0a 2020 2020 2020 2020  RATORS,.        
-00008920: 2020 2020 2020 2020 6365 7263 6973 2e67          cercis.g
-00008930: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
-00008940: 286e 6f64 6529 2c0a 2020 2020 2020 2020  (node),.        
-00008950: 2020 2020 2020 2020 6d73 673d 280a 2020          msg=(.  
-00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008970: 2020 6622 6465 636f 7261 746f 7220 277b    f"decorator '{
-00008980: 6465 636f 7261 746f 727d 2720 666f 6c6c  decorator}' foll
-00008990: 6f77 7320 7079 7468 6f6e 3c3d 332e 3820  ows python<=3.8 
-000089a0: 7379 6e74 6178 220a 2020 2020 2020 2020  syntax".        
-000089b0: 2020 2020 2020 2020 2020 2020 2262 7574              "but
-000089c0: 2069 7320 6465 7465 6374 6564 2061 7320   is detected as 
-000089d0: 332e 392b 220a 2020 2020 2020 2020 2020  3.9+".          
-000089e0: 2020 2020 2020 2020 2020 2320 6622 5468            # f"Th
-000089f0: 6520 6675 6c6c 206e 6f64 6520 6973 5c6e  e full node is\n
-00008a00: 7b6e 6f64 6521 727d 220a 2020 2020 2020  {node!r}".      
-00008a10: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00008a20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00008a30: 2020 2023 2073 6b69 7020 7468 6520 2723     # skip the '#
-00008a40: 206f 7574 7075 7427 2063 6f6d 6d65 6e74   output' comment
-00008a50: 2061 7420 7468 6520 746f 7020 6f66 2074   at the top of t
-00008a60: 6865 206f 7574 7075 7420 7061 7274 0a20  he output part. 
-00008a70: 2020 2020 2020 2066 6f72 2072 656c 6178         for relax
-00008a80: 6564 5f74 6573 7420 696e 2072 656c 6178  ed_test in relax
-00008a90: 6564 2e73 706c 6974 2822 2323 2229 5b31  ed.split("##")[1
-00008aa0: 3a5d 3a0a 2020 2020 2020 2020 2020 2020  :]:.            
-00008ab0: 6e6f 6465 203d 2063 6572 6369 732e 6c69  node = cercis.li
-00008ac0: 6232 746f 335f 7061 7273 6528 7265 6c61  b2to3_parse(rela
-00008ad0: 7865 645f 7465 7374 290a 2020 2020 2020  xed_test).      
-00008ae0: 2020 2020 2020 6465 636f 7261 746f 7220        decorator 
-00008af0: 3d20 7374 7228 6e6f 6465 2e63 6869 6c64  = str(node.child
-00008b00: 7265 6e5b 305d 2e63 6869 6c64 7265 6e5b  ren[0].children[
-00008b10: 305d 292e 7374 7269 7028 290a 2020 2020  0]).strip().    
-00008b20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008b30: 6572 7449 6e28 0a20 2020 2020 2020 2020  ertIn(.         
-00008b40: 2020 2020 2020 2046 6561 7475 7265 2e52         Feature.R
-00008b50: 454c 4158 4544 5f44 4543 4f52 4154 4f52  ELAXED_DECORATOR
-00008b60: 532c 0a20 2020 2020 2020 2020 2020 2020  S,.             
-00008b70: 2020 2063 6572 6369 732e 6765 745f 6665     cercis.get_fe
-00008b80: 6174 7572 6573 5f75 7365 6428 6e6f 6465  atures_used(node
-00008b90: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00008ba0: 2020 206d 7367 3d28 0a20 2020 2020 2020     msg=(.       
-00008bb0: 2020 2020 2020 2020 2020 2020 2066 2264               f"d
-00008bc0: 6563 6f72 6174 6f72 2027 7b64 6563 6f72  ecorator '{decor
-00008bd0: 6174 6f72 7d27 2075 7365 7320 7079 7468  ator}' uses pyth
-00008be0: 6f6e 332e 392b 2073 796e 7461 7822 0a20  on3.9+ syntax". 
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c00: 2020 2022 6275 7420 6973 2064 6574 6563     "but is detec
-00008c10: 7465 6420 6173 2070 7974 686f 6e3c 3d33  ted as python<=3
-00008c20: 2e38 220a 2020 2020 2020 2020 2020 2020  .8".            
-00008c30: 2020 2020 2020 2020 2320 6622 5468 6520          # f"The 
-00008c40: 6675 6c6c 206e 6f64 6520 6973 5c6e 7b6e  full node is\n{n
-00008c50: 6f64 6521 727d 220a 2020 2020 2020 2020  ode!r}".        
-00008c60: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00008c70: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00008c80: 6620 7465 7374 5f67 6574 5f66 6561 7475  f test_get_featu
-00008c90: 7265 735f 7573 6564 2873 656c 6629 202d  res_used(self) -
-00008ca0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00008cb0: 6e6f 6465 203d 2063 6572 6369 732e 6c69  node = cercis.li
-00008cc0: 6232 746f 335f 7061 7273 6528 2264 6566  b2to3_parse("def
-00008cd0: 2066 282a 2c20 6172 6729 3a20 2e2e 2e5c   f(*, arg): ...\
-00008ce0: 6e22 290a 2020 2020 2020 2020 7365 6c66  n").        self
-00008cf0: 2e61 7373 6572 7445 7175 616c 2863 6572  .assertEqual(cer
-00008d00: 6369 732e 6765 745f 6665 6174 7572 6573  cis.get_features
-00008d10: 5f75 7365 6428 6e6f 6465 292c 2073 6574  _used(node), set
-00008d20: 2829 290a 2020 2020 2020 2020 6e6f 6465  ()).        node
-00008d30: 203d 2063 6572 6369 732e 6c69 6232 746f   = cercis.lib2to
-00008d40: 335f 7061 7273 6528 2264 6566 2066 282a  3_parse("def f(*
-00008d50: 2c20 6172 672c 293a 202e 2e2e 5c6e 2229  , arg,): ...\n")
-00008d60: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00008d70: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-00008d80: 2020 2020 2020 2063 6572 6369 732e 6765         cercis.ge
-00008d90: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
-00008da0: 6e6f 6465 292c 207b 4665 6174 7572 652e  node), {Feature.
-00008db0: 5452 4149 4c49 4e47 5f43 4f4d 4d41 5f49  TRAILING_COMMA_I
-00008dc0: 4e5f 4445 467d 0a20 2020 2020 2020 2029  N_DEF}.        )
-00008dd0: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
-00008de0: 6365 7263 6973 2e6c 6962 3274 6f33 5f70  cercis.lib2to3_p
-00008df0: 6172 7365 2822 6628 2a61 7267 2c29 5c6e  arse("f(*arg,)\n
-00008e00: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00008e10: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00008e20: 2020 2020 2020 2020 2063 6572 6369 732e           cercis.
-00008e30: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
-00008e40: 6428 6e6f 6465 292c 207b 4665 6174 7572  d(node), {Featur
-00008e50: 652e 5452 4149 4c49 4e47 5f43 4f4d 4d41  e.TRAILING_COMMA
-00008e60: 5f49 4e5f 4341 4c4c 7d0a 2020 2020 2020  _IN_CALL}.      
-00008e70: 2020 290a 2020 2020 2020 2020 6e6f 6465    ).        node
-00008e80: 203d 2063 6572 6369 732e 6c69 6232 746f   = cercis.lib2to
-00008e90: 335f 7061 7273 6528 2264 6566 2066 282a  3_parse("def f(*
-00008ea0: 2c20 6172 6729 3a20 6627 7374 7269 6e67  , arg): f'string
-00008eb0: 275c 6e22 290a 2020 2020 2020 2020 7365  '\n").        se
-00008ec0: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
-00008ed0: 6572 6369 732e 6765 745f 6665 6174 7572  ercis.get_featur
-00008ee0: 6573 5f75 7365 6428 6e6f 6465 292c 207b  es_used(node), {
-00008ef0: 4665 6174 7572 652e 465f 5354 5249 4e47  Feature.F_STRING
-00008f00: 537d 290a 2020 2020 2020 2020 6e6f 6465  S}).        node
-00008f10: 203d 2063 6572 6369 732e 6c69 6232 746f   = cercis.lib2to
-00008f20: 335f 7061 7273 6528 2231 3233 5f34 3536  3_parse("123_456
-00008f30: 5c6e 2229 0a20 2020 2020 2020 2073 656c  \n").        sel
-00008f40: 662e 6173 7365 7274 4571 7561 6c28 6365  f.assertEqual(ce
-00008f50: 7263 6973 2e67 6574 5f66 6561 7475 7265  rcis.get_feature
-00008f60: 735f 7573 6564 286e 6f64 6529 2c20 7b46  s_used(node), {F
-00008f70: 6561 7475 7265 2e4e 554d 4552 4943 5f55  eature.NUMERIC_U
-00008f80: 4e44 4552 5343 4f52 4553 7d29 0a20 2020  NDERSCORES}).   
-00008f90: 2020 2020 206e 6f64 6520 3d20 6365 7263       node = cerc
-00008fa0: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
-00008fb0: 2822 3132 3334 3536 5c6e 2229 0a20 2020  ("123456\n").   
-00008fc0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00008fd0: 4571 7561 6c28 6365 7263 6973 2e67 6574  Equal(cercis.get
-00008fe0: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
-00008ff0: 6f64 6529 2c20 7365 7428 2929 0a20 2020  ode), set()).   
-00009000: 2020 2020 2073 6f75 7263 652c 2065 7870       source, exp
-00009010: 6563 7465 6420 3d20 7265 6164 5f64 6174  ected = read_dat
-00009020: 6128 2273 696d 706c 655f 6361 7365 7322  a("simple_cases"
-00009030: 2c20 2266 756e 6374 696f 6e22 290a 2020  , "function").  
-00009040: 2020 2020 2020 6e6f 6465 203d 2063 6572        node = cer
-00009050: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
-00009060: 6528 736f 7572 6365 290a 2020 2020 2020  e(source).      
-00009070: 2020 6578 7065 6374 6564 5f66 6561 7475    expected_featu
-00009080: 7265 7320 3d20 7b0a 2020 2020 2020 2020  res = {.        
-00009090: 2020 2020 4665 6174 7572 652e 5452 4149      Feature.TRAI
-000090a0: 4c49 4e47 5f43 4f4d 4d41 5f49 4e5f 4341  LING_COMMA_IN_CA
-000090b0: 4c4c 2c0a 2020 2020 2020 2020 2020 2020  LL,.            
-000090c0: 4665 6174 7572 652e 5452 4149 4c49 4e47  Feature.TRAILING
-000090d0: 5f43 4f4d 4d41 5f49 4e5f 4445 462c 0a20  _COMMA_IN_DEF,. 
-000090e0: 2020 2020 2020 2020 2020 2046 6561 7475             Featu
-000090f0: 7265 2e46 5f53 5452 494e 4753 2c0a 2020  re.F_STRINGS,.  
-00009100: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00009110: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00009120: 2863 6572 6369 732e 6765 745f 6665 6174  (cercis.get_feat
-00009130: 7572 6573 5f75 7365 6428 6e6f 6465 292c  ures_used(node),
-00009140: 2065 7870 6563 7465 645f 6665 6174 7572   expected_featur
-00009150: 6573 290a 2020 2020 2020 2020 6e6f 6465  es).        node
-00009160: 203d 2063 6572 6369 732e 6c69 6232 746f   = cercis.lib2to
-00009170: 335f 7061 7273 6528 6578 7065 6374 6564  3_parse(expected
-00009180: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00009190: 7373 6572 7445 7175 616c 2863 6572 6369  ssertEqual(cerci
-000091a0: 732e 6765 745f 6665 6174 7572 6573 5f75  s.get_features_u
-000091b0: 7365 6428 6e6f 6465 292c 2065 7870 6563  sed(node), expec
-000091c0: 7465 645f 6665 6174 7572 6573 290a 2020  ted_features).  
-000091d0: 2020 2020 2020 736f 7572 6365 2c20 6578        source, ex
-000091e0: 7065 6374 6564 203d 2072 6561 645f 6461  pected = read_da
-000091f0: 7461 2822 7369 6d70 6c65 5f63 6173 6573  ta("simple_cases
-00009200: 222c 2022 6578 7072 6573 7369 6f6e 2229  ", "expression")
-00009210: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
-00009220: 6365 7263 6973 2e6c 6962 3274 6f33 5f70  cercis.lib2to3_p
-00009230: 6172 7365 2873 6f75 7263 6529 0a20 2020  arse(source).   
-00009240: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009250: 4571 7561 6c28 6365 7263 6973 2e67 6574  Equal(cercis.get
-00009260: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
-00009270: 6f64 6529 2c20 7365 7428 2929 0a20 2020  ode), set()).   
-00009280: 2020 2020 206e 6f64 6520 3d20 6365 7263       node = cerc
-00009290: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
-000092a0: 2865 7870 6563 7465 6429 0a20 2020 2020  (expected).     
-000092b0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000092c0: 7561 6c28 6365 7263 6973 2e67 6574 5f66  ual(cercis.get_f
-000092d0: 6561 7475 7265 735f 7573 6564 286e 6f64  eatures_used(nod
-000092e0: 6529 2c20 7365 7428 2929 0a20 2020 2020  e), set()).     
-000092f0: 2020 206e 6f64 6520 3d20 6365 7263 6973     node = cercis
-00009300: 2e6c 6962 3274 6f33 5f70 6172 7365 2822  .lib2to3_parse("
-00009310: 6c61 6d62 6461 2061 2c20 2f2c 2062 3a20  lambda a, /, b: 
-00009320: 2e2e 2e22 290a 2020 2020 2020 2020 7365  ...").        se
-00009330: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
-00009340: 6572 6369 732e 6765 745f 6665 6174 7572  ercis.get_featur
-00009350: 6573 5f75 7365 6428 6e6f 6465 292c 207b  es_used(node), {
-00009360: 4665 6174 7572 652e 504f 535f 4f4e 4c59  Feature.POS_ONLY
-00009370: 5f41 5247 554d 454e 5453 7d29 0a20 2020  _ARGUMENTS}).   
-00009380: 2020 2020 206e 6f64 6520 3d20 6365 7263       node = cerc
-00009390: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
-000093a0: 2822 6465 6620 666e 2861 2c20 2f2c 2062  ("def fn(a, /, b
-000093b0: 293a 202e 2e2e 2229 0a20 2020 2020 2020  ): ...").       
-000093c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000093d0: 6c28 6365 7263 6973 2e67 6574 5f66 6561  l(cercis.get_fea
-000093e0: 7475 7265 735f 7573 6564 286e 6f64 6529  tures_used(node)
-000093f0: 2c20 7b46 6561 7475 7265 2e50 4f53 5f4f  , {Feature.POS_O
-00009400: 4e4c 595f 4152 4755 4d45 4e54 537d 290a  NLY_ARGUMENTS}).
-00009410: 2020 2020 2020 2020 6e6f 6465 203d 2063          node = c
-00009420: 6572 6369 732e 6c69 6232 746f 335f 7061  ercis.lib2to3_pa
-00009430: 7273 6528 2264 6566 2066 6e28 293a 2079  rse("def fn(): y
-00009440: 6965 6c64 2061 2c20 6222 290a 2020 2020  ield a, b").    
-00009450: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00009460: 7175 616c 2863 6572 6369 732e 6765 745f  qual(cercis.get_
-00009470: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
-00009480: 6465 292c 2073 6574 2829 290a 2020 2020  de), set()).    
-00009490: 2020 2020 6e6f 6465 203d 2063 6572 6369      node = cerci
-000094a0: 732e 6c69 6232 746f 335f 7061 7273 6528  s.lib2to3_parse(
-000094b0: 2264 6566 2066 6e28 293a 2072 6574 7572  "def fn(): retur
-000094c0: 6e20 612c 2062 2229 0a20 2020 2020 2020  n a, b").       
-000094d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000094e0: 6c28 6365 7263 6973 2e67 6574 5f66 6561  l(cercis.get_fea
-000094f0: 7475 7265 735f 7573 6564 286e 6f64 6529  tures_used(node)
-00009500: 2c20 7365 7428 2929 0a20 2020 2020 2020  , set()).       
-00009510: 206e 6f64 6520 3d20 6365 7263 6973 2e6c   node = cercis.l
-00009520: 6962 3274 6f33 5f70 6172 7365 2822 6465  ib2to3_parse("de
-00009530: 6620 666e 2829 3a20 7969 656c 6420 2a62  f fn(): yield *b
-00009540: 2c20 6322 290a 2020 2020 2020 2020 7365  , c").        se
-00009550: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
-00009560: 6572 6369 732e 6765 745f 6665 6174 7572  ercis.get_featur
-00009570: 6573 5f75 7365 6428 6e6f 6465 292c 207b  es_used(node), {
-00009580: 4665 6174 7572 652e 554e 5041 434b 494e  Feature.UNPACKIN
-00009590: 475f 4f4e 5f46 4c4f 577d 290a 2020 2020  G_ON_FLOW}).    
-000095a0: 2020 2020 6e6f 6465 203d 2063 6572 6369      node = cerci
-000095b0: 732e 6c69 6232 746f 335f 7061 7273 6528  s.lib2to3_parse(
-000095c0: 2264 6566 2066 6e28 293a 2072 6574 7572  "def fn(): retur
-000095d0: 6e20 612c 202a 622c 2063 2229 0a20 2020  n a, *b, c").   
-000095e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000095f0: 4571 7561 6c28 6365 7263 6973 2e67 6574  Equal(cercis.get
-00009600: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
-00009610: 6f64 6529 2c20 7b46 6561 7475 7265 2e55  ode), {Feature.U
-00009620: 4e50 4143 4b49 4e47 5f4f 4e5f 464c 4f57  NPACKING_ON_FLOW
-00009630: 7d29 0a20 2020 2020 2020 206e 6f64 6520  }).        node 
-00009640: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
-00009650: 5f70 6172 7365 2822 7820 3d20 612c 202a  _parse("x = a, *
-00009660: 622c 2063 2229 0a20 2020 2020 2020 2073  b, c").        s
-00009670: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00009680: 6365 7263 6973 2e67 6574 5f66 6561 7475  cercis.get_featu
-00009690: 7265 735f 7573 6564 286e 6f64 6529 2c20  res_used(node), 
-000096a0: 7365 7428 2929 0a20 2020 2020 2020 206e  set()).        n
-000096b0: 6f64 6520 3d20 6365 7263 6973 2e6c 6962  ode = cercis.lib
-000096c0: 3274 6f33 5f70 6172 7365 2822 783a 2041  2to3_parse("x: A
-000096d0: 6e79 203d 2072 6567 756c 6172 2229 0a20  ny = regular"). 
-000096e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000096f0: 7274 4571 7561 6c28 6365 7263 6973 2e67  rtEqual(cercis.g
-00009700: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
-00009710: 286e 6f64 6529 2c20 7365 7428 2929 0a20  (node), set()). 
-00009720: 2020 2020 2020 206e 6f64 6520 3d20 6365         node = ce
-00009730: 7263 6973 2e6c 6962 3274 6f33 5f70 6172  rcis.lib2to3_par
-00009740: 7365 2822 783a 2041 6e79 203d 2028 7265  se("x: Any = (re
-00009750: 6775 6c61 722c 2072 6567 756c 6172 2922  gular, regular)"
-00009760: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00009770: 7373 6572 7445 7175 616c 2863 6572 6369  ssertEqual(cerci
-00009780: 732e 6765 745f 6665 6174 7572 6573 5f75  s.get_features_u
-00009790: 7365 6428 6e6f 6465 292c 2073 6574 2829  sed(node), set()
-000097a0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-000097b0: 2063 6572 6369 732e 6c69 6232 746f 335f   cercis.lib2to3_
-000097c0: 7061 7273 6528 2278 3a20 416e 7920 3d20  parse("x: Any = 
-000097d0: 436f 6d70 6c65 7828 5479 7065 2831 2929  Complex(Type(1))
-000097e0: 5b73 6f6d 6574 6869 6e67 5d22 290a 2020  [something]").  
-000097f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00009800: 7445 7175 616c 2863 6572 6369 732e 6765  tEqual(cercis.ge
-00009810: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
-00009820: 6e6f 6465 292c 2073 6574 2829 290a 2020  node), set()).  
-00009830: 2020 2020 2020 6e6f 6465 203d 2063 6572        node = cer
-00009840: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
-00009850: 6528 2278 3a20 5475 706c 655b 696e 742c  e("x: Tuple[int,
-00009860: 202e 2e2e 5d20 3d20 612c 2062 2c20 6322   ...] = a, b, c"
-00009870: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00009880: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00009890: 2020 2020 2020 2020 6365 7263 6973 2e67          cercis.g
-000098a0: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
-000098b0: 286e 6f64 6529 2c20 7b46 6561 7475 7265  (node), {Feature
-000098c0: 2e41 4e4e 5f41 5353 4947 4e5f 4558 5445  .ANN_ASSIGN_EXTE
-000098d0: 4e44 4544 5f52 4853 7d0a 2020 2020 2020  NDED_RHS}.      
-000098e0: 2020 290a 2020 2020 2020 2020 6e6f 6465    ).        node
-000098f0: 203d 2063 6572 6369 732e 6c69 6232 746f   = cercis.lib2to
-00009900: 335f 7061 7273 6528 2274 7279 3a20 7061  3_parse("try: pa
-00009910: 7373 5c6e 6578 6365 7074 2053 6f6d 6574  ss\nexcept Somet
-00009920: 6869 6e67 3a20 7061 7373 2229 0a20 2020  hing: pass").   
-00009930: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009940: 4571 7561 6c28 6365 7263 6973 2e67 6574  Equal(cercis.get
-00009950: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
-00009960: 6f64 6529 2c20 7365 7428 2929 0a20 2020  ode), set()).   
-00009970: 2020 2020 206e 6f64 6520 3d20 6365 7263       node = cerc
-00009980: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
-00009990: 2822 7472 793a 2070 6173 735c 6e65 7863  ("try: pass\nexc
-000099a0: 6570 7420 282a 536f 6d65 7468 696e 672c  ept (*Something,
-000099b0: 293a 2070 6173 7322 290a 2020 2020 2020  ): pass").      
-000099c0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000099d0: 616c 2863 6572 6369 732e 6765 745f 6665  al(cercis.get_fe
-000099e0: 6174 7572 6573 5f75 7365 6428 6e6f 6465  atures_used(node
-000099f0: 292c 2073 6574 2829 290a 2020 2020 2020  ), set()).      
-00009a00: 2020 6e6f 6465 203d 2063 6572 6369 732e    node = cercis.
-00009a10: 6c69 6232 746f 335f 7061 7273 6528 2274  lib2to3_parse("t
-00009a20: 7279 3a20 7061 7373 5c6e 6578 6365 7074  ry: pass\nexcept
-00009a30: 202a 4772 6f75 703a 2070 6173 7322 290a   *Group: pass").
-00009a40: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00009a50: 6572 7445 7175 616c 2863 6572 6369 732e  ertEqual(cercis.
-00009a60: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
-00009a70: 6428 6e6f 6465 292c 207b 4665 6174 7572  d(node), {Featur
-00009a80: 652e 4558 4345 5054 5f53 5441 527d 290a  e.EXCEPT_STAR}).
-00009a90: 2020 2020 2020 2020 6e6f 6465 203d 2063          node = c
-00009aa0: 6572 6369 732e 6c69 6232 746f 335f 7061  ercis.lib2to3_pa
-00009ab0: 7273 6528 2261 5b2a 625d 2229 0a20 2020  rse("a[*b]").   
-00009ac0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009ad0: 4571 7561 6c28 6365 7263 6973 2e67 6574  Equal(cercis.get
-00009ae0: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
-00009af0: 6f64 6529 2c20 7b46 6561 7475 7265 2e56  ode), {Feature.V
-00009b00: 4152 4941 4449 435f 4745 4e45 5249 4353  ARIADIC_GENERICS
-00009b10: 7d29 0a20 2020 2020 2020 206e 6f64 6520  }).        node 
-00009b20: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
-00009b30: 5f70 6172 7365 2822 615b 782c 202a 7928  _parse("a[x, *y(
-00009b40: 292c 207a 5d20 3d20 7422 290a 2020 2020  ), z] = t").    
-00009b50: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00009b60: 7175 616c 2863 6572 6369 732e 6765 745f  qual(cercis.get_
-00009b70: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
-00009b80: 6465 292c 207b 4665 6174 7572 652e 5641  de), {Feature.VA
-00009b90: 5249 4144 4943 5f47 454e 4552 4943 537d  RIADIC_GENERICS}
-00009ba0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-00009bb0: 2063 6572 6369 732e 6c69 6232 746f 335f   cercis.lib2to3_
-00009bc0: 7061 7273 6528 2264 6566 2066 6e28 2a61  parse("def fn(*a
-00009bd0: 7267 733a 202a 5429 3a20 7061 7373 2229  rgs: *T): pass")
-00009be0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00009bf0: 7365 7274 4571 7561 6c28 6365 7263 6973  sertEqual(cercis
-00009c00: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
-00009c10: 6564 286e 6f64 6529 2c20 7b46 6561 7475  ed(node), {Featu
-00009c20: 7265 2e56 4152 4941 4449 435f 4745 4e45  re.VARIADIC_GENE
-00009c30: 5249 4353 7d29 0a0a 2020 2020 6465 6620  RICS})..    def 
-00009c40: 7465 7374 5f67 6574 5f66 6561 7475 7265  test_get_feature
-00009c50: 735f 7573 6564 5f66 6f72 5f66 7574 7572  s_used_for_futur
-00009c60: 655f 666c 6167 7328 7365 6c66 2920 2d3e  e_flags(self) ->
-00009c70: 204e 6f6e 653a 0a20 2020 2020 2020 2066   None:.        f
-00009c80: 6f72 2073 7263 2c20 6665 6174 7572 6573  or src, features
-00009c90: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-00009ca0: 2020 2822 6672 6f6d 205f 5f66 7574 7572    ("from __futur
-00009cb0: 655f 5f20 696d 706f 7274 2061 6e6e 6f74  e__ import annot
-00009cc0: 6174 696f 6e73 222c 207b 4665 6174 7572  ations", {Featur
-00009cd0: 652e 4655 5455 5245 5f41 4e4e 4f54 4154  e.FUTURE_ANNOTAT
-00009ce0: 494f 4e53 7d29 2c0a 2020 2020 2020 2020  IONS}),.        
-00009cf0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00009d00: 2020 2020 2020 2266 726f 6d20 5f5f 6675        "from __fu
-00009d10: 7475 7265 5f5f 2069 6d70 6f72 7420 286f  ture__ import (o
-00009d20: 7468 6572 2c20 616e 6e6f 7461 7469 6f6e  ther, annotation
-00009d30: 7329 222c 0a20 2020 2020 2020 2020 2020  s)",.           
-00009d40: 2020 2020 207b 4665 6174 7572 652e 4655       {Feature.FU
-00009d50: 5455 5245 5f41 4e4e 4f54 4154 494f 4e53  TURE_ANNOTATIONS
-00009d60: 7d2c 0a20 2020 2020 2020 2020 2020 2029  },.            )
-00009d70: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-00009d80: 6120 3d20 3120 2b20 325c 6e66 726f 6d20  a = 1 + 2\nfrom 
-00009d90: 736f 6d65 7468 696e 6720 696d 706f 7274  something import
-00009da0: 2061 6e6e 6f74 6174 696f 6e73 222c 2073   annotations", s
-00009db0: 6574 2829 292c 0a20 2020 2020 2020 2020  et()),.         
-00009dc0: 2020 2028 2266 726f 6d20 5f5f 6675 7475     ("from __futu
-00009dd0: 7265 5f5f 2069 6d70 6f72 7420 782c 2079  re__ import x, y
-00009de0: 222c 2073 6574 2829 292c 0a20 2020 2020  ", set()),.     
-00009df0: 2020 205d 3a0a 2020 2020 2020 2020 2020     ]:.          
-00009e00: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00009e10: 6573 7428 7372 633d 7372 632c 2066 6561  est(src=src, fea
-00009e20: 7475 7265 733d 6665 6174 7572 6573 293a  tures=features):
-00009e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e40: 206e 6f64 6520 3d20 6365 7263 6973 2e6c   node = cercis.l
-00009e50: 6962 3274 6f33 5f70 6172 7365 2873 7263  ib2to3_parse(src
-00009e60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009e70: 2020 6675 7475 7265 5f69 6d70 6f72 7473    future_imports
-00009e80: 203d 2063 6572 6369 732e 6765 745f 6675   = cercis.get_fu
-00009e90: 7475 7265 5f69 6d70 6f72 7473 286e 6f64  ture_imports(nod
-00009ea0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00009eb0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00009ec0: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
-00009ed0: 2020 2020 2020 2020 2063 6572 6369 732e           cercis.
-00009ee0: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
-00009ef0: 6428 6e6f 6465 2c20 6675 7475 7265 5f69  d(node, future_i
-00009f00: 6d70 6f72 7473 3d66 7574 7572 655f 696d  mports=future_im
-00009f10: 706f 7274 7329 2c0a 2020 2020 2020 2020  ports),.        
-00009f20: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00009f30: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
-00009f40: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00009f50: 2074 6573 745f 6765 745f 6675 7475 7265   test_get_future
-00009f60: 5f69 6d70 6f72 7473 2873 656c 6629 202d  _imports(self) -
-00009f70: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00009f80: 6e6f 6465 203d 2063 6572 6369 732e 6c69  node = cercis.li
-00009f90: 6232 746f 335f 7061 7273 6528 225c 6e22  b2to3_parse("\n"
-00009fa0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00009fb0: 7373 6572 7445 7175 616c 2873 6574 2829  ssertEqual(set()
-00009fc0: 2c20 6365 7263 6973 2e67 6574 5f66 7574  , cercis.get_fut
-00009fd0: 7572 655f 696d 706f 7274 7328 6e6f 6465  ure_imports(node
-00009fe0: 2929 0a20 2020 2020 2020 206e 6f64 6520  )).        node 
-00009ff0: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
-0000a000: 5f70 6172 7365 2822 6672 6f6d 205f 5f66  _parse("from __f
-0000a010: 7574 7572 655f 5f20 696d 706f 7274 2063  uture__ import c
-0000a020: 6572 6369 735c 6e22 290a 2020 2020 2020  ercis\n").      
-0000a030: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000a040: 616c 287b 2263 6572 6369 7322 7d2c 2063  al({"cercis"}, c
-0000a050: 6572 6369 732e 6765 745f 6675 7475 7265  ercis.get_future
-0000a060: 5f69 6d70 6f72 7473 286e 6f64 6529 290a  _imports(node)).
-0000a070: 2020 2020 2020 2020 6e6f 6465 203d 2063          node = c
-0000a080: 6572 6369 732e 6c69 6232 746f 335f 7061  ercis.lib2to3_pa
-0000a090: 7273 6528 2266 726f 6d20 5f5f 6675 7475  rse("from __futu
-0000a0a0: 7265 5f5f 2069 6d70 6f72 7420 6d75 6c74  re__ import mult
-0000a0b0: 6970 6c65 2c20 696d 706f 7274 735c 6e22  iple, imports\n"
-0000a0c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000a0d0: 7373 6572 7445 7175 616c 287b 226d 756c  ssertEqual({"mul
-0000a0e0: 7469 706c 6522 2c20 2269 6d70 6f72 7473  tiple", "imports
-0000a0f0: 227d 2c20 6365 7263 6973 2e67 6574 5f66  "}, cercis.get_f
-0000a100: 7574 7572 655f 696d 706f 7274 7328 6e6f  uture_imports(no
-0000a110: 6465 2929 0a20 2020 2020 2020 206e 6f64  de)).        nod
-0000a120: 6520 3d20 6365 7263 6973 2e6c 6962 3274  e = cercis.lib2t
-0000a130: 6f33 5f70 6172 7365 2822 6672 6f6d 205f  o3_parse("from _
-0000a140: 5f66 7574 7572 655f 5f20 696d 706f 7274  _future__ import
-0000a150: 2028 7061 7265 6e74 6865 7369 7a65 642c   (parenthesized,
-0000a160: 2069 6d70 6f72 7473 295c 6e22 290a 2020   imports)\n").  
-0000a170: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a180: 7445 7175 616c 287b 2270 6172 656e 7468  tEqual({"parenth
-0000a190: 6573 697a 6564 222c 2022 696d 706f 7274  esized", "import
-0000a1a0: 7322 7d2c 2063 6572 6369 732e 6765 745f  s"}, cercis.get_
-0000a1b0: 6675 7475 7265 5f69 6d70 6f72 7473 286e  future_imports(n
-0000a1c0: 6f64 6529 290a 2020 2020 2020 2020 6e6f  ode)).        no
-0000a1d0: 6465 203d 2063 6572 6369 732e 6c69 6232  de = cercis.lib2
-0000a1e0: 746f 335f 7061 7273 6528 0a20 2020 2020  to3_parse(.     
-0000a1f0: 2020 2020 2020 2022 6672 6f6d 205f 5f66         "from __f
-0000a200: 7574 7572 655f 5f20 696d 706f 7274 206d  uture__ import m
-0000a210: 756c 7469 706c 655c 6e66 726f 6d20 5f5f  ultiple\nfrom __
-0000a220: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
-0000a230: 696d 706f 7274 735c 6e22 0a20 2020 2020  imports\n".     
-0000a240: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000a250: 662e 6173 7365 7274 4571 7561 6c28 7b22  f.assertEqual({"
-0000a260: 6d75 6c74 6970 6c65 222c 2022 696d 706f  multiple", "impo
-0000a270: 7274 7322 7d2c 2063 6572 6369 732e 6765  rts"}, cercis.ge
-0000a280: 745f 6675 7475 7265 5f69 6d70 6f72 7473  t_future_imports
-0000a290: 286e 6f64 6529 290a 2020 2020 2020 2020  (node)).        
-0000a2a0: 6e6f 6465 203d 2063 6572 6369 732e 6c69  node = cercis.li
-0000a2b0: 6232 746f 335f 7061 7273 6528 2223 2063  b2to3_parse("# c
-0000a2c0: 6f6d 6d65 6e74 5c6e 6672 6f6d 205f 5f66  omment\nfrom __f
-0000a2d0: 7574 7572 655f 5f20 696d 706f 7274 2063  uture__ import c
-0000a2e0: 6572 6369 735c 6e22 290a 2020 2020 2020  ercis\n").      
-0000a2f0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000a300: 616c 287b 2263 6572 6369 7322 7d2c 2063  al({"cercis"}, c
-0000a310: 6572 6369 732e 6765 745f 6675 7475 7265  ercis.get_future
-0000a320: 5f69 6d70 6f72 7473 286e 6f64 6529 290a  _imports(node)).
-0000a330: 2020 2020 2020 2020 6e6f 6465 203d 2063          node = c
-0000a340: 6572 6369 732e 6c69 6232 746f 335f 7061  ercis.lib2to3_pa
-0000a350: 7273 6528 2722 2222 646f 6373 7472 696e  rse('"""docstrin
-0000a360: 6722 2222 5c6e 6672 6f6d 205f 5f66 7574  g"""\nfrom __fut
-0000a370: 7572 655f 5f20 696d 706f 7274 2063 6572  ure__ import cer
-0000a380: 6369 735c 6e27 290a 2020 2020 2020 2020  cis\n').        
-0000a390: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000a3a0: 287b 2263 6572 6369 7322 7d2c 2063 6572  ({"cercis"}, cer
-0000a3b0: 6369 732e 6765 745f 6675 7475 7265 5f69  cis.get_future_i
-0000a3c0: 6d70 6f72 7473 286e 6f64 6529 290a 2020  mports(node)).  
-0000a3d0: 2020 2020 2020 6e6f 6465 203d 2063 6572        node = cer
-0000a3e0: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
-0000a3f0: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-0000a400: 736f 6d65 286f 7468 6572 2c20 636f 6465  some(other, code
-0000a410: 295c 6e66 726f 6d20 5f5f 6675 7475 7265  )\nfrom __future
-0000a420: 5f5f 2069 6d70 6f72 7420 6365 7263 6973  __ import cercis
-0000a430: 5c6e 220a 2020 2020 2020 2020 290a 2020  \n".        ).  
-0000a440: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a450: 7445 7175 616c 2873 6574 2829 2c20 6365  tEqual(set(), ce
-0000a460: 7263 6973 2e67 6574 5f66 7574 7572 655f  rcis.get_future_
-0000a470: 696d 706f 7274 7328 6e6f 6465 2929 0a20  imports(node)). 
-0000a480: 2020 2020 2020 206e 6f64 6520 3d20 6365         node = ce
-0000a490: 7263 6973 2e6c 6962 3274 6f33 5f70 6172  rcis.lib2to3_par
-0000a4a0: 7365 2822 6672 6f6d 2073 6f6d 652e 6d6f  se("from some.mo
-0000a4b0: 6475 6c65 2069 6d70 6f72 7420 6365 7263  dule import cerc
-0000a4c0: 6973 5c6e 2229 0a20 2020 2020 2020 2073  is\n").        s
-0000a4d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000a4e0: 7365 7428 292c 2063 6572 6369 732e 6765  set(), cercis.ge
-0000a4f0: 745f 6675 7475 7265 5f69 6d70 6f72 7473  t_future_imports
-0000a500: 286e 6f64 6529 290a 2020 2020 2020 2020  (node)).        
-0000a510: 6e6f 6465 203d 2063 6572 6369 732e 6c69  node = cercis.li
-0000a520: 6232 746f 335f 7061 7273 6528 0a20 2020  b2to3_parse(.   
-0000a530: 2020 2020 2020 2020 2022 6672 6f6d 205f           "from _
-0000a540: 5f66 7574 7572 655f 5f20 696d 706f 7274  _future__ import
-0000a550: 2075 6e69 636f 6465 5f6c 6974 6572 616c   unicode_literal
-0000a560: 7320 6173 205f 756e 6963 6f64 655f 6c69  s as _unicode_li
-0000a570: 7465 7261 6c73 220a 2020 2020 2020 2020  terals".        
-0000a580: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000a590: 7373 6572 7445 7175 616c 287b 2275 6e69  ssertEqual({"uni
-0000a5a0: 636f 6465 5f6c 6974 6572 616c 7322 7d2c  code_literals"},
-0000a5b0: 2063 6572 6369 732e 6765 745f 6675 7475   cercis.get_futu
-0000a5c0: 7265 5f69 6d70 6f72 7473 286e 6f64 6529  re_imports(node)
-0000a5d0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-0000a5e0: 2063 6572 6369 732e 6c69 6232 746f 335f   cercis.lib2to3_
-0000a5f0: 7061 7273 6528 0a20 2020 2020 2020 2020  parse(.         
-0000a600: 2020 2022 6672 6f6d 205f 5f66 7574 7572     "from __futur
-0000a610: 655f 5f20 696d 706f 7274 2075 6e69 636f  e__ import unico
-0000a620: 6465 5f6c 6974 6572 616c 7320 6173 205f  de_literals as _
-0000a630: 6c6f 6c2c 2070 7269 6e74 220a 2020 2020  lol, print".    
-0000a640: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0000a650: 6c66 2e61 7373 6572 7445 7175 616c 287b  lf.assertEqual({
-0000a660: 2275 6e69 636f 6465 5f6c 6974 6572 616c  "unicode_literal
-0000a670: 7322 2c20 2270 7269 6e74 227d 2c20 6365  s", "print"}, ce
-0000a680: 7263 6973 2e67 6574 5f66 7574 7572 655f  rcis.get_future_
-0000a690: 696d 706f 7274 7328 6e6f 6465 2929 0a0a  imports(node))..
-0000a6a0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0000a6b0: 2e69 6e63 6f6d 7061 7469 626c 655f 7769  .incompatible_wi
-0000a6c0: 7468 5f6d 7970 7963 0a20 2020 2064 6566  th_mypyc.    def
-0000a6d0: 2074 6573 745f 6465 6275 675f 7669 7369   test_debug_visi
-0000a6e0: 746f 7228 7365 6c66 2920 2d3e 204e 6f6e  tor(self) -> Non
-0000a6f0: 653a 0a20 2020 2020 2020 2073 6f75 7263  e:.        sourc
-0000a700: 652c 205f 203d 2072 6561 645f 6461 7461  e, _ = read_data
-0000a710: 2822 6d69 7363 656c 6c61 6e65 6f75 7322  ("miscellaneous"
-0000a720: 2c20 2264 6562 7567 5f76 6973 6974 6f72  , "debug_visitor
-0000a730: 2229 0a20 2020 2020 2020 2065 7870 6563  ").        expec
-0000a740: 7465 642c 205f 203d 2072 6561 645f 6461  ted, _ = read_da
-0000a750: 7461 2822 6d69 7363 656c 6c61 6e65 6f75  ta("miscellaneou
-0000a760: 7322 2c20 2264 6562 7567 5f76 6973 6974  s", "debug_visit
-0000a770: 6f72 2e6f 7574 2229 0a20 2020 2020 2020  or.out").       
-0000a780: 206f 7574 5f6c 696e 6573 203d 205b 5d0a   out_lines = [].
-0000a790: 2020 2020 2020 2020 6572 725f 6c69 6e65          err_line
-0000a7a0: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
-0000a7b0: 6465 6620 6f75 7428 6d73 673a 2073 7472  def out(msg: str
-0000a7c0: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
-0000a7d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000a7e0: 2020 2020 2020 6f75 745f 6c69 6e65 732e        out_lines.
-0000a7f0: 6170 7065 6e64 286d 7367 290a 0a20 2020  append(msg)..   
-0000a800: 2020 2020 2064 6566 2065 7272 286d 7367       def err(msg
-0000a810: 3a20 7374 722c 202a 2a6b 7761 7267 733a  : str, **kwargs:
-0000a820: 2041 6e79 2920 2d3e 204e 6f6e 653a 0a20   Any) -> None:. 
-0000a830: 2020 2020 2020 2020 2020 2065 7272 5f6c             err_l
-0000a840: 696e 6573 2e61 7070 656e 6428 6d73 6729  ines.append(msg)
-0000a850: 0a0a 2020 2020 2020 2020 7769 7468 2070  ..        with p
-0000a860: 6174 6368 2822 6365 7263 6973 2e64 6562  atch("cercis.deb
-0000a870: 7567 2e6f 7574 222c 206f 7574 293a 0a20  ug.out", out):. 
-0000a880: 2020 2020 2020 2020 2020 2044 6562 7567             Debug
-0000a890: 5669 7369 746f 722e 7368 6f77 2873 6f75  Visitor.show(sou
-0000a8a0: 7263 6529 0a20 2020 2020 2020 2061 6374  rce).        act
-0000a8b0: 7561 6c20 3d20 225c 6e22 2e6a 6f69 6e28  ual = "\n".join(
-0000a8c0: 6f75 745f 6c69 6e65 7329 202b 2022 5c6e  out_lines) + "\n
-0000a8d0: 220a 2020 2020 2020 2020 6c6f 675f 6e61  ".        log_na
-0000a8e0: 6d65 203d 2022 220a 2020 2020 2020 2020  me = "".        
-0000a8f0: 6966 2065 7870 6563 7465 6420 213d 2061  if expected != a
-0000a900: 6374 7561 6c3a 0a20 2020 2020 2020 2020  ctual:.         
-0000a910: 2020 206c 6f67 5f6e 616d 6520 3d20 6365     log_name = ce
-0000a920: 7263 6973 2e64 756d 705f 746f 5f66 696c  rcis.dump_to_fil
-0000a930: 6528 2a6f 7574 5f6c 696e 6573 290a 2020  e(*out_lines).  
-0000a940: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a950: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
-0000a960: 2020 2020 6578 7065 6374 6564 2c0a 2020      expected,.  
-0000a970: 2020 2020 2020 2020 2020 6163 7475 616c            actual
-0000a980: 2c0a 2020 2020 2020 2020 2020 2020 6622  ,.            f"
-0000a990: 4153 5420 7072 696e 7420 6f75 7420 6973  AST print out is
-0000a9a0: 2064 6966 6665 7265 6e74 2e20 4163 7475   different. Actu
-0000a9b0: 616c 2076 6572 7369 6f6e 2064 756d 7065  al version dumpe
-0000a9c0: 6420 746f 207b 6c6f 675f 6e61 6d65 7d22  d to {log_name}"
-0000a9d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000a9e0: 2064 6566 2074 6573 745f 666f 726d 6174   def test_format
-0000a9f0: 5f66 696c 655f 636f 6e74 656e 7473 2873  _file_contents(s
-0000aa00: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-0000aa10: 2020 2020 2020 6d6f 6465 203d 2044 4546        mode = DEF
-0000aa20: 4155 4c54 5f4d 4f44 450a 2020 2020 2020  AULT_MODE.      
-0000aa30: 2020 656d 7074 7920 3d20 2222 0a20 2020    empty = "".   
-0000aa40: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-0000aa50: 7373 6572 7452 6169 7365 7328 6365 7263  ssertRaises(cerc
-0000aa60: 6973 2e4e 6f74 6869 6e67 4368 616e 6765  is.NothingChange
-0000aa70: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
-0000aa80: 6365 7263 6973 2e66 6f72 6d61 745f 6669  cercis.format_fi
-0000aa90: 6c65 5f63 6f6e 7465 6e74 7328 656d 7074  le_contents(empt
-0000aaa0: 792c 206d 6f64 653d 6d6f 6465 2c20 6661  y, mode=mode, fa
-0000aab0: 7374 3d46 616c 7365 290a 2020 2020 2020  st=False).      
-0000aac0: 2020 6a75 7374 5f6e 6c20 3d20 225c 6e22    just_nl = "\n"
-0000aad0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000aae0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-0000aaf0: 6365 7263 6973 2e4e 6f74 6869 6e67 4368  cercis.NothingCh
-0000ab00: 616e 6765 6429 3a0a 2020 2020 2020 2020  anged):.        
-0000ab10: 2020 2020 6365 7263 6973 2e66 6f72 6d61      cercis.forma
-0000ab20: 745f 6669 6c65 5f63 6f6e 7465 6e74 7328  t_file_contents(
-0000ab30: 6a75 7374 5f6e 6c2c 206d 6f64 653d 6d6f  just_nl, mode=mo
-0000ab40: 6465 2c20 6661 7374 3d46 616c 7365 290a  de, fast=False).
-0000ab50: 2020 2020 2020 2020 7361 6d65 203d 2022          same = "
-0000ab60: 6a20 3d20 5b31 2c20 322c 2033 5d5c 6e22  j = [1, 2, 3]\n"
-0000ab70: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000ab80: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-0000ab90: 6365 7263 6973 2e4e 6f74 6869 6e67 4368  cercis.NothingCh
-0000aba0: 616e 6765 6429 3a0a 2020 2020 2020 2020  anged):.        
-0000abb0: 2020 2020 6365 7263 6973 2e66 6f72 6d61      cercis.forma
-0000abc0: 745f 6669 6c65 5f63 6f6e 7465 6e74 7328  t_file_contents(
-0000abd0: 7361 6d65 2c20 6d6f 6465 3d6d 6f64 652c  same, mode=mode,
-0000abe0: 2066 6173 743d 4661 6c73 6529 0a20 2020   fast=False).   
-0000abf0: 2020 2020 2064 6966 6665 7265 6e74 203d       different =
-0000ac00: 2022 6a20 3d20 5b31 2c32 2c33 5d22 0a20   "j = [1,2,3]". 
-0000ac10: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
-0000ac20: 3d20 7361 6d65 0a20 2020 2020 2020 2061  = same.        a
-0000ac30: 6374 7561 6c20 3d20 6365 7263 6973 2e66  ctual = cercis.f
-0000ac40: 6f72 6d61 745f 6669 6c65 5f63 6f6e 7465  ormat_file_conte
-0000ac50: 6e74 7328 6469 6666 6572 656e 742c 206d  nts(different, m
-0000ac60: 6f64 653d 6d6f 6465 2c20 6661 7374 3d46  ode=mode, fast=F
-0000ac70: 616c 7365 290a 2020 2020 2020 2020 7365  alse).        se
-0000ac80: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-0000ac90: 7870 6563 7465 642c 2061 6374 7561 6c29  xpected, actual)
-0000aca0: 0a20 2020 2020 2020 2069 6e76 616c 6964  .        invalid
-0000acb0: 203d 2022 7265 7475 726e 2069 6620 796f   = "return if yo
-0000acc0: 7520 6361 6e22 0a20 2020 2020 2020 2077  u can".        w
-0000acd0: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
-0000ace0: 6169 7365 7328 6365 7263 6973 2e49 6e76  aises(cercis.Inv
-0000acf0: 616c 6964 496e 7075 7429 2061 7320 653a  alidInput) as e:
-0000ad00: 0a20 2020 2020 2020 2020 2020 2063 6572  .            cer
-0000ad10: 6369 732e 666f 726d 6174 5f66 696c 655f  cis.format_file_
-0000ad20: 636f 6e74 656e 7473 2869 6e76 616c 6964  contents(invalid
-0000ad30: 2c20 6d6f 6465 3d6d 6f64 652c 2066 6173  , mode=mode, fas
-0000ad40: 743d 4661 6c73 6529 0a20 2020 2020 2020  t=False).       
-0000ad50: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000ad60: 6c28 7374 7228 652e 6578 6365 7074 696f  l(str(e.exceptio
-0000ad70: 6e29 2c20 2243 616e 6e6f 7420 7061 7273  n), "Cannot pars
-0000ad80: 653a 2031 3a37 3a20 7265 7475 726e 2069  e: 1:7: return i
-0000ad90: 6620 796f 7520 6361 6e22 290a 0a20 2020  f you can")..   
-0000ada0: 2020 2020 206d 6f64 6520 3d20 6365 7263       mode = cerc
-0000adb0: 6973 2e4d 6f64 6528 7072 6576 6965 773d  is.Mode(preview=
-0000adc0: 5472 7565 290a 2020 2020 2020 2020 6a75  True).        ju
-0000add0: 7374 5f63 726c 6620 3d20 225c 725c 6e22  st_crlf = "\r\n"
-0000ade0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000adf0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-0000ae00: 6365 7263 6973 2e4e 6f74 6869 6e67 4368  cercis.NothingCh
-0000ae10: 616e 6765 6429 3a0a 2020 2020 2020 2020  anged):.        
-0000ae20: 2020 2020 6365 7263 6973 2e66 6f72 6d61      cercis.forma
-0000ae30: 745f 6669 6c65 5f63 6f6e 7465 6e74 7328  t_file_contents(
-0000ae40: 6a75 7374 5f63 726c 662c 206d 6f64 653d  just_crlf, mode=
-0000ae50: 6d6f 6465 2c20 6661 7374 3d46 616c 7365  mode, fast=False
-0000ae60: 290a 2020 2020 2020 2020 6a75 7374 5f77  ).        just_w
-0000ae70: 6869 7465 7370 6163 655f 6e6c 203d 2022  hitespace_nl = "
-0000ae80: 5c6e 5c74 5c6e 205c 6e5c 7420 5c6e 205c  \n\t\n \n\t \n \
-0000ae90: 745c 6e5c 6e22 0a20 2020 2020 2020 2061  t\n\n".        a
-0000aea0: 6374 7561 6c20 3d20 6365 7263 6973 2e66  ctual = cercis.f
-0000aeb0: 6f72 6d61 745f 6669 6c65 5f63 6f6e 7465  ormat_file_conte
-0000aec0: 6e74 7328 6a75 7374 5f77 6869 7465 7370  nts(just_whitesp
-0000aed0: 6163 655f 6e6c 2c20 6d6f 6465 3d6d 6f64  ace_nl, mode=mod
-0000aee0: 652c 2066 6173 743d 4661 6c73 6529 0a20  e, fast=False). 
-0000aef0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000af00: 7274 4571 7561 6c28 225c 6e22 2c20 6163  rtEqual("\n", ac
-0000af10: 7475 616c 290a 2020 2020 2020 2020 6a75  tual).        ju
-0000af20: 7374 5f77 6869 7465 7370 6163 655f 6372  st_whitespace_cr
-0000af30: 6c66 203d 2022 5c72 5c6e 5c74 5c72 5c6e  lf = "\r\n\t\r\n
-0000af40: 205c 725c 6e5c 7420 5c72 5c6e 205c 745c   \r\n\t \r\n \t\
-0000af50: 725c 6e5c 725c 6e22 0a20 2020 2020 2020  r\n\r\n".       
-0000af60: 2061 6374 7561 6c20 3d20 6365 7263 6973   actual = cercis
-0000af70: 2e66 6f72 6d61 745f 6669 6c65 5f63 6f6e  .format_file_con
-0000af80: 7465 6e74 7328 0a20 2020 2020 2020 2020  tents(.         
-0000af90: 2020 206a 7573 745f 7768 6974 6573 7061     just_whitespa
-0000afa0: 6365 5f63 726c 662c 206d 6f64 653d 6d6f  ce_crlf, mode=mo
-0000afb0: 6465 2c20 6661 7374 3d46 616c 7365 0a20  de, fast=False. 
-0000afc0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000afd0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000afe0: 6c28 225c 725c 6e22 2c20 6163 7475 616c  l("\r\n", actual
-0000aff0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0000b000: 656e 646d 6172 6b65 7228 7365 6c66 2920  endmarker(self) 
-0000b010: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000b020: 206e 203d 2063 6572 6369 732e 6c69 6232   n = cercis.lib2
-0000b030: 746f 335f 7061 7273 6528 225c 6e22 290a  to3_parse("\n").
-0000b040: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000b050: 6572 7445 7175 616c 286e 2e74 7970 652c  ertEqual(n.type,
-0000b060: 2063 6572 6369 732e 7379 6d73 2e66 696c   cercis.syms.fil
-0000b070: 655f 696e 7075 7429 0a20 2020 2020 2020  e_input).       
-0000b080: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000b090: 6c28 6c65 6e28 6e2e 6368 696c 6472 656e  l(len(n.children
-0000b0a0: 292c 2031 290a 2020 2020 2020 2020 7365  ), 1).        se
-0000b0b0: 6c66 2e61 7373 6572 7445 7175 616c 286e  lf.assertEqual(n
-0000b0c0: 2e63 6869 6c64 7265 6e5b 305d 2e74 7970  .children[0].typ
-0000b0d0: 652c 2063 6572 6369 732e 746f 6b65 6e2e  e, cercis.token.
-0000b0e0: 454e 444d 4152 4b45 5229 0a0a 2020 2020  ENDMARKER)..    
-0000b0f0: 4070 7974 6573 742e 6d61 726b 2e69 6e63  @pytest.mark.inc
-0000b100: 6f6d 7061 7469 626c 655f 7769 7468 5f6d  ompatible_with_m
-0000b110: 7970 7963 0a20 2020 2040 756e 6974 7465  ypyc.    @unitte
-0000b120: 7374 2e73 6b69 7049 6628 6f73 2e65 6e76  st.skipIf(os.env
-0000b130: 6972 6f6e 2e67 6574 2822 534b 4950 5f41  iron.get("SKIP_A
-0000b140: 5354 5f50 5249 4e54 2229 2c20 2275 7365  ST_PRINT"), "use
-0000b150: 7220 7365 7420 534b 4950 5f41 5354 5f50  r set SKIP_AST_P
-0000b160: 5249 4e54 2229 0a20 2020 2064 6566 2074  RINT").    def t
-0000b170: 6573 745f 6173 7365 7274 466f 726d 6174  est_assertFormat
-0000b180: 4571 7561 6c28 7365 6c66 2920 2d3e 204e  Equal(self) -> N
-0000b190: 6f6e 653a 0a20 2020 2020 2020 206f 7574  one:.        out
-0000b1a0: 5f6c 696e 6573 203d 205b 5d0a 2020 2020  _lines = [].    
-0000b1b0: 2020 2020 6572 725f 6c69 6e65 7320 3d20      err_lines = 
-0000b1c0: 5b5d 0a0a 2020 2020 2020 2020 6465 6620  []..        def 
-0000b1d0: 6f75 7428 6d73 673a 2073 7472 2c20 2a2a  out(msg: str, **
-0000b1e0: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
-0000b1f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000b200: 2020 6f75 745f 6c69 6e65 732e 6170 7065    out_lines.appe
-0000b210: 6e64 286d 7367 290a 0a20 2020 2020 2020  nd(msg)..       
-0000b220: 2064 6566 2065 7272 286d 7367 3a20 7374   def err(msg: st
-0000b230: 722c 202a 2a6b 7761 7267 733a 2041 6e79  r, **kwargs: Any
-0000b240: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000b250: 2020 2020 2020 2065 7272 5f6c 696e 6573         err_lines
-0000b260: 2e61 7070 656e 6428 6d73 6729 0a0a 2020  .append(msg)..  
-0000b270: 2020 2020 2020 7769 7468 2070 6174 6368        with patch
-0000b280: 2822 6365 7263 6973 2e6f 7574 7075 742e  ("cercis.output.
-0000b290: 5f6f 7574 222c 206f 7574 292c 2070 6174  _out", out), pat
-0000b2a0: 6368 2822 6365 7263 6973 2e6f 7574 7075  ch("cercis.outpu
-0000b2b0: 742e 5f65 7272 222c 2065 7272 293a 0a20  t._err", err):. 
-0000b2c0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000b2d0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-0000b2e0: 7328 4173 7365 7274 696f 6e45 7272 6f72  s(AssertionError
-0000b2f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000b300: 2020 2073 656c 662e 6173 7365 7274 466f     self.assertFo
-0000b310: 726d 6174 4571 7561 6c28 226a 203d 205b  rmatEqual("j = [
-0000b320: 312c 2032 2c20 335d 222c 2022 6a20 3d20  1, 2, 3]", "j = 
-0000b330: 5b31 2c20 322c 2033 2c5d 2229 0a0a 2020  [1, 2, 3,]")..  
-0000b340: 2020 2020 2020 6f75 745f 7374 7220 3d20        out_str = 
-0000b350: 2222 2e6a 6f69 6e28 6f75 745f 6c69 6e65  "".join(out_line
-0000b360: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0000b370: 6173 7365 7274 496e 2822 4578 7065 6374  assertIn("Expect
-0000b380: 6564 2074 7265 653a 222c 206f 7574 5f73  ed tree:", out_s
-0000b390: 7472 290a 2020 2020 2020 2020 7365 6c66  tr).        self
-0000b3a0: 2e61 7373 6572 7449 6e28 2241 6374 7561  .assertIn("Actua
-0000b3b0: 6c20 7472 6565 3a22 2c20 6f75 745f 7374  l tree:", out_st
-0000b3c0: 7229 0a20 2020 2020 2020 2073 656c 662e  r).        self.
-0000b3d0: 6173 7365 7274 4571 7561 6c28 2222 2e6a  assertEqual("".j
-0000b3e0: 6f69 6e28 6572 725f 6c69 6e65 7329 2c20  oin(err_lines), 
-0000b3f0: 2222 290a 0a20 2020 2040 6576 656e 745f  "")..    @event_
-0000b400: 6c6f 6f70 2829 0a20 2020 2040 7061 7463  loop().    @patc
-0000b410: 6828 2263 6f6e 6375 7272 656e 742e 6675  h("concurrent.fu
-0000b420: 7475 7265 732e 5072 6f63 6573 7350 6f6f  tures.ProcessPoo
-0000b430: 6c45 7865 6375 746f 7222 2c20 4d61 6769  lExecutor", Magi
-0000b440: 634d 6f63 6b28 7369 6465 5f65 6666 6563  cMock(side_effec
-0000b450: 743d 4f53 4572 726f 7229 290a 2020 2020  t=OSError)).    
-0000b460: 6465 6620 7465 7374 5f77 6f72 6b73 5f69  def test_works_i
-0000b470: 6e5f 6d6f 6e6f 5f70 726f 6365 7373 5f6f  n_mono_process_o
-0000b480: 6e6c 795f 656e 7669 726f 6e6d 656e 7428  nly_environment(
-0000b490: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000b4a0: 2020 2020 2020 2077 6974 6820 6361 6368         with cach
-0000b4b0: 655f 6469 7228 2920 6173 2077 6f72 6b73  e_dir() as works
-0000b4c0: 7061 6365 3a0a 2020 2020 2020 2020 2020  pace:.          
-0000b4d0: 2020 666f 7220 6620 696e 205b 0a20 2020    for f in [.   
-0000b4e0: 2020 2020 2020 2020 2020 2020 2028 776f               (wo
-0000b4f0: 726b 7370 6163 6520 2f20 226f 6e65 2e70  rkspace / "one.p
-0000b500: 7922 292e 7265 736f 6c76 6528 292c 0a20  y").resolve(),. 
-0000b510: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000b520: 776f 726b 7370 6163 6520 2f20 2274 776f  workspace / "two
-0000b530: 2e70 7922 292e 7265 736f 6c76 6528 292c  .py").resolve(),
-0000b540: 0a20 2020 2020 2020 2020 2020 205d 3a0a  .            ]:.
-0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b560: 662e 7772 6974 655f 7465 7874 2827 7072  f.write_text('pr
-0000b570: 696e 7428 2268 656c 6c6f 2229 5c6e 2729  int("hello")\n')
-0000b580: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b590: 662e 696e 766f 6b65 426c 6163 6b28 5b73  f.invokeBlack([s
-0000b5a0: 7472 2877 6f72 6b73 7061 6365 295d 290a  tr(workspace)]).
-0000b5b0: 0a20 2020 2040 6576 656e 745f 6c6f 6f70  .    @event_loop
-0000b5c0: 2829 0a20 2020 2064 6566 2074 6573 745f  ().    def test_
-0000b5d0: 6368 6563 6b5f 6469 6666 5f75 7365 5f74  check_diff_use_t
-0000b5e0: 6f67 6574 6865 7228 7365 6c66 2920 2d3e  ogether(self) ->
-0000b5f0: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-0000b600: 7120 3d20 222d 2d73 696e 676c 652d 7175  q = "--single-qu
-0000b610: 6f74 653d 4661 6c73 6522 0a20 2020 2020  ote=False".     
-0000b620: 2020 206c 6c20 3d20 222d 2d6c 696e 652d     ll = "--line-
-0000b630: 6c65 6e67 7468 3d38 3822 0a20 2020 2020  length=88".     
-0000b640: 2020 2077 6974 6820 6361 6368 655f 6469     with cache_di
-0000b650: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
-0000b660: 2023 2046 696c 6573 2077 6869 6368 2077   # Files which w
-0000b670: 696c 6c20 6265 2072 6566 6f72 6d61 7474  ill be reformatt
-0000b680: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-0000b690: 7372 6331 203d 2067 6574 5f63 6173 655f  src1 = get_case_
-0000b6a0: 7061 7468 2822 6d69 7363 656c 6c61 6e65  path("miscellane
-0000b6b0: 6f75 7322 2c20 2273 7472 696e 675f 7175  ous", "string_qu
-0000b6c0: 6f74 6573 2229 0a20 2020 2020 2020 2020  otes").         
-0000b6d0: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
-0000b6e0: 6163 6b28 5b73 7472 2873 7263 3129 2c20  ack([str(src1), 
-0000b6f0: 222d 2d64 6966 6622 2c20 222d 2d63 6865  "--diff", "--che
-0000b700: 636b 222c 2073 712c 206c 6c5d 2c20 6578  ck", sq, ll], ex
-0000b710: 6974 5f63 6f64 653d 3129 0a20 2020 2020  it_code=1).     
-0000b720: 2020 2020 2020 2023 2046 696c 6573 2077         # Files w
-0000b730: 6869 6368 2077 696c 6c20 6e6f 7420 6265  hich will not be
-0000b740: 2072 6566 6f72 6d61 7474 6564 2e0a 2020   reformatted..  
-0000b750: 2020 2020 2020 2020 2020 7372 6332 203d            src2 =
-0000b760: 2067 6574 5f63 6173 655f 7061 7468 2822   get_case_path("
-0000b770: 7369 6d70 6c65 5f63 6173 6573 222c 2022  simple_cases", "
-0000b780: 636f 6d70 6f73 6974 696f 6e22 290a 2020  composition").  
-0000b790: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-0000b7a0: 6e76 6f6b 6542 6c61 636b 285b 7374 7228  nvokeBlack([str(
-0000b7b0: 7372 6332 292c 2022 2d2d 6469 6666 222c  src2), "--diff",
-0000b7c0: 2022 2d2d 6368 6563 6b22 2c20 7371 2c20   "--check", sq, 
-0000b7d0: 6c6c 5d29 0a20 2020 2020 2020 2020 2020  ll]).           
-0000b7e0: 2023 204d 756c 7469 2066 696c 6520 636f   # Multi file co
-0000b7f0: 6d6d 616e 642e 0a20 2020 2020 2020 2020  mmand..         
-0000b800: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
-0000b810: 6163 6b28 0a20 2020 2020 2020 2020 2020  ack(.           
-0000b820: 2020 2020 205b 7374 7228 7372 6331 292c       [str(src1),
-0000b830: 2073 7472 2873 7263 3229 2c20 222d 2d64   str(src2), "--d
-0000b840: 6966 6622 2c20 222d 2d63 6865 636b 222c  iff", "--check",
-0000b850: 2073 712c 206c 6c5d 2c0a 2020 2020 2020   sq, ll],.      
-0000b860: 2020 2020 2020 2020 2020 6578 6974 5f63            exit_c
-0000b870: 6f64 653d 312c 0a20 2020 2020 2020 2020  ode=1,.         
-0000b880: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-0000b890: 7374 5f6e 6f5f 7372 635f 6661 696c 7328  st_no_src_fails(
-0000b8a0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000b8b0: 2020 2020 2020 2077 6974 6820 6361 6368         with cach
-0000b8c0: 655f 6469 7228 293a 0a20 2020 2020 2020  e_dir():.       
-0000b8d0: 2020 2020 2073 656c 662e 696e 766f 6b65       self.invoke
-0000b8e0: 426c 6163 6b28 5b5d 2c20 6578 6974 5f63  Black([], exit_c
-0000b8f0: 6f64 653d 3129 0a0a 2020 2020 6465 6620  ode=1)..    def 
-0000b900: 7465 7374 5f73 7263 5f61 6e64 5f63 6f64  test_src_and_cod
-0000b910: 655f 6661 696c 7328 7365 6c66 2920 2d3e  e_fails(self) ->
-0000b920: 204e 6f6e 653a 0a20 2020 2020 2020 2077   None:.        w
-0000b930: 6974 6820 6361 6368 655f 6469 7228 293a  ith cache_dir():
-0000b940: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b950: 662e 696e 766f 6b65 426c 6163 6b28 5b22  f.invokeBlack(["
-0000b960: 2e22 2c20 222d 6322 2c20 2230 225d 2c20  .", "-c", "0"], 
-0000b970: 6578 6974 5f63 6f64 653d 3129 0a0a 2020  exit_code=1)..  
-0000b980: 2020 6465 6620 7465 7374 5f62 726f 6b65    def test_broke
-0000b990: 6e5f 7379 6d6c 696e 6b28 7365 6c66 2920  n_symlink(self) 
-0000b9a0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000b9b0: 2077 6974 6820 6361 6368 655f 6469 7228   with cache_dir(
-0000b9c0: 2920 6173 2077 6f72 6b73 7061 6365 3a0a  ) as workspace:.
-0000b9d0: 2020 2020 2020 2020 2020 2020 7379 6d6c              syml
-0000b9e0: 696e 6b20 3d20 776f 726b 7370 6163 6520  ink = workspace 
-0000b9f0: 2f20 2262 726f 6b65 6e5f 6c69 6e6b 2e70  / "broken_link.p
-0000ba00: 7922 0a20 2020 2020 2020 2020 2020 2074  y".            t
-0000ba10: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000ba20: 2020 2020 7379 6d6c 696e 6b2e 7379 6d6c      symlink.syml
-0000ba30: 696e 6b5f 746f 2822 6e6f 6e65 7869 7374  ink_to("nonexist
-0000ba40: 656e 742e 7079 2229 0a20 2020 2020 2020  ent.py").       
-0000ba50: 2020 2020 2065 7863 6570 7420 284f 5345       except (OSE
-0000ba60: 7272 6f72 2c20 4e6f 7449 6d70 6c65 6d65  rror, NotImpleme
-0000ba70: 6e74 6564 4572 726f 7229 2061 7320 653a  ntedError) as e:
-0000ba80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ba90: 2073 656c 662e 736b 6970 5465 7374 2866   self.skipTest(f
-0000baa0: 2243 616e 2774 2063 7265 6174 6520 7379  "Can't create sy
-0000bab0: 6d6c 696e 6b73 3a20 7b65 7d22 290a 2020  mlinks: {e}").  
-0000bac0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-0000bad0: 6e76 6f6b 6542 6c61 636b 285b 7374 7228  nvokeBlack([str(
-0000bae0: 776f 726b 7370 6163 652e 7265 736f 6c76  workspace.resolv
-0000baf0: 6528 2929 5d29 0a0a 2020 2020 6465 6620  e())])..    def 
-0000bb00: 7465 7374 5f73 696e 676c 655f 6669 6c65  test_single_file
-0000bb10: 5f66 6f72 6365 5f70 7969 2873 656c 6629  _force_pyi(self)
-0000bb20: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000bb30: 2020 7079 695f 6d6f 6465 203d 2072 6570    pyi_mode = rep
-0000bb40: 6c61 6365 2844 4546 4155 4c54 5f4d 4f44  lace(DEFAULT_MOD
-0000bb50: 452c 2069 735f 7079 693d 5472 7565 290a  E, is_pyi=True).
-0000bb60: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-0000bb70: 2c20 6578 7065 6374 6564 203d 2072 6561  , expected = rea
-0000bb80: 645f 6461 7461 2822 6d69 7363 656c 6c61  d_data("miscella
-0000bb90: 6e65 6f75 7322 2c20 2266 6f72 6365 5f70  neous", "force_p
-0000bba0: 7969 2229 0a20 2020 2020 2020 2077 6974  yi").        wit
-0000bbb0: 6820 6361 6368 655f 6469 7228 2920 6173  h cache_dir() as
-0000bbc0: 2077 6f72 6b73 7061 6365 3a0a 2020 2020   workspace:.    
-0000bbd0: 2020 2020 2020 2020 7061 7468 203d 2028          path = (
-0000bbe0: 776f 726b 7370 6163 6520 2f20 2266 696c  workspace / "fil
-0000bbf0: 652e 7079 2229 2e72 6573 6f6c 7665 2829  e.py").resolve()
-0000bc00: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000bc10: 6820 6f70 656e 2870 6174 682c 2022 7722  h open(path, "w"
-0000bc20: 2920 6173 2066 683a 0a20 2020 2020 2020  ) as fh:.       
-0000bc30: 2020 2020 2020 2020 2066 682e 7772 6974           fh.writ
-0000bc40: 6528 636f 6e74 656e 7473 290a 2020 2020  e(contents).    
-0000bc50: 2020 2020 2020 2020 7365 6c66 2e69 6e76          self.inv
-0000bc60: 6f6b 6542 6c61 636b 285b 7374 7228 7061  okeBlack([str(pa
-0000bc70: 7468 292c 2022 2d2d 7079 6922 5d29 0a20  th), "--pyi"]). 
-0000bc80: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000bc90: 6f70 656e 2870 6174 682c 2022 7222 2920  open(path, "r") 
-0000bca0: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
-0000bcb0: 2020 2020 2020 2061 6374 7561 6c20 3d20         actual = 
-0000bcc0: 6668 2e72 6561 6428 290a 2020 2020 2020  fh.read().      
-0000bcd0: 2020 2020 2020 2320 7665 7269 6679 2063        # verify c
-0000bce0: 6163 6865 2077 6974 6820 2d2d 7079 6920  ache with --pyi 
-0000bcf0: 6973 2073 6570 6172 6174 650a 2020 2020  is separate.    
-0000bd00: 2020 2020 2020 2020 7079 695f 6361 6368          pyi_cach
-0000bd10: 6520 3d20 6365 7263 6973 2e72 6561 645f  e = cercis.read_
-0000bd20: 6361 6368 6528 7079 695f 6d6f 6465 290a  cache(pyi_mode).
-0000bd30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000bd40: 2e61 7373 6572 7449 6e28 7374 7228 7061  .assertIn(str(pa
-0000bd50: 7468 292c 2070 7969 5f63 6163 6865 290a  th), pyi_cache).
-0000bd60: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
-0000bd70: 616c 5f63 6163 6865 203d 2063 6572 6369  al_cache = cerci
-0000bd80: 732e 7265 6164 5f63 6163 6865 2844 4546  s.read_cache(DEF
-0000bd90: 4155 4c54 5f4d 4f44 4529 0a20 2020 2020  AULT_MODE).     
-0000bda0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000bdb0: 7274 4e6f 7449 6e28 7374 7228 7061 7468  rtNotIn(str(path
-0000bdc0: 292c 206e 6f72 6d61 6c5f 6361 6368 6529  ), normal_cache)
-0000bdd0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000bde0: 7365 7274 466f 726d 6174 4571 7561 6c28  sertFormatEqual(
-0000bdf0: 6578 7065 6374 6564 2c20 6163 7475 616c  expected, actual
-0000be00: 290a 2020 2020 2020 2020 6365 7263 6973  ).        cercis
-0000be10: 2e61 7373 6572 745f 6571 7569 7661 6c65  .assert_equivale
-0000be20: 6e74 2863 6f6e 7465 6e74 732c 2061 6374  nt(contents, act
-0000be30: 7561 6c29 0a20 2020 2020 2020 2063 6572  ual).        cer
-0000be40: 6369 732e 6173 7365 7274 5f73 7461 626c  cis.assert_stabl
-0000be50: 6528 636f 6e74 656e 7473 2c20 6163 7475  e(contents, actu
-0000be60: 616c 2c20 7079 695f 6d6f 6465 290a 0a20  al, pyi_mode).. 
-0000be70: 2020 2040 6576 656e 745f 6c6f 6f70 2829     @event_loop()
-0000be80: 0a20 2020 2064 6566 2074 6573 745f 6d75  .    def test_mu
-0000be90: 6c74 695f 6669 6c65 5f66 6f72 6365 5f70  lti_file_force_p
-0000bea0: 7969 2873 656c 6629 202d 3e20 4e6f 6e65  yi(self) -> None
-0000beb0: 3a0a 2020 2020 2020 2020 7265 675f 6d6f  :.        reg_mo
-0000bec0: 6465 203d 2044 4546 4155 4c54 5f4d 4f44  de = DEFAULT_MOD
-0000bed0: 450a 2020 2020 2020 2020 7079 695f 6d6f  E.        pyi_mo
-0000bee0: 6465 203d 2072 6570 6c61 6365 2844 4546  de = replace(DEF
-0000bef0: 4155 4c54 5f4d 4f44 452c 2069 735f 7079  AULT_MODE, is_py
-0000bf00: 693d 5472 7565 290a 2020 2020 2020 2020  i=True).        
-0000bf10: 636f 6e74 656e 7473 2c20 6578 7065 6374  contents, expect
-0000bf20: 6564 203d 2072 6561 645f 6461 7461 2822  ed = read_data("
-0000bf30: 6d69 7363 656c 6c61 6e65 6f75 7322 2c20  miscellaneous", 
-0000bf40: 2266 6f72 6365 5f70 7969 2229 0a20 2020  "force_pyi").   
-0000bf50: 2020 2020 2077 6974 6820 6361 6368 655f       with cache_
-0000bf60: 6469 7228 2920 6173 2077 6f72 6b73 7061  dir() as workspa
-0000bf70: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-0000bf80: 7061 7468 7320 3d20 5b0a 2020 2020 2020  paths = [.      
-0000bf90: 2020 2020 2020 2020 2020 2877 6f72 6b73            (works
-0000bfa0: 7061 6365 202f 2022 6669 6c65 312e 7079  pace / "file1.py
-0000bfb0: 2229 2e72 6573 6f6c 7665 2829 2c0a 2020  ").resolve(),.  
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2877                (w
-0000bfd0: 6f72 6b73 7061 6365 202f 2022 6669 6c65  orkspace / "file
-0000bfe0: 322e 7079 2229 2e72 6573 6f6c 7665 2829  2.py").resolve()
-0000bff0: 2c0a 2020 2020 2020 2020 2020 2020 5d0a  ,.            ].
-0000c000: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000c010: 7061 7468 2069 6e20 7061 7468 733a 0a20  path in paths:. 
-0000c020: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000c030: 6974 6820 6f70 656e 2870 6174 682c 2022  ith open(path, "
-0000c040: 7722 2920 6173 2066 683a 0a20 2020 2020  w") as fh:.     
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c060: 682e 7772 6974 6528 636f 6e74 656e 7473  h.write(contents
-0000c070: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000c080: 6c66 2e69 6e76 6f6b 6542 6c61 636b 285b  lf.invokeBlack([
-0000c090: 7374 7228 7029 2066 6f72 2070 2069 6e20  str(p) for p in 
-0000c0a0: 7061 7468 735d 202b 205b 222d 2d70 7969  paths] + ["--pyi
-0000c0b0: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
-0000c0c0: 666f 7220 7061 7468 2069 6e20 7061 7468  for path in path
-0000c0d0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000c0e0: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
-0000c0f0: 682c 2022 7222 2920 6173 2066 683a 0a20  h, "r") as fh:. 
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2061 6374 7561 6c20 3d20 6668 2e72     actual = fh.r
-0000c120: 6561 6428 290a 2020 2020 2020 2020 2020  ead().          
-0000c130: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000c140: 7445 7175 616c 2861 6374 7561 6c2c 2065  tEqual(actual, e
-0000c150: 7870 6563 7465 6429 0a20 2020 2020 2020  xpected).       
-0000c160: 2020 2020 2023 2076 6572 6966 7920 6361       # verify ca
-0000c170: 6368 6520 7769 7468 202d 2d70 7969 2069  che with --pyi i
-0000c180: 7320 7365 7061 7261 7465 0a20 2020 2020  s separate.     
-0000c190: 2020 2020 2020 2070 7969 5f63 6163 6865         pyi_cache
-0000c1a0: 203d 2063 6572 6369 732e 7265 6164 5f63   = cercis.read_c
-0000c1b0: 6163 6865 2870 7969 5f6d 6f64 6529 0a20  ache(pyi_mode). 
-0000c1c0: 2020 2020 2020 2020 2020 206e 6f72 6d61             norma
-0000c1d0: 6c5f 6361 6368 6520 3d20 6365 7263 6973  l_cache = cercis
-0000c1e0: 2e72 6561 645f 6361 6368 6528 7265 675f  .read_cache(reg_
-0000c1f0: 6d6f 6465 290a 2020 2020 2020 2020 2020  mode).          
-0000c200: 2020 666f 7220 7061 7468 2069 6e20 7061    for path in pa
-0000c210: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
-0000c220: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000c230: 496e 2873 7472 2870 6174 6829 2c20 7079  In(str(path), py
-0000c240: 695f 6361 6368 6529 0a20 2020 2020 2020  i_cache).       
-0000c250: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000c260: 7365 7274 4e6f 7449 6e28 7374 7228 7061  sertNotIn(str(pa
-0000c270: 7468 292c 206e 6f72 6d61 6c5f 6361 6368  th), normal_cach
-0000c280: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
-0000c290: 5f70 6970 655f 666f 7263 655f 7079 6928  _pipe_force_pyi(
-0000c2a0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000c2b0: 2020 2020 2020 2073 6f75 7263 652c 2065         source, e
-0000c2c0: 7870 6563 7465 6420 3d20 7265 6164 5f64  xpected = read_d
-0000c2d0: 6174 6128 226d 6973 6365 6c6c 616e 656f  ata("miscellaneo
-0000c2e0: 7573 222c 2022 666f 7263 655f 7079 6922  us", "force_pyi"
-0000c2f0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-0000c300: 203d 2043 6c69 5275 6e6e 6572 2829 2e69   = CliRunner().i
-0000c310: 6e76 6f6b 6528 0a20 2020 2020 2020 2020  nvoke(.         
-0000c320: 2020 2063 6572 6369 732e 6d61 696e 2c20     cercis.main, 
-0000c330: 5b22 2d22 2c20 222d 7122 2c20 222d 2d70  ["-", "-q", "--p
-0000c340: 7969 225d 2c20 696e 7075 743d 4279 7465  yi"], input=Byte
-0000c350: 7349 4f28 736f 7572 6365 2e65 6e63 6f64  sIO(source.encod
-0000c360: 6528 2275 7466 3822 2929 0a20 2020 2020  e("utf8")).     
-0000c370: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000c380: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-0000c390: 7375 6c74 2e65 7869 745f 636f 6465 2c20  sult.exit_code, 
-0000c3a0: 3029 0a20 2020 2020 2020 2061 6374 7561  0).        actua
-0000c3b0: 6c20 3d20 7265 7375 6c74 2e6f 7574 7075  l = result.outpu
-0000c3c0: 740a 2020 2020 2020 2020 7365 6c66 2e61  t.        self.a
-0000c3d0: 7373 6572 7446 6f72 6d61 7445 7175 616c  ssertFormatEqual
-0000c3e0: 2861 6374 7561 6c2c 2065 7870 6563 7465  (actual, expecte
-0000c3f0: 6429 0a0a 2020 2020 6465 6620 7465 7374  d)..    def test
-0000c400: 5f73 696e 676c 655f 6669 6c65 5f66 6f72  _single_file_for
-0000c410: 6365 5f70 7933 3628 7365 6c66 2920 2d3e  ce_py36(self) ->
-0000c420: 204e 6f6e 653a 0a20 2020 2020 2020 2072   None:.        r
-0000c430: 6567 5f6d 6f64 6520 3d20 4445 4641 554c  eg_mode = DEFAUL
-0000c440: 545f 4d4f 4445 0a20 2020 2020 2020 2070  T_MODE.        p
-0000c450: 7933 365f 6d6f 6465 203d 2072 6570 6c61  y36_mode = repla
-0000c460: 6365 2844 4546 4155 4c54 5f4d 4f44 452c  ce(DEFAULT_MODE,
-0000c470: 2074 6172 6765 745f 7665 7273 696f 6e73   target_versions
-0000c480: 3d50 5933 365f 5645 5253 494f 4e53 290a  =PY36_VERSIONS).
-0000c490: 2020 2020 2020 2020 736f 7572 6365 2c20          source, 
-0000c4a0: 6578 7065 6374 6564 203d 2072 6561 645f  expected = read_
-0000c4b0: 6461 7461 2822 6d69 7363 656c 6c61 6e65  data("miscellane
-0000c4c0: 6f75 7322 2c20 2266 6f72 6365 5f70 7933  ous", "force_py3
-0000c4d0: 3622 290a 2020 2020 2020 2020 7769 7468  6").        with
-0000c4e0: 2063 6163 6865 5f64 6972 2829 2061 7320   cache_dir() as 
-0000c4f0: 776f 726b 7370 6163 653a 0a20 2020 2020  workspace:.     
-0000c500: 2020 2020 2020 2070 6174 6820 3d20 2877         path = (w
-0000c510: 6f72 6b73 7061 6365 202f 2022 6669 6c65  orkspace / "file
-0000c520: 2e70 7922 292e 7265 736f 6c76 6528 290a  .py").resolve().
-0000c530: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000c540: 206f 7065 6e28 7061 7468 2c20 2277 2229   open(path, "w")
-0000c550: 2061 7320 6668 3a0a 2020 2020 2020 2020   as fh:.        
-0000c560: 2020 2020 2020 2020 6668 2e77 7269 7465          fh.write
-0000c570: 2873 6f75 7263 6529 0a20 2020 2020 2020  (source).       
-0000c580: 2020 2020 2073 656c 662e 696e 766f 6b65       self.invoke
-0000c590: 426c 6163 6b28 5b73 7472 2870 6174 6829  Black([str(path)
-0000c5a0: 2c20 2a50 5933 365f 4152 4753 5d29 0a20  , *PY36_ARGS]). 
-0000c5b0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000c5c0: 6f70 656e 2870 6174 682c 2022 7222 2920  open(path, "r") 
-0000c5d0: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
-0000c5e0: 2020 2020 2020 2061 6374 7561 6c20 3d20         actual = 
-0000c5f0: 6668 2e72 6561 6428 290a 2020 2020 2020  fh.read().      
-0000c600: 2020 2020 2020 2320 7665 7269 6679 2063        # verify c
-0000c610: 6163 6865 2077 6974 6820 2d2d 7461 7267  ache with --targ
-0000c620: 6574 2d76 6572 7369 6f6e 2069 7320 7365  et-version is se
-0000c630: 7061 7261 7465 0a20 2020 2020 2020 2020  parate.         
-0000c640: 2020 2070 7933 365f 6361 6368 6520 3d20     py36_cache = 
-0000c650: 6365 7263 6973 2e72 6561 645f 6361 6368  cercis.read_cach
-0000c660: 6528 7079 3336 5f6d 6f64 6529 0a20 2020  e(py36_mode).   
-0000c670: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000c680: 7365 7274 496e 2873 7472 2870 6174 6829  sertIn(str(path)
-0000c690: 2c20 7079 3336 5f63 6163 6865 290a 2020  , py36_cache).  
-0000c6a0: 2020 2020 2020 2020 2020 6e6f 726d 616c            normal
-0000c6b0: 5f63 6163 6865 203d 2063 6572 6369 732e  _cache = cercis.
-0000c6c0: 7265 6164 5f63 6163 6865 2872 6567 5f6d  read_cache(reg_m
-0000c6d0: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
-0000c6e0: 2073 656c 662e 6173 7365 7274 4e6f 7449   self.assertNotI
-0000c6f0: 6e28 7374 7228 7061 7468 292c 206e 6f72  n(str(path), nor
-0000c700: 6d61 6c5f 6361 6368 6529 0a20 2020 2020  mal_cache).     
-0000c710: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000c720: 7561 6c28 6163 7475 616c 2c20 6578 7065  ual(actual, expe
-0000c730: 6374 6564 290a 0a20 2020 2040 6576 656e  cted)..    @even
-0000c740: 745f 6c6f 6f70 2829 0a20 2020 2064 6566  t_loop().    def
-0000c750: 2074 6573 745f 6d75 6c74 695f 6669 6c65   test_multi_file
-0000c760: 5f66 6f72 6365 5f70 7933 3628 7365 6c66  _force_py36(self
-0000c770: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000c780: 2020 2072 6567 5f6d 6f64 6520 3d20 4445     reg_mode = DE
-0000c790: 4641 554c 545f 4d4f 4445 0a20 2020 2020  FAULT_MODE.     
-0000c7a0: 2020 2070 7933 365f 6d6f 6465 203d 2072     py36_mode = r
-0000c7b0: 6570 6c61 6365 2844 4546 4155 4c54 5f4d  eplace(DEFAULT_M
-0000c7c0: 4f44 452c 2074 6172 6765 745f 7665 7273  ODE, target_vers
-0000c7d0: 696f 6e73 3d50 5933 365f 5645 5253 494f  ions=PY36_VERSIO
-0000c7e0: 4e53 290a 2020 2020 2020 2020 736f 7572  NS).        sour
-0000c7f0: 6365 2c20 6578 7065 6374 6564 203d 2072  ce, expected = r
-0000c800: 6561 645f 6461 7461 2822 6d69 7363 656c  ead_data("miscel
-0000c810: 6c61 6e65 6f75 7322 2c20 2266 6f72 6365  laneous", "force
-0000c820: 5f70 7933 3622 290a 2020 2020 2020 2020  _py36").        
-0000c830: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
-0000c840: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
-0000c850: 2020 2020 2020 2020 2020 2070 6174 6873             paths
-0000c860: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-0000c870: 2020 2020 2028 776f 726b 7370 6163 6520       (workspace 
-0000c880: 2f20 2266 696c 6531 2e70 7922 292e 7265  / "file1.py").re
-0000c890: 736f 6c76 6528 292c 0a20 2020 2020 2020  solve(),.       
-0000c8a0: 2020 2020 2020 2020 2028 776f 726b 7370           (worksp
-0000c8b0: 6163 6520 2f20 2266 696c 6532 2e70 7922  ace / "file2.py"
-0000c8c0: 292e 7265 736f 6c76 6528 292c 0a20 2020  ).resolve(),.   
-0000c8d0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-0000c8e0: 2020 2020 2020 2066 6f72 2070 6174 6820         for path 
-0000c8f0: 696e 2070 6174 6873 3a0a 2020 2020 2020  in paths:.      
-0000c900: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-0000c910: 7065 6e28 7061 7468 2c20 2277 2229 2061  pen(path, "w") a
-0000c920: 7320 6668 3a0a 2020 2020 2020 2020 2020  s fh:.          
-0000c930: 2020 2020 2020 2020 2020 6668 2e77 7269            fh.wri
-0000c940: 7465 2873 6f75 7263 6529 0a20 2020 2020  te(source).     
-0000c950: 2020 2020 2020 2073 656c 662e 696e 766f         self.invo
-0000c960: 6b65 426c 6163 6b28 5b73 7472 2870 2920  keBlack([str(p) 
-0000c970: 666f 7220 7020 696e 2070 6174 6873 5d20  for p in paths] 
-0000c980: 2b20 5059 3336 5f41 5247 5329 0a20 2020  + PY36_ARGS).   
-0000c990: 2020 2020 2020 2020 2066 6f72 2070 6174           for pat
-0000c9a0: 6820 696e 2070 6174 6873 3a0a 2020 2020  h in paths:.    
-0000c9b0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000c9c0: 206f 7065 6e28 7061 7468 2c20 2272 2229   open(path, "r")
-0000c9d0: 2061 7320 6668 3a0a 2020 2020 2020 2020   as fh:.        
-0000c9e0: 2020 2020 2020 2020 2020 2020 6163 7475              actu
-0000c9f0: 616c 203d 2066 682e 7265 6164 2829 0a20  al = fh.read(). 
-0000ca00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ca10: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000ca20: 6163 7475 616c 2c20 6578 7065 6374 6564  actual, expected
-0000ca30: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0000ca40: 7665 7269 6679 2063 6163 6865 2077 6974  verify cache wit
-0000ca50: 6820 2d2d 7461 7267 6574 2d76 6572 7369  h --target-versi
-0000ca60: 6f6e 2069 7320 7365 7061 7261 7465 0a20  on is separate. 
-0000ca70: 2020 2020 2020 2020 2020 2070 7969 5f63             pyi_c
-0000ca80: 6163 6865 203d 2063 6572 6369 732e 7265  ache = cercis.re
-0000ca90: 6164 5f63 6163 6865 2870 7933 365f 6d6f  ad_cache(py36_mo
-0000caa0: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
-0000cab0: 6e6f 726d 616c 5f63 6163 6865 203d 2063  normal_cache = c
-0000cac0: 6572 6369 732e 7265 6164 5f63 6163 6865  ercis.read_cache
-0000cad0: 2872 6567 5f6d 6f64 6529 0a20 2020 2020  (reg_mode).     
-0000cae0: 2020 2020 2020 2066 6f72 2070 6174 6820         for path 
-0000caf0: 696e 2070 6174 6873 3a0a 2020 2020 2020  in paths:.      
-0000cb00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000cb10: 7373 6572 7449 6e28 7374 7228 7061 7468  ssertIn(str(path
-0000cb20: 292c 2070 7969 5f63 6163 6865 290a 2020  ), pyi_cache).  
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000cb40: 6c66 2e61 7373 6572 744e 6f74 496e 2873  lf.assertNotIn(s
-0000cb50: 7472 2870 6174 6829 2c20 6e6f 726d 616c  tr(path), normal
-0000cb60: 5f63 6163 6865 290a 0a20 2020 2064 6566  _cache)..    def
-0000cb70: 2074 6573 745f 7069 7065 5f66 6f72 6365   test_pipe_force
-0000cb80: 5f70 7933 3628 7365 6c66 2920 2d3e 204e  _py36(self) -> N
-0000cb90: 6f6e 653a 0a20 2020 2020 2020 2073 6f75  one:.        sou
-0000cba0: 7263 652c 2065 7870 6563 7465 6420 3d20  rce, expected = 
-0000cbb0: 7265 6164 5f64 6174 6128 226d 6973 6365  read_data("misce
-0000cbc0: 6c6c 616e 656f 7573 222c 2022 666f 7263  llaneous", "forc
-0000cbd0: 655f 7079 3336 2229 0a20 2020 2020 2020  e_py36").       
-0000cbe0: 2072 6573 756c 7420 3d20 436c 6952 756e   result = CliRun
-0000cbf0: 6e65 7228 292e 696e 766f 6b65 280a 2020  ner().invoke(.  
-0000cc00: 2020 2020 2020 2020 2020 6365 7263 6973            cercis
-0000cc10: 2e6d 6169 6e2c 0a20 2020 2020 2020 2020  .main,.         
-0000cc20: 2020 205b 222d 222c 2022 2d71 222c 2022     ["-", "-q", "
-0000cc30: 2d2d 7461 7267 6574 2d76 6572 7369 6f6e  --target-version
-0000cc40: 3d70 7933 3622 5d2c 0a20 2020 2020 2020  =py36"],.       
-0000cc50: 2020 2020 2069 6e70 7574 3d42 7974 6573       input=Bytes
-0000cc60: 494f 2873 6f75 7263 652e 656e 636f 6465  IO(source.encode
-0000cc70: 2822 7574 6638 2229 292c 0a20 2020 2020  ("utf8")),.     
-0000cc80: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000cc90: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-0000cca0: 7375 6c74 2e65 7869 745f 636f 6465 2c20  sult.exit_code, 
-0000ccb0: 3029 0a20 2020 2020 2020 2061 6374 7561  0).        actua
-0000ccc0: 6c20 3d20 7265 7375 6c74 2e6f 7574 7075  l = result.outpu
-0000ccd0: 740a 2020 2020 2020 2020 7365 6c66 2e61  t.        self.a
-0000cce0: 7373 6572 7446 6f72 6d61 7445 7175 616c  ssertFormatEqual
-0000ccf0: 2861 6374 7561 6c2c 2065 7870 6563 7465  (actual, expecte
-0000cd00: 6429 0a0a 2020 2020 4070 7974 6573 742e  d)..    @pytest.
-0000cd10: 6d61 726b 2e69 6e63 6f6d 7061 7469 626c  mark.incompatibl
-0000cd20: 655f 7769 7468 5f6d 7970 7963 0a20 2020  e_with_mypyc.   
-0000cd30: 2064 6566 2074 6573 745f 7265 666f 726d   def test_reform
-0000cd40: 6174 5f6f 6e65 5f77 6974 685f 7374 6469  at_one_with_stdi
-0000cd50: 6e28 7365 6c66 2920 2d3e 204e 6f6e 653a  n(self) -> None:
-0000cd60: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
-0000cd70: 7463 6828 0a20 2020 2020 2020 2020 2020  tch(.           
-0000cd80: 2022 6365 7263 6973 2e66 6f72 6d61 745f   "cercis.format_
-0000cd90: 7374 6469 6e5f 746f 5f73 7464 6f75 7422  stdin_to_stdout"
-0000cda0: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-0000cdb0: 7475 726e 5f76 616c 7565 3d6c 616d 6264  turn_value=lambd
-0000cdc0: 6120 2a61 7267 732c 202a 2a6b 7761 7267  a *args, **kwarg
-0000cdd0: 733a 2063 6572 6369 732e 4368 616e 6765  s: cercis.Change
-0000cde0: 642e 5945 532c 0a20 2020 2020 2020 2029  d.YES,.        )
-0000cdf0: 2061 7320 6673 7473 3a0a 2020 2020 2020   as fsts:.      
-0000ce00: 2020 2020 2020 7265 706f 7274 203d 204d        report = M
-0000ce10: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
-0000ce20: 2020 2020 2020 2070 6174 6820 3d20 5061         path = Pa
-0000ce30: 7468 2822 2d22 290a 2020 2020 2020 2020  th("-").        
-0000ce40: 2020 2020 6365 7263 6973 2e72 6566 6f72      cercis.refor
-0000ce50: 6d61 745f 6f6e 6528 0a20 2020 2020 2020  mat_one(.       
-0000ce60: 2020 2020 2020 2020 2070 6174 682c 0a20           path,. 
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ce80: 6173 743d 5472 7565 2c0a 2020 2020 2020  ast=True,.      
-0000ce90: 2020 2020 2020 2020 2020 7772 6974 655f            write_
-0000cea0: 6261 636b 3d63 6572 6369 732e 5772 6974  back=cercis.Writ
-0000ceb0: 6542 6163 6b2e 5945 532c 0a20 2020 2020  eBack.YES,.     
-0000cec0: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
-0000ced0: 4445 4641 554c 545f 4d4f 4445 2c0a 2020  DEFAULT_MODE,.  
-0000cee0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000cef0: 706f 7274 3d72 6570 6f72 742c 0a20 2020  port=report,.   
-0000cf00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000cf10: 2020 2020 2020 2066 7374 732e 6173 7365         fsts.asse
-0000cf20: 7274 5f63 616c 6c65 645f 6f6e 6365 2829  rt_called_once()
-0000cf30: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-0000cf40: 6f72 742e 646f 6e65 2e61 7373 6572 745f  ort.done.assert_
-0000cf50: 6361 6c6c 6564 5f77 6974 6828 7061 7468  called_with(path
-0000cf60: 2c20 6365 7263 6973 2e43 6861 6e67 6564  , cercis.Changed
-0000cf70: 2e59 4553 290a 0a20 2020 2040 7079 7465  .YES)..    @pyte
-0000cf80: 7374 2e6d 6172 6b2e 696e 636f 6d70 6174  st.mark.incompat
-0000cf90: 6962 6c65 5f77 6974 685f 6d79 7079 630a  ible_with_mypyc.
-0000cfa0: 2020 2020 6465 6620 7465 7374 5f72 6566      def test_ref
-0000cfb0: 6f72 6d61 745f 6f6e 655f 7769 7468 5f73  ormat_one_with_s
-0000cfc0: 7464 696e 5f66 696c 656e 616d 6528 7365  tdin_filename(se
-0000cfd0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000cfe0: 2020 2020 2077 6974 6820 7061 7463 6828       with patch(
-0000cff0: 0a20 2020 2020 2020 2020 2020 2022 6365  .            "ce
-0000d000: 7263 6973 2e66 6f72 6d61 745f 7374 6469  rcis.format_stdi
-0000d010: 6e5f 746f 5f73 7464 6f75 7422 2c0a 2020  n_to_stdout",.  
-0000d020: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d030: 5f76 616c 7565 3d6c 616d 6264 6120 2a61  _value=lambda *a
-0000d040: 7267 732c 202a 2a6b 7761 7267 733a 2063  rgs, **kwargs: c
-0000d050: 6572 6369 732e 4368 616e 6765 642e 5945  ercis.Changed.YE
-0000d060: 532c 0a20 2020 2020 2020 2029 2061 7320  S,.        ) as 
-0000d070: 6673 7473 3a0a 2020 2020 2020 2020 2020  fsts:.          
-0000d080: 2020 7265 706f 7274 203d 204d 6167 6963    report = Magic
-0000d090: 4d6f 636b 2829 0a20 2020 2020 2020 2020  Mock().         
-0000d0a0: 2020 2070 203d 2022 666f 6f2e 7079 220a     p = "foo.py".
-0000d0b0: 2020 2020 2020 2020 2020 2020 7061 7468              path
-0000d0c0: 203d 2050 6174 6828 6622 5f5f 424c 4143   = Path(f"__BLAC
-0000d0d0: 4b5f 5354 4449 4e5f 4649 4c45 4e41 4d45  K_STDIN_FILENAME
-0000d0e0: 5f5f 7b70 7d22 290a 2020 2020 2020 2020  __{p}").        
-0000d0f0: 2020 2020 6578 7065 6374 6564 203d 2050      expected = P
-0000d100: 6174 6828 7029 0a20 2020 2020 2020 2020  ath(p).         
-0000d110: 2020 2063 6572 6369 732e 7265 666f 726d     cercis.reform
-0000d120: 6174 5f6f 6e65 280a 2020 2020 2020 2020  at_one(.        
-0000d130: 2020 2020 2020 2020 7061 7468 2c0a 2020          path,.  
-0000d140: 2020 2020 2020 2020 2020 2020 2020 6661                fa
-0000d150: 7374 3d54 7275 652c 0a20 2020 2020 2020  st=True,.       
-0000d160: 2020 2020 2020 2020 2077 7269 7465 5f62           write_b
-0000d170: 6163 6b3d 6365 7263 6973 2e57 7269 7465  ack=cercis.Write
-0000d180: 4261 636b 2e59 4553 2c0a 2020 2020 2020  Back.YES,.      
-0000d190: 2020 2020 2020 2020 2020 6d6f 6465 3d44            mode=D
-0000d1a0: 4546 4155 4c54 5f4d 4f44 452c 0a20 2020  EFAULT_MODE,.   
-0000d1b0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-0000d1c0: 6f72 743d 7265 706f 7274 2c0a 2020 2020  ort=report,.    
-0000d1d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d1e0: 2020 2020 2020 6673 7473 2e61 7373 6572        fsts.asser
-0000d1f0: 745f 6361 6c6c 6564 5f6f 6e63 655f 7769  t_called_once_wi
-0000d200: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
-0000d210: 2020 2020 6661 7374 3d54 7275 652c 2077      fast=True, w
-0000d220: 7269 7465 5f62 6163 6b3d 6365 7263 6973  rite_back=cercis
-0000d230: 2e57 7269 7465 4261 636b 2e59 4553 2c20  .WriteBack.YES, 
-0000d240: 6d6f 6465 3d44 4546 4155 4c54 5f4d 4f44  mode=DEFAULT_MOD
-0000d250: 450a 2020 2020 2020 2020 2020 2020 290a  E.            ).
-0000d260: 2020 2020 2020 2020 2020 2020 2320 5f5f              # __
-0000d270: 424c 4143 4b5f 5354 4449 4e5f 4649 4c45  BLACK_STDIN_FILE
-0000d280: 4e41 4d45 5f5f 2073 686f 756c 6420 6861  NAME__ should ha
-0000d290: 7665 2062 6565 6e20 7374 7269 7070 6564  ve been stripped
-0000d2a0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-0000d2b0: 6f72 742e 646f 6e65 2e61 7373 6572 745f  ort.done.assert_
-0000d2c0: 6361 6c6c 6564 5f77 6974 6828 6578 7065  called_with(expe
-0000d2d0: 6374 6564 2c20 6365 7263 6973 2e43 6861  cted, cercis.Cha
-0000d2e0: 6e67 6564 2e59 4553 290a 0a20 2020 2040  nged.YES)..    @
-0000d2f0: 7079 7465 7374 2e6d 6172 6b2e 696e 636f  pytest.mark.inco
-0000d300: 6d70 6174 6962 6c65 5f77 6974 685f 6d79  mpatible_with_my
-0000d310: 7079 630a 2020 2020 6465 6620 7465 7374  pyc.    def test
-0000d320: 5f72 6566 6f72 6d61 745f 6f6e 655f 7769  _reformat_one_wi
-0000d330: 7468 5f73 7464 696e 5f66 696c 656e 616d  th_stdin_filenam
-0000d340: 655f 7079 6928 7365 6c66 2920 2d3e 204e  e_pyi(self) -> N
-0000d350: 6f6e 653a 0a20 2020 2020 2020 2077 6974  one:.        wit
-0000d360: 6820 7061 7463 6828 0a20 2020 2020 2020  h patch(.       
-0000d370: 2020 2020 2022 6365 7263 6973 2e66 6f72       "cercis.for
-0000d380: 6d61 745f 7374 6469 6e5f 746f 5f73 7464  mat_stdin_to_std
-0000d390: 6f75 7422 2c0a 2020 2020 2020 2020 2020  out",.          
-0000d3a0: 2020 7265 7475 726e 5f76 616c 7565 3d6c    return_value=l
-0000d3b0: 616d 6264 6120 2a61 7267 732c 202a 2a6b  ambda *args, **k
-0000d3c0: 7761 7267 733a 2063 6572 6369 732e 4368  wargs: cercis.Ch
-0000d3d0: 616e 6765 642e 5945 532c 0a20 2020 2020  anged.YES,.     
-0000d3e0: 2020 2029 2061 7320 6673 7473 3a0a 2020     ) as fsts:.  
-0000d3f0: 2020 2020 2020 2020 2020 7265 706f 7274            report
-0000d400: 203d 204d 6167 6963 4d6f 636b 2829 0a20   = MagicMock(). 
-0000d410: 2020 2020 2020 2020 2020 2070 203d 2022             p = "
-0000d420: 666f 6f2e 7079 6922 0a20 2020 2020 2020  foo.pyi".       
-0000d430: 2020 2020 2070 6174 6820 3d20 5061 7468       path = Path
-0000d440: 2866 225f 5f42 4c41 434b 5f53 5444 494e  (f"__BLACK_STDIN
-0000d450: 5f46 494c 454e 414d 455f 5f7b 707d 2229  _FILENAME__{p}")
-0000d460: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-0000d470: 6563 7465 6420 3d20 5061 7468 2870 290a  ected = Path(p).
-0000d480: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
-0000d490: 6973 2e72 6566 6f72 6d61 745f 6f6e 6528  is.reformat_one(
-0000d4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d4b0: 2070 6174 682c 0a20 2020 2020 2020 2020   path,.         
-0000d4c0: 2020 2020 2020 2066 6173 743d 5472 7565         fast=True
-0000d4d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d4e0: 2020 7772 6974 655f 6261 636b 3d63 6572    write_back=cer
-0000d4f0: 6369 732e 5772 6974 6542 6163 6b2e 5945  cis.WriteBack.YE
-0000d500: 532c 0a20 2020 2020 2020 2020 2020 2020  S,.             
-0000d510: 2020 206d 6f64 653d 4445 4641 554c 545f     mode=DEFAULT_
-0000d520: 4d4f 4445 2c0a 2020 2020 2020 2020 2020  MODE,.          
-0000d530: 2020 2020 2020 7265 706f 7274 3d72 6570        report=rep
-0000d540: 6f72 742c 0a20 2020 2020 2020 2020 2020  ort,.           
-0000d550: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
-0000d560: 7374 732e 6173 7365 7274 5f63 616c 6c65  sts.assert_calle
-0000d570: 645f 6f6e 6365 5f77 6974 6828 0a20 2020  d_once_with(.   
-0000d580: 2020 2020 2020 2020 2020 2020 2066 6173               fas
-0000d590: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
-0000d5a0: 2020 2020 2020 2020 7772 6974 655f 6261          write_ba
-0000d5b0: 636b 3d63 6572 6369 732e 5772 6974 6542  ck=cercis.WriteB
-0000d5c0: 6163 6b2e 5945 532c 0a20 2020 2020 2020  ack.YES,.       
-0000d5d0: 2020 2020 2020 2020 206d 6f64 653d 7265           mode=re
-0000d5e0: 706c 6163 6528 4445 4641 554c 545f 4d4f  place(DEFAULT_MO
-0000d5f0: 4445 2c20 6973 5f70 7969 3d54 7275 6529  DE, is_pyi=True)
-0000d600: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000d610: 2020 2020 2020 2020 2020 2020 2320 5f5f              # __
-0000d620: 424c 4143 4b5f 5354 4449 4e5f 4649 4c45  BLACK_STDIN_FILE
-0000d630: 4e41 4d45 5f5f 2073 686f 756c 6420 6861  NAME__ should ha
-0000d640: 7665 2062 6565 6e20 7374 7269 7070 6564  ve been stripped
-0000d650: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-0000d660: 6f72 742e 646f 6e65 2e61 7373 6572 745f  ort.done.assert_
-0000d670: 6361 6c6c 6564 5f77 6974 6828 6578 7065  called_with(expe
-0000d680: 6374 6564 2c20 6365 7263 6973 2e43 6861  cted, cercis.Cha
-0000d690: 6e67 6564 2e59 4553 290a 0a20 2020 2040  nged.YES)..    @
-0000d6a0: 7079 7465 7374 2e6d 6172 6b2e 696e 636f  pytest.mark.inco
-0000d6b0: 6d70 6174 6962 6c65 5f77 6974 685f 6d79  mpatible_with_my
-0000d6c0: 7079 630a 2020 2020 6465 6620 7465 7374  pyc.    def test
-0000d6d0: 5f72 6566 6f72 6d61 745f 6f6e 655f 7769  _reformat_one_wi
-0000d6e0: 7468 5f73 7464 696e 5f66 696c 656e 616d  th_stdin_filenam
-0000d6f0: 655f 6970 796e 6228 7365 6c66 2920 2d3e  e_ipynb(self) ->
-0000d700: 204e 6f6e 653a 0a20 2020 2020 2020 2077   None:.        w
-0000d710: 6974 6820 7061 7463 6828 0a20 2020 2020  ith patch(.     
-0000d720: 2020 2020 2020 2022 6365 7263 6973 2e66         "cercis.f
-0000d730: 6f72 6d61 745f 7374 6469 6e5f 746f 5f73  ormat_stdin_to_s
-0000d740: 7464 6f75 7422 2c0a 2020 2020 2020 2020  tdout",.        
-0000d750: 2020 2020 7265 7475 726e 5f76 616c 7565      return_value
-0000d760: 3d6c 616d 6264 6120 2a61 7267 732c 202a  =lambda *args, *
-0000d770: 2a6b 7761 7267 733a 2063 6572 6369 732e  *kwargs: cercis.
-0000d780: 4368 616e 6765 642e 5945 532c 0a20 2020  Changed.YES,.   
-0000d790: 2020 2020 2029 2061 7320 6673 7473 3a0a       ) as fsts:.
-0000d7a0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-0000d7b0: 7274 203d 204d 6167 6963 4d6f 636b 2829  rt = MagicMock()
-0000d7c0: 0a20 2020 2020 2020 2020 2020 2070 203d  .            p =
-0000d7d0: 2022 666f 6f2e 6970 796e 6222 0a20 2020   "foo.ipynb".   
-0000d7e0: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
-0000d7f0: 5061 7468 2866 225f 5f42 4c41 434b 5f53  Path(f"__BLACK_S
-0000d800: 5444 494e 5f46 494c 454e 414d 455f 5f7b  TDIN_FILENAME__{
-0000d810: 707d 2229 0a20 2020 2020 2020 2020 2020  p}").           
-0000d820: 2065 7870 6563 7465 6420 3d20 5061 7468   expected = Path
-0000d830: 2870 290a 2020 2020 2020 2020 2020 2020  (p).            
-0000d840: 6365 7263 6973 2e72 6566 6f72 6d61 745f  cercis.reformat_
-0000d850: 6f6e 6528 0a20 2020 2020 2020 2020 2020  one(.           
-0000d860: 2020 2020 2070 6174 682c 0a20 2020 2020       path,.     
-0000d870: 2020 2020 2020 2020 2020 2066 6173 743d             fast=
-0000d880: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000d890: 2020 2020 2020 7772 6974 655f 6261 636b        write_back
-0000d8a0: 3d63 6572 6369 732e 5772 6974 6542 6163  =cercis.WriteBac
-0000d8b0: 6b2e 5945 532c 0a20 2020 2020 2020 2020  k.YES,.         
-0000d8c0: 2020 2020 2020 206d 6f64 653d 4445 4641         mode=DEFA
-0000d8d0: 554c 545f 4d4f 4445 2c0a 2020 2020 2020  ULT_MODE,.      
-0000d8e0: 2020 2020 2020 2020 2020 7265 706f 7274            report
-0000d8f0: 3d72 6570 6f72 742c 0a20 2020 2020 2020  =report,.       
-0000d900: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000d910: 2020 2066 7374 732e 6173 7365 7274 5f63     fsts.assert_c
-0000d920: 616c 6c65 645f 6f6e 6365 5f77 6974 6828  alled_once_with(
-0000d930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d940: 2066 6173 743d 5472 7565 2c0a 2020 2020   fast=True,.    
-0000d950: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-0000d960: 655f 6261 636b 3d63 6572 6369 732e 5772  e_back=cercis.Wr
-0000d970: 6974 6542 6163 6b2e 5945 532c 0a20 2020  iteBack.YES,.   
-0000d980: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-0000d990: 653d 7265 706c 6163 6528 4445 4641 554c  e=replace(DEFAUL
-0000d9a0: 545f 4d4f 4445 2c20 6973 5f69 7079 6e62  T_MODE, is_ipynb
-0000d9b0: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-0000d9c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000d9d0: 2020 2320 5f5f 424c 4143 4b5f 5354 4449    # __BLACK_STDI
-0000d9e0: 4e5f 4649 4c45 4e41 4d45 5f5f 2073 686f  N_FILENAME__ sho
-0000d9f0: 756c 6420 6861 7665 2062 6565 6e20 7374  uld have been st
-0000da00: 7269 7070 6564 0a20 2020 2020 2020 2020  ripped.         
-0000da10: 2020 2072 6570 6f72 742e 646f 6e65 2e61     report.done.a
-0000da20: 7373 6572 745f 6361 6c6c 6564 5f77 6974  ssert_called_wit
-0000da30: 6828 6578 7065 6374 6564 2c20 6365 7263  h(expected, cerc
-0000da40: 6973 2e43 6861 6e67 6564 2e59 4553 290a  is.Changed.YES).
-0000da50: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-0000da60: 6b2e 696e 636f 6d70 6174 6962 6c65 5f77  k.incompatible_w
-0000da70: 6974 685f 6d79 7079 630a 2020 2020 6465  ith_mypyc.    de
-0000da80: 6620 7465 7374 5f72 6566 6f72 6d61 745f  f test_reformat_
-0000da90: 6f6e 655f 7769 7468 5f73 7464 696e 5f61  one_with_stdin_a
-0000daa0: 6e64 5f65 7869 7374 696e 675f 7061 7468  nd_existing_path
-0000dab0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000dac0: 2020 2020 2020 2020 7769 7468 2070 6174          with pat
-0000dad0: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
-0000dae0: 2263 6572 6369 732e 666f 726d 6174 5f73  "cercis.format_s
-0000daf0: 7464 696e 5f74 6f5f 7374 646f 7574 222c  tdin_to_stdout",
-0000db00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000db10: 7572 6e5f 7661 6c75 653d 6c61 6d62 6461  urn_value=lambda
-0000db20: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-0000db30: 3a20 6365 7263 6973 2e43 6861 6e67 6564  : cercis.Changed
-0000db40: 2e59 4553 2c0a 2020 2020 2020 2020 2920  .YES,.        ) 
-0000db50: 6173 2066 7374 733a 0a20 2020 2020 2020  as fsts:.       
-0000db60: 2020 2020 2072 6570 6f72 7420 3d20 4d61       report = Ma
-0000db70: 6769 634d 6f63 6b28 290a 2020 2020 2020  gicMock().      
-0000db80: 2020 2020 2020 2320 4576 656e 2077 6974        # Even wit
-0000db90: 6820 616e 2065 7869 7374 696e 6720 6669  h an existing fi
-0000dba0: 6c65 2c20 7369 6e63 6520 7765 2061 7265  le, since we are
-0000dbb0: 2066 6f72 6369 6e67 2073 7464 696e 2c20   forcing stdin, 
-0000dbc0: 6365 7263 6973 0a20 2020 2020 2020 2020  cercis.         
-0000dbd0: 2020 2023 2073 686f 756c 6420 6f75 7470     # should outp
-0000dbe0: 7574 2074 6f20 7374 646f 7574 2061 6e64  ut to stdout and
-0000dbf0: 206e 6f74 206d 6f64 6966 7920 7468 6520   not modify the 
-0000dc00: 6669 6c65 2069 6e70 6c61 6365 0a20 2020  file inplace.   
-0000dc10: 2020 2020 2020 2020 2070 203d 2054 4849           p = THI
-0000dc20: 535f 4449 5220 2f20 2264 6174 6122 202f  S_DIR / "data" /
-0000dc30: 2022 7369 6d70 6c65 5f63 6173 6573 2220   "simple_cases" 
-0000dc40: 2f20 2263 6f6c 6c65 6374 696f 6e73 2e70  / "collections.p
-0000dc50: 7922 0a20 2020 2020 2020 2020 2020 2023  y".            #
-0000dc60: 204d 616b 6520 7375 7265 2069 735f 6669   Make sure is_fi
-0000dc70: 6c65 2061 6374 7561 6c6c 7920 7265 7475  le actually retu
-0000dc80: 726e 7320 5472 7565 0a20 2020 2020 2020  rns True.       
-0000dc90: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000dca0: 5472 7565 2870 2e69 735f 6669 6c65 2829  True(p.is_file()
-0000dcb0: 290a 2020 2020 2020 2020 2020 2020 7061  ).            pa
-0000dcc0: 7468 203d 2050 6174 6828 6622 5f5f 424c  th = Path(f"__BL
-0000dcd0: 4143 4b5f 5354 4449 4e5f 4649 4c45 4e41  ACK_STDIN_FILENA
-0000dce0: 4d45 5f5f 7b70 7d22 290a 2020 2020 2020  ME__{p}").      
-0000dcf0: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
-0000dd00: 2050 6174 6828 7029 0a20 2020 2020 2020   Path(p).       
-0000dd10: 2020 2020 2063 6572 6369 732e 7265 666f       cercis.refo
-0000dd20: 726d 6174 5f6f 6e65 280a 2020 2020 2020  rmat_one(.      
-0000dd30: 2020 2020 2020 2020 2020 7061 7468 2c0a            path,.
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 6661 7374 3d54 7275 652c 0a20 2020 2020  fast=True,.     
-0000dd60: 2020 2020 2020 2020 2020 2077 7269 7465             write
-0000dd70: 5f62 6163 6b3d 6365 7263 6973 2e57 7269  _back=cercis.Wri
-0000dd80: 7465 4261 636b 2e59 4553 2c0a 2020 2020  teBack.YES,.    
-0000dd90: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-0000dda0: 3d44 4546 4155 4c54 5f4d 4f44 452c 0a20  =DEFAULT_MODE,. 
-0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000ddc0: 6570 6f72 743d 7265 706f 7274 2c0a 2020  eport=report,.  
-0000ddd0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000dde0: 2020 2020 2020 2020 6673 7473 2e61 7373          fsts.ass
-0000ddf0: 6572 745f 6361 6c6c 6564 5f6f 6e63 6528  ert_called_once(
-0000de00: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0000de10: 5f5f 424c 4143 4b5f 5354 4449 4e5f 4649  __BLACK_STDIN_FI
-0000de20: 4c45 4e41 4d45 5f5f 2073 686f 756c 6420  LENAME__ should 
-0000de30: 6861 7665 2062 6565 6e20 7374 7269 7070  have been stripp
-0000de40: 6564 0a20 2020 2020 2020 2020 2020 2072  ed.            r
-0000de50: 6570 6f72 742e 646f 6e65 2e61 7373 6572  eport.done.asser
-0000de60: 745f 6361 6c6c 6564 5f77 6974 6828 6578  t_called_with(ex
-0000de70: 7065 6374 6564 2c20 6365 7263 6973 2e43  pected, cercis.C
-0000de80: 6861 6e67 6564 2e59 4553 290a 0a20 2020  hanged.YES)..   
-0000de90: 2064 6566 2074 6573 745f 7265 666f 726d   def test_reform
-0000dea0: 6174 5f6f 6e65 5f77 6974 685f 7374 6469  at_one_with_stdi
-0000deb0: 6e5f 656d 7074 7928 7365 6c66 2920 2d3e  n_empty(self) ->
-0000dec0: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
-0000ded0: 6173 6573 203d 205b 0a20 2020 2020 2020  ases = [.       
-0000dee0: 2020 2020 2028 2222 2c20 2222 292c 0a20       ("", ""),. 
-0000def0: 2020 2020 2020 2020 2020 2028 225c 6e22             ("\n"
-0000df00: 2c20 225c 6e22 292c 0a20 2020 2020 2020  , "\n"),.       
-0000df10: 2020 2020 2028 225c 725c 6e22 2c20 225c       ("\r\n", "\
-0000df20: 725c 6e22 292c 0a20 2020 2020 2020 2020  r\n"),.         
-0000df30: 2020 2028 2220 5c74 222c 2022 2229 2c0a     (" \t", ""),.
-0000df40: 2020 2020 2020 2020 2020 2020 2822 205c              (" \
-0000df50: 745c 6e5c 7420 222c 2022 5c6e 2229 2c0a  t\n\t ", "\n"),.
-0000df60: 2020 2020 2020 2020 2020 2020 2822 205c              (" \
-0000df70: 745c 725c 6e5c 7420 222c 2022 5c72 5c6e  t\r\n\t ", "\r\n
-0000df80: 2229 2c0a 2020 2020 2020 2020 5d0a 0a20  "),.        ].. 
-0000df90: 2020 2020 2020 2064 6566 205f 6e65 775f         def _new_
-0000dfa0: 7772 6170 7065 7228 0a20 2020 2020 2020  wrapper(.       
-0000dfb0: 2020 2020 2020 2020 206f 7574 7075 743a           output:
-0000dfc0: 2069 6f2e 5374 7269 6e67 494f 2c20 696f   io.StringIO, io
-0000dfd0: 5f54 6578 7449 4f57 7261 7070 6572 3a20  _TextIOWrapper: 
-0000dfe0: 5479 7065 5b69 6f2e 5465 7874 494f 5772  Type[io.TextIOWr
-0000dff0: 6170 7065 725d 0a20 2020 2020 2020 2029  apper].        )
-0000e000: 202d 3e20 4361 6c6c 6162 6c65 5b5b 416e   -> Callable[[An
-0000e010: 792c 2041 6e79 5d2c 2069 6f2e 5465 7874  y, Any], io.Text
-0000e020: 494f 5772 6170 7065 725d 3a0a 2020 2020  IOWrapper]:.    
-0000e030: 2020 2020 2020 2020 6465 6620 6765 745f          def get_
-0000e040: 6f75 7470 7574 282a 6172 6773 3a20 416e  output(*args: An
-0000e050: 792c 202a 2a6b 7761 7267 733a 2041 6e79  y, **kwargs: Any
-0000e060: 2920 2d3e 2069 6f2e 5465 7874 494f 5772  ) -> io.TextIOWr
-0000e070: 6170 7065 723a 0a20 2020 2020 2020 2020  apper:.         
-0000e080: 2020 2020 2020 2069 6620 6172 6773 203d         if args =
-0000e090: 3d20 2873 7973 2e73 7464 6f75 742e 6275  = (sys.stdout.bu
-0000e0a0: 6666 6572 2c29 3a0a 2020 2020 2020 2020  ffer,):.        
-0000e0b0: 2020 2020 2020 2020 2020 2020 2320 4974              # It
-0000e0c0: 2773 2060 666f 726d 6174 5f73 7464 696e  's `format_stdin
-0000e0d0: 5f74 6f5f 7374 646f 7574 2829 6020 6361  _to_stdout()` ca
-0000e0e0: 6c6c 696e 6720 6069 6f2e 5465 7874 494f  lling `io.TextIO
-0000e0f0: 5772 6170 7065 7228 2960 2c0a 2020 2020  Wrapper()`,.    
-0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e110: 2320 7265 7475 726e 206f 7572 206d 6f63  # return our moc
-0000e120: 6b20 6f62 6a65 6374 2e0a 2020 2020 2020  k object..      
-0000e130: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000e140: 7475 726e 206f 7574 7075 740a 2020 2020  turn output.    
-0000e150: 2020 2020 2020 2020 2020 2020 2320 4974              # It
-0000e160: 2773 2073 6f6d 6574 6869 6e67 2065 6c73  's something els
-0000e170: 6520 2869 2e65 2e20 6064 6563 6f64 655f  e (i.e. `decode_
-0000e180: 6279 7465 7328 2960 2920 6361 6c6c 696e  bytes()`) callin
-0000e190: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-0000e1a0: 2020 2320 6069 6f2e 5465 7874 494f 5772    # `io.TextIOWr
-0000e1b0: 6170 7065 7228 2960 2c20 7061 7373 2074  apper()`, pass t
-0000e1c0: 6872 6f75 6768 2074 6f20 7468 6520 6f72  hrough to the or
-0000e1d0: 6967 696e 616c 2069 6d70 6c65 6d65 6e74  iginal implement
-0000e1e0: 6174 696f 6e2e 0a20 2020 2020 2020 2020  ation..         
-0000e1f0: 2020 2020 2020 2023 2053 6565 2064 6973         # See dis
-0000e200: 6375 7373 696f 6e20 696e 2068 7474 7073  cussion in https
-0000e210: 3a2f 2f67 6974 6875 622e 636f 6d2f 7073  ://github.com/ps
-0000e220: 662f 626c 6163 6b2f 7075 6c6c 2f32 3438  f/black/pull/248
-0000e230: 390a 2020 2020 2020 2020 2020 2020 2020  9.              
-0000e240: 2020 7265 7475 726e 2069 6f5f 5465 7874    return io_Text
-0000e250: 494f 5772 6170 7065 7228 2a61 7267 732c  IOWrapper(*args,
-0000e260: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-0000e270: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-0000e280: 6574 5f6f 7574 7075 740a 0a20 2020 2020  et_output..     
-0000e290: 2020 206d 6f64 6520 3d20 6365 7263 6973     mode = cercis
-0000e2a0: 2e4d 6f64 6528 7072 6576 6965 773d 5472  .Mode(preview=Tr
-0000e2b0: 7565 290a 2020 2020 2020 2020 666f 7220  ue).        for 
-0000e2c0: 636f 6e74 656e 742c 2065 7870 6563 7465  content, expecte
-0000e2d0: 6420 696e 2063 6173 6573 3a0a 2020 2020  d in cases:.    
-0000e2e0: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
-0000e2f0: 2069 6f2e 5374 7269 6e67 494f 2829 0a20   io.StringIO(). 
-0000e300: 2020 2020 2020 2020 2020 2069 6f5f 5465             io_Te
-0000e310: 7874 494f 5772 6170 7065 7220 3d20 696f  xtIOWrapper = io
-0000e320: 2e54 6578 7449 4f57 7261 7070 6572 0a0a  .TextIOWrapper..
-0000e330: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000e340: 2070 6174 6368 2822 696f 2e54 6578 7449   patch("io.TextI
-0000e350: 4f57 7261 7070 6572 222c 205f 6e65 775f  OWrapper", _new_
-0000e360: 7772 6170 7065 7228 6f75 7470 7574 2c20  wrapper(output, 
-0000e370: 696f 5f54 6578 7449 4f57 7261 7070 6572  io_TextIOWrapper
-0000e380: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0000e390: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000e3a0: 2020 2020 2020 2020 2020 2020 2063 6572               cer
-0000e3b0: 6369 732e 666f 726d 6174 5f73 7464 696e  cis.format_stdin
-0000e3c0: 5f74 6f5f 7374 646f 7574 280a 2020 2020  _to_stdout(.    
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3e0: 2020 2020 6661 7374 3d54 7275 652c 0a20      fast=True,. 
-0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e400: 2020 2020 2020 2063 6f6e 7465 6e74 3d63         content=c
-0000e410: 6f6e 7465 6e74 2c0a 2020 2020 2020 2020  ontent,.        
-0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e430: 7772 6974 655f 6261 636b 3d63 6572 6369  write_back=cerci
-0000e440: 732e 5772 6974 6542 6163 6b2e 5945 532c  s.WriteBack.YES,
-0000e450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e460: 2020 2020 2020 2020 206d 6f64 653d 6d6f           mode=mo
-0000e470: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-0000e480: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e490: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0000e4a0: 2069 6f2e 556e 7375 7070 6f72 7465 644f   io.UnsupportedO
-0000e4b0: 7065 7261 7469 6f6e 3a0a 2020 2020 2020  peration:.      
-0000e4c0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000e4d0: 7373 2020 2320 5374 7269 6e67 494f 2064  ss  # StringIO d
-0000e4e0: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-0000e4f0: 6465 7461 6368 0a20 2020 2020 2020 2020  detach.         
-0000e500: 2020 2020 2020 2061 7373 6572 7420 6f75         assert ou
-0000e510: 7470 7574 2e67 6574 7661 6c75 6528 2920  tput.getvalue() 
-0000e520: 3d3d 2065 7870 6563 7465 640a 0a20 2020  == expected..   
-0000e530: 2020 2020 2023 2041 6e20 656d 7074 7920       # An empty 
-0000e540: 7374 7269 6e67 2069 7320 7468 6520 6f6e  string is the on
-0000e550: 6c79 2074 6573 7420 6361 7365 2066 6f72  ly test case for
-0000e560: 2060 7072 6576 6965 773d 4661 6c73 6560   `preview=False`
-0000e570: 0a20 2020 2020 2020 206f 7574 7075 7420  .        output 
-0000e580: 3d20 696f 2e53 7472 696e 6749 4f28 290a  = io.StringIO().
-0000e590: 2020 2020 2020 2020 696f 5f54 6578 7449          io_TextI
-0000e5a0: 4f57 7261 7070 6572 203d 2069 6f2e 5465  OWrapper = io.Te
-0000e5b0: 7874 494f 5772 6170 7065 720a 2020 2020  xtIOWrapper.    
-0000e5c0: 2020 2020 7769 7468 2070 6174 6368 2822      with patch("
-0000e5d0: 696f 2e54 6578 7449 4f57 7261 7070 6572  io.TextIOWrapper
-0000e5e0: 222c 205f 6e65 775f 7772 6170 7065 7228  ", _new_wrapper(
-0000e5f0: 6f75 7470 7574 2c20 696f 5f54 6578 7449  output, io_TextI
-0000e600: 4f57 7261 7070 6572 2929 3a0a 2020 2020  OWrapper)):.    
-0000e610: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000e620: 2020 2020 2020 2020 2020 2020 2063 6572               cer
-0000e630: 6369 732e 666f 726d 6174 5f73 7464 696e  cis.format_stdin
-0000e640: 5f74 6f5f 7374 646f 7574 280a 2020 2020  _to_stdout(.    
-0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e660: 6661 7374 3d54 7275 652c 0a20 2020 2020  fast=True,.     
-0000e670: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000e680: 6f6e 7465 6e74 3d22 222c 0a20 2020 2020  ontent="",.     
-0000e690: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000e6a0: 7269 7465 5f62 6163 6b3d 6365 7263 6973  rite_back=cercis
-0000e6b0: 2e57 7269 7465 4261 636b 2e59 4553 2c0a  .WriteBack.YES,.
-0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6d0: 2020 2020 6d6f 6465 3d44 4546 4155 4c54      mode=DEFAULT
-0000e6e0: 5f4d 4f44 452c 0a20 2020 2020 2020 2020  _MODE,.         
-0000e6f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e700: 2020 2020 2065 7863 6570 7420 696f 2e55       except io.U
-0000e710: 6e73 7570 706f 7274 6564 4f70 6572 6174  nsupportedOperat
-0000e720: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-0000e730: 2020 2020 2070 6173 7320 2023 2053 7472       pass  # Str
-0000e740: 696e 6749 4f20 646f 6573 206e 6f74 2073  ingIO does not s
-0000e750: 7570 706f 7274 2064 6574 6163 680a 2020  upport detach.  
-0000e760: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000e770: 206f 7574 7075 742e 6765 7476 616c 7565   output.getvalue
-0000e780: 2829 203d 3d20 2222 0a0a 2020 2020 6465  () == ""..    de
-0000e790: 6620 7465 7374 5f69 6e76 616c 6964 5f63  f test_invalid_c
-0000e7a0: 6c69 5f72 6567 6578 2873 656c 6629 202d  li_regex(self) -
-0000e7b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000e7c0: 666f 7220 6f70 7469 6f6e 2069 6e20 5b22  for option in ["
-0000e7d0: 2d2d 696e 636c 7564 6522 2c20 222d 2d65  --include", "--e
-0000e7e0: 7863 6c75 6465 222c 2022 2d2d 6578 7465  xclude", "--exte
-0000e7f0: 6e64 2d65 7863 6c75 6465 222c 2022 2d2d  nd-exclude", "--
-0000e800: 666f 7263 652d 6578 636c 7564 6522 5d3a  force-exclude"]:
-0000e810: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e820: 662e 696e 766f 6b65 426c 6163 6b28 5b22  f.invokeBlack(["
-0000e830: 2d22 2c20 6f70 7469 6f6e 2c20 222a 2a28  -", option, "**(
-0000e840: 2928 2121 2a29 225d 2c20 6578 6974 5f63  )(!!*)"], exit_c
-0000e850: 6f64 653d 3229 0a0a 2020 2020 6465 6620  ode=2)..    def 
-0000e860: 7465 7374 5f72 6571 7569 7265 645f 7665  test_required_ve
-0000e870: 7273 696f 6e5f 6d61 7463 6865 735f 7665  rsion_matches_ve
-0000e880: 7273 696f 6e28 7365 6c66 2920 2d3e 204e  rsion(self) -> N
-0000e890: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
-0000e8a0: 662e 696e 766f 6b65 426c 6163 6b28 0a20  f.invokeBlack(. 
-0000e8b0: 2020 2020 2020 2020 2020 205b 222d 2d72             ["--r
-0000e8c0: 6571 7569 7265 642d 7665 7273 696f 6e22  equired-version"
-0000e8d0: 2c20 6365 7263 6973 2e5f 5f76 6572 7369  , cercis.__versi
-0000e8e0: 6f6e 5f5f 2c20 222d 6322 2c20 2230 225d  on__, "-c", "0"]
-0000e8f0: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
-0000e900: 6974 5f63 6f64 653d 302c 0a20 2020 2020  it_code=0,.     
-0000e910: 2020 2020 2020 2069 676e 6f72 655f 636f         ignore_co
-0000e920: 6e66 6967 3d54 7275 652c 0a20 2020 2020  nfig=True,.     
-0000e930: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-0000e940: 7374 5f72 6571 7569 7265 645f 7665 7273  st_required_vers
-0000e950: 696f 6e5f 6d61 7463 6865 735f 7061 7274  ion_matches_part
-0000e960: 6961 6c5f 7665 7273 696f 6e28 7365 6c66  ial_version(self
-0000e970: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000e980: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
-0000e990: 6163 6b28 0a20 2020 2020 2020 2020 2020  ack(.           
-0000e9a0: 205b 222d 2d72 6571 7569 7265 642d 7665   ["--required-ve
-0000e9b0: 7273 696f 6e22 2c20 6365 7263 6973 2e5f  rsion", cercis._
-0000e9c0: 5f76 6572 7369 6f6e 5f5f 2e73 706c 6974  _version__.split
-0000e9d0: 2822 2e22 295b 305d 2c20 222d 6322 2c20  (".")[0], "-c", 
-0000e9e0: 2230 225d 2c0a 2020 2020 2020 2020 2020  "0"],.          
-0000e9f0: 2020 6578 6974 5f63 6f64 653d 302c 0a20    exit_code=0,. 
-0000ea00: 2020 2020 2020 2020 2020 2069 676e 6f72             ignor
-0000ea10: 655f 636f 6e66 6967 3d54 7275 652c 0a20  e_config=True,. 
-0000ea20: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0000ea30: 6620 7465 7374 5f72 6571 7569 7265 645f  f test_required_
-0000ea40: 7665 7273 696f 6e5f 646f 6573 5f6e 6f74  version_does_not
-0000ea50: 5f6d 6174 6368 5f6f 6e5f 6d69 6e6f 725f  _match_on_minor_
-0000ea60: 7665 7273 696f 6e28 7365 6c66 2920 2d3e  version(self) ->
-0000ea70: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-0000ea80: 656c 662e 696e 766f 6b65 426c 6163 6b28  elf.invokeBlack(
-0000ea90: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000eab0: 2d2d 7265 7175 6972 6564 2d76 6572 7369  --required-versi
-0000eac0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
-0000ead0: 2020 2020 2063 6572 6369 732e 5f5f 7665       cercis.__ve
-0000eae0: 7273 696f 6e5f 5f2e 7370 6c69 7428 222e  rsion__.split(".
-0000eaf0: 2229 5b30 5d20 2b20 222e 3939 3922 2c0a  ")[0] + ".999",.
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 222d 6322 2c0a 2020 2020 2020 2020 2020  "-c",.          
-0000eb20: 2020 2020 2020 2230 222c 0a20 2020 2020        "0",.     
-0000eb30: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-0000eb40: 2020 2020 2020 6578 6974 5f63 6f64 653d        exit_code=
-0000eb50: 312c 0a20 2020 2020 2020 2020 2020 2069  1,.            i
-0000eb60: 676e 6f72 655f 636f 6e66 6967 3d54 7275  gnore_config=Tru
-0000eb70: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
-0000eb80: 2020 6465 6620 7465 7374 5f72 6571 7569    def test_requi
-0000eb90: 7265 645f 7665 7273 696f 6e5f 646f 6573  red_version_does
-0000eba0: 5f6e 6f74 5f6d 6174 6368 5f76 6572 7369  _not_match_versi
-0000ebb0: 6f6e 2873 656c 6629 202d 3e20 4e6f 6e65  on(self) -> None
-0000ebc0: 3a0a 2020 2020 2020 2020 7265 7375 6c74  :.        result
-0000ebd0: 203d 2042 6c61 636b 5275 6e6e 6572 2829   = BlackRunner()
-0000ebe0: 2e69 6e76 6f6b 6528 0a20 2020 2020 2020  .invoke(.       
-0000ebf0: 2020 2020 2063 6572 6369 732e 6d61 696e       cercis.main
-0000ec00: 2c0a 2020 2020 2020 2020 2020 2020 5b22  ,.            ["
-0000ec10: 2d2d 7265 7175 6972 6564 2d76 6572 7369  --required-versi
-0000ec20: 6f6e 222c 2022 3230 2e39 3962 222c 2022  on", "20.99b", "
-0000ec30: 2d63 222c 2022 3022 5d2c 0a20 2020 2020  -c", "0"],.     
-0000ec40: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000ec50: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-0000ec60: 7375 6c74 2e65 7869 745f 636f 6465 2c20  sult.exit_code, 
-0000ec70: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-0000ec80: 6173 7365 7274 496e 2822 7265 7175 6972  assertIn("requir
-0000ec90: 6564 2076 6572 7369 6f6e 222c 2072 6573  ed version", res
-0000eca0: 756c 742e 7374 6465 7272 290a 0a20 2020  ult.stderr)..   
-0000ecb0: 2064 6566 2074 6573 745f 7072 6573 6572   def test_preser
-0000ecc0: 7665 735f 6c69 6e65 5f65 6e64 696e 6773  ves_line_endings
-0000ecd0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000ece0: 2020 2020 2020 2020 7769 7468 2054 656d          with Tem
-0000ecf0: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
-0000ed00: 2920 6173 2077 6f72 6b73 7061 6365 3a0a  ) as workspace:.
-0000ed10: 2020 2020 2020 2020 2020 2020 7465 7374              test
-0000ed20: 5f66 696c 6520 3d20 5061 7468 2877 6f72  _file = Path(wor
-0000ed30: 6b73 7061 6365 2920 2f20 2274 6573 742e  kspace) / "test.
-0000ed40: 7079 220a 2020 2020 2020 2020 2020 2020  py".            
-0000ed50: 666f 7220 6e6c 2069 6e20 5b22 5c6e 222c  for nl in ["\n",
-0000ed60: 2022 5c72 5c6e 225d 3a0a 2020 2020 2020   "\r\n"]:.      
-0000ed70: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-0000ed80: 7473 203d 206e 6c2e 6a6f 696e 285b 2264  ts = nl.join(["d
-0000ed90: 6566 2066 2820 2029 3a22 2c20 2220 2020  ef f(  ):", "   
-0000eda0: 2070 6173 7322 5d29 0a20 2020 2020 2020   pass"]).       
-0000edb0: 2020 2020 2020 2020 2074 6573 745f 6669           test_fi
-0000edc0: 6c65 2e77 7269 7465 5f62 7974 6573 2863  le.write_bytes(c
-0000edd0: 6f6e 7465 6e74 732e 656e 636f 6465 2829  ontents.encode()
-0000ede0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000edf0: 2020 6666 2874 6573 745f 6669 6c65 2c20    ff(test_file, 
-0000ee00: 7772 6974 655f 6261 636b 3d63 6572 6369  write_back=cerci
-0000ee10: 732e 5772 6974 6542 6163 6b2e 5945 5329  s.WriteBack.YES)
-0000ee20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ee30: 2075 7064 6174 6564 5f63 6f6e 7465 6e74   updated_content
-0000ee40: 733a 2062 7974 6573 203d 2074 6573 745f  s: bytes = test_
-0000ee50: 6669 6c65 2e72 6561 645f 6279 7465 7328  file.read_bytes(
-0000ee60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ee70: 2020 7365 6c66 2e61 7373 6572 7449 6e28    self.assertIn(
-0000ee80: 6e6c 2e65 6e63 6f64 6528 292c 2075 7064  nl.encode(), upd
-0000ee90: 6174 6564 5f63 6f6e 7465 6e74 7329 0a20  ated_contents). 
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000eeb0: 6620 6e6c 203d 3d20 225c 6e22 3a0a 2020  f nl == "\n":.  
-0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eed0: 2020 7365 6c66 2e61 7373 6572 744e 6f74    self.assertNot
-0000eee0: 496e 2862 225c 725c 6e22 2c20 7570 6461  In(b"\r\n", upda
-0000eef0: 7465 645f 636f 6e74 656e 7473 290a 0a20  ted_contents).. 
-0000ef00: 2020 2064 6566 2074 6573 745f 7072 6573     def test_pres
-0000ef10: 6572 7665 735f 6c69 6e65 5f65 6e64 696e  erves_line_endin
-0000ef20: 6773 5f76 6961 5f73 7464 696e 2873 656c  gs_via_stdin(sel
-0000ef30: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000ef40: 2020 2020 666f 7220 6e6c 2069 6e20 5b22      for nl in ["
-0000ef50: 5c6e 222c 2022 5c72 5c6e 225d 3a0a 2020  \n", "\r\n"]:.  
-0000ef60: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-0000ef70: 7473 203d 206e 6c2e 6a6f 696e 285b 2264  ts = nl.join(["d
-0000ef80: 6566 2066 2820 2029 3a22 2c20 2220 2020  ef f(  ):", "   
-0000ef90: 2070 6173 7322 5d29 0a20 2020 2020 2020   pass"]).       
-0000efa0: 2020 2020 2072 756e 6e65 7220 3d20 426c       runner = Bl
-0000efb0: 6163 6b52 756e 6e65 7228 290a 2020 2020  ackRunner().    
-0000efc0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000efd0: 2072 756e 6e65 722e 696e 766f 6b65 280a   runner.invoke(.
+00002210: 0a0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
+00002220: 6570 5f36 3935 5f76 6572 7369 6f6e 5f64  ep_695_version_d
+00002230: 6574 6563 7469 6f6e 2873 656c 6629 202d  etection(self) -
+00002240: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00002250: 666f 7220 6669 6c65 2069 6e20 2822 7479  for file in ("ty
+00002260: 7065 5f61 6c69 6173 6573 222c 2022 7479  pe_aliases", "ty
+00002270: 7065 5f70 6172 616d 7322 293a 0a20 2020  pe_params"):.   
+00002280: 2020 2020 2020 2020 2073 6f75 7263 652c           source,
+00002290: 205f 203d 2072 6561 645f 6461 7461 2822   _ = read_data("
+000022a0: 7079 5f33 3132 222c 2066 696c 6529 0a20  py_312", file). 
+000022b0: 2020 2020 2020 2020 2020 2072 6f6f 7420             root 
+000022c0: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
+000022d0: 5f70 6172 7365 2873 6f75 7263 6529 0a20  _parse(source). 
+000022e0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+000022f0: 7265 7320 3d20 6365 7263 6973 2e67 6574  res = cercis.get
+00002300: 5f66 6561 7475 7265 735f 7573 6564 2872  _features_used(r
+00002310: 6f6f 7429 0a20 2020 2020 2020 2020 2020  oot).           
+00002320: 2073 656c 662e 6173 7365 7274 496e 2863   self.assertIn(c
+00002330: 6572 6369 732e 4665 6174 7572 652e 5459  ercis.Feature.TY
+00002340: 5045 5f50 4152 414d 532c 2066 6561 7475  PE_PARAMS, featu
+00002350: 7265 7329 0a20 2020 2020 2020 2020 2020  res).           
+00002360: 2076 6572 7369 6f6e 7320 3d20 6365 7263   versions = cerc
+00002370: 6973 2e64 6574 6563 745f 7461 7267 6574  is.detect_target
+00002380: 5f76 6572 7369 6f6e 7328 726f 6f74 290a  _versions(root).
+00002390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000023a0: 2e61 7373 6572 7449 6e28 6365 7263 6973  .assertIn(cercis
+000023b0: 2e54 6172 6765 7456 6572 7369 6f6e 2e50  .TargetVersion.P
+000023c0: 5933 3132 2c20 7665 7273 696f 6e73 290a  Y312, versions).
+000023d0: 0a20 2020 2064 6566 2074 6573 745f 6578  .    def test_ex
+000023e0: 7072 6573 7369 6f6e 5f66 6628 7365 6c66  pression_ff(self
+000023f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00002400: 2020 2073 6f75 7263 652c 2065 7870 6563     source, expec
+00002410: 7465 6420 3d20 7265 6164 5f64 6174 6128  ted = read_data(
+00002420: 2273 696d 706c 655f 6361 7365 7322 2c20  "simple_cases", 
+00002430: 2265 7870 7265 7373 696f 6e2e 7079 2229  "expression.py")
+00002440: 0a20 2020 2020 2020 2074 6d70 5f66 696c  .        tmp_fil
+00002450: 6520 3d20 5061 7468 2863 6572 6369 732e  e = Path(cercis.
+00002460: 6475 6d70 5f74 6f5f 6669 6c65 2873 6f75  dump_to_file(sou
+00002470: 7263 6529 290a 2020 2020 2020 2020 6d6f  rce)).        mo
+00002480: 6465 203d 2072 6570 6c61 6365 2844 4546  de = replace(DEF
+00002490: 4155 4c54 5f4d 4f44 452c 206c 696e 655f  AULT_MODE, line_
+000024a0: 6c65 6e67 7468 3d38 3829 0a20 2020 2020  length=88).     
+000024b0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000024c0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+000024d0: 7275 6528 6666 2874 6d70 5f66 696c 652c  rue(ff(tmp_file,
+000024e0: 2077 7269 7465 5f62 6163 6b3d 6365 7263   write_back=cerc
+000024f0: 6973 2e57 7269 7465 4261 636b 2e59 4553  is.WriteBack.YES
+00002500: 2c20 6d6f 6465 3d6d 6f64 6529 290a 2020  , mode=mode)).  
+00002510: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+00002520: 7065 6e28 746d 705f 6669 6c65 2c20 656e  pen(tmp_file, en
+00002530: 636f 6469 6e67 3d22 7574 6638 2229 2061  coding="utf8") a
+00002540: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+00002550: 2020 2020 2061 6374 7561 6c20 3d20 662e       actual = f.
+00002560: 7265 6164 2829 0a20 2020 2020 2020 2066  read().        f
+00002570: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
+00002580: 2020 2020 6f73 2e75 6e6c 696e 6b28 746d      os.unlink(tm
+00002590: 705f 6669 6c65 290a 2020 2020 2020 2020  p_file).        
+000025a0: 7365 6c66 2e61 7373 6572 7446 6f72 6d61  self.assertForma
+000025b0: 7445 7175 616c 2865 7870 6563 7465 642c  tEqual(expected,
+000025c0: 2061 6374 7561 6c29 0a20 2020 2020 2020   actual).       
+000025d0: 2077 6974 6820 7061 7463 6828 2263 6572   with patch("cer
+000025e0: 6369 732e 6475 6d70 5f74 6f5f 6669 6c65  cis.dump_to_file
+000025f0: 222c 2064 756d 705f 746f 5f73 7464 6572  ", dump_to_stder
+00002600: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00002610: 6365 7263 6973 2e61 7373 6572 745f 6571  cercis.assert_eq
+00002620: 7569 7661 6c65 6e74 2873 6f75 7263 652c  uivalent(source,
+00002630: 2061 6374 7561 6c29 0a20 2020 2020 2020   actual).       
+00002640: 2020 2020 2063 6572 6369 732e 6173 7365       cercis.asse
+00002650: 7274 5f73 7461 626c 6528 736f 7572 6365  rt_stable(source
+00002660: 2c20 6163 7475 616c 2c20 6d6f 6465 290a  , actual, mode).
+00002670: 0a20 2020 2064 6566 2074 6573 745f 6578  .    def test_ex
+00002680: 7072 6573 7369 6f6e 5f64 6966 6628 7365  pression_diff(se
+00002690: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+000026a0: 2020 2020 2073 6f75 7263 652c 205f 203d       source, _ =
+000026b0: 2072 6561 645f 6461 7461 2822 7369 6d70   read_data("simp
+000026c0: 6c65 5f63 6173 6573 222c 2022 6578 7072  le_cases", "expr
+000026d0: 6573 7369 6f6e 2e70 7922 290a 2020 2020  ession.py").    
+000026e0: 2020 2020 6578 7065 6374 6564 2c20 5f20      expected, _ 
+000026f0: 3d20 7265 6164 5f64 6174 6128 2273 696d  = read_data("sim
+00002700: 706c 655f 6361 7365 7322 2c20 2265 7870  ple_cases", "exp
+00002710: 7265 7373 696f 6e2e 6469 6666 2229 0a20  ression.diff"). 
+00002720: 2020 2020 2020 2074 6d70 5f66 696c 6520         tmp_file 
+00002730: 3d20 5061 7468 2863 6572 6369 732e 6475  = Path(cercis.du
+00002740: 6d70 5f74 6f5f 6669 6c65 2873 6f75 7263  mp_to_file(sourc
+00002750: 6529 290a 2020 2020 2020 2020 6469 6666  e)).        diff
+00002760: 5f68 6561 6465 7220 3d20 7265 2e63 6f6d  _header = re.com
+00002770: 7069 6c65 280a 2020 2020 2020 2020 2020  pile(.          
+00002780: 2020 7266 227b 7265 2e65 7363 6170 6528    rf"{re.escape(
+00002790: 7374 7228 746d 705f 6669 6c65 2929 7d5c  str(tmp_file))}\
+000027a0: 745c 645c 645c 645c 642d 5c64 5c64 2d5c  t\d\d\d\d-\d\d-\
+000027b0: 645c 6420 220a 2020 2020 2020 2020 2020  d\d ".          
+000027c0: 2020 7222 5c64 5c64 3a5c 645c 643a 5c64    r"\d\d:\d\d:\d
+000027d0: 5c64 5c2e 5c64 5c64 5c64 5c64 5c64 5c64  \d\.\d\d\d\d\d\d
+000027e0: 5c2b 5c64 5c64 3a5c 645c 6422 0a20 2020  \+\d\d:\d\d".   
+000027f0: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
+00002800: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00002810: 7265 7375 6c74 203d 2042 6c61 636b 5275  result = BlackRu
+00002820: 6e6e 6572 2829 2e69 6e76 6f6b 6528 0a20  nner().invoke(. 
+00002830: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002840: 6572 6369 732e 6d61 696e 2c0a 2020 2020  ercis.main,.    
+00002850: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 222d 2d64 6966 6622 2c0a 2020 2020    "--diff",.    
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 7374 7228 746d 705f 6669 6c65 292c 0a20  str(tmp_file),. 
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2066 222d 2d63 6f6e 6669 673d 7b45     f"--config={E
+000028c0: 4d50 5459 5f43 4f4e 4649 477d 222c 0a20  MPTY_CONFIG}",. 
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028e0: 2020 2022 2d2d 6c69 6e65 2d6c 656e 6774     "--line-lengt
+000028f0: 683d 3838 222c 0a20 2020 2020 2020 2020  h=88",.         
+00002900: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00002910: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002920: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00002930: 7175 616c 2872 6573 756c 742e 6578 6974  qual(result.exit
+00002940: 5f63 6f64 652c 2030 290a 2020 2020 2020  _code, 0).      
+00002950: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
+00002960: 2020 2020 2020 206f 732e 756e 6c69 6e6b         os.unlink
+00002970: 2874 6d70 5f66 696c 6529 0a20 2020 2020  (tmp_file).     
+00002980: 2020 2061 6374 7561 6c20 3d20 7265 7375     actual = resu
+00002990: 6c74 2e6f 7574 7075 740a 2020 2020 2020  lt.output.      
+000029a0: 2020 6163 7475 616c 203d 2064 6966 665f    actual = diff_
+000029b0: 6865 6164 6572 2e73 7562 2844 4554 4552  header.sub(DETER
+000029c0: 4d49 4e49 5354 4943 5f48 4541 4445 522c  MINISTIC_HEADER,
+000029d0: 2061 6374 7561 6c29 0a20 2020 2020 2020   actual).       
+000029e0: 2069 6620 6578 7065 6374 6564 2021 3d20   if expected != 
+000029f0: 6163 7475 616c 3a0a 2020 2020 2020 2020  actual:.        
+00002a00: 2020 2020 6475 6d70 203d 2063 6572 6369      dump = cerci
+00002a10: 732e 6475 6d70 5f74 6f5f 6669 6c65 2861  s.dump_to_file(a
+00002a20: 6374 7561 6c29 0a20 2020 2020 2020 2020  ctual).         
+00002a30: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
+00002a40: 2020 2020 2020 2020 2020 2022 4578 7065             "Expe
+00002a50: 6374 6564 2064 6966 6620 6973 6e27 7420  cted diff isn't 
+00002a60: 6571 7561 6c20 746f 2074 6865 2061 6374  equal to the act
+00002a70: 7561 6c2e 2049 6620 796f 7520 6d61 6465  ual. If you made
+00002a80: 2063 6861 6e67 6573 2074 6f22 0a20 2020   changes to".   
+00002a90: 2020 2020 2020 2020 2020 2020 2022 2065               " e
+00002aa0: 7870 7265 7373 696f 6e2e 7079 2061 6e64  xpression.py and
+00002ab0: 2074 6869 7320 6973 2061 6e20 616e 7469   this is an anti
+00002ac0: 6369 7061 7465 6420 6469 6666 6572 656e  cipated differen
+00002ad0: 6365 2c20 6f76 6572 7772 6974 6522 0a20  ce, overwrite". 
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00002af0: 2220 7465 7374 732f 6461 7461 2f65 7870  " tests/data/exp
+00002b00: 7265 7373 696f 6e2e 6469 6666 2077 6974  ression.diff wit
+00002b10: 6820 7b64 756d 707d 220a 2020 2020 2020  h {dump}".      
+00002b20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002b30: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00002b40: 7175 616c 2865 7870 6563 7465 642c 2061  qual(expected, a
+00002b50: 6374 7561 6c2c 206d 7367 290a 0a20 2020  ctual, msg)..   
+00002b60: 2064 6566 2074 6573 745f 6578 7072 6573   def test_expres
+00002b70: 7369 6f6e 5f64 6966 665f 7769 7468 5f63  sion_diff_with_c
+00002b80: 6f6c 6f72 2873 656c 6629 202d 3e20 4e6f  olor(self) -> No
+00002b90: 6e65 3a0a 2020 2020 2020 2020 736f 7572  ne:.        sour
+00002ba0: 6365 2c20 5f20 3d20 7265 6164 5f64 6174  ce, _ = read_dat
+00002bb0: 6128 2273 696d 706c 655f 6361 7365 7322  a("simple_cases"
+00002bc0: 2c20 2265 7870 7265 7373 696f 6e2e 7079  , "expression.py
+00002bd0: 2229 0a20 2020 2020 2020 2065 7870 6563  ").        expec
+00002be0: 7465 642c 205f 203d 2072 6561 645f 6461  ted, _ = read_da
+00002bf0: 7461 2822 7369 6d70 6c65 5f63 6173 6573  ta("simple_cases
+00002c00: 222c 2022 6578 7072 6573 7369 6f6e 2e64  ", "expression.d
+00002c10: 6966 6622 290a 2020 2020 2020 2020 746d  iff").        tm
+00002c20: 705f 6669 6c65 203d 2050 6174 6828 6365  p_file = Path(ce
+00002c30: 7263 6973 2e64 756d 705f 746f 5f66 696c  rcis.dump_to_fil
+00002c40: 6528 736f 7572 6365 2929 0a20 2020 2020  e(source)).     
+00002c50: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00002c60: 2020 2020 7265 7375 6c74 203d 2042 6c61      result = Bla
+00002c70: 636b 5275 6e6e 6572 2829 2e69 6e76 6f6b  ckRunner().invok
+00002c80: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00002c90: 2020 2063 6572 6369 732e 6d61 696e 2c0a     cercis.main,.
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 5b22 2d2d 6469 6666 222c 2022 2d2d 636f  ["--diff", "--co
+00002cc0: 6c6f 7222 2c20 7374 7228 746d 705f 6669  lor", str(tmp_fi
+00002cd0: 6c65 292c 2066 222d 2d63 6f6e 6669 673d  le), f"--config=
+00002ce0: 7b45 4d50 5459 5f43 4f4e 4649 477d 225d  {EMPTY_CONFIG}"]
+00002cf0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00002d00: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
+00002d10: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+00002d20: 756e 6c69 6e6b 2874 6d70 5f66 696c 6529  unlink(tmp_file)
+00002d30: 0a20 2020 2020 2020 2061 6374 7561 6c20  .        actual 
+00002d40: 3d20 7265 7375 6c74 2e6f 7574 7075 740a  = result.output.
+00002d50: 2020 2020 2020 2020 2320 5765 2063 6865          # We che
+00002d60: 636b 2074 6865 2063 6f6e 7465 6e74 7320  ck the contents 
+00002d70: 6f66 2074 6865 2064 6966 6620 696e 2060  of the diff in `
+00002d80: 7465 7374 5f65 7870 7265 7373 696f 6e5f  test_expression_
+00002d90: 6469 6666 602e 2041 6c6c 0a20 2020 2020  diff`. All.     
+00002da0: 2020 2023 2077 6520 6e65 6564 2074 6f20     # we need to 
+00002db0: 6368 6563 6b20 6865 7265 2069 7320 7468  check here is th
+00002dc0: 6174 2063 6f6c 6f72 2063 6f64 6573 2065  at color codes e
+00002dd0: 7869 7374 2069 6e20 7468 6520 7265 7375  xist in the resu
+00002de0: 6c74 2e0a 2020 2020 2020 2020 7365 6c66  lt..        self
+00002df0: 2e61 7373 6572 7449 6e28 225c 3033 335b  .assertIn("\033[
+00002e00: 316d 222c 2061 6374 7561 6c29 0a20 2020  1m", actual).   
+00002e10: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00002e20: 496e 2822 5c30 3333 5b33 366d 222c 2061  In("\033[36m", a
+00002e30: 6374 7561 6c29 0a20 2020 2020 2020 2073  ctual).        s
+00002e40: 656c 662e 6173 7365 7274 496e 2822 5c30  elf.assertIn("\0
+00002e50: 3333 5b33 326d 222c 2061 6374 7561 6c29  33[32m", actual)
+00002e60: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00002e70: 7365 7274 496e 2822 5c30 3333 5b33 316d  sertIn("\033[31m
+00002e80: 222c 2061 6374 7561 6c29 0a20 2020 2020  ", actual).     
+00002e90: 2020 2073 656c 662e 6173 7365 7274 496e     self.assertIn
+00002ea0: 2822 5c30 3333 5b30 6d22 2c20 6163 7475  ("\033[0m", actu
+00002eb0: 616c 290a 0a20 2020 2064 6566 2074 6573  al)..    def tes
+00002ec0: 745f 6465 7465 6374 5f70 6f73 5f6f 6e6c  t_detect_pos_onl
+00002ed0: 795f 6172 6775 6d65 6e74 7328 7365 6c66  y_arguments(self
+00002ee0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00002ef0: 2020 2073 6f75 7263 652c 205f 203d 2072     source, _ = r
+00002f00: 6561 645f 6461 7461 2822 7079 5f33 3822  ead_data("py_38"
+00002f10: 2c20 2270 6570 5f35 3730 2229 0a20 2020  , "pep_570").   
+00002f20: 2020 2020 2072 6f6f 7420 3d20 6365 7263       root = cerc
+00002f30: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
+00002f40: 2873 6f75 7263 6529 0a20 2020 2020 2020  (source).       
+00002f50: 2066 6561 7475 7265 7320 3d20 6365 7263   features = cerc
+00002f60: 6973 2e67 6574 5f66 6561 7475 7265 735f  is.get_features_
+00002f70: 7573 6564 2872 6f6f 7429 0a20 2020 2020  used(root).     
+00002f80: 2020 2073 656c 662e 6173 7365 7274 496e     self.assertIn
+00002f90: 2863 6572 6369 732e 4665 6174 7572 652e  (cercis.Feature.
+00002fa0: 504f 535f 4f4e 4c59 5f41 5247 554d 454e  POS_ONLY_ARGUMEN
+00002fb0: 5453 2c20 6665 6174 7572 6573 290a 2020  TS, features).  
+00002fc0: 2020 2020 2020 7665 7273 696f 6e73 203d        versions =
+00002fd0: 2063 6572 6369 732e 6465 7465 6374 5f74   cercis.detect_t
+00002fe0: 6172 6765 745f 7665 7273 696f 6e73 2872  arget_versions(r
+00002ff0: 6f6f 7429 0a20 2020 2020 2020 2073 656c  oot).        sel
+00003000: 662e 6173 7365 7274 496e 2863 6572 6369  f.assertIn(cerci
+00003010: 732e 5461 7267 6574 5665 7273 696f 6e2e  s.TargetVersion.
+00003020: 5059 3338 2c20 7665 7273 696f 6e73 290a  PY38, versions).
+00003030: 0a20 2020 2064 6566 2074 6573 745f 6465  .    def test_de
+00003040: 7465 6374 5f64 6562 7567 5f66 5f73 7472  tect_debug_f_str
+00003050: 696e 6773 2873 656c 6629 202d 3e20 4e6f  ings(self) -> No
+00003060: 6e65 3a0a 2020 2020 2020 2020 726f 6f74  ne:.        root
+00003070: 203d 2063 6572 6369 732e 6c69 6232 746f   = cercis.lib2to
+00003080: 335f 7061 7273 6528 2222 2266 227b 783d  3_parse("""f"{x=
+00003090: 7d22 2022 2222 290a 2020 2020 2020 2020  }" """).        
+000030a0: 6665 6174 7572 6573 203d 2063 6572 6369  features = cerci
+000030b0: 732e 6765 745f 6665 6174 7572 6573 5f75  s.get_features_u
+000030c0: 7365 6428 726f 6f74 290a 2020 2020 2020  sed(root).      
+000030d0: 2020 7365 6c66 2e61 7373 6572 7449 6e28    self.assertIn(
+000030e0: 6365 7263 6973 2e46 6561 7475 7265 2e44  cercis.Feature.D
+000030f0: 4542 5547 5f46 5f53 5452 494e 4753 2c20  EBUG_F_STRINGS, 
+00003100: 6665 6174 7572 6573 290a 2020 2020 2020  features).      
+00003110: 2020 7665 7273 696f 6e73 203d 2063 6572    versions = cer
+00003120: 6369 732e 6465 7465 6374 5f74 6172 6765  cis.detect_targe
+00003130: 745f 7665 7273 696f 6e73 2872 6f6f 7429  t_versions(root)
+00003140: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00003150: 7365 7274 496e 2863 6572 6369 732e 5461  sertIn(cercis.Ta
+00003160: 7267 6574 5665 7273 696f 6e2e 5059 3338  rgetVersion.PY38
+00003170: 2c20 7665 7273 696f 6e73 290a 0a20 2020  , versions)..   
+00003180: 2020 2020 2072 6f6f 7420 3d20 6365 7263       root = cerc
+00003190: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
+000031a0: 280a 2020 2020 2020 2020 2020 2020 2222  (.            ""
+000031b0: 2266 227b 787d 225c 6e66 277b 223d 227d  "f"{x}"\nf'{"="}
+000031c0: 275c 6e66 277b 2878 3a3d 3529 7d27 5c6e  '\nf'{(x:=5)}'\n
+000031d0: 6627 7b66 2861 3d22 333d 2229 7d27 5c6e  f'{f(a="3=")}'\n
+000031e0: 6627 7b78 3a3d 3130 7d27 5c6e 2222 220a  f'{x:=10}'\n""".
+000031f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00003200: 2020 6665 6174 7572 6573 203d 2063 6572    features = cer
+00003210: 6369 732e 6765 745f 6665 6174 7572 6573  cis.get_features
+00003220: 5f75 7365 6428 726f 6f74 290a 2020 2020  _used(root).    
+00003230: 2020 2020 7365 6c66 2e61 7373 6572 744e      self.assertN
+00003240: 6f74 496e 2863 6572 6369 732e 4665 6174  otIn(cercis.Feat
+00003250: 7572 652e 4445 4255 475f 465f 5354 5249  ure.DEBUG_F_STRI
+00003260: 4e47 532c 2066 6561 7475 7265 7329 0a0a  NGS, features)..
+00003270: 2020 2020 2020 2020 2320 5765 2064 6f6e          # We don
+00003280: 2774 2079 6574 2073 7570 706f 7274 2066  't yet support f
+00003290: 6561 7475 7265 2076 6572 7369 6f6e 2064  eature version d
+000032a0: 6574 6563 7469 6f6e 2069 6e20 6e65 7374  etection in nest
+000032b0: 6564 2066 2d73 7472 696e 6773 0a20 2020  ed f-strings.   
+000032c0: 2020 2020 2072 6f6f 7420 3d20 6365 7263       root = cerc
+000032d0: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
+000032e0: 280a 2020 2020 2020 2020 2020 2020 2222  (.            ""
+000032f0: 2266 2268 6561 7264 2061 2072 756d 6f75  "f"heard a rumou
+00003300: 7220 7468 6174 207b 2066 277b 312b 313d  r that { f'{1+1=
+00003310: 7d27 207d 202e 2e2e 2073 6565 6d73 206c  }' } ... seems l
+00003320: 696b 6520 6974 2063 6f75 6c64 2062 6520  ike it could be 
+00003330: 7472 7565 2220 2222 220a 2020 2020 2020  true" """.      
+00003340: 2020 290a 2020 2020 2020 2020 6665 6174    ).        feat
+00003350: 7572 6573 203d 2063 6572 6369 732e 6765  ures = cercis.ge
+00003360: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
+00003370: 726f 6f74 290a 2020 2020 2020 2020 7365  root).        se
+00003380: 6c66 2e61 7373 6572 744e 6f74 496e 2863  lf.assertNotIn(c
+00003390: 6572 6369 732e 4665 6174 7572 652e 4445  ercis.Feature.DE
+000033a0: 4255 475f 465f 5354 5249 4e47 532c 2066  BUG_F_STRINGS, f
+000033b0: 6561 7475 7265 7329 0a0a 2020 2020 4070  eatures)..    @p
+000033c0: 6174 6368 2822 6365 7263 6973 2e64 756d  atch("cercis.dum
+000033d0: 705f 746f 5f66 696c 6522 2c20 6475 6d70  p_to_file", dump
+000033e0: 5f74 6f5f 7374 6465 7272 290a 2020 2020  _to_stderr).    
+000033f0: 6465 6620 7465 7374 5f73 7472 696e 675f  def test_string_
+00003400: 7175 6f74 6573 2873 656c 6629 202d 3e20  quotes(self) -> 
+00003410: 4e6f 6e65 3a0a 2020 2020 2020 2020 736f  None:.        so
+00003420: 7572 6365 2c20 6578 7065 6374 6564 203d  urce, expected =
+00003430: 2072 6561 645f 6461 7461 2822 6d69 7363   read_data("misc
+00003440: 656c 6c61 6e65 6f75 7322 2c20 2273 7472  ellaneous", "str
+00003450: 696e 675f 7175 6f74 6573 2229 0a20 2020  ing_quotes").   
+00003460: 2020 2020 206d 6f64 6520 3d20 6365 7263       mode = cerc
+00003470: 6973 2e4d 6f64 6528 7072 6576 6965 773d  is.Mode(preview=
+00003480: 5472 7565 2c20 7369 6e67 6c65 5f71 756f  True, single_quo
+00003490: 7465 3d46 616c 7365 290a 2020 2020 2020  te=False).      
+000034a0: 2020 6173 7365 7274 5f66 6f72 6d61 7428    assert_format(
+000034b0: 736f 7572 6365 2c20 6578 7065 6374 6564  source, expected
+000034c0: 2c20 6d6f 6465 290a 2020 2020 2020 2020  , mode).        
+000034d0: 6d6f 6465 203d 2072 6570 6c61 6365 286d  mode = replace(m
+000034e0: 6f64 652c 2073 7472 696e 675f 6e6f 726d  ode, string_norm
+000034f0: 616c 697a 6174 696f 6e3d 4661 6c73 6529  alization=False)
+00003500: 0a20 2020 2020 2020 206e 6f74 5f6e 6f72  .        not_nor
+00003510: 6d61 6c69 7a65 6420 3d20 6673 2873 6f75  malized = fs(sou
+00003520: 7263 652c 206d 6f64 653d 6d6f 6465 290a  rce, mode=mode).
+00003530: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00003540: 6572 7446 6f72 6d61 7445 7175 616c 2873  ertFormatEqual(s
+00003550: 6f75 7263 652e 7265 706c 6163 6528 225c  ource.replace("\
+00003560: 5c5c 6e22 2c20 2222 292c 206e 6f74 5f6e  \\n", ""), not_n
+00003570: 6f72 6d61 6c69 7a65 6429 0a20 2020 2020  ormalized).     
+00003580: 2020 2063 6572 6369 732e 6173 7365 7274     cercis.assert
+00003590: 5f65 7175 6976 616c 656e 7428 736f 7572  _equivalent(sour
+000035a0: 6365 2c20 6e6f 745f 6e6f 726d 616c 697a  ce, not_normaliz
+000035b0: 6564 290a 2020 2020 2020 2020 6365 7263  ed).        cerc
+000035c0: 6973 2e61 7373 6572 745f 7374 6162 6c65  is.assert_stable
+000035d0: 2873 6f75 7263 652c 206e 6f74 5f6e 6f72  (source, not_nor
+000035e0: 6d61 6c69 7a65 642c 206d 6f64 653d 6d6f  malized, mode=mo
+000035f0: 6465 290a 0a20 2020 2064 6566 2074 6573  de)..    def tes
+00003600: 745f 736b 6970 5f73 6f75 7263 655f 6669  t_skip_source_fi
+00003610: 7273 745f 6c69 6e65 2873 656c 6629 202d  rst_line(self) -
+00003620: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00003630: 736f 7572 6365 2c20 5f20 3d20 7265 6164  source, _ = read
+00003640: 5f64 6174 6128 226d 6973 6365 6c6c 616e  _data("miscellan
+00003650: 656f 7573 222c 2022 696e 7661 6c69 645f  eous", "invalid_
+00003660: 6865 6164 6572 2229 0a20 2020 2020 2020  header").       
+00003670: 2074 6d70 5f66 696c 6520 3d20 5061 7468   tmp_file = Path
+00003680: 2863 6572 6369 732e 6475 6d70 5f74 6f5f  (cercis.dump_to_
+00003690: 6669 6c65 2873 6f75 7263 6529 290a 2020  file(source)).  
+000036a0: 2020 2020 2020 2320 4675 6c6c 2073 6f75        # Full sou
+000036b0: 7263 6520 7368 6f75 6c64 2066 6169 6c20  rce should fail 
+000036c0: 2869 6e76 616c 6964 2073 796e 7461 7820  (invalid syntax 
+000036d0: 6174 2068 6561 6465 7229 0a20 2020 2020  at header).     
+000036e0: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
+000036f0: 6163 6b28 5b73 7472 2874 6d70 5f66 696c  ack([str(tmp_fil
+00003700: 6529 2c20 222d 2d64 6966 6622 2c20 222d  e), "--diff", "-
+00003710: 2d63 6865 636b 225d 2c20 6578 6974 5f63  -check"], exit_c
+00003720: 6f64 653d 3132 3329 0a20 2020 2020 2020  ode=123).       
+00003730: 2023 2053 6f2c 2073 6b69 7070 696e 6720   # So, skipping 
+00003740: 7468 6520 6669 7273 7420 6c69 6e65 2073  the first line s
+00003750: 686f 756c 6420 776f 726b 0a20 2020 2020  hould work.     
+00003760: 2020 2072 6573 756c 7420 3d20 426c 6163     result = Blac
+00003770: 6b52 756e 6e65 7228 292e 696e 766f 6b65  kRunner().invoke
+00003780: 280a 2020 2020 2020 2020 2020 2020 6365  (.            ce
+00003790: 7263 6973 2e6d 6169 6e2c 205b 7374 7228  rcis.main, [str(
+000037a0: 746d 705f 6669 6c65 292c 2022 2d78 222c  tmp_file), "-x",
+000037b0: 2066 222d 2d63 6f6e 6669 673d 7b45 4d50   f"--config={EMP
+000037c0: 5459 5f43 4f4e 4649 477d 225d 0a20 2020  TY_CONFIG}"].   
+000037d0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+000037e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000037f0: 7265 7375 6c74 2e65 7869 745f 636f 6465  result.exit_code
+00003800: 2c20 3029 0a20 2020 2020 2020 2077 6974  , 0).        wit
+00003810: 6820 6f70 656e 2874 6d70 5f66 696c 652c  h open(tmp_file,
+00003820: 2065 6e63 6f64 696e 673d 2275 7466 3822   encoding="utf8"
+00003830: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+00003840: 2020 2020 6163 7475 616c 203d 2066 2e72      actual = f.r
+00003850: 6561 6428 290a 2020 2020 2020 2020 7365  ead().        se
+00003860: 6c66 2e61 7373 6572 7446 6f72 6d61 7445  lf.assertFormatE
+00003870: 7175 616c 2873 6f75 7263 652c 2061 6374  qual(source, act
+00003880: 7561 6c29 0a0a 2020 2020 6465 6620 7465  ual)..    def te
+00003890: 7374 5f73 6b69 705f 736f 7572 6365 5f66  st_skip_source_f
+000038a0: 6972 7374 5f6c 696e 655f 7768 656e 5f6d  irst_line_when_m
+000038b0: 6978 696e 675f 6e65 776c 696e 6573 2873  ixing_newlines(s
+000038c0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+000038d0: 2020 2020 2020 636f 6465 5f6d 6978 696e        code_mixin
+000038e0: 675f 6e65 776c 696e 6573 203d 2062 2248  g_newlines = b"H
+000038f0: 6561 6465 7220 7769 6c6c 2062 6520 736b  eader will be sk
+00003900: 6970 7065 645c 725c 6e69 203d 205b 312c  ipped\r\ni = [1,
+00003910: 322c 335d 5c6e 6a20 3d20 5b31 2c32 2c33  2,3]\nj = [1,2,3
+00003920: 5d5c 6e22 0a20 2020 2020 2020 2065 7870  ]\n".        exp
+00003930: 6563 7465 6420 3d20 6222 4865 6164 6572  ected = b"Header
+00003940: 2077 696c 6c20 6265 2073 6b69 7070 6564   will be skipped
+00003950: 5c72 5c6e 6920 3d20 5b31 2c20 322c 2033  \r\ni = [1, 2, 3
+00003960: 5d5c 6e6a 203d 205b 312c 2032 2c20 335d  ]\nj = [1, 2, 3]
+00003970: 5c6e 220a 2020 2020 2020 2020 7769 7468  \n".        with
+00003980: 2054 656d 706f 7261 7279 4469 7265 6374   TemporaryDirect
+00003990: 6f72 7928 2920 6173 2077 6f72 6b73 7061  ory() as workspa
+000039a0: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+000039b0: 7465 7374 5f66 696c 6520 3d20 5061 7468  test_file = Path
+000039c0: 2877 6f72 6b73 7061 6365 2920 2f20 2273  (workspace) / "s
+000039d0: 6b69 705f 6865 6164 6572 2e70 7922 0a20  kip_header.py". 
+000039e0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+000039f0: 6669 6c65 2e77 7269 7465 5f62 7974 6573  file.write_bytes
+00003a00: 2863 6f64 655f 6d69 7869 6e67 5f6e 6577  (code_mixing_new
+00003a10: 6c69 6e65 7329 0a20 2020 2020 2020 2020  lines).         
+00003a20: 2020 206d 6f64 6520 3d20 7265 706c 6163     mode = replac
+00003a30: 6528 4445 4641 554c 545f 4d4f 4445 2c20  e(DEFAULT_MODE, 
+00003a40: 736b 6970 5f73 6f75 7263 655f 6669 7273  skip_source_firs
+00003a50: 745f 6c69 6e65 3d54 7275 6529 0a20 2020  t_line=True).   
+00003a60: 2020 2020 2020 2020 2066 6628 7465 7374           ff(test
+00003a70: 5f66 696c 652c 206d 6f64 653d 6d6f 6465  _file, mode=mode
+00003a80: 2c20 7772 6974 655f 6261 636b 3d63 6572  , write_back=cer
+00003a90: 6369 732e 5772 6974 6542 6163 6b2e 5945  cis.WriteBack.YE
+00003aa0: 5329 0a20 2020 2020 2020 2020 2020 2073  S).            s
+00003ab0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00003ac0: 7465 7374 5f66 696c 652e 7265 6164 5f62  test_file.read_b
+00003ad0: 7974 6573 2829 2c20 6578 7065 6374 6564  ytes(), expected
+00003ae0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00003af0: 736b 6970 5f6d 6167 6963 5f74 7261 696c  skip_magic_trail
+00003b00: 696e 675f 636f 6d6d 6128 7365 6c66 2920  ing_comma(self) 
+00003b10: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00003b20: 2073 6f75 7263 652c 205f 203d 2072 6561   source, _ = rea
+00003b30: 645f 6461 7461 2822 7369 6d70 6c65 5f63  d_data("simple_c
+00003b40: 6173 6573 222c 2022 6578 7072 6573 7369  ases", "expressi
+00003b50: 6f6e 2229 0a20 2020 2020 2020 2065 7870  on").        exp
+00003b60: 6563 7465 642c 205f 203d 2072 6561 645f  ected, _ = read_
+00003b70: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
+00003b80: 2020 226d 6973 6365 6c6c 616e 656f 7573    "miscellaneous
+00003b90: 222c 2022 6578 7072 6573 7369 6f6e 5f73  ", "expression_s
+00003ba0: 6b69 705f 6d61 6769 635f 7472 6169 6c69  kip_magic_traili
+00003bb0: 6e67 5f63 6f6d 6d61 2e64 6966 6622 0a20  ng_comma.diff". 
+00003bc0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00003bd0: 2074 6d70 5f66 696c 6520 3d20 5061 7468   tmp_file = Path
+00003be0: 2863 6572 6369 732e 6475 6d70 5f74 6f5f  (cercis.dump_to_
+00003bf0: 6669 6c65 2873 6f75 7263 6529 290a 2020  file(source)).  
+00003c00: 2020 2020 2020 6469 6666 5f68 6561 6465        diff_heade
+00003c10: 7220 3d20 7265 2e63 6f6d 7069 6c65 280a  r = re.compile(.
+00003c20: 2020 2020 2020 2020 2020 2020 7266 227b              rf"{
+00003c30: 7265 2e65 7363 6170 6528 7374 7228 746d  re.escape(str(tm
+00003c40: 705f 6669 6c65 2929 7d5c 745c 645c 645c  p_file))}\t\d\d\
+00003c50: 645c 642d 5c64 5c64 2d5c 645c 6420 220a  d\d-\d\d-\d\d ".
+00003c60: 2020 2020 2020 2020 2020 2020 7222 5c64              r"\d
+00003c70: 5c64 3a5c 645c 643a 5c64 5c64 5c2e 5c64  \d:\d\d:\d\d\.\d
+00003c80: 5c64 5c64 5c64 5c64 5c64 5c2b 5c64 5c64  \d\d\d\d\d\+\d\d
+00003c90: 3a5c 645c 6422 0a20 2020 2020 2020 2029  :\d\d".        )
+00003ca0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00003cb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00003cc0: 203d 2042 6c61 636b 5275 6e6e 6572 2829   = BlackRunner()
+00003cd0: 2e69 6e76 6f6b 6528 0a20 2020 2020 2020  .invoke(.       
+00003ce0: 2020 2020 2020 2020 2063 6572 6369 732e           cercis.
+00003cf0: 6d61 696e 2c0a 2020 2020 2020 2020 2020  main,.          
+00003d00: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00003d10: 2020 2020 2020 2020 2020 2020 222d 4322              "-C"
+00003d20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003d30: 2020 2020 2020 222d 2d64 6966 6622 2c0a        "--diff",.
+00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d50: 2020 2020 7374 7228 746d 705f 6669 6c65      str(tmp_file
+00003d60: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00003d70: 2020 2020 2020 2066 222d 2d63 6f6e 6669         f"--confi
+00003d80: 673d 7b45 4d50 5459 5f43 4f4e 4649 477d  g={EMPTY_CONFIG}
+00003d90: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003da0: 2020 2020 2020 2022 2d2d 6c69 6e65 2d6c         "--line-l
+00003db0: 656e 6774 683d 3838 222c 0a20 2020 2020  ength=88",.     
+00003dc0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+00003dd0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00003de0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00003df0: 6572 7445 7175 616c 2872 6573 756c 742e  ertEqual(result.
+00003e00: 6578 6974 5f63 6f64 652c 2030 290a 2020  exit_code, 0).  
+00003e10: 2020 2020 2020 6669 6e61 6c6c 793a 0a20        finally:. 
+00003e20: 2020 2020 2020 2020 2020 206f 732e 756e             os.un
+00003e30: 6c69 6e6b 2874 6d70 5f66 696c 6529 0a20  link(tmp_file). 
+00003e40: 2020 2020 2020 2061 6374 7561 6c20 3d20         actual = 
+00003e50: 7265 7375 6c74 2e6f 7574 7075 740a 2020  result.output.  
+00003e60: 2020 2020 2020 6163 7475 616c 203d 2064        actual = d
+00003e70: 6966 665f 6865 6164 6572 2e73 7562 2844  iff_header.sub(D
+00003e80: 4554 4552 4d49 4e49 5354 4943 5f48 4541  ETERMINISTIC_HEA
+00003e90: 4445 522c 2061 6374 7561 6c29 0a20 2020  DER, actual).   
+00003ea0: 2020 2020 2061 6374 7561 6c20 3d20 6163       actual = ac
+00003eb0: 7475 616c 2e72 7374 7269 7028 2920 2b20  tual.rstrip() + 
+00003ec0: 225c 6e22 2020 2320 7468 6520 6469 6666  "\n"  # the diff
+00003ed0: 206f 7574 7075 7420 6861 7320 6120 7472   output has a tr
+00003ee0: 6169 6c69 6e67 2073 7061 6365 0a20 2020  ailing space.   
+00003ef0: 2020 2020 2069 6620 6578 7065 6374 6564       if expected
+00003f00: 2021 3d20 6163 7475 616c 3a0a 2020 2020   != actual:.    
+00003f10: 2020 2020 2020 2020 6475 6d70 203d 2063          dump = c
+00003f20: 6572 6369 732e 6475 6d70 5f74 6f5f 6669  ercis.dump_to_fi
+00003f30: 6c65 2861 6374 7561 6c29 0a20 2020 2020  le(actual).     
+00003f40: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
+00003f50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003f60: 4578 7065 6374 6564 2064 6966 6620 6973  Expected diff is
+00003f70: 6e27 7420 6571 7561 6c20 746f 2074 6865  n't equal to the
+00003f80: 2061 6374 7561 6c2e 2049 6620 796f 7520   actual. If you 
+00003f90: 6d61 6465 2063 6861 6e67 6573 2074 6f22  made changes to"
+00003fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003fb0: 2022 2065 7870 7265 7373 696f 6e2e 7079   " expression.py
+00003fc0: 2061 6e64 2074 6869 7320 6973 2061 6e20   and this is an 
+00003fd0: 616e 7469 6369 7061 7465 6420 6469 6666  anticipated diff
+00003fe0: 6572 656e 6365 2c20 6f76 6572 7772 6974  erence, overwrit
+00003ff0: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+00004000: 2020 2022 2074 6573 7473 2f64 6174 612f     " tests/data/
+00004010: 6d69 7363 656c 6c61 6e65 6f75 732f 6578  miscellaneous/ex
+00004020: 7072 6573 7369 6f6e 5f73 6b69 705f 6d61  pression_skip_ma
+00004030: 6769 635f 7472 6169 6c69 6e67 5f63 6f6d  gic_trailing_com
+00004040: 6d61 2e64 6966 6622 0a20 2020 2020 2020  ma.diff".       
+00004050: 2020 2020 2020 2020 2066 2220 7769 7468           f" with
+00004060: 207b 6475 6d70 7d22 0a20 2020 2020 2020   {dump}".       
+00004070: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00004080: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00004090: 7561 6c28 6578 7065 6374 6564 2c20 6163  ual(expected, ac
+000040a0: 7475 616c 2c20 6d73 6729 0a0a 2020 2020  tual, msg)..    
+000040b0: 4070 6174 6368 2822 6365 7263 6973 2e64  @patch("cercis.d
+000040c0: 756d 705f 746f 5f66 696c 6522 2c20 6475  ump_to_file", du
+000040d0: 6d70 5f74 6f5f 7374 6465 7272 290a 2020  mp_to_stderr).  
+000040e0: 2020 6465 6620 7465 7374 5f61 7379 6e63    def test_async
+000040f0: 5f61 735f 6964 656e 7469 6669 6572 2873  _as_identifier(s
+00004100: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00004110: 2020 2020 2020 736f 7572 6365 5f70 6174        source_pat
+00004120: 6820 3d20 6765 745f 6361 7365 5f70 6174  h = get_case_pat
+00004130: 6828 226d 6973 6365 6c6c 616e 656f 7573  h("miscellaneous
+00004140: 222c 2022 6173 796e 635f 6173 5f69 6465  ", "async_as_ide
+00004150: 6e74 6966 6965 7222 290a 2020 2020 2020  ntifier").      
+00004160: 2020 736f 7572 6365 2c20 6578 7065 6374    source, expect
+00004170: 6564 203d 2072 6561 645f 6461 7461 5f66  ed = read_data_f
+00004180: 726f 6d5f 6669 6c65 2873 6f75 7263 655f  rom_file(source_
+00004190: 7061 7468 290a 2020 2020 2020 2020 6163  path).        ac
+000041a0: 7475 616c 203d 2066 7328 736f 7572 6365  tual = fs(source
+000041b0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000041c0: 7373 6572 7446 6f72 6d61 7445 7175 616c  ssertFormatEqual
+000041d0: 2865 7870 6563 7465 642c 2061 6374 7561  (expected, actua
+000041e0: 6c29 0a20 2020 2020 2020 206d 616a 6f72  l).        major
+000041f0: 2c20 6d69 6e6f 7220 3d20 7379 732e 7665  , minor = sys.ve
+00004200: 7273 696f 6e5f 696e 666f 5b3a 325d 0a20  rsion_info[:2]. 
+00004210: 2020 2020 2020 2069 6620 6d61 6a6f 7220         if major 
+00004220: 3c20 3320 6f72 2028 6d61 6a6f 7220 3c3d  < 3 or (major <=
+00004230: 2033 2061 6e64 206d 696e 6f72 203c 2037   3 and minor < 7
+00004240: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00004250: 6572 6369 732e 6173 7365 7274 5f65 7175  ercis.assert_equ
+00004260: 6976 616c 656e 7428 736f 7572 6365 2c20  ivalent(source, 
+00004270: 6163 7475 616c 290a 2020 2020 2020 2020  actual).        
+00004280: 6365 7263 6973 2e61 7373 6572 745f 7374  cercis.assert_st
+00004290: 6162 6c65 2873 6f75 7263 652c 2061 6374  able(source, act
+000042a0: 7561 6c2c 2044 4546 4155 4c54 5f4d 4f44  ual, DEFAULT_MOD
+000042b0: 4529 0a20 2020 2020 2020 2023 2065 6e73  E).        # ens
+000042c0: 7572 6520 6365 7263 6973 2063 616e 2070  ure cercis can p
+000042d0: 6172 7365 2074 6869 7320 7768 656e 2074  arse this when t
+000042e0: 6865 2074 6172 6765 7420 6973 2033 2e36  he target is 3.6
+000042f0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00004300: 766f 6b65 426c 6163 6b28 5b73 7472 2873  vokeBlack([str(s
+00004310: 6f75 7263 655f 7061 7468 292c 2022 2d2d  ource_path), "--
+00004320: 7461 7267 6574 2d76 6572 7369 6f6e 222c  target-version",
+00004330: 2022 7079 3336 225d 290a 2020 2020 2020   "py36"]).      
+00004340: 2020 2320 6275 7420 6e6f 7420 6f6e 2033    # but not on 3
+00004350: 2e37 2c20 6265 6361 7573 6520 6173 796e  .7, because asyn
+00004360: 632f 6177 6169 7420 6973 206e 6f20 6c6f  c/await is no lo
+00004370: 6e67 6572 2061 6e20 6964 656e 7469 6669  nger an identifi
+00004380: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+00004390: 696e 766f 6b65 426c 6163 6b28 5b73 7472  invokeBlack([str
+000043a0: 2873 6f75 7263 655f 7061 7468 292c 2022  (source_path), "
+000043b0: 2d2d 7461 7267 6574 2d76 6572 7369 6f6e  --target-version
+000043c0: 222c 2022 7079 3337 225d 2c20 6578 6974  ", "py37"], exit
+000043d0: 5f63 6f64 653d 3132 3329 0a0a 2020 2020  _code=123)..    
+000043e0: 4070 6174 6368 2822 6365 7263 6973 2e64  @patch("cercis.d
+000043f0: 756d 705f 746f 5f66 696c 6522 2c20 6475  ump_to_file", du
+00004400: 6d70 5f74 6f5f 7374 6465 7272 290a 2020  mp_to_stderr).  
+00004410: 2020 6465 6620 7465 7374 5f70 7974 686f    def test_pytho
+00004420: 6e33 3728 7365 6c66 2920 2d3e 204e 6f6e  n37(self) -> Non
+00004430: 653a 0a20 2020 2020 2020 2073 6f75 7263  e:.        sourc
+00004440: 655f 7061 7468 203d 2067 6574 5f63 6173  e_path = get_cas
+00004450: 655f 7061 7468 2822 7079 5f33 3722 2c20  e_path("py_37", 
+00004460: 2270 7974 686f 6e33 3722 290a 2020 2020  "python37").    
+00004470: 2020 2020 736f 7572 6365 2c20 6578 7065      source, expe
+00004480: 6374 6564 203d 2072 6561 645f 6461 7461  cted = read_data
+00004490: 5f66 726f 6d5f 6669 6c65 2873 6f75 7263  _from_file(sourc
+000044a0: 655f 7061 7468 290a 2020 2020 2020 2020  e_path).        
+000044b0: 6163 7475 616c 203d 2066 7328 736f 7572  actual = fs(sour
+000044c0: 6365 290a 2020 2020 2020 2020 7365 6c66  ce).        self
+000044d0: 2e61 7373 6572 7446 6f72 6d61 7445 7175  .assertFormatEqu
+000044e0: 616c 2865 7870 6563 7465 642c 2061 6374  al(expected, act
+000044f0: 7561 6c29 0a20 2020 2020 2020 206d 616a  ual).        maj
+00004500: 6f72 2c20 6d69 6e6f 7220 3d20 7379 732e  or, minor = sys.
+00004510: 7665 7273 696f 6e5f 696e 666f 5b3a 325d  version_info[:2]
+00004520: 0a20 2020 2020 2020 2069 6620 6d61 6a6f  .        if majo
+00004530: 7220 3e20 3320 6f72 2028 6d61 6a6f 7220  r > 3 or (major 
+00004540: 3d3d 2033 2061 6e64 206d 696e 6f72 203e  == 3 and minor >
+00004550: 3d20 3729 3a0a 2020 2020 2020 2020 2020  = 7):.          
+00004560: 2020 6365 7263 6973 2e61 7373 6572 745f    cercis.assert_
+00004570: 6571 7569 7661 6c65 6e74 2873 6f75 7263  equivalent(sourc
+00004580: 652c 2061 6374 7561 6c29 0a20 2020 2020  e, actual).     
+00004590: 2020 2063 6572 6369 732e 6173 7365 7274     cercis.assert
+000045a0: 5f73 7461 626c 6528 736f 7572 6365 2c20  _stable(source, 
+000045b0: 6163 7475 616c 2c20 4445 4641 554c 545f  actual, DEFAULT_
+000045c0: 4d4f 4445 290a 2020 2020 2020 2020 2320  MODE).        # 
+000045d0: 656e 7375 7265 2063 6572 6369 7320 6361  ensure cercis ca
+000045e0: 6e20 7061 7273 6520 7468 6973 2077 6865  n parse this whe
+000045f0: 6e20 7468 6520 7461 7267 6574 2069 7320  n the target is 
+00004600: 332e 370a 2020 2020 2020 2020 7365 6c66  3.7.        self
+00004610: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
+00004620: 7228 736f 7572 6365 5f70 6174 6829 2c20  r(source_path), 
+00004630: 222d 2d74 6172 6765 742d 7665 7273 696f  "--target-versio
+00004640: 6e22 2c20 2270 7933 3722 5d29 0a20 2020  n", "py37"]).   
+00004650: 2020 2020 2023 2062 7574 206e 6f74 206f       # but not o
+00004660: 6e20 332e 362c 2062 6563 6175 7365 2077  n 3.6, because w
+00004670: 6520 7573 6520 6173 796e 6320 6173 2061  e use async as a
+00004680: 2072 6573 6572 7665 6420 6b65 7977 6f72   reserved keywor
+00004690: 640a 2020 2020 2020 2020 7365 6c66 2e69  d.        self.i
+000046a0: 6e76 6f6b 6542 6c61 636b 285b 7374 7228  nvokeBlack([str(
+000046b0: 736f 7572 6365 5f70 6174 6829 2c20 222d  source_path), "-
+000046c0: 2d74 6172 6765 742d 7665 7273 696f 6e22  -target-version"
+000046d0: 2c20 2270 7933 3622 5d2c 2065 7869 745f  , "py36"], exit_
+000046e0: 636f 6465 3d31 3233 290a 0a20 2020 2064  code=123)..    d
+000046f0: 6566 2074 6573 745f 7461 625f 636f 6d6d  ef test_tab_comm
+00004700: 656e 745f 696e 6465 6e74 6174 696f 6e28  ent_indentation(
+00004710: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00004720: 2020 2020 2020 2063 6f6e 7465 6e74 735f         contents_
+00004730: 7461 6220 3d20 2269 6620 313a 5c6e 5c74  tab = "if 1:\n\t
+00004740: 6966 2032 3a5c 6e5c 745c 7470 6173 735c  if 2:\n\t\tpass\
+00004750: 6e5c 7423 2063 6f6d 6d65 6e74 5c6e 5c74  n\t# comment\n\t
+00004760: 7061 7373 5c6e 220a 2020 2020 2020 2020  pass\n".        
+00004770: 636f 6e74 656e 7473 5f73 7063 203d 2022  contents_spc = "
+00004780: 6966 2031 3a5c 6e20 2020 2069 6620 323a  if 1:\n    if 2:
+00004790: 5c6e 2020 2020 2020 2020 7061 7373 5c6e  \n        pass\n
+000047a0: 2020 2020 2320 636f 6d6d 656e 745c 6e20      # comment\n 
+000047b0: 2020 2070 6173 735c 6e22 0a20 2020 2020     pass\n".     
+000047c0: 2020 2073 656c 662e 6173 7365 7274 466f     self.assertFo
+000047d0: 726d 6174 4571 7561 6c28 636f 6e74 656e  rmatEqual(conten
+000047e0: 7473 5f73 7063 2c20 6673 2863 6f6e 7465  ts_spc, fs(conte
+000047f0: 6e74 735f 7370 6329 290a 2020 2020 2020  nts_spc)).      
+00004800: 2020 7365 6c66 2e61 7373 6572 7446 6f72    self.assertFor
+00004810: 6d61 7445 7175 616c 2863 6f6e 7465 6e74  matEqual(content
+00004820: 735f 7370 632c 2066 7328 636f 6e74 656e  s_spc, fs(conten
+00004830: 7473 5f74 6162 2929 0a0a 2020 2020 2020  ts_tab))..      
+00004840: 2020 636f 6e74 656e 7473 5f74 6162 203d    contents_tab =
+00004850: 2022 6966 2031 3a5c 6e5c 7469 6620 323a   "if 1:\n\tif 2:
+00004860: 5c6e 5c74 5c74 7061 7373 5c6e 5c74 5c74  \n\t\tpass\n\t\t
+00004870: 2320 636f 6d6d 656e 745c 6e5c 7470 6173  # comment\n\tpas
+00004880: 735c 6e22 0a20 2020 2020 2020 2063 6f6e  s\n".        con
+00004890: 7465 6e74 735f 7370 6320 3d20 2269 6620  tents_spc = "if 
+000048a0: 313a 5c6e 2020 2020 6966 2032 3a5c 6e20  1:\n    if 2:\n 
+000048b0: 2020 2020 2020 2070 6173 735c 6e20 2020         pass\n   
+000048c0: 2020 2020 2023 2063 6f6d 6d65 6e74 5c6e       # comment\n
+000048d0: 2020 2020 7061 7373 5c6e 220a 2020 2020      pass\n".    
+000048e0: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
+000048f0: 6f72 6d61 7445 7175 616c 2863 6f6e 7465  ormatEqual(conte
+00004900: 6e74 735f 7370 632c 2066 7328 636f 6e74  nts_spc, fs(cont
+00004910: 656e 7473 5f73 7063 2929 0a20 2020 2020  ents_spc)).     
+00004920: 2020 2073 656c 662e 6173 7365 7274 466f     self.assertFo
+00004930: 726d 6174 4571 7561 6c28 636f 6e74 656e  rmatEqual(conten
+00004940: 7473 5f73 7063 2c20 6673 2863 6f6e 7465  ts_spc, fs(conte
+00004950: 6e74 735f 7461 6229 290a 0a20 2020 2020  nts_tab))..     
+00004960: 2020 2023 206d 6978 6564 2074 6162 7320     # mixed tabs 
+00004970: 616e 6420 7370 6163 6573 2028 7661 6c69  and spaces (vali
+00004980: 6420 5079 7468 6f6e 2032 2063 6f64 6529  d Python 2 code)
+00004990: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
+000049a0: 735f 7461 6220 3d20 2269 6620 313a 5c6e  s_tab = "if 1:\n
+000049b0: 2020 2020 2020 2020 6966 2032 3a5c 6e5c          if 2:\n\
+000049c0: 745c 7470 6173 735c 6e5c 7423 2063 6f6d  t\tpass\n\t# com
+000049d0: 6d65 6e74 5c6e 2020 2020 2020 2020 7061  ment\n        pa
+000049e0: 7373 5c6e 220a 2020 2020 2020 2020 636f  ss\n".        co
+000049f0: 6e74 656e 7473 5f73 7063 203d 2022 6966  ntents_spc = "if
+00004a00: 2031 3a5c 6e20 2020 2069 6620 323a 5c6e   1:\n    if 2:\n
+00004a10: 2020 2020 2020 2020 7061 7373 5c6e 2020          pass\n  
+00004a20: 2020 2320 636f 6d6d 656e 745c 6e20 2020    # comment\n   
+00004a30: 2070 6173 735c 6e22 0a20 2020 2020 2020   pass\n".       
+00004a40: 2073 656c 662e 6173 7365 7274 466f 726d   self.assertForm
+00004a50: 6174 4571 7561 6c28 636f 6e74 656e 7473  atEqual(contents
+00004a60: 5f73 7063 2c20 6673 2863 6f6e 7465 6e74  _spc, fs(content
+00004a70: 735f 7370 6329 290a 2020 2020 2020 2020  s_spc)).        
+00004a80: 7365 6c66 2e61 7373 6572 7446 6f72 6d61  self.assertForma
+00004a90: 7445 7175 616c 2863 6f6e 7465 6e74 735f  tEqual(contents_
+00004aa0: 7370 632c 2066 7328 636f 6e74 656e 7473  spc, fs(contents
+00004ab0: 5f74 6162 2929 0a0a 2020 2020 2020 2020  _tab))..        
+00004ac0: 636f 6e74 656e 7473 5f74 6162 203d 2022  contents_tab = "
+00004ad0: 6966 2031 3a5c 6e20 2020 2020 2020 2069  if 1:\n        i
+00004ae0: 6620 323a 5c6e 5c74 5c74 7061 7373 5c6e  f 2:\n\t\tpass\n
+00004af0: 5c74 5c74 2320 636f 6d6d 656e 745c 6e20  \t\t# comment\n 
+00004b00: 2020 2020 2020 2070 6173 735c 6e22 0a20         pass\n". 
+00004b10: 2020 2020 2020 2063 6f6e 7465 6e74 735f         contents_
+00004b20: 7370 6320 3d20 2269 6620 313a 5c6e 2020  spc = "if 1:\n  
+00004b30: 2020 6966 2032 3a5c 6e20 2020 2020 2020    if 2:\n       
+00004b40: 2070 6173 735c 6e20 2020 2020 2020 2023   pass\n        #
+00004b50: 2063 6f6d 6d65 6e74 5c6e 2020 2020 7061   comment\n    pa
+00004b60: 7373 5c6e 220a 2020 2020 2020 2020 7365  ss\n".        se
+00004b70: 6c66 2e61 7373 6572 7446 6f72 6d61 7445  lf.assertFormatE
+00004b80: 7175 616c 2863 6f6e 7465 6e74 735f 7370  qual(contents_sp
+00004b90: 632c 2066 7328 636f 6e74 656e 7473 5f73  c, fs(contents_s
+00004ba0: 7063 2929 0a20 2020 2020 2020 2073 656c  pc)).        sel
+00004bb0: 662e 6173 7365 7274 466f 726d 6174 4571  f.assertFormatEq
+00004bc0: 7561 6c28 636f 6e74 656e 7473 5f73 7063  ual(contents_spc
+00004bd0: 2c20 6673 2863 6f6e 7465 6e74 735f 7461  , fs(contents_ta
+00004be0: 6229 290a 0a20 2020 2064 6566 2074 6573  b))..    def tes
+00004bf0: 745f 6661 6c73 655f 706f 7369 7469 7665  t_false_positive
+00004c00: 5f73 796d 6c69 6e6b 5f6f 7574 7075 745f  _symlink_output_
+00004c10: 6973 7375 655f 3333 3834 2873 656c 6629  issue_3384(self)
+00004c20: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00004c30: 2020 2320 456d 756c 6174 6520 7468 6520    # Emulate the 
+00004c40: 6265 6861 7669 6f72 2077 6865 6e20 7573  behavior when us
+00004c50: 696e 6720 7468 6520 434c 4920 2860 6365  ing the CLI (`ce
+00004c60: 7263 6973 202e 2f63 6869 6c64 2020 2d2d  rcis ./child  --
+00004c70: 7665 7262 6f73 6560 292c 2077 6869 6368  verbose`), which
+00004c80: 0a20 2020 2020 2020 2023 2069 6e76 6f6c  .        # invol
+00004c90: 7665 7320 7061 7463 6869 6e67 2073 6f6d  ves patching som
+00004ca0: 6520 6070 6174 686c 6962 2e50 6174 6860  e `pathlib.Path`
+00004cb0: 206d 6574 686f 6473 2e20 496e 2070 6172   methods. In par
+00004cc0: 7469 6375 6c61 722c 2060 6973 5f64 6972  ticular, `is_dir
+00004cd0: 6020 6973 0a20 2020 2020 2020 2023 2070  ` is.        # p
+00004ce0: 6174 6368 6564 206f 6e6c 7920 6f6e 2069  atched only on i
+00004cf0: 7473 2066 6972 7374 2063 616c 6c3a 2077  ts first call: w
+00004d00: 6865 6e20 6368 6563 6b69 6e67 2069 6620  hen checking if 
+00004d10: 222e 2f63 6869 6c64 2220 6973 2061 2064  "./child" is a d
+00004d20: 6972 6563 746f 7279 2069 740a 2020 2020  irectory it.    
+00004d30: 2020 2020 2320 7368 6f75 6c64 2072 6574      # should ret
+00004d40: 7572 6e20 5472 7565 2e20 5468 6520 222e  urn True. The ".
+00004d50: 2f63 6869 6c64 2220 666f 6c64 6572 2065  /child" folder e
+00004d60: 7869 7374 7320 7265 6c61 7469 7665 2074  xists relative t
+00004d70: 6f20 7468 6520 6377 6420 7768 656e 0a20  o the cwd when. 
+00004d80: 2020 2020 2020 2023 2072 756e 6e69 6e67         # running
+00004d90: 2066 726f 6d20 434c 492c 2062 7574 2066   from CLI, but f
+00004da0: 6169 6c73 2077 6865 6e20 7275 6e6e 696e  ails when runnin
+00004db0: 6720 7468 6520 7465 7374 7320 6265 6361  g the tests beca
+00004dc0: 7573 6520 6377 6420 6973 2064 6966 6665  use cwd is diffe
+00004dd0: 7265 6e74 0a20 2020 2020 2020 2070 726f  rent.        pro
+00004de0: 6a65 6374 5f72 6f6f 7420 3d20 5061 7468  ject_root = Path
+00004df0: 2854 4849 535f 4449 5220 2f20 2264 6174  (THIS_DIR / "dat
+00004e00: 6122 202f 2022 6e65 7374 6564 5f67 6974  a" / "nested_git
+00004e10: 6967 6e6f 7265 5f74 6573 7473 2229 0a20  ignore_tests"). 
+00004e20: 2020 2020 2020 2077 6f72 6b69 6e67 5f64         working_d
+00004e30: 6972 6563 746f 7279 203d 2070 726f 6a65  irectory = proje
+00004e40: 6374 5f72 6f6f 7420 2f20 2272 6f6f 7422  ct_root / "root"
+00004e50: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
+00004e60: 6162 7370 6174 6820 3d20 776f 726b 696e  abspath = workin
+00004e70: 675f 6469 7265 6374 6f72 7920 2f20 2263  g_directory / "c
+00004e80: 6869 6c64 220a 2020 2020 2020 2020 7461  hild".        ta
+00004e90: 7267 6574 5f63 6f6e 7465 6e74 7320 3d20  rget_contents = 
+00004ea0: 280a 2020 2020 2020 2020 2020 2020 7372  (.            sr
+00004eb0: 632e 7265 6c61 7469 7665 5f74 6f28 776f  c.relative_to(wo
+00004ec0: 726b 696e 675f 6469 7265 6374 6f72 7929  rking_directory)
+00004ed0: 2066 6f72 2073 7263 2069 6e20 7461 7267   for src in targ
+00004ee0: 6574 5f61 6273 7061 7468 2e69 7465 7264  et_abspath.iterd
+00004ef0: 6972 2829 0a20 2020 2020 2020 2029 0a0a  ir().        )..
+00004f00: 2020 2020 2020 2020 6465 6620 6d6f 636b          def mock
+00004f10: 5f6e 5f63 616c 6c73 2872 6573 706f 6e73  _n_calls(respons
+00004f20: 6573 3a20 4c69 7374 5b62 6f6f 6c5d 2920  es: List[bool]) 
+00004f30: 2d3e 2043 616c 6c61 626c 655b 5b5d 2c20  -> Callable[[], 
+00004f40: 626f 6f6c 5d3a 0a20 2020 2020 2020 2020  bool]:.         
+00004f50: 2020 2064 6566 205f 6d6f 636b 6564 5f63     def _mocked_c
+00004f60: 616c 6c73 2829 202d 3e20 626f 6f6c 3a0a  alls() -> bool:.
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 6966 2072 6573 706f 6e73 6573 3a0a 2020  if responses:.  
+00004f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fa0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00004fb0: 6573 2e70 6f70 2830 290a 2020 2020 2020  es.pop(0).      
+00004fc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00004fd0: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+00004fe0: 2020 2020 7265 7475 726e 205f 6d6f 636b      return _mock
+00004ff0: 6564 5f63 616c 6c73 0a0a 2020 2020 2020  ed_calls..      
+00005000: 2020 7769 7468 2070 6174 6368 2822 7061    with patch("pa
+00005010: 7468 6c69 622e 5061 7468 2e69 7465 7264  thlib.Path.iterd
+00005020: 6972 222c 2072 6574 7572 6e5f 7661 6c75  ir", return_valu
+00005030: 653d 7461 7267 6574 5f63 6f6e 7465 6e74  e=target_content
+00005040: 7329 2c20 7061 7463 6828 0a20 2020 2020  s), patch(.     
+00005050: 2020 2020 2020 2022 7061 7468 6c69 622e         "pathlib.
+00005060: 5061 7468 2e63 7764 222c 2072 6574 7572  Path.cwd", retur
+00005070: 6e5f 7661 6c75 653d 776f 726b 696e 675f  n_value=working_
+00005080: 6469 7265 6374 6f72 790a 2020 2020 2020  directory.      
+00005090: 2020 292c 2070 6174 6368 2822 7061 7468    ), patch("path
+000050a0: 6c69 622e 5061 7468 2e69 735f 6469 7222  lib.Path.is_dir"
+000050b0: 2c20 7369 6465 5f65 6666 6563 743d 6d6f  , side_effect=mo
+000050c0: 636b 5f6e 5f63 616c 6c73 285b 5472 7565  ck_n_calls([True
+000050d0: 5d29 293a 0a20 2020 2020 2020 2020 2020  ])):.           
+000050e0: 2063 7478 203d 2046 616b 6543 6f6e 7465   ctx = FakeConte
+000050f0: 7874 2829 0a20 2020 2020 2020 2020 2020  xt().           
+00005100: 2063 7478 2e6f 626a 5b22 726f 6f74 225d   ctx.obj["root"]
+00005110: 203d 2070 726f 6a65 6374 5f72 6f6f 740a   = project_root.
+00005120: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00005130: 7274 203d 204d 6167 6963 4d6f 636b 2876  rt = MagicMock(v
+00005140: 6572 626f 7365 3d54 7275 6529 0a20 2020  erbose=True).   
+00005150: 2020 2020 2020 2020 2063 6572 6369 732e           cercis.
+00005160: 6765 745f 736f 7572 6365 7328 0a20 2020  get_sources(.   
+00005170: 2020 2020 2020 2020 2020 2020 2063 7478               ctx
+00005180: 3d63 7478 2c0a 2020 2020 2020 2020 2020  =ctx,.          
+00005190: 2020 2020 2020 7372 633d 2822 2e2f 6368        src=("./ch
+000051a0: 696c 6422 2c29 2c0a 2020 2020 2020 2020  ild",),.        
+000051b0: 2020 2020 2020 2020 7175 6965 743d 4661          quiet=Fa
+000051c0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000051d0: 2020 2020 2076 6572 626f 7365 3d54 7275       verbose=Tru
+000051e0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000051f0: 2020 2069 6e63 6c75 6465 3d44 4546 4155     include=DEFAU
+00005200: 4c54 5f49 4e43 4c55 4445 2c0a 2020 2020  LT_INCLUDE,.    
+00005210: 2020 2020 2020 2020 2020 2020 6578 636c              excl
+00005220: 7564 653d 4e6f 6e65 2c0a 2020 2020 2020  ude=None,.      
+00005230: 2020 2020 2020 2020 2020 7265 706f 7274            report
+00005240: 3d72 6570 6f72 742c 0a20 2020 2020 2020  =report,.       
+00005250: 2020 2020 2020 2020 2065 7874 656e 645f           extend_
+00005260: 6578 636c 7564 653d 4e6f 6e65 2c0a 2020  exclude=None,.  
+00005270: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00005280: 7263 655f 6578 636c 7564 653d 4e6f 6e65  rce_exclude=None
+00005290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000052a0: 2020 7374 6469 6e5f 6669 6c65 6e61 6d65    stdin_filename
+000052b0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+000052c0: 2020 2029 0a20 2020 2020 2020 2061 7373     ).        ass
+000052d0: 6572 7420 6e6f 7420 616e 7928 0a20 2020  ert not any(.   
+000052e0: 2020 2020 2020 2020 206d 6f63 6b5f 6172           mock_ar
+000052f0: 6773 5b31 5d2e 7374 6172 7473 7769 7468  gs[1].startswith
+00005300: 2822 6973 2061 2073 796d 626f 6c69 6320  ("is a symbolic 
+00005310: 6c69 6e6b 2074 6861 7420 706f 696e 7473  link that points
+00005320: 206f 7574 7369 6465 2229 0a20 2020 2020   outside").     
+00005330: 2020 2020 2020 2066 6f72 205f 2c20 6d6f         for _, mo
+00005340: 636b 5f61 7267 732c 205f 2069 6e20 7265  ck_args, _ in re
+00005350: 706f 7274 2e70 6174 685f 6967 6e6f 7265  port.path_ignore
+00005360: 642e 6d6f 636b 5f63 616c 6c73 0a20 2020  d.mock_calls.   
+00005370: 2020 2020 2029 2c20 2241 2073 796d 626f       ), "A symbo
+00005380: 6c69 6320 6c69 6e6b 2077 6173 2072 6570  lic link was rep
+00005390: 6f72 7465 642e 220a 2020 2020 2020 2020  orted.".        
+000053a0: 7265 706f 7274 2e70 6174 685f 6967 6e6f  report.path_igno
+000053b0: 7265 642e 6173 7365 7274 5f63 616c 6c65  red.assert_calle
+000053c0: 645f 6f6e 6365 5f77 6974 6828 0a20 2020  d_once_with(.   
+000053d0: 2020 2020 2020 2020 2050 6174 6828 2263           Path("c
+000053e0: 6869 6c64 222c 2022 622e 7079 2229 2c20  hild", "b.py"), 
+000053f0: 226d 6174 6368 6573 2061 202e 6769 7469  "matches a .giti
+00005400: 676e 6f72 6520 6669 6c65 2063 6f6e 7465  gnore file conte
+00005410: 6e74 220a 2020 2020 2020 2020 290a 0a20  nt".        ).. 
+00005420: 2020 2064 6566 2074 6573 745f 7265 706f     def test_repo
+00005430: 7274 5f76 6572 626f 7365 2873 656c 6629  rt_verbose(self)
+00005440: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00005450: 2020 7265 706f 7274 203d 2052 6570 6f72    report = Repor
+00005460: 7428 7665 7262 6f73 653d 5472 7565 290a  t(verbose=True).
+00005470: 2020 2020 2020 2020 6f75 745f 6c69 6e65          out_line
+00005480: 7320 3d20 5b5d 0a20 2020 2020 2020 2065  s = [].        e
+00005490: 7272 5f6c 696e 6573 203d 205b 5d0a 0a20  rr_lines = [].. 
+000054a0: 2020 2020 2020 2064 6566 206f 7574 286d         def out(m
+000054b0: 7367 3a20 7374 722c 202a 2a6b 7761 7267  sg: str, **kwarg
+000054c0: 733a 2041 6e79 2920 2d3e 204e 6f6e 653a  s: Any) -> None:
+000054d0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000054e0: 5f6c 696e 6573 2e61 7070 656e 6428 6d73  _lines.append(ms
+000054f0: 6729 0a0a 2020 2020 2020 2020 6465 6620  g)..        def 
+00005500: 6572 7228 6d73 673a 2073 7472 2c20 2a2a  err(msg: str, **
+00005510: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
+00005520: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00005530: 2020 6572 725f 6c69 6e65 732e 6170 7065    err_lines.appe
+00005540: 6e64 286d 7367 290a 0a20 2020 2020 2020  nd(msg)..       
+00005550: 2077 6974 6820 7061 7463 6828 2263 6572   with patch("cer
+00005560: 6369 732e 6f75 7470 7574 2e5f 6f75 7422  cis.output._out"
+00005570: 2c20 6f75 7429 2c20 7061 7463 6828 2263  , out), patch("c
+00005580: 6572 6369 732e 6f75 7470 7574 2e5f 6572  ercis.output._er
+00005590: 7222 2c20 6572 7229 3a0a 2020 2020 2020  r", err):.      
+000055a0: 2020 2020 2020 7265 706f 7274 2e64 6f6e        report.don
+000055b0: 6528 5061 7468 2822 6631 2229 2c20 6365  e(Path("f1"), ce
+000055c0: 7263 6973 2e43 6861 6e67 6564 2e4e 4f29  rcis.Changed.NO)
+000055d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000055e0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+000055f0: 6e28 6f75 745f 6c69 6e65 7329 2c20 3129  n(out_lines), 1)
+00005600: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005610: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00005620: 6e28 6572 725f 6c69 6e65 7329 2c20 3029  n(err_lines), 0)
+00005630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005640: 662e 6173 7365 7274 4571 7561 6c28 6f75  f.assertEqual(ou
+00005650: 745f 6c69 6e65 735b 2d31 5d2c 2022 6631  t_lines[-1], "f1
+00005660: 2061 6c72 6561 6479 2077 656c 6c20 666f   already well fo
+00005670: 726d 6174 7465 642c 2067 6f6f 6420 6a6f  rmatted, good jo
+00005680: 622e 2229 0a20 2020 2020 2020 2020 2020  b.").           
+00005690: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000056a0: 6c28 756e 7374 796c 6528 7374 7228 7265  l(unstyle(str(re
+000056b0: 706f 7274 2929 2c20 2231 2066 696c 6520  port)), "1 file 
+000056c0: 6c65 6674 2075 6e63 6861 6e67 6564 2e22  left unchanged."
+000056d0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000056e0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+000056f0: 6570 6f72 742e 7265 7475 726e 5f63 6f64  eport.return_cod
+00005700: 652c 2030 290a 2020 2020 2020 2020 2020  e, 0).          
+00005710: 2020 7265 706f 7274 2e64 6f6e 6528 5061    report.done(Pa
+00005720: 7468 2822 6632 2229 2c20 6365 7263 6973  th("f2"), cercis
+00005730: 2e43 6861 6e67 6564 2e59 4553 290a 2020  .Changed.YES).  
+00005740: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00005750: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+00005760: 7574 5f6c 696e 6573 292c 2032 290a 2020  ut_lines), 2).  
+00005770: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00005780: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+00005790: 7272 5f6c 696e 6573 292c 2030 290a 2020  rr_lines), 0).  
+000057a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000057b0: 7373 6572 7445 7175 616c 286f 7574 5f6c  ssertEqual(out_l
+000057c0: 696e 6573 5b2d 315d 2c20 2272 6566 6f72  ines[-1], "refor
+000057d0: 6d61 7474 6564 2066 3222 290a 2020 2020  matted f2").    
+000057e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000057f0: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00005800: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
+00005810: 6528 7374 7228 7265 706f 7274 2929 2c20  e(str(report)), 
+00005820: 2231 2066 696c 6520 7265 666f 726d 6174  "1 file reformat
+00005830: 7465 642c 2031 2066 696c 6520 6c65 6674  ted, 1 file left
+00005840: 2075 6e63 6861 6e67 6564 2e22 0a20 2020   unchanged.".   
+00005850: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00005860: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
+00005870: 6e65 2850 6174 6828 2266 3322 292c 2063  ne(Path("f3"), c
+00005880: 6572 6369 732e 4368 616e 6765 642e 4341  ercis.Changed.CA
+00005890: 4348 4544 290a 2020 2020 2020 2020 2020  CHED).          
+000058a0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000058b0: 616c 286c 656e 286f 7574 5f6c 696e 6573  al(len(out_lines
+000058c0: 292c 2033 290a 2020 2020 2020 2020 2020  ), 3).          
+000058d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000058e0: 616c 286c 656e 2865 7272 5f6c 696e 6573  al(len(err_lines
+000058f0: 292c 2030 290a 2020 2020 2020 2020 2020  ), 0).          
+00005900: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00005910: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00005920: 2020 2020 6f75 745f 6c69 6e65 735b 2d31      out_lines[-1
+00005930: 5d2c 2022 6633 2077 6173 6e27 7420 6d6f  ], "f3 wasn't mo
+00005940: 6469 6669 6564 206f 6e20 6469 736b 2073  dified on disk s
+00005950: 696e 6365 206c 6173 7420 7275 6e2e 220a  ince last run.".
+00005960: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00005970: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00005980: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00005990: 2020 2020 2020 2020 2020 2020 756e 7374              unst
+000059a0: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
+000059b0: 2c20 2231 2066 696c 6520 7265 666f 726d  , "1 file reform
+000059c0: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
+000059d0: 6566 7420 756e 6368 616e 6765 642e 220a  eft unchanged.".
+000059e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000059f0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00005a00: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
+00005a10: 742e 7265 7475 726e 5f63 6f64 652c 2030  t.return_code, 0
+00005a20: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00005a30: 706f 7274 2e63 6865 636b 203d 2054 7275  port.check = Tru
+00005a40: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00005a50: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00005a60: 6570 6f72 742e 7265 7475 726e 5f63 6f64  eport.return_cod
+00005a70: 652c 2031 290a 2020 2020 2020 2020 2020  e, 1).          
+00005a80: 2020 7265 706f 7274 2e63 6865 636b 203d    report.check =
+00005a90: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00005aa0: 2020 2072 6570 6f72 742e 6661 696c 6564     report.failed
+00005ab0: 2850 6174 6828 2265 3122 292c 2022 626f  (Path("e1"), "bo
+00005ac0: 6f6d 2229 0a20 2020 2020 2020 2020 2020  om").           
+00005ad0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00005ae0: 6c28 6c65 6e28 6f75 745f 6c69 6e65 7329  l(len(out_lines)
+00005af0: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
+00005b00: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00005b10: 6c28 6c65 6e28 6572 725f 6c69 6e65 7329  l(len(err_lines)
+00005b20: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
+00005b30: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00005b40: 6c28 6572 725f 6c69 6e65 735b 2d31 5d2c  l(err_lines[-1],
+00005b50: 2022 6572 726f 723a 2063 616e 6e6f 7420   "error: cannot 
+00005b60: 666f 726d 6174 2065 313a 2062 6f6f 6d22  format e1: boom"
+00005b70: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00005b80: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ba0: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
+00005bb0: 7274 2929 2c0a 2020 2020 2020 2020 2020  rt)),.          
+00005bc0: 2020 2020 2020 2231 2066 696c 6520 7265        "1 file re
+00005bd0: 666f 726d 6174 7465 642c 2032 2066 696c  formatted, 2 fil
+00005be0: 6573 206c 6566 7420 756e 6368 616e 6765  es left unchange
+00005bf0: 642c 2031 2066 696c 6520 6661 696c 6564  d, 1 file failed
+00005c00: 2074 6f22 0a20 2020 2020 2020 2020 2020   to".           
+00005c10: 2020 2020 2022 2072 6566 6f72 6d61 742e       " reformat.
+00005c20: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00005c30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005c40: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00005c50: 706f 7274 2e72 6574 7572 6e5f 636f 6465  port.return_code
+00005c60: 2c20 3132 3329 0a20 2020 2020 2020 2020  , 123).         
+00005c70: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
+00005c80: 6174 6828 2266 3322 292c 2063 6572 6369  ath("f3"), cerci
+00005c90: 732e 4368 616e 6765 642e 5945 5329 0a20  s.Changed.YES). 
+00005ca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005cb0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+00005cc0: 6f75 745f 6c69 6e65 7329 2c20 3429 0a20  out_lines), 4). 
+00005cd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005ce0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+00005cf0: 6572 725f 6c69 6e65 7329 2c20 3129 0a20  err_lines), 1). 
+00005d00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005d10: 6173 7365 7274 4571 7561 6c28 6f75 745f  assertEqual(out_
+00005d20: 6c69 6e65 735b 2d31 5d2c 2022 7265 666f  lines[-1], "refo
+00005d30: 726d 6174 7465 6420 6633 2229 0a20 2020  rmatted f3").   
+00005d40: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00005d50: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+00005d60: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
+00005d70: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
+00005d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d90: 2022 3220 6669 6c65 7320 7265 666f 726d   "2 files reform
+00005da0: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
+00005db0: 6566 7420 756e 6368 616e 6765 642c 2031  eft unchanged, 1
+00005dc0: 2066 696c 6520 6661 696c 6564 2074 6f22   file failed to"
+00005dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005de0: 2022 2072 6566 6f72 6d61 742e 222c 0a20   " reformat.",. 
+00005df0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00005e00: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00005e10: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
+00005e20: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
+00005e30: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
+00005e40: 6570 6f72 742e 6661 696c 6564 2850 6174  eport.failed(Pat
+00005e50: 6828 2265 3222 292c 2022 626f 6f6d 2229  h("e2"), "boom")
+00005e60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005e70: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00005e80: 6e28 6f75 745f 6c69 6e65 7329 2c20 3429  n(out_lines), 4)
+00005e90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005ea0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00005eb0: 6e28 6572 725f 6c69 6e65 7329 2c20 3229  n(err_lines), 2)
+00005ec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005ed0: 662e 6173 7365 7274 4571 7561 6c28 6572  f.assertEqual(er
+00005ee0: 725f 6c69 6e65 735b 2d31 5d2c 2022 6572  r_lines[-1], "er
+00005ef0: 726f 723a 2063 616e 6e6f 7420 666f 726d  ror: cannot form
+00005f00: 6174 2065 323a 2062 6f6f 6d22 290a 2020  at e2: boom").  
+00005f10: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00005f20: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00005f30: 2020 2020 2020 2020 2020 2020 756e 7374              unst
+00005f40: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
+00005f50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005f60: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
+00005f70: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
+00005f80: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
+00005f90: 3220 6669 6c65 7320 6661 696c 6564 2074  2 files failed t
+00005fa0: 6f22 0a20 2020 2020 2020 2020 2020 2020  o".             
+00005fb0: 2020 2022 2072 6566 6f72 6d61 742e 222c     " reformat.",
+00005fc0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00005fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005fe0: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
+00005ff0: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
+00006000: 3132 3329 0a20 2020 2020 2020 2020 2020  123).           
+00006010: 2072 6570 6f72 742e 7061 7468 5f69 676e   report.path_ign
+00006020: 6f72 6564 2850 6174 6828 2277 6174 2229  ored(Path("wat")
+00006030: 2c20 226e 6f20 6d61 7463 6822 290a 2020  , "no match").  
+00006040: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006050: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+00006060: 7574 5f6c 696e 6573 292c 2035 290a 2020  ut_lines), 5).  
+00006070: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006080: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+00006090: 7272 5f6c 696e 6573 292c 2032 290a 2020  rr_lines), 2).  
+000060a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000060b0: 7373 6572 7445 7175 616c 286f 7574 5f6c  ssertEqual(out_l
+000060c0: 696e 6573 5b2d 315d 2c20 2277 6174 2069  ines[-1], "wat i
+000060d0: 676e 6f72 6564 3a20 6e6f 206d 6174 6368  gnored: no match
+000060e0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+000060f0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00006100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006110: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
+00006120: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
+00006130: 2020 2020 2020 2022 3220 6669 6c65 7320         "2 files 
+00006140: 7265 666f 726d 6174 7465 642c 2032 2066  reformatted, 2 f
+00006150: 696c 6573 206c 6566 7420 756e 6368 616e  iles left unchan
+00006160: 6765 642c 2032 2066 696c 6573 2066 6169  ged, 2 files fai
+00006170: 6c65 6420 746f 220a 2020 2020 2020 2020  led to".        
+00006180: 2020 2020 2020 2020 2220 7265 666f 726d          " reform
+00006190: 6174 2e22 2c0a 2020 2020 2020 2020 2020  at.",.          
+000061a0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000061b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000061c0: 2872 6570 6f72 742e 7265 7475 726e 5f63  (report.return_c
+000061d0: 6f64 652c 2031 3233 290a 2020 2020 2020  ode, 123).      
+000061e0: 2020 2020 2020 7265 706f 7274 2e64 6f6e        report.don
+000061f0: 6528 5061 7468 2822 6634 2229 2c20 6365  e(Path("f4"), ce
+00006200: 7263 6973 2e43 6861 6e67 6564 2e4e 4f29  rcis.Changed.NO)
+00006210: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006220: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00006230: 6e28 6f75 745f 6c69 6e65 7329 2c20 3629  n(out_lines), 6)
+00006240: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006250: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00006260: 6e28 6572 725f 6c69 6e65 7329 2c20 3229  n(err_lines), 2)
+00006270: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006280: 662e 6173 7365 7274 4571 7561 6c28 6f75  f.assertEqual(ou
+00006290: 745f 6c69 6e65 735b 2d31 5d2c 2022 6634  t_lines[-1], "f4
+000062a0: 2061 6c72 6561 6479 2077 656c 6c20 666f   already well fo
+000062b0: 726d 6174 7465 642c 2067 6f6f 6420 6a6f  rmatted, good jo
+000062c0: 622e 2229 0a20 2020 2020 2020 2020 2020  b.").           
+000062d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000062e0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+000062f0: 2020 2075 6e73 7479 6c65 2873 7472 2872     unstyle(str(r
+00006300: 6570 6f72 7429 292c 0a20 2020 2020 2020  eport)),.       
+00006310: 2020 2020 2020 2020 2022 3220 6669 6c65           "2 file
+00006320: 7320 7265 666f 726d 6174 7465 642c 2033  s reformatted, 3
+00006330: 2066 696c 6573 206c 6566 7420 756e 6368   files left unch
+00006340: 616e 6765 642c 2032 2066 696c 6573 2066  anged, 2 files f
+00006350: 6169 6c65 6420 746f 220a 2020 2020 2020  ailed to".      
+00006360: 2020 2020 2020 2020 2020 2220 7265 666f            " refo
+00006370: 726d 6174 2e22 2c0a 2020 2020 2020 2020  rmat.",.        
+00006380: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00006390: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000063a0: 616c 2872 6570 6f72 742e 7265 7475 726e  al(report.return
+000063b0: 5f63 6f64 652c 2031 3233 290a 2020 2020  _code, 123).    
+000063c0: 2020 2020 2020 2020 7265 706f 7274 2e63          report.c
+000063d0: 6865 636b 203d 2054 7275 650a 2020 2020  heck = True.    
+000063e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000063f0: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00006400: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
+00006410: 6528 7374 7228 7265 706f 7274 2929 2c0a  e(str(report)),.
+00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006430: 2232 2066 696c 6573 2077 6f75 6c64 2062  "2 files would b
+00006440: 6520 7265 666f 726d 6174 7465 642c 2033  e reformatted, 3
+00006450: 2066 696c 6573 2077 6f75 6c64 2062 6520   files would be 
+00006460: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
+00006470: 3222 0a20 2020 2020 2020 2020 2020 2020  2".             
+00006480: 2020 2022 2066 696c 6573 2077 6f75 6c64     " files would
+00006490: 2066 6169 6c20 746f 2072 6566 6f72 6d61   fail to reforma
+000064a0: 742e 222c 0a20 2020 2020 2020 2020 2020  t.",.           
+000064b0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+000064c0: 6570 6f72 742e 6368 6563 6b20 3d20 4661  eport.check = Fa
+000064d0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+000064e0: 7265 706f 7274 2e64 6966 6620 3d20 5472  report.diff = Tr
+000064f0: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
+00006500: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00006510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006520: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
+00006530: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
+00006540: 2020 2020 2020 2022 3220 6669 6c65 7320         "2 files 
+00006550: 776f 756c 6420 6265 2072 6566 6f72 6d61  would be reforma
+00006560: 7474 6564 2c20 3320 6669 6c65 7320 776f  tted, 3 files wo
+00006570: 756c 6420 6265 206c 6566 7420 756e 6368  uld be left unch
+00006580: 616e 6765 642c 2032 220a 2020 2020 2020  anged, 2".      
+00006590: 2020 2020 2020 2020 2020 2220 6669 6c65            " file
+000065a0: 7320 776f 756c 6420 6661 696c 2074 6f20  s would fail to 
+000065b0: 7265 666f 726d 6174 2e22 2c0a 2020 2020  reformat.",.    
+000065c0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+000065d0: 6566 2074 6573 745f 7265 706f 7274 5f71  ef test_report_q
+000065e0: 7569 6574 2873 656c 6629 202d 3e20 4e6f  uiet(self) -> No
+000065f0: 6e65 3a0a 2020 2020 2020 2020 7265 706f  ne:.        repo
+00006600: 7274 203d 2052 6570 6f72 7428 7175 6965  rt = Report(quie
+00006610: 743d 5472 7565 290a 2020 2020 2020 2020  t=True).        
+00006620: 6f75 745f 6c69 6e65 7320 3d20 5b5d 0a20  out_lines = []. 
+00006630: 2020 2020 2020 2065 7272 5f6c 696e 6573         err_lines
+00006640: 203d 205b 5d0a 0a20 2020 2020 2020 2064   = []..        d
+00006650: 6566 206f 7574 286d 7367 3a20 7374 722c  ef out(msg: str,
+00006660: 202a 2a6b 7761 7267 733a 2041 6e79 2920   **kwargs: Any) 
+00006670: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00006680: 2020 2020 206f 7574 5f6c 696e 6573 2e61       out_lines.a
+00006690: 7070 656e 6428 6d73 6729 0a0a 2020 2020  ppend(msg)..    
+000066a0: 2020 2020 6465 6620 6572 7228 6d73 673a      def err(msg:
+000066b0: 2073 7472 2c20 2a2a 6b77 6172 6773 3a20   str, **kwargs: 
+000066c0: 416e 7929 202d 3e20 4e6f 6e65 3a0a 2020  Any) -> None:.  
+000066d0: 2020 2020 2020 2020 2020 6572 725f 6c69            err_li
+000066e0: 6e65 732e 6170 7065 6e64 286d 7367 290a  nes.append(msg).
+000066f0: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
+00006700: 7463 6828 2263 6572 6369 732e 6f75 7470  tch("cercis.outp
+00006710: 7574 2e5f 6f75 7422 2c20 6f75 7429 2c20  ut._out", out), 
+00006720: 7061 7463 6828 2263 6572 6369 732e 6f75  patch("cercis.ou
+00006730: 7470 7574 2e5f 6572 7222 2c20 6572 7229  tput._err", err)
+00006740: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00006750: 706f 7274 2e64 6f6e 6528 5061 7468 2822  port.done(Path("
+00006760: 6631 2229 2c20 6365 7263 6973 2e43 6861  f1"), cercis.Cha
+00006770: 6e67 6564 2e4e 4f29 0a20 2020 2020 2020  nged.NO).       
+00006780: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00006790: 4571 7561 6c28 6c65 6e28 6f75 745f 6c69  Equal(len(out_li
+000067a0: 6e65 7329 2c20 3029 0a20 2020 2020 2020  nes), 0).       
+000067b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000067c0: 4571 7561 6c28 6c65 6e28 6572 725f 6c69  Equal(len(err_li
+000067d0: 6e65 7329 2c20 3029 0a20 2020 2020 2020  nes), 0).       
+000067e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000067f0: 4571 7561 6c28 756e 7374 796c 6528 7374  Equal(unstyle(st
+00006800: 7228 7265 706f 7274 2929 2c20 2231 2066  r(report)), "1 f
+00006810: 696c 6520 6c65 6674 2075 6e63 6861 6e67  ile left unchang
+00006820: 6564 2e22 290a 2020 2020 2020 2020 2020  ed.").          
+00006830: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00006840: 616c 2872 6570 6f72 742e 7265 7475 726e  al(report.return
+00006850: 5f63 6f64 652c 2030 290a 2020 2020 2020  _code, 0).      
+00006860: 2020 2020 2020 7265 706f 7274 2e64 6f6e        report.don
+00006870: 6528 5061 7468 2822 6632 2229 2c20 6365  e(Path("f2"), ce
+00006880: 7263 6973 2e43 6861 6e67 6564 2e59 4553  rcis.Changed.YES
+00006890: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000068a0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+000068b0: 656e 286f 7574 5f6c 696e 6573 292c 2030  en(out_lines), 0
+000068c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000068d0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+000068e0: 656e 2865 7272 5f6c 696e 6573 292c 2030  en(err_lines), 0
+000068f0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00006900: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006920: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
+00006930: 7274 2929 2c20 2231 2066 696c 6520 7265  rt)), "1 file re
+00006940: 666f 726d 6174 7465 642c 2031 2066 696c  formatted, 1 fil
+00006950: 6520 6c65 6674 2075 6e63 6861 6e67 6564  e left unchanged
+00006960: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
+00006970: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00006980: 6f72 742e 646f 6e65 2850 6174 6828 2266  ort.done(Path("f
+00006990: 3322 292c 2063 6572 6369 732e 4368 616e  3"), cercis.Chan
+000069a0: 6765 642e 4341 4348 4544 290a 2020 2020  ged.CACHED).    
+000069b0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000069c0: 6572 7445 7175 616c 286c 656e 286f 7574  ertEqual(len(out
+000069d0: 5f6c 696e 6573 292c 2030 290a 2020 2020  _lines), 0).    
+000069e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000069f0: 6572 7445 7175 616c 286c 656e 2865 7272  ertEqual(len(err
+00006a00: 5f6c 696e 6573 292c 2030 290a 2020 2020  _lines), 0).    
+00006a10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00006a20: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00006a30: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
+00006a40: 6528 7374 7228 7265 706f 7274 2929 2c20  e(str(report)), 
+00006a50: 2231 2066 696c 6520 7265 666f 726d 6174  "1 file reformat
+00006a60: 7465 642c 2032 2066 696c 6573 206c 6566  ted, 2 files lef
+00006a70: 7420 756e 6368 616e 6765 642e 220a 2020  t unchanged.".  
+00006a80: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00006a90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00006aa0: 6572 7445 7175 616c 2872 6570 6f72 742e  ertEqual(report.
+00006ab0: 7265 7475 726e 5f63 6f64 652c 2030 290a  return_code, 0).
+00006ac0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00006ad0: 7274 2e63 6865 636b 203d 2054 7275 650a  rt.check = True.
+00006ae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006af0: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
+00006b00: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
+00006b10: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00006b20: 7265 706f 7274 2e63 6865 636b 203d 2046  report.check = F
+00006b30: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00006b40: 2072 6570 6f72 742e 6661 696c 6564 2850   report.failed(P
+00006b50: 6174 6828 2265 3122 292c 2022 626f 6f6d  ath("e1"), "boom
+00006b60: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00006b70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00006b80: 6c65 6e28 6f75 745f 6c69 6e65 7329 2c20  len(out_lines), 
+00006b90: 3029 0a20 2020 2020 2020 2020 2020 2073  0).            s
+00006ba0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00006bb0: 6c65 6e28 6572 725f 6c69 6e65 7329 2c20  len(err_lines), 
+00006bc0: 3129 0a20 2020 2020 2020 2020 2020 2073  1).            s
+00006bd0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00006be0: 6572 725f 6c69 6e65 735b 2d31 5d2c 2022  err_lines[-1], "
+00006bf0: 6572 726f 723a 2063 616e 6e6f 7420 666f  error: cannot fo
+00006c00: 726d 6174 2065 313a 2062 6f6f 6d22 290a  rmat e1: boom").
+00006c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006c20: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
+00006c30: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00006c40: 7374 796c 6528 7374 7228 7265 706f 7274  style(str(report
+00006c50: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00006c60: 2020 2020 2231 2066 696c 6520 7265 666f      "1 file refo
+00006c70: 726d 6174 7465 642c 2032 2066 696c 6573  rmatted, 2 files
+00006c80: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
+00006c90: 2031 2066 696c 6520 6661 696c 6564 2074   1 file failed t
+00006ca0: 6f22 0a20 2020 2020 2020 2020 2020 2020  o".             
+00006cb0: 2020 2022 2072 6566 6f72 6d61 742e 222c     " reformat.",
+00006cc0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00006cd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006ce0: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
+00006cf0: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
+00006d00: 3132 3329 0a20 2020 2020 2020 2020 2020  123).           
+00006d10: 2072 6570 6f72 742e 646f 6e65 2850 6174   report.done(Pat
+00006d20: 6828 2266 3322 292c 2063 6572 6369 732e  h("f3"), cercis.
+00006d30: 4368 616e 6765 642e 5945 5329 0a20 2020  Changed.YES).   
+00006d40: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006d50: 7365 7274 4571 7561 6c28 6c65 6e28 6f75  sertEqual(len(ou
+00006d60: 745f 6c69 6e65 7329 2c20 3029 0a20 2020  t_lines), 0).   
+00006d70: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006d80: 7365 7274 4571 7561 6c28 6c65 6e28 6572  sertEqual(len(er
+00006d90: 725f 6c69 6e65 7329 2c20 3129 0a20 2020  r_lines), 1).   
+00006da0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006db0: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+00006dc0: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
+00006dd0: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
+00006de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006df0: 2022 3220 6669 6c65 7320 7265 666f 726d   "2 files reform
+00006e00: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
+00006e10: 6566 7420 756e 6368 616e 6765 642c 2031  eft unchanged, 1
+00006e20: 2066 696c 6520 6661 696c 6564 2074 6f22   file failed to"
+00006e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e40: 2022 2072 6566 6f72 6d61 742e 222c 0a20   " reformat.",. 
+00006e50: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006e60: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006e70: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
+00006e80: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
+00006e90: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
+00006ea0: 6570 6f72 742e 6661 696c 6564 2850 6174  eport.failed(Pat
+00006eb0: 6828 2265 3222 292c 2022 626f 6f6d 2229  h("e2"), "boom")
+00006ec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006ed0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00006ee0: 6e28 6f75 745f 6c69 6e65 7329 2c20 3029  n(out_lines), 0)
+00006ef0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006f00: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00006f10: 6e28 6572 725f 6c69 6e65 7329 2c20 3229  n(err_lines), 2)
+00006f20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006f30: 662e 6173 7365 7274 4571 7561 6c28 6572  f.assertEqual(er
+00006f40: 725f 6c69 6e65 735b 2d31 5d2c 2022 6572  r_lines[-1], "er
+00006f50: 726f 723a 2063 616e 6e6f 7420 666f 726d  ror: cannot form
+00006f60: 6174 2065 323a 2062 6f6f 6d22 290a 2020  at e2: boom").  
+00006f70: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006f80: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00006f90: 2020 2020 2020 2020 2020 2020 756e 7374              unst
+00006fa0: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
+00006fb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006fc0: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
+00006fd0: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
+00006fe0: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
+00006ff0: 3220 6669 6c65 7320 6661 696c 6564 2074  2 files failed t
+00007000: 6f22 0a20 2020 2020 2020 2020 2020 2020  o".             
+00007010: 2020 2022 2072 6566 6f72 6d61 742e 222c     " reformat.",
+00007020: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00007030: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007040: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
+00007050: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
+00007060: 3132 3329 0a20 2020 2020 2020 2020 2020  123).           
+00007070: 2072 6570 6f72 742e 7061 7468 5f69 676e   report.path_ign
+00007080: 6f72 6564 2850 6174 6828 2277 6174 2229  ored(Path("wat")
+00007090: 2c20 226e 6f20 6d61 7463 6822 290a 2020  , "no match").  
+000070a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000070b0: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+000070c0: 7574 5f6c 696e 6573 292c 2030 290a 2020  ut_lines), 0).  
+000070d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000070e0: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+000070f0: 7272 5f6c 696e 6573 292c 2032 290a 2020  rr_lines), 2).  
+00007100: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007110: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00007120: 2020 2020 2020 2020 2020 2020 756e 7374              unst
+00007130: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
+00007140: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007150: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
+00007160: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
+00007170: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
+00007180: 3220 6669 6c65 7320 6661 696c 6564 2074  2 files failed t
+00007190: 6f22 0a20 2020 2020 2020 2020 2020 2020  o".             
+000071a0: 2020 2022 2072 6566 6f72 6d61 742e 222c     " reformat.",
+000071b0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000071c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000071d0: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
+000071e0: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
+000071f0: 3132 3329 0a20 2020 2020 2020 2020 2020  123).           
+00007200: 2072 6570 6f72 742e 646f 6e65 2850 6174   report.done(Pat
+00007210: 6828 2266 3422 292c 2063 6572 6369 732e  h("f4"), cercis.
+00007220: 4368 616e 6765 642e 4e4f 290a 2020 2020  Changed.NO).    
+00007230: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00007240: 6572 7445 7175 616c 286c 656e 286f 7574  ertEqual(len(out
+00007250: 5f6c 696e 6573 292c 2030 290a 2020 2020  _lines), 0).    
+00007260: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00007270: 6572 7445 7175 616c 286c 656e 2865 7272  ertEqual(len(err
+00007280: 5f6c 696e 6573 292c 2032 290a 2020 2020  _lines), 2).    
+00007290: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000072a0: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+000072b0: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
+000072c0: 6528 7374 7228 7265 706f 7274 2929 2c0a  e(str(report)),.
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 2232 2066 696c 6573 2072 6566 6f72 6d61  "2 files reforma
+000072f0: 7474 6564 2c20 3320 6669 6c65 7320 6c65  tted, 3 files le
+00007300: 6674 2075 6e63 6861 6e67 6564 2c20 3220  ft unchanged, 2 
+00007310: 6669 6c65 7320 6661 696c 6564 2074 6f22  files failed to"
+00007320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007330: 2022 2072 6566 6f72 6d61 742e 222c 0a20   " reformat.",. 
+00007340: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00007350: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00007360: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
+00007370: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
+00007380: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
+00007390: 6570 6f72 742e 6368 6563 6b20 3d20 5472  eport.check = Tr
+000073a0: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
+000073b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000073c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000073d0: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
+000073e0: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
+000073f0: 2020 2020 2020 2022 3220 6669 6c65 7320         "2 files 
+00007400: 776f 756c 6420 6265 2072 6566 6f72 6d61  would be reforma
+00007410: 7474 6564 2c20 3320 6669 6c65 7320 776f  tted, 3 files wo
+00007420: 756c 6420 6265 206c 6566 7420 756e 6368  uld be left unch
+00007430: 616e 6765 642c 2032 220a 2020 2020 2020  anged, 2".      
+00007440: 2020 2020 2020 2020 2020 2220 6669 6c65            " file
+00007450: 7320 776f 756c 6420 6661 696c 2074 6f20  s would fail to 
+00007460: 7265 666f 726d 6174 2e22 2c0a 2020 2020  reformat.",.    
+00007470: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00007480: 2020 2020 2020 7265 706f 7274 2e63 6865        report.che
+00007490: 636b 203d 2046 616c 7365 0a20 2020 2020  ck = False.     
+000074a0: 2020 2020 2020 2072 6570 6f72 742e 6469         report.di
+000074b0: 6666 203d 2054 7275 650a 2020 2020 2020  ff = True.      
+000074c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000074d0: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+000074e0: 2020 2020 2020 2020 756e 7374 796c 6528          unstyle(
+000074f0: 7374 7228 7265 706f 7274 2929 2c0a 2020  str(report)),.  
+00007500: 2020 2020 2020 2020 2020 2020 2020 2232                "2
+00007510: 2066 696c 6573 2077 6f75 6c64 2062 6520   files would be 
+00007520: 7265 666f 726d 6174 7465 642c 2033 2066  reformatted, 3 f
+00007530: 696c 6573 2077 6f75 6c64 2062 6520 6c65  iles would be le
+00007540: 6674 2075 6e63 6861 6e67 6564 2c20 3222  ft unchanged, 2"
+00007550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007560: 2022 2066 696c 6573 2077 6f75 6c64 2066   " files would f
+00007570: 6169 6c20 746f 2072 6566 6f72 6d61 742e  ail to reformat.
+00007580: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00007590: 0a0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
+000075a0: 6570 6f72 745f 6e6f 726d 616c 2873 656c  eport_normal(sel
+000075b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+000075c0: 2020 2020 7265 706f 7274 203d 2063 6572      report = cer
+000075d0: 6369 732e 5265 706f 7274 2829 0a20 2020  cis.Report().   
+000075e0: 2020 2020 206f 7574 5f6c 696e 6573 203d       out_lines =
+000075f0: 205b 5d0a 2020 2020 2020 2020 6572 725f   [].        err_
+00007600: 6c69 6e65 7320 3d20 5b5d 0a0a 2020 2020  lines = []..    
+00007610: 2020 2020 6465 6620 6f75 7428 6d73 673a      def out(msg:
+00007620: 2073 7472 2c20 2a2a 6b77 6172 6773 3a20   str, **kwargs: 
+00007630: 416e 7929 202d 3e20 4e6f 6e65 3a0a 2020  Any) -> None:.  
+00007640: 2020 2020 2020 2020 2020 6f75 745f 6c69            out_li
+00007650: 6e65 732e 6170 7065 6e64 286d 7367 290a  nes.append(msg).
+00007660: 0a20 2020 2020 2020 2064 6566 2065 7272  .        def err
+00007670: 286d 7367 3a20 7374 722c 202a 2a6b 7761  (msg: str, **kwa
+00007680: 7267 733a 2041 6e79 2920 2d3e 204e 6f6e  rgs: Any) -> Non
+00007690: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
+000076a0: 7272 5f6c 696e 6573 2e61 7070 656e 6428  rr_lines.append(
+000076b0: 6d73 6729 0a0a 2020 2020 2020 2020 7769  msg)..        wi
+000076c0: 7468 2070 6174 6368 2822 6365 7263 6973  th patch("cercis
+000076d0: 2e6f 7574 7075 742e 5f6f 7574 222c 206f  .output._out", o
+000076e0: 7574 292c 2070 6174 6368 2822 6365 7263  ut), patch("cerc
+000076f0: 6973 2e6f 7574 7075 742e 5f65 7272 222c  is.output._err",
+00007700: 2065 7272 293a 0a20 2020 2020 2020 2020   err):.         
+00007710: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
+00007720: 6174 6828 2266 3122 292c 2063 6572 6369  ath("f1"), cerci
+00007730: 732e 4368 616e 6765 642e 4e4f 290a 2020  s.Changed.NO).  
+00007740: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007750: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+00007760: 7574 5f6c 696e 6573 292c 2030 290a 2020  ut_lines), 0).  
+00007770: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007780: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+00007790: 7272 5f6c 696e 6573 292c 2030 290a 2020  rr_lines), 0).  
+000077a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000077b0: 7373 6572 7445 7175 616c 2875 6e73 7479  ssertEqual(unsty
+000077c0: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
+000077d0: 2022 3120 6669 6c65 206c 6566 7420 756e   "1 file left un
+000077e0: 6368 616e 6765 642e 2229 0a20 2020 2020  changed.").     
+000077f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00007800: 7274 4571 7561 6c28 7265 706f 7274 2e72  rtEqual(report.r
+00007810: 6574 7572 6e5f 636f 6465 2c20 3029 0a20  eturn_code, 0). 
+00007820: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
+00007830: 742e 646f 6e65 2850 6174 6828 2266 3222  t.done(Path("f2"
+00007840: 292c 2063 6572 6369 732e 4368 616e 6765  ), cercis.Change
+00007850: 642e 5945 5329 0a20 2020 2020 2020 2020  d.YES).         
+00007860: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007870: 7561 6c28 6c65 6e28 6f75 745f 6c69 6e65  ual(len(out_line
+00007880: 7329 2c20 3129 0a20 2020 2020 2020 2020  s), 1).         
+00007890: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000078a0: 7561 6c28 6c65 6e28 6572 725f 6c69 6e65  ual(len(err_line
+000078b0: 7329 2c20 3029 0a20 2020 2020 2020 2020  s), 0).         
+000078c0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000078d0: 7561 6c28 6f75 745f 6c69 6e65 735b 2d31  ual(out_lines[-1
+000078e0: 5d2c 2022 7265 666f 726d 6174 7465 6420  ], "reformatted 
+000078f0: 6632 2229 0a20 2020 2020 2020 2020 2020  f2").           
+00007900: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00007910: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00007920: 2020 2075 6e73 7479 6c65 2873 7472 2872     unstyle(str(r
+00007930: 6570 6f72 7429 292c 2022 3120 6669 6c65  eport)), "1 file
+00007940: 2072 6566 6f72 6d61 7474 6564 2c20 3120   reformatted, 1 
+00007950: 6669 6c65 206c 6566 7420 756e 6368 616e  file left unchan
+00007960: 6765 642e 220a 2020 2020 2020 2020 2020  ged.".          
+00007970: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00007980: 7265 706f 7274 2e64 6f6e 6528 5061 7468  report.done(Path
+00007990: 2822 6633 2229 2c20 6365 7263 6973 2e43  ("f3"), cercis.C
+000079a0: 6861 6e67 6564 2e43 4143 4845 4429 0a20  hanged.CACHED). 
+000079b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000079c0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+000079d0: 6f75 745f 6c69 6e65 7329 2c20 3129 0a20  out_lines), 1). 
+000079e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000079f0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+00007a00: 6572 725f 6c69 6e65 7329 2c20 3029 0a20  err_lines), 0). 
+00007a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007a20: 6173 7365 7274 4571 7561 6c28 6f75 745f  assertEqual(out_
+00007a30: 6c69 6e65 735b 2d31 5d2c 2022 7265 666f  lines[-1], "refo
+00007a40: 726d 6174 7465 6420 6632 2229 0a20 2020  rmatted f2").   
+00007a50: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00007a60: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+00007a70: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
+00007a80: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
+00007a90: 2022 3120 6669 6c65 2072 6566 6f72 6d61   "1 file reforma
+00007aa0: 7474 6564 2c20 3220 6669 6c65 7320 6c65  tted, 2 files le
+00007ab0: 6674 2075 6e63 6861 6e67 6564 2e22 0a20  ft unchanged.". 
+00007ac0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00007ad0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00007ae0: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
+00007af0: 2e72 6574 7572 6e5f 636f 6465 2c20 3029  .return_code, 0)
+00007b00: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00007b10: 6f72 742e 6368 6563 6b20 3d20 5472 7565  ort.check = True
+00007b20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007b30: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00007b40: 706f 7274 2e72 6574 7572 6e5f 636f 6465  port.return_code
+00007b50: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
+00007b60: 2072 6570 6f72 742e 6368 6563 6b20 3d20   report.check = 
+00007b70: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00007b80: 2020 7265 706f 7274 2e66 6169 6c65 6428    report.failed(
+00007b90: 5061 7468 2822 6531 2229 2c20 2262 6f6f  Path("e1"), "boo
+00007ba0: 6d22 290a 2020 2020 2020 2020 2020 2020  m").            
+00007bb0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00007bc0: 286c 656e 286f 7574 5f6c 696e 6573 292c  (len(out_lines),
+00007bd0: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00007be0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00007bf0: 286c 656e 2865 7272 5f6c 696e 6573 292c  (len(err_lines),
+00007c00: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00007c10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00007c20: 2865 7272 5f6c 696e 6573 5b2d 315d 2c20  (err_lines[-1], 
+00007c30: 2265 7272 6f72 3a20 6361 6e6e 6f74 2066  "error: cannot f
+00007c40: 6f72 6d61 7420 6531 3a20 626f 6f6d 2229  ormat e1: boom")
+00007c50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007c60: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00007c80: 6e73 7479 6c65 2873 7472 2872 6570 6f72  nstyle(str(repor
+00007c90: 7429 292c 0a20 2020 2020 2020 2020 2020  t)),.           
+00007ca0: 2020 2020 2022 3120 6669 6c65 2072 6566       "1 file ref
+00007cb0: 6f72 6d61 7474 6564 2c20 3220 6669 6c65  ormatted, 2 file
+00007cc0: 7320 6c65 6674 2075 6e63 6861 6e67 6564  s left unchanged
+00007cd0: 2c20 3120 6669 6c65 2066 6169 6c65 6420  , 1 file failed 
+00007ce0: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
+00007cf0: 2020 2020 2220 7265 666f 726d 6174 2e22      " reformat."
+00007d00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00007d10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007d20: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
+00007d30: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
+00007d40: 2031 3233 290a 2020 2020 2020 2020 2020   123).          
+00007d50: 2020 7265 706f 7274 2e64 6f6e 6528 5061    report.done(Pa
+00007d60: 7468 2822 6633 2229 2c20 6365 7263 6973  th("f3"), cercis
+00007d70: 2e43 6861 6e67 6564 2e59 4553 290a 2020  .Changed.YES).  
+00007d80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007d90: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+00007da0: 7574 5f6c 696e 6573 292c 2032 290a 2020  ut_lines), 2).  
+00007db0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007dc0: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+00007dd0: 7272 5f6c 696e 6573 292c 2031 290a 2020  rr_lines), 1).  
+00007de0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007df0: 7373 6572 7445 7175 616c 286f 7574 5f6c  ssertEqual(out_l
+00007e00: 696e 6573 5b2d 315d 2c20 2272 6566 6f72  ines[-1], "refor
+00007e10: 6d61 7474 6564 2066 3322 290a 2020 2020  matted f3").    
+00007e20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00007e30: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00007e40: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
+00007e50: 6528 7374 7228 7265 706f 7274 2929 2c0a  e(str(report)),.
+00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e70: 2232 2066 696c 6573 2072 6566 6f72 6d61  "2 files reforma
+00007e80: 7474 6564 2c20 3220 6669 6c65 7320 6c65  tted, 2 files le
+00007e90: 6674 2075 6e63 6861 6e67 6564 2c20 3120  ft unchanged, 1 
+00007ea0: 6669 6c65 2066 6169 6c65 6420 746f 220a  file failed to".
+00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ec0: 2220 7265 666f 726d 6174 2e22 2c0a 2020  " reformat.",.  
+00007ed0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00007ee0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00007ef0: 6572 7445 7175 616c 2872 6570 6f72 742e  ertEqual(report.
+00007f00: 7265 7475 726e 5f63 6f64 652c 2031 3233  return_code, 123
+00007f10: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007f20: 706f 7274 2e66 6169 6c65 6428 5061 7468  port.failed(Path
+00007f30: 2822 6532 2229 2c20 2262 6f6f 6d22 290a  ("e2"), "boom").
+00007f40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007f50: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+00007f60: 286f 7574 5f6c 696e 6573 292c 2032 290a  (out_lines), 2).
+00007f70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007f80: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+00007f90: 2865 7272 5f6c 696e 6573 292c 2032 290a  (err_lines), 2).
+00007fa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007fb0: 2e61 7373 6572 7445 7175 616c 2865 7272  .assertEqual(err
+00007fc0: 5f6c 696e 6573 5b2d 315d 2c20 2265 7272  _lines[-1], "err
+00007fd0: 6f72 3a20 6361 6e6e 6f74 2066 6f72 6d61  or: cannot forma
+00007fe0: 7420 6532 3a20 626f 6f6d 2229 0a20 2020  t e2: boom").   
+00007ff0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00008000: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+00008010: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
+00008020: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
+00008030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008040: 2022 3220 6669 6c65 7320 7265 666f 726d   "2 files reform
+00008050: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
+00008060: 6566 7420 756e 6368 616e 6765 642c 2032  eft unchanged, 2
+00008070: 2066 696c 6573 2066 6169 6c65 6420 746f   files failed to
+00008080: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00008090: 2020 2220 7265 666f 726d 6174 2e22 2c0a    " reformat.",.
+000080a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000080b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000080c0: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
+000080d0: 742e 7265 7475 726e 5f63 6f64 652c 2031  t.return_code, 1
+000080e0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
+000080f0: 7265 706f 7274 2e70 6174 685f 6967 6e6f  report.path_igno
+00008100: 7265 6428 5061 7468 2822 7761 7422 292c  red(Path("wat"),
+00008110: 2022 6e6f 206d 6174 6368 2229 0a20 2020   "no match").   
+00008120: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00008130: 7365 7274 4571 7561 6c28 6c65 6e28 6f75  sertEqual(len(ou
+00008140: 745f 6c69 6e65 7329 2c20 3229 0a20 2020  t_lines), 2).   
+00008150: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00008160: 7365 7274 4571 7561 6c28 6c65 6e28 6572  sertEqual(len(er
+00008170: 725f 6c69 6e65 7329 2c20 3229 0a20 2020  r_lines), 2).   
+00008180: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00008190: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+000081a0: 2020 2020 2020 2020 2020 2075 6e73 7479             unsty
+000081b0: 6c65 2873 7472 2872 6570 6f72 7429 292c  le(str(report)),
+000081c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081d0: 2022 3220 6669 6c65 7320 7265 666f 726d   "2 files reform
+000081e0: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
+000081f0: 6566 7420 756e 6368 616e 6765 642c 2032  eft unchanged, 2
+00008200: 2066 696c 6573 2066 6169 6c65 6420 746f   files failed to
+00008210: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00008220: 2020 2220 7265 666f 726d 6174 2e22 2c0a    " reformat.",.
+00008230: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00008240: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00008250: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
+00008260: 742e 7265 7475 726e 5f63 6f64 652c 2031  t.return_code, 1
+00008270: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
+00008280: 7265 706f 7274 2e64 6f6e 6528 5061 7468  report.done(Path
+00008290: 2822 6634 2229 2c20 6365 7263 6973 2e43  ("f4"), cercis.C
+000082a0: 6861 6e67 6564 2e4e 4f29 0a20 2020 2020  hanged.NO).     
+000082b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000082c0: 7274 4571 7561 6c28 6c65 6e28 6f75 745f  rtEqual(len(out_
+000082d0: 6c69 6e65 7329 2c20 3229 0a20 2020 2020  lines), 2).     
+000082e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000082f0: 7274 4571 7561 6c28 6c65 6e28 6572 725f  rtEqual(len(err_
+00008300: 6c69 6e65 7329 2c20 3229 0a20 2020 2020  lines), 2).     
+00008310: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00008320: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
+00008330: 2020 2020 2020 2020 2075 6e73 7479 6c65           unstyle
+00008340: 2873 7472 2872 6570 6f72 7429 292c 0a20  (str(report)),. 
+00008350: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00008360: 3220 6669 6c65 7320 7265 666f 726d 6174  2 files reformat
+00008370: 7465 642c 2033 2066 696c 6573 206c 6566  ted, 3 files lef
+00008380: 7420 756e 6368 616e 6765 642c 2032 2066  t unchanged, 2 f
+00008390: 696c 6573 2066 6169 6c65 6420 746f 220a  iles failed to".
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 2220 7265 666f 726d 6174 2e22 2c0a 2020  " reformat.",.  
+000083c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000083d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000083e0: 6572 7445 7175 616c 2872 6570 6f72 742e  ertEqual(report.
+000083f0: 7265 7475 726e 5f63 6f64 652c 2031 3233  return_code, 123
+00008400: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00008410: 706f 7274 2e63 6865 636b 203d 2054 7275  port.check = Tru
+00008420: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00008430: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008450: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
+00008460: 7274 2929 2c0a 2020 2020 2020 2020 2020  rt)),.          
+00008470: 2020 2020 2020 2232 2066 696c 6573 2077        "2 files w
+00008480: 6f75 6c64 2062 6520 7265 666f 726d 6174  ould be reformat
+00008490: 7465 642c 2033 2066 696c 6573 2077 6f75  ted, 3 files wou
+000084a0: 6c64 2062 6520 6c65 6674 2075 6e63 6861  ld be left uncha
+000084b0: 6e67 6564 2c20 3222 0a20 2020 2020 2020  nged, 2".       
+000084c0: 2020 2020 2020 2020 2022 2066 696c 6573           " files
+000084d0: 2077 6f75 6c64 2066 6169 6c20 746f 2072   would fail to r
+000084e0: 6566 6f72 6d61 742e 222c 0a20 2020 2020  eformat.",.     
+000084f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008500: 2020 2020 2072 6570 6f72 742e 6368 6563       report.chec
+00008510: 6b20 3d20 4661 6c73 650a 2020 2020 2020  k = False.      
+00008520: 2020 2020 2020 7265 706f 7274 2e64 6966        report.dif
+00008530: 6620 3d20 5472 7565 0a20 2020 2020 2020  f = True.       
+00008540: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00008550: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+00008560: 2020 2020 2020 2075 6e73 7479 6c65 2873         unstyle(s
+00008570: 7472 2872 6570 6f72 7429 292c 0a20 2020  tr(report)),.   
+00008580: 2020 2020 2020 2020 2020 2020 2022 3220               "2 
+00008590: 6669 6c65 7320 776f 756c 6420 6265 2072  files would be r
+000085a0: 6566 6f72 6d61 7474 6564 2c20 3320 6669  eformatted, 3 fi
+000085b0: 6c65 7320 776f 756c 6420 6265 206c 6566  les would be lef
+000085c0: 7420 756e 6368 616e 6765 642c 2032 220a  t unchanged, 2".
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2220 6669 6c65 7320 776f 756c 6420 6661  " files would fa
+000085f0: 696c 2074 6f20 7265 666f 726d 6174 2e22  il to reformat."
+00008600: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00008610: 0a20 2020 2064 6566 2074 6573 745f 6c69  .    def test_li
+00008620: 6232 746f 335f 7061 7273 6528 7365 6c66  b2to3_parse(self
+00008630: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00008640: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+00008650: 6572 7452 6169 7365 7328 6365 7263 6973  ertRaises(cercis
+00008660: 2e49 6e76 616c 6964 496e 7075 7429 3a0a  .InvalidInput):.
+00008670: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+00008680: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
+00008690: 2822 696e 7661 6c69 6420 7379 6e74 6178  ("invalid syntax
+000086a0: 2229 0a0a 2020 2020 2020 2020 7374 7261  ")..        stra
+000086b0: 6464 6c69 6e67 203d 2022 7820 2b20 7922  ddling = "x + y"
+000086c0: 0a20 2020 2020 2020 2063 6572 6369 732e  .        cercis.
+000086d0: 6c69 6232 746f 335f 7061 7273 6528 7374  lib2to3_parse(st
+000086e0: 7261 6464 6c69 6e67 290a 2020 2020 2020  raddling).      
+000086f0: 2020 6365 7263 6973 2e6c 6962 3274 6f33    cercis.lib2to3
+00008700: 5f70 6172 7365 2873 7472 6164 646c 696e  _parse(straddlin
+00008710: 672c 207b 5461 7267 6574 5665 7273 696f  g, {TargetVersio
+00008720: 6e2e 5059 3336 7d29 0a0a 2020 2020 2020  n.PY36})..      
+00008730: 2020 7079 325f 6f6e 6c79 203d 2022 7072    py2_only = "pr
+00008740: 696e 7420 7822 0a20 2020 2020 2020 2077  int x".        w
+00008750: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
+00008760: 6169 7365 7328 6365 7263 6973 2e49 6e76  aises(cercis.Inv
+00008770: 616c 6964 496e 7075 7429 3a0a 2020 2020  alidInput):.    
+00008780: 2020 2020 2020 2020 6365 7263 6973 2e6c          cercis.l
+00008790: 6962 3274 6f33 5f70 6172 7365 2870 7932  ib2to3_parse(py2
+000087a0: 5f6f 6e6c 792c 207b 5461 7267 6574 5665  _only, {TargetVe
+000087b0: 7273 696f 6e2e 5059 3336 7d29 0a0a 2020  rsion.PY36})..  
+000087c0: 2020 2020 2020 7079 335f 6f6e 6c79 203d        py3_only =
+000087d0: 2022 6578 6563 2878 2c20 656e 643d 7929   "exec(x, end=y)
+000087e0: 220a 2020 2020 2020 2020 6365 7263 6973  ".        cercis
+000087f0: 2e6c 6962 3274 6f33 5f70 6172 7365 2870  .lib2to3_parse(p
+00008800: 7933 5f6f 6e6c 7929 0a20 2020 2020 2020  y3_only).       
+00008810: 2063 6572 6369 732e 6c69 6232 746f 335f   cercis.lib2to3_
+00008820: 7061 7273 6528 7079 335f 6f6e 6c79 2c20  parse(py3_only, 
+00008830: 7b54 6172 6765 7456 6572 7369 6f6e 2e50  {TargetVersion.P
+00008840: 5933 367d 290a 0a20 2020 2064 6566 2074  Y36})..    def t
+00008850: 6573 745f 6765 745f 6665 6174 7572 6573  est_get_features
+00008860: 5f75 7365 645f 6465 636f 7261 746f 7228  _used_decorator(
+00008870: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00008880: 2020 2020 2020 2023 2054 6573 7420 7468         # Test th
+00008890: 6520 6665 6174 7572 6520 6465 7465 6374  e feature detect
+000088a0: 696f 6e20 6f66 206e 6577 2064 6563 6f72  ion of new decor
+000088b0: 6174 6f72 2073 796e 7461 780a 2020 2020  ator syntax.    
+000088c0: 2020 2020 2320 7369 6e63 6520 7468 6973      # since this
+000088d0: 206d 616b 6573 2073 6f6d 6520 7465 7374   makes some test
+000088e0: 2063 6173 6573 206f 6620 7465 7374 5f67   cases of test_g
+000088f0: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
+00008900: 2829 0a20 2020 2020 2020 2023 2066 6169  ().        # fai
+00008910: 6c73 2069 6620 6974 2066 6169 6c73 2c20  ls if it fails, 
+00008920: 7468 6973 2069 7320 7465 7374 6564 2066  this is tested f
+00008930: 6972 7374 2073 6f20 7468 6174 2061 2075  irst so that a u
+00008940: 7365 6675 6c20 6361 7365 0a20 2020 2020  seful case.     
+00008950: 2020 2023 2069 7320 6964 656e 7469 6669     # is identifi
+00008960: 6564 0a20 2020 2020 2020 2073 696d 706c  ed.        simpl
+00008970: 6573 2c20 7265 6c61 7865 6420 3d20 7265  es, relaxed = re
+00008980: 6164 5f64 6174 6128 226d 6973 6365 6c6c  ad_data("miscell
+00008990: 616e 656f 7573 222c 2022 6465 636f 7261  aneous", "decora
+000089a0: 746f 7273 2229 0a20 2020 2020 2020 2023  tors").        #
+000089b0: 2073 6b69 7020 6578 706c 616e 6174 696f   skip explanatio
+000089c0: 6e20 636f 6d6d 656e 7473 2061 7420 7468  n comments at th
+000089d0: 6520 746f 7020 6f66 2074 6865 2066 696c  e top of the fil
+000089e0: 650a 2020 2020 2020 2020 666f 7220 7369  e.        for si
+000089f0: 6d70 6c65 5f74 6573 7420 696e 2073 696d  mple_test in sim
+00008a00: 706c 6573 2e73 706c 6974 2822 2323 2229  ples.split("##")
+00008a10: 5b31 3a5d 3a0a 2020 2020 2020 2020 2020  [1:]:.          
+00008a20: 2020 6e6f 6465 203d 2063 6572 6369 732e    node = cercis.
+00008a30: 6c69 6232 746f 335f 7061 7273 6528 7369  lib2to3_parse(si
+00008a40: 6d70 6c65 5f74 6573 7429 0a20 2020 2020  mple_test).     
+00008a50: 2020 2020 2020 2064 6563 6f72 6174 6f72         decorator
+00008a60: 203d 2073 7472 286e 6f64 652e 6368 696c   = str(node.chil
+00008a70: 6472 656e 5b30 5d2e 6368 696c 6472 656e  dren[0].children
+00008a80: 5b30 5d29 2e73 7472 6970 2829 0a20 2020  [0]).strip().   
+00008a90: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00008aa0: 7365 7274 4e6f 7449 6e28 0a20 2020 2020  sertNotIn(.     
+00008ab0: 2020 2020 2020 2020 2020 2046 6561 7475             Featu
+00008ac0: 7265 2e52 454c 4158 4544 5f44 4543 4f52  re.RELAXED_DECOR
+00008ad0: 4154 4f52 532c 0a20 2020 2020 2020 2020  ATORS,.         
+00008ae0: 2020 2020 2020 2063 6572 6369 732e 6765         cercis.ge
+00008af0: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
+00008b00: 6e6f 6465 292c 0a20 2020 2020 2020 2020  node),.         
+00008b10: 2020 2020 2020 206d 7367 3d28 0a20 2020         msg=(.   
+00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b30: 2066 2264 6563 6f72 6174 6f72 2027 7b64   f"decorator '{d
+00008b40: 6563 6f72 6174 6f72 7d27 2066 6f6c 6c6f  ecorator}' follo
+00008b50: 7773 2070 7974 686f 6e3c 3d33 2e38 2073  ws python<=3.8 s
+00008b60: 796e 7461 7822 0a20 2020 2020 2020 2020  yntax".         
+00008b70: 2020 2020 2020 2020 2020 2022 6275 7420             "but 
+00008b80: 6973 2064 6574 6563 7465 6420 6173 2033  is detected as 3
+00008b90: 2e39 2b22 0a20 2020 2020 2020 2020 2020  .9+".           
+00008ba0: 2020 2020 2020 2020 2023 2066 2254 6865           # f"The
+00008bb0: 2066 756c 6c20 6e6f 6465 2069 735c 6e7b   full node is\n{
+00008bc0: 6e6f 6465 2172 7d22 0a20 2020 2020 2020  node!r}".       
+00008bd0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00008be0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00008bf0: 2020 2320 736b 6970 2074 6865 2027 2320    # skip the '# 
+00008c00: 6f75 7470 7574 2720 636f 6d6d 656e 7420  output' comment 
+00008c10: 6174 2074 6865 2074 6f70 206f 6620 7468  at the top of th
+00008c20: 6520 6f75 7470 7574 2070 6172 740a 2020  e output part.  
+00008c30: 2020 2020 2020 666f 7220 7265 6c61 7865        for relaxe
+00008c40: 645f 7465 7374 2069 6e20 7265 6c61 7865  d_test in relaxe
+00008c50: 642e 7370 6c69 7428 2223 2322 295b 313a  d.split("##")[1:
+00008c60: 5d3a 0a20 2020 2020 2020 2020 2020 206e  ]:.            n
+00008c70: 6f64 6520 3d20 6365 7263 6973 2e6c 6962  ode = cercis.lib
+00008c80: 3274 6f33 5f70 6172 7365 2872 656c 6178  2to3_parse(relax
+00008c90: 6564 5f74 6573 7429 0a20 2020 2020 2020  ed_test).       
+00008ca0: 2020 2020 2064 6563 6f72 6174 6f72 203d       decorator =
+00008cb0: 2073 7472 286e 6f64 652e 6368 696c 6472   str(node.childr
+00008cc0: 656e 5b30 5d2e 6368 696c 6472 656e 5b30  en[0].children[0
+00008cd0: 5d29 2e73 7472 6970 2829 0a20 2020 2020  ]).strip().     
+00008ce0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00008cf0: 7274 496e 280a 2020 2020 2020 2020 2020  rtIn(.          
+00008d00: 2020 2020 2020 4665 6174 7572 652e 5245        Feature.RE
+00008d10: 4c41 5845 445f 4445 434f 5241 544f 5253  LAXED_DECORATORS
+00008d20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008d30: 2020 6365 7263 6973 2e67 6574 5f66 6561    cercis.get_fea
+00008d40: 7475 7265 735f 7573 6564 286e 6f64 6529  tures_used(node)
+00008d50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008d60: 2020 6d73 673d 280a 2020 2020 2020 2020    msg=(.        
+00008d70: 2020 2020 2020 2020 2020 2020 6622 6465              f"de
+00008d80: 636f 7261 746f 7220 277b 6465 636f 7261  corator '{decora
+00008d90: 746f 727d 2720 7573 6573 2070 7974 686f  tor}' uses pytho
+00008da0: 6e33 2e39 2b20 7379 6e74 6178 220a 2020  n3.9+ syntax".  
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dc0: 2020 2262 7574 2069 7320 6465 7465 6374    "but is detect
+00008dd0: 6564 2061 7320 7079 7468 6f6e 3c3d 332e  ed as python<=3.
+00008de0: 3822 0a20 2020 2020 2020 2020 2020 2020  8".             
+00008df0: 2020 2020 2020 2023 2066 2254 6865 2066         # f"The f
+00008e00: 756c 6c20 6e6f 6465 2069 735c 6e7b 6e6f  ull node is\n{no
+00008e10: 6465 2172 7d22 0a20 2020 2020 2020 2020  de!r}".         
+00008e20: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00008e30: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00008e40: 2074 6573 745f 6765 745f 6665 6174 7572   test_get_featur
+00008e50: 6573 5f75 7365 6428 7365 6c66 2920 2d3e  es_used(self) ->
+00008e60: 204e 6f6e 653a 0a20 2020 2020 2020 206e   None:.        n
+00008e70: 6f64 6520 3d20 6365 7263 6973 2e6c 6962  ode = cercis.lib
+00008e80: 3274 6f33 5f70 6172 7365 2822 6465 6620  2to3_parse("def 
+00008e90: 6628 2a2c 2061 7267 293a 202e 2e2e 5c6e  f(*, arg): ...\n
+00008ea0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00008eb0: 6173 7365 7274 4571 7561 6c28 6365 7263  assertEqual(cerc
+00008ec0: 6973 2e67 6574 5f66 6561 7475 7265 735f  is.get_features_
+00008ed0: 7573 6564 286e 6f64 6529 2c20 7365 7428  used(node), set(
+00008ee0: 2929 0a20 2020 2020 2020 206e 6f64 6520  )).        node 
+00008ef0: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
+00008f00: 5f70 6172 7365 2822 6465 6620 6628 2a2c  _parse("def f(*,
+00008f10: 2061 7267 2c29 3a20 2e2e 2e5c 6e22 290a   arg,): ...\n").
+00008f20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008f30: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00008f40: 2020 2020 2020 6365 7263 6973 2e67 6574        cercis.get
+00008f50: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
+00008f60: 6f64 6529 2c20 7b46 6561 7475 7265 2e54  ode), {Feature.T
+00008f70: 5241 494c 494e 475f 434f 4d4d 415f 494e  RAILING_COMMA_IN
+00008f80: 5f44 4546 7d0a 2020 2020 2020 2020 290a  _DEF}.        ).
+00008f90: 2020 2020 2020 2020 6e6f 6465 203d 2063          node = c
+00008fa0: 6572 6369 732e 6c69 6232 746f 335f 7061  ercis.lib2to3_pa
+00008fb0: 7273 6528 2266 282a 6172 672c 295c 6e22  rse("f(*arg,)\n"
+00008fc0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00008fd0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00008fe0: 2020 2020 2020 2020 6365 7263 6973 2e67          cercis.g
+00008ff0: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
+00009000: 286e 6f64 6529 2c20 7b46 6561 7475 7265  (node), {Feature
+00009010: 2e54 5241 494c 494e 475f 434f 4d4d 415f  .TRAILING_COMMA_
+00009020: 494e 5f43 414c 4c7d 0a20 2020 2020 2020  IN_CALL}.       
+00009030: 2029 0a20 2020 2020 2020 206e 6f64 6520   ).        node 
+00009040: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
+00009050: 5f70 6172 7365 2822 6465 6620 6628 2a2c  _parse("def f(*,
+00009060: 2061 7267 293a 2066 2773 7472 696e 6727   arg): f'string'
+00009070: 5c6e 2229 0a20 2020 2020 2020 2073 656c  \n").        sel
+00009080: 662e 6173 7365 7274 4571 7561 6c28 6365  f.assertEqual(ce
+00009090: 7263 6973 2e67 6574 5f66 6561 7475 7265  rcis.get_feature
+000090a0: 735f 7573 6564 286e 6f64 6529 2c20 7b46  s_used(node), {F
+000090b0: 6561 7475 7265 2e46 5f53 5452 494e 4753  eature.F_STRINGS
+000090c0: 7d29 0a20 2020 2020 2020 206e 6f64 6520  }).        node 
+000090d0: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
+000090e0: 5f70 6172 7365 2822 3132 335f 3435 365c  _parse("123_456\
+000090f0: 6e22 290a 2020 2020 2020 2020 7365 6c66  n").        self
+00009100: 2e61 7373 6572 7445 7175 616c 2863 6572  .assertEqual(cer
+00009110: 6369 732e 6765 745f 6665 6174 7572 6573  cis.get_features
+00009120: 5f75 7365 6428 6e6f 6465 292c 207b 4665  _used(node), {Fe
+00009130: 6174 7572 652e 4e55 4d45 5249 435f 554e  ature.NUMERIC_UN
+00009140: 4445 5253 434f 5245 537d 290a 2020 2020  DERSCORES}).    
+00009150: 2020 2020 6e6f 6465 203d 2063 6572 6369      node = cerci
+00009160: 732e 6c69 6232 746f 335f 7061 7273 6528  s.lib2to3_parse(
+00009170: 2231 3233 3435 365c 6e22 290a 2020 2020  "123456\n").    
+00009180: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009190: 7175 616c 2863 6572 6369 732e 6765 745f  qual(cercis.get_
+000091a0: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+000091b0: 6465 292c 2073 6574 2829 290a 2020 2020  de), set()).    
+000091c0: 2020 2020 736f 7572 6365 2c20 6578 7065      source, expe
+000091d0: 6374 6564 203d 2072 6561 645f 6461 7461  cted = read_data
+000091e0: 2822 7369 6d70 6c65 5f63 6173 6573 222c  ("simple_cases",
+000091f0: 2022 6675 6e63 7469 6f6e 2229 0a20 2020   "function").   
+00009200: 2020 2020 206e 6f64 6520 3d20 6365 7263       node = cerc
+00009210: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
+00009220: 2873 6f75 7263 6529 0a20 2020 2020 2020  (source).       
+00009230: 2065 7870 6563 7465 645f 6665 6174 7572   expected_featur
+00009240: 6573 203d 207b 0a20 2020 2020 2020 2020  es = {.         
+00009250: 2020 2046 6561 7475 7265 2e54 5241 494c     Feature.TRAIL
+00009260: 494e 475f 434f 4d4d 415f 494e 5f43 414c  ING_COMMA_IN_CAL
+00009270: 4c2c 0a20 2020 2020 2020 2020 2020 2046  L,.            F
+00009280: 6561 7475 7265 2e54 5241 494c 494e 475f  eature.TRAILING_
+00009290: 434f 4d4d 415f 494e 5f44 4546 2c0a 2020  COMMA_IN_DEF,.  
+000092a0: 2020 2020 2020 2020 2020 4665 6174 7572            Featur
+000092b0: 652e 465f 5354 5249 4e47 532c 0a20 2020  e.F_STRINGS,.   
+000092c0: 2020 2020 207d 0a20 2020 2020 2020 2073       }.        s
+000092d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000092e0: 6365 7263 6973 2e67 6574 5f66 6561 7475  cercis.get_featu
+000092f0: 7265 735f 7573 6564 286e 6f64 6529 2c20  res_used(node), 
+00009300: 6578 7065 6374 6564 5f66 6561 7475 7265  expected_feature
+00009310: 7329 0a20 2020 2020 2020 206e 6f64 6520  s).        node 
+00009320: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
+00009330: 5f70 6172 7365 2865 7870 6563 7465 6429  _parse(expected)
+00009340: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00009350: 7365 7274 4571 7561 6c28 6365 7263 6973  sertEqual(cercis
+00009360: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
+00009370: 6564 286e 6f64 6529 2c20 6578 7065 6374  ed(node), expect
+00009380: 6564 5f66 6561 7475 7265 7329 0a20 2020  ed_features).   
+00009390: 2020 2020 2073 6f75 7263 652c 2065 7870       source, exp
+000093a0: 6563 7465 6420 3d20 7265 6164 5f64 6174  ected = read_dat
+000093b0: 6128 2273 696d 706c 655f 6361 7365 7322  a("simple_cases"
+000093c0: 2c20 2265 7870 7265 7373 696f 6e22 290a  , "expression").
+000093d0: 2020 2020 2020 2020 6e6f 6465 203d 2063          node = c
+000093e0: 6572 6369 732e 6c69 6232 746f 335f 7061  ercis.lib2to3_pa
+000093f0: 7273 6528 736f 7572 6365 290a 2020 2020  rse(source).    
+00009400: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009410: 7175 616c 2863 6572 6369 732e 6765 745f  qual(cercis.get_
+00009420: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+00009430: 6465 292c 2073 6574 2829 290a 2020 2020  de), set()).    
+00009440: 2020 2020 6e6f 6465 203d 2063 6572 6369      node = cerci
+00009450: 732e 6c69 6232 746f 335f 7061 7273 6528  s.lib2to3_parse(
+00009460: 6578 7065 6374 6564 290a 2020 2020 2020  expected).      
+00009470: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00009480: 616c 2863 6572 6369 732e 6765 745f 6665  al(cercis.get_fe
+00009490: 6174 7572 6573 5f75 7365 6428 6e6f 6465  atures_used(node
+000094a0: 292c 2073 6574 2829 290a 2020 2020 2020  ), set()).      
+000094b0: 2020 6e6f 6465 203d 2063 6572 6369 732e    node = cercis.
+000094c0: 6c69 6232 746f 335f 7061 7273 6528 226c  lib2to3_parse("l
+000094d0: 616d 6264 6120 612c 202f 2c20 623a 202e  ambda a, /, b: .
+000094e0: 2e2e 2229 0a20 2020 2020 2020 2073 656c  ..").        sel
+000094f0: 662e 6173 7365 7274 4571 7561 6c28 6365  f.assertEqual(ce
+00009500: 7263 6973 2e67 6574 5f66 6561 7475 7265  rcis.get_feature
+00009510: 735f 7573 6564 286e 6f64 6529 2c20 7b46  s_used(node), {F
+00009520: 6561 7475 7265 2e50 4f53 5f4f 4e4c 595f  eature.POS_ONLY_
+00009530: 4152 4755 4d45 4e54 537d 290a 2020 2020  ARGUMENTS}).    
+00009540: 2020 2020 6e6f 6465 203d 2063 6572 6369      node = cerci
+00009550: 732e 6c69 6232 746f 335f 7061 7273 6528  s.lib2to3_parse(
+00009560: 2264 6566 2066 6e28 612c 202f 2c20 6229  "def fn(a, /, b)
+00009570: 3a20 2e2e 2e22 290a 2020 2020 2020 2020  : ...").        
+00009580: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00009590: 2863 6572 6369 732e 6765 745f 6665 6174  (cercis.get_feat
+000095a0: 7572 6573 5f75 7365 6428 6e6f 6465 292c  ures_used(node),
+000095b0: 207b 4665 6174 7572 652e 504f 535f 4f4e   {Feature.POS_ON
+000095c0: 4c59 5f41 5247 554d 454e 5453 7d29 0a20  LY_ARGUMENTS}). 
+000095d0: 2020 2020 2020 206e 6f64 6520 3d20 6365         node = ce
+000095e0: 7263 6973 2e6c 6962 3274 6f33 5f70 6172  rcis.lib2to3_par
+000095f0: 7365 2822 6465 6620 666e 2829 3a20 7969  se("def fn(): yi
+00009600: 656c 6420 612c 2062 2229 0a20 2020 2020  eld a, b").     
+00009610: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00009620: 7561 6c28 6365 7263 6973 2e67 6574 5f66  ual(cercis.get_f
+00009630: 6561 7475 7265 735f 7573 6564 286e 6f64  eatures_used(nod
+00009640: 6529 2c20 7365 7428 2929 0a20 2020 2020  e), set()).     
+00009650: 2020 206e 6f64 6520 3d20 6365 7263 6973     node = cercis
+00009660: 2e6c 6962 3274 6f33 5f70 6172 7365 2822  .lib2to3_parse("
+00009670: 6465 6620 666e 2829 3a20 7265 7475 726e  def fn(): return
+00009680: 2061 2c20 6222 290a 2020 2020 2020 2020   a, b").        
+00009690: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000096a0: 2863 6572 6369 732e 6765 745f 6665 6174  (cercis.get_feat
+000096b0: 7572 6573 5f75 7365 6428 6e6f 6465 292c  ures_used(node),
+000096c0: 2073 6574 2829 290a 2020 2020 2020 2020   set()).        
+000096d0: 6e6f 6465 203d 2063 6572 6369 732e 6c69  node = cercis.li
+000096e0: 6232 746f 335f 7061 7273 6528 2264 6566  b2to3_parse("def
+000096f0: 2066 6e28 293a 2079 6965 6c64 202a 622c   fn(): yield *b,
+00009700: 2063 2229 0a20 2020 2020 2020 2073 656c   c").        sel
+00009710: 662e 6173 7365 7274 4571 7561 6c28 6365  f.assertEqual(ce
+00009720: 7263 6973 2e67 6574 5f66 6561 7475 7265  rcis.get_feature
+00009730: 735f 7573 6564 286e 6f64 6529 2c20 7b46  s_used(node), {F
+00009740: 6561 7475 7265 2e55 4e50 4143 4b49 4e47  eature.UNPACKING
+00009750: 5f4f 4e5f 464c 4f57 7d29 0a20 2020 2020  _ON_FLOW}).     
+00009760: 2020 206e 6f64 6520 3d20 6365 7263 6973     node = cercis
+00009770: 2e6c 6962 3274 6f33 5f70 6172 7365 2822  .lib2to3_parse("
+00009780: 6465 6620 666e 2829 3a20 7265 7475 726e  def fn(): return
+00009790: 2061 2c20 2a62 2c20 6322 290a 2020 2020   a, *b, c").    
+000097a0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000097b0: 7175 616c 2863 6572 6369 732e 6765 745f  qual(cercis.get_
+000097c0: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+000097d0: 6465 292c 207b 4665 6174 7572 652e 554e  de), {Feature.UN
+000097e0: 5041 434b 494e 475f 4f4e 5f46 4c4f 577d  PACKING_ON_FLOW}
+000097f0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
+00009800: 2063 6572 6369 732e 6c69 6232 746f 335f   cercis.lib2to3_
+00009810: 7061 7273 6528 2278 203d 2061 2c20 2a62  parse("x = a, *b
+00009820: 2c20 6322 290a 2020 2020 2020 2020 7365  , c").        se
+00009830: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
+00009840: 6572 6369 732e 6765 745f 6665 6174 7572  ercis.get_featur
+00009850: 6573 5f75 7365 6428 6e6f 6465 292c 2073  es_used(node), s
+00009860: 6574 2829 290a 2020 2020 2020 2020 6e6f  et()).        no
+00009870: 6465 203d 2063 6572 6369 732e 6c69 6232  de = cercis.lib2
+00009880: 746f 335f 7061 7273 6528 2278 3a20 416e  to3_parse("x: An
+00009890: 7920 3d20 7265 6775 6c61 7222 290a 2020  y = regular").  
+000098a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000098b0: 7445 7175 616c 2863 6572 6369 732e 6765  tEqual(cercis.ge
+000098c0: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
+000098d0: 6e6f 6465 292c 2073 6574 2829 290a 2020  node), set()).  
+000098e0: 2020 2020 2020 6e6f 6465 203d 2063 6572        node = cer
+000098f0: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
+00009900: 6528 2278 3a20 416e 7920 3d20 2872 6567  e("x: Any = (reg
+00009910: 756c 6172 2c20 7265 6775 6c61 7229 2229  ular, regular)")
+00009920: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00009930: 7365 7274 4571 7561 6c28 6365 7263 6973  sertEqual(cercis
+00009940: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
+00009950: 6564 286e 6f64 6529 2c20 7365 7428 2929  ed(node), set())
+00009960: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
+00009970: 6365 7263 6973 2e6c 6962 3274 6f33 5f70  cercis.lib2to3_p
+00009980: 6172 7365 2822 783a 2041 6e79 203d 2043  arse("x: Any = C
+00009990: 6f6d 706c 6578 2854 7970 6528 3129 295b  omplex(Type(1))[
+000099a0: 736f 6d65 7468 696e 675d 2229 0a20 2020  something]").   
+000099b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000099c0: 4571 7561 6c28 6365 7263 6973 2e67 6574  Equal(cercis.get
+000099d0: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
+000099e0: 6f64 6529 2c20 7365 7428 2929 0a20 2020  ode), set()).   
+000099f0: 2020 2020 206e 6f64 6520 3d20 6365 7263       node = cerc
+00009a00: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
+00009a10: 2822 783a 2054 7570 6c65 5b69 6e74 2c20  ("x: Tuple[int, 
+00009a20: 2e2e 2e5d 203d 2061 2c20 622c 2063 2229  ...] = a, b, c")
+00009a30: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00009a40: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+00009a50: 2020 2020 2020 2063 6572 6369 732e 6765         cercis.ge
+00009a60: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
+00009a70: 6e6f 6465 292c 207b 4665 6174 7572 652e  node), {Feature.
+00009a80: 414e 4e5f 4153 5349 474e 5f45 5854 454e  ANN_ASSIGN_EXTEN
+00009a90: 4445 445f 5248 537d 0a20 2020 2020 2020  DED_RHS}.       
+00009aa0: 2029 0a20 2020 2020 2020 206e 6f64 6520   ).        node 
+00009ab0: 3d20 6365 7263 6973 2e6c 6962 3274 6f33  = cercis.lib2to3
+00009ac0: 5f70 6172 7365 2822 7472 793a 2070 6173  _parse("try: pas
+00009ad0: 735c 6e65 7863 6570 7420 536f 6d65 7468  s\nexcept Someth
+00009ae0: 696e 673a 2070 6173 7322 290a 2020 2020  ing: pass").    
+00009af0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009b00: 7175 616c 2863 6572 6369 732e 6765 745f  qual(cercis.get_
+00009b10: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+00009b20: 6465 292c 2073 6574 2829 290a 2020 2020  de), set()).    
+00009b30: 2020 2020 6e6f 6465 203d 2063 6572 6369      node = cerci
+00009b40: 732e 6c69 6232 746f 335f 7061 7273 6528  s.lib2to3_parse(
+00009b50: 2274 7279 3a20 7061 7373 5c6e 6578 6365  "try: pass\nexce
+00009b60: 7074 2028 2a53 6f6d 6574 6869 6e67 2c29  pt (*Something,)
+00009b70: 3a20 7061 7373 2229 0a20 2020 2020 2020  : pass").       
+00009b80: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00009b90: 6c28 6365 7263 6973 2e67 6574 5f66 6561  l(cercis.get_fea
+00009ba0: 7475 7265 735f 7573 6564 286e 6f64 6529  tures_used(node)
+00009bb0: 2c20 7365 7428 2929 0a20 2020 2020 2020  , set()).       
+00009bc0: 206e 6f64 6520 3d20 6365 7263 6973 2e6c   node = cercis.l
+00009bd0: 6962 3274 6f33 5f70 6172 7365 2822 7472  ib2to3_parse("tr
+00009be0: 793a 2070 6173 735c 6e65 7863 6570 7420  y: pass\nexcept 
+00009bf0: 2a47 726f 7570 3a20 7061 7373 2229 0a20  *Group: pass"). 
+00009c00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00009c10: 7274 4571 7561 6c28 6365 7263 6973 2e67  rtEqual(cercis.g
+00009c20: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
+00009c30: 286e 6f64 6529 2c20 7b46 6561 7475 7265  (node), {Feature
+00009c40: 2e45 5843 4550 545f 5354 4152 7d29 0a20  .EXCEPT_STAR}). 
+00009c50: 2020 2020 2020 206e 6f64 6520 3d20 6365         node = ce
+00009c60: 7263 6973 2e6c 6962 3274 6f33 5f70 6172  rcis.lib2to3_par
+00009c70: 7365 2822 615b 2a62 5d22 290a 2020 2020  se("a[*b]").    
+00009c80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009c90: 7175 616c 2863 6572 6369 732e 6765 745f  qual(cercis.get_
+00009ca0: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+00009cb0: 6465 292c 207b 4665 6174 7572 652e 5641  de), {Feature.VA
+00009cc0: 5249 4144 4943 5f47 454e 4552 4943 537d  RIADIC_GENERICS}
+00009cd0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
+00009ce0: 2063 6572 6369 732e 6c69 6232 746f 335f   cercis.lib2to3_
+00009cf0: 7061 7273 6528 2261 5b78 2c20 2a79 2829  parse("a[x, *y()
+00009d00: 2c20 7a5d 203d 2074 2229 0a20 2020 2020  , z] = t").     
+00009d10: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00009d20: 7561 6c28 6365 7263 6973 2e67 6574 5f66  ual(cercis.get_f
+00009d30: 6561 7475 7265 735f 7573 6564 286e 6f64  eatures_used(nod
+00009d40: 6529 2c20 7b46 6561 7475 7265 2e56 4152  e), {Feature.VAR
+00009d50: 4941 4449 435f 4745 4e45 5249 4353 7d29  IADIC_GENERICS})
+00009d60: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
+00009d70: 6365 7263 6973 2e6c 6962 3274 6f33 5f70  cercis.lib2to3_p
+00009d80: 6172 7365 2822 6465 6620 666e 282a 6172  arse("def fn(*ar
+00009d90: 6773 3a20 2a54 293a 2070 6173 7322 290a  gs: *T): pass").
+00009da0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00009db0: 6572 7445 7175 616c 2863 6572 6369 732e  ertEqual(cercis.
+00009dc0: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
+00009dd0: 6428 6e6f 6465 292c 207b 4665 6174 7572  d(node), {Featur
+00009de0: 652e 5641 5249 4144 4943 5f47 454e 4552  e.VARIADIC_GENER
+00009df0: 4943 537d 290a 0a20 2020 2064 6566 2074  ICS})..    def t
+00009e00: 6573 745f 6765 745f 6665 6174 7572 6573  est_get_features
+00009e10: 5f75 7365 645f 666f 725f 6675 7475 7265  _used_for_future
+00009e20: 5f66 6c61 6773 2873 656c 6629 202d 3e20  _flags(self) -> 
+00009e30: 4e6f 6e65 3a0a 2020 2020 2020 2020 666f  None:.        fo
+00009e40: 7220 7372 632c 2066 6561 7475 7265 7320  r src, features 
+00009e50: 696e 205b 0a20 2020 2020 2020 2020 2020  in [.           
+00009e60: 2028 2266 726f 6d20 5f5f 6675 7475 7265   ("from __future
+00009e70: 5f5f 2069 6d70 6f72 7420 616e 6e6f 7461  __ import annota
+00009e80: 7469 6f6e 7322 2c20 7b46 6561 7475 7265  tions", {Feature
+00009e90: 2e46 5554 5552 455f 414e 4e4f 5441 5449  .FUTURE_ANNOTATI
+00009ea0: 4f4e 537d 292c 0a20 2020 2020 2020 2020  ONS}),.         
+00009eb0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00009ec0: 2020 2020 2022 6672 6f6d 205f 5f66 7574       "from __fut
+00009ed0: 7572 655f 5f20 696d 706f 7274 2028 6f74  ure__ import (ot
+00009ee0: 6865 722c 2061 6e6e 6f74 6174 696f 6e73  her, annotations
+00009ef0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+00009f00: 2020 2020 7b46 6561 7475 7265 2e46 5554      {Feature.FUT
+00009f10: 5552 455f 414e 4e4f 5441 5449 4f4e 537d  URE_ANNOTATIONS}
+00009f20: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
+00009f30: 0a20 2020 2020 2020 2020 2020 2028 2261  .            ("a
+00009f40: 203d 2031 202b 2032 5c6e 6672 6f6d 2073   = 1 + 2\nfrom s
+00009f50: 6f6d 6574 6869 6e67 2069 6d70 6f72 7420  omething import 
+00009f60: 616e 6e6f 7461 7469 6f6e 7322 2c20 7365  annotations", se
+00009f70: 7428 2929 2c0a 2020 2020 2020 2020 2020  t()),.          
+00009f80: 2020 2822 6672 6f6d 205f 5f66 7574 7572    ("from __futur
+00009f90: 655f 5f20 696d 706f 7274 2078 2c20 7922  e__ import x, y"
+00009fa0: 2c20 7365 7428 2929 2c0a 2020 2020 2020  , set()),.      
+00009fb0: 2020 5d3a 0a20 2020 2020 2020 2020 2020    ]:.           
+00009fc0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00009fd0: 7374 2873 7263 3d73 7263 2c20 6665 6174  st(src=src, feat
+00009fe0: 7572 6573 3d66 6561 7475 7265 7329 3a0a  ures=features):.
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 6e6f 6465 203d 2063 6572 6369 732e 6c69  node = cercis.li
+0000a010: 6232 746f 335f 7061 7273 6528 7372 6329  b2to3_parse(src)
+0000a020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a030: 2066 7574 7572 655f 696d 706f 7274 7320   future_imports 
+0000a040: 3d20 6365 7263 6973 2e67 6574 5f66 7574  = cercis.get_fut
+0000a050: 7572 655f 696d 706f 7274 7328 6e6f 6465  ure_imports(node
+0000a060: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a070: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000a080: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+0000a090: 2020 2020 2020 2020 6365 7263 6973 2e67          cercis.g
+0000a0a0: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
+0000a0b0: 286e 6f64 652c 2066 7574 7572 655f 696d  (node, future_im
+0000a0c0: 706f 7274 733d 6675 7475 7265 5f69 6d70  ports=future_imp
+0000a0d0: 6f72 7473 292c 0a20 2020 2020 2020 2020  orts),.         
+0000a0e0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+0000a0f0: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
+0000a100: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0000a110: 7465 7374 5f67 6574 5f66 7574 7572 655f  test_get_future_
+0000a120: 696d 706f 7274 7328 7365 6c66 2920 2d3e  imports(self) ->
+0000a130: 204e 6f6e 653a 0a20 2020 2020 2020 206e   None:.        n
+0000a140: 6f64 6520 3d20 6365 7263 6973 2e6c 6962  ode = cercis.lib
+0000a150: 3274 6f33 5f70 6172 7365 2822 5c6e 2229  2to3_parse("\n")
+0000a160: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000a170: 7365 7274 4571 7561 6c28 7365 7428 292c  sertEqual(set(),
+0000a180: 2063 6572 6369 732e 6765 745f 6675 7475   cercis.get_futu
+0000a190: 7265 5f69 6d70 6f72 7473 286e 6f64 6529  re_imports(node)
+0000a1a0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
+0000a1b0: 2063 6572 6369 732e 6c69 6232 746f 335f   cercis.lib2to3_
+0000a1c0: 7061 7273 6528 2266 726f 6d20 5f5f 6675  parse("from __fu
+0000a1d0: 7475 7265 5f5f 2069 6d70 6f72 7420 6365  ture__ import ce
+0000a1e0: 7263 6973 5c6e 2229 0a20 2020 2020 2020  rcis\n").       
+0000a1f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000a200: 6c28 7b22 6365 7263 6973 227d 2c20 6365  l({"cercis"}, ce
+0000a210: 7263 6973 2e67 6574 5f66 7574 7572 655f  rcis.get_future_
+0000a220: 696d 706f 7274 7328 6e6f 6465 2929 0a20  imports(node)). 
+0000a230: 2020 2020 2020 206e 6f64 6520 3d20 6365         node = ce
+0000a240: 7263 6973 2e6c 6962 3274 6f33 5f70 6172  rcis.lib2to3_par
+0000a250: 7365 2822 6672 6f6d 205f 5f66 7574 7572  se("from __futur
+0000a260: 655f 5f20 696d 706f 7274 206d 756c 7469  e__ import multi
+0000a270: 706c 652c 2069 6d70 6f72 7473 5c6e 2229  ple, imports\n")
+0000a280: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000a290: 7365 7274 4571 7561 6c28 7b22 6d75 6c74  sertEqual({"mult
+0000a2a0: 6970 6c65 222c 2022 696d 706f 7274 7322  iple", "imports"
+0000a2b0: 7d2c 2063 6572 6369 732e 6765 745f 6675  }, cercis.get_fu
+0000a2c0: 7475 7265 5f69 6d70 6f72 7473 286e 6f64  ture_imports(nod
+0000a2d0: 6529 290a 2020 2020 2020 2020 6e6f 6465  e)).        node
+0000a2e0: 203d 2063 6572 6369 732e 6c69 6232 746f   = cercis.lib2to
+0000a2f0: 335f 7061 7273 6528 2266 726f 6d20 5f5f  3_parse("from __
+0000a300: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
+0000a310: 2870 6172 656e 7468 6573 697a 6564 2c20  (parenthesized, 
+0000a320: 696d 706f 7274 7329 5c6e 2229 0a20 2020  imports)\n").   
+0000a330: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000a340: 4571 7561 6c28 7b22 7061 7265 6e74 6865  Equal({"parenthe
+0000a350: 7369 7a65 6422 2c20 2269 6d70 6f72 7473  sized", "imports
+0000a360: 227d 2c20 6365 7263 6973 2e67 6574 5f66  "}, cercis.get_f
+0000a370: 7574 7572 655f 696d 706f 7274 7328 6e6f  uture_imports(no
+0000a380: 6465 2929 0a20 2020 2020 2020 206e 6f64  de)).        nod
+0000a390: 6520 3d20 6365 7263 6973 2e6c 6962 3274  e = cercis.lib2t
+0000a3a0: 6f33 5f70 6172 7365 280a 2020 2020 2020  o3_parse(.      
+0000a3b0: 2020 2020 2020 2266 726f 6d20 5f5f 6675        "from __fu
+0000a3c0: 7475 7265 5f5f 2069 6d70 6f72 7420 6d75  ture__ import mu
+0000a3d0: 6c74 6970 6c65 5c6e 6672 6f6d 205f 5f66  ltiple\nfrom __f
+0000a3e0: 7574 7572 655f 5f20 696d 706f 7274 2069  uture__ import i
+0000a3f0: 6d70 6f72 7473 5c6e 220a 2020 2020 2020  mports\n".      
+0000a400: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+0000a410: 2e61 7373 6572 7445 7175 616c 287b 226d  .assertEqual({"m
+0000a420: 756c 7469 706c 6522 2c20 2269 6d70 6f72  ultiple", "impor
+0000a430: 7473 227d 2c20 6365 7263 6973 2e67 6574  ts"}, cercis.get
+0000a440: 5f66 7574 7572 655f 696d 706f 7274 7328  _future_imports(
+0000a450: 6e6f 6465 2929 0a20 2020 2020 2020 206e  node)).        n
+0000a460: 6f64 6520 3d20 6365 7263 6973 2e6c 6962  ode = cercis.lib
+0000a470: 3274 6f33 5f70 6172 7365 2822 2320 636f  2to3_parse("# co
+0000a480: 6d6d 656e 745c 6e66 726f 6d20 5f5f 6675  mment\nfrom __fu
+0000a490: 7475 7265 5f5f 2069 6d70 6f72 7420 6365  ture__ import ce
+0000a4a0: 7263 6973 5c6e 2229 0a20 2020 2020 2020  rcis\n").       
+0000a4b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000a4c0: 6c28 7b22 6365 7263 6973 227d 2c20 6365  l({"cercis"}, ce
+0000a4d0: 7263 6973 2e67 6574 5f66 7574 7572 655f  rcis.get_future_
+0000a4e0: 696d 706f 7274 7328 6e6f 6465 2929 0a20  imports(node)). 
+0000a4f0: 2020 2020 2020 206e 6f64 6520 3d20 6365         node = ce
+0000a500: 7263 6973 2e6c 6962 3274 6f33 5f70 6172  rcis.lib2to3_par
+0000a510: 7365 2827 2222 2264 6f63 7374 7269 6e67  se('"""docstring
+0000a520: 2222 225c 6e66 726f 6d20 5f5f 6675 7475  """\nfrom __futu
+0000a530: 7265 5f5f 2069 6d70 6f72 7420 6365 7263  re__ import cerc
+0000a540: 6973 5c6e 2729 0a20 2020 2020 2020 2073  is\n').        s
+0000a550: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000a560: 7b22 6365 7263 6973 227d 2c20 6365 7263  {"cercis"}, cerc
+0000a570: 6973 2e67 6574 5f66 7574 7572 655f 696d  is.get_future_im
+0000a580: 706f 7274 7328 6e6f 6465 2929 0a20 2020  ports(node)).   
+0000a590: 2020 2020 206e 6f64 6520 3d20 6365 7263       node = cerc
+0000a5a0: 6973 2e6c 6962 3274 6f33 5f70 6172 7365  is.lib2to3_parse
+0000a5b0: 280a 2020 2020 2020 2020 2020 2020 2273  (.            "s
+0000a5c0: 6f6d 6528 6f74 6865 722c 2063 6f64 6529  ome(other, code)
+0000a5d0: 5c6e 6672 6f6d 205f 5f66 7574 7572 655f  \nfrom __future_
+0000a5e0: 5f20 696d 706f 7274 2063 6572 6369 735c  _ import cercis\
+0000a5f0: 6e22 0a20 2020 2020 2020 2029 0a20 2020  n".        ).   
+0000a600: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000a610: 4571 7561 6c28 7365 7428 292c 2063 6572  Equal(set(), cer
+0000a620: 6369 732e 6765 745f 6675 7475 7265 5f69  cis.get_future_i
+0000a630: 6d70 6f72 7473 286e 6f64 6529 290a 2020  mports(node)).  
+0000a640: 2020 2020 2020 6e6f 6465 203d 2063 6572        node = cer
+0000a650: 6369 732e 6c69 6232 746f 335f 7061 7273  cis.lib2to3_pars
+0000a660: 6528 2266 726f 6d20 736f 6d65 2e6d 6f64  e("from some.mod
+0000a670: 756c 6520 696d 706f 7274 2063 6572 6369  ule import cerci
+0000a680: 735c 6e22 290a 2020 2020 2020 2020 7365  s\n").        se
+0000a690: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+0000a6a0: 6574 2829 2c20 6365 7263 6973 2e67 6574  et(), cercis.get
+0000a6b0: 5f66 7574 7572 655f 696d 706f 7274 7328  _future_imports(
+0000a6c0: 6e6f 6465 2929 0a20 2020 2020 2020 206e  node)).        n
+0000a6d0: 6f64 6520 3d20 6365 7263 6973 2e6c 6962  ode = cercis.lib
+0000a6e0: 3274 6f33 5f70 6172 7365 280a 2020 2020  2to3_parse(.    
+0000a6f0: 2020 2020 2020 2020 2266 726f 6d20 5f5f          "from __
+0000a700: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
+0000a710: 756e 6963 6f64 655f 6c69 7465 7261 6c73  unicode_literals
+0000a720: 2061 7320 5f75 6e69 636f 6465 5f6c 6974   as _unicode_lit
+0000a730: 6572 616c 7322 0a20 2020 2020 2020 2029  erals".        )
+0000a740: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000a750: 7365 7274 4571 7561 6c28 7b22 756e 6963  sertEqual({"unic
+0000a760: 6f64 655f 6c69 7465 7261 6c73 227d 2c20  ode_literals"}, 
+0000a770: 6365 7263 6973 2e67 6574 5f66 7574 7572  cercis.get_futur
+0000a780: 655f 696d 706f 7274 7328 6e6f 6465 2929  e_imports(node))
+0000a790: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
+0000a7a0: 6365 7263 6973 2e6c 6962 3274 6f33 5f70  cercis.lib2to3_p
+0000a7b0: 6172 7365 280a 2020 2020 2020 2020 2020  arse(.          
+0000a7c0: 2020 2266 726f 6d20 5f5f 6675 7475 7265    "from __future
+0000a7d0: 5f5f 2069 6d70 6f72 7420 756e 6963 6f64  __ import unicod
+0000a7e0: 655f 6c69 7465 7261 6c73 2061 7320 5f6c  e_literals as _l
+0000a7f0: 6f6c 2c20 7072 696e 7422 0a20 2020 2020  ol, print".     
+0000a800: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+0000a810: 662e 6173 7365 7274 4571 7561 6c28 7b22  f.assertEqual({"
+0000a820: 756e 6963 6f64 655f 6c69 7465 7261 6c73  unicode_literals
+0000a830: 222c 2022 7072 696e 7422 7d2c 2063 6572  ", "print"}, cer
+0000a840: 6369 732e 6765 745f 6675 7475 7265 5f69  cis.get_future_i
+0000a850: 6d70 6f72 7473 286e 6f64 6529 290a 0a20  mports(node)).. 
+0000a860: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0000a870: 696e 636f 6d70 6174 6962 6c65 5f77 6974  incompatible_wit
+0000a880: 685f 6d79 7079 630a 2020 2020 6465 6620  h_mypyc.    def 
+0000a890: 7465 7374 5f64 6562 7567 5f76 6973 6974  test_debug_visit
+0000a8a0: 6f72 2873 656c 6629 202d 3e20 4e6f 6e65  or(self) -> None
+0000a8b0: 3a0a 2020 2020 2020 2020 736f 7572 6365  :.        source
+0000a8c0: 2c20 5f20 3d20 7265 6164 5f64 6174 6128  , _ = read_data(
+0000a8d0: 226d 6973 6365 6c6c 616e 656f 7573 222c  "miscellaneous",
+0000a8e0: 2022 6465 6275 675f 7669 7369 746f 7222   "debug_visitor"
+0000a8f0: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
+0000a900: 6564 2c20 5f20 3d20 7265 6164 5f64 6174  ed, _ = read_dat
+0000a910: 6128 226d 6973 6365 6c6c 616e 656f 7573  a("miscellaneous
+0000a920: 222c 2022 6465 6275 675f 7669 7369 746f  ", "debug_visito
+0000a930: 722e 6f75 7422 290a 2020 2020 2020 2020  r.out").        
+0000a940: 6f75 745f 6c69 6e65 7320 3d20 5b5d 0a20  out_lines = []. 
+0000a950: 2020 2020 2020 2065 7272 5f6c 696e 6573         err_lines
+0000a960: 203d 205b 5d0a 0a20 2020 2020 2020 2064   = []..        d
+0000a970: 6566 206f 7574 286d 7367 3a20 7374 722c  ef out(msg: str,
+0000a980: 202a 2a6b 7761 7267 733a 2041 6e79 2920   **kwargs: Any) 
+0000a990: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000a9a0: 2020 2020 206f 7574 5f6c 696e 6573 2e61       out_lines.a
+0000a9b0: 7070 656e 6428 6d73 6729 0a0a 2020 2020  ppend(msg)..    
+0000a9c0: 2020 2020 6465 6620 6572 7228 6d73 673a      def err(msg:
+0000a9d0: 2073 7472 2c20 2a2a 6b77 6172 6773 3a20   str, **kwargs: 
+0000a9e0: 416e 7929 202d 3e20 4e6f 6e65 3a0a 2020  Any) -> None:.  
+0000a9f0: 2020 2020 2020 2020 2020 6572 725f 6c69            err_li
+0000aa00: 6e65 732e 6170 7065 6e64 286d 7367 290a  nes.append(msg).
+0000aa10: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
+0000aa20: 7463 6828 2263 6572 6369 732e 6465 6275  tch("cercis.debu
+0000aa30: 672e 6f75 7422 2c20 6f75 7429 3a0a 2020  g.out", out):.  
+0000aa40: 2020 2020 2020 2020 2020 4465 6275 6756            DebugV
+0000aa50: 6973 6974 6f72 2e73 686f 7728 736f 7572  isitor.show(sour
+0000aa60: 6365 290a 2020 2020 2020 2020 6163 7475  ce).        actu
+0000aa70: 616c 203d 2022 5c6e 222e 6a6f 696e 286f  al = "\n".join(o
+0000aa80: 7574 5f6c 696e 6573 2920 2b20 225c 6e22  ut_lines) + "\n"
+0000aa90: 0a20 2020 2020 2020 206c 6f67 5f6e 616d  .        log_nam
+0000aaa0: 6520 3d20 2222 0a20 2020 2020 2020 2069  e = "".        i
+0000aab0: 6620 6578 7065 6374 6564 2021 3d20 6163  f expected != ac
+0000aac0: 7475 616c 3a0a 2020 2020 2020 2020 2020  tual:.          
+0000aad0: 2020 6c6f 675f 6e61 6d65 203d 2063 6572    log_name = cer
+0000aae0: 6369 732e 6475 6d70 5f74 6f5f 6669 6c65  cis.dump_to_file
+0000aaf0: 282a 6f75 745f 6c69 6e65 7329 0a20 2020  (*out_lines).   
+0000ab00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000ab10: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+0000ab20: 2020 2065 7870 6563 7465 642c 0a20 2020     expected,.   
+0000ab30: 2020 2020 2020 2020 2061 6374 7561 6c2c           actual,
+0000ab40: 0a20 2020 2020 2020 2020 2020 2066 2241  .            f"A
+0000ab50: 5354 2070 7269 6e74 206f 7574 2069 7320  ST print out is 
+0000ab60: 6469 6666 6572 656e 742e 2041 6374 7561  different. Actua
+0000ab70: 6c20 7665 7273 696f 6e20 6475 6d70 6564  l version dumped
+0000ab80: 2074 6f20 7b6c 6f67 5f6e 616d 657d 222c   to {log_name}",
+0000ab90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000aba0: 6465 6620 7465 7374 5f66 6f72 6d61 745f  def test_format_
+0000abb0: 6669 6c65 5f63 6f6e 7465 6e74 7328 7365  file_contents(se
+0000abc0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+0000abd0: 2020 2020 206d 6f64 6520 3d20 4445 4641       mode = DEFA
+0000abe0: 554c 545f 4d4f 4445 0a20 2020 2020 2020  ULT_MODE.       
+0000abf0: 2065 6d70 7479 203d 2022 220a 2020 2020   empty = "".    
+0000ac00: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+0000ac10: 7365 7274 5261 6973 6573 2863 6572 6369  sertRaises(cerci
+0000ac20: 732e 4e6f 7468 696e 6743 6861 6e67 6564  s.NothingChanged
+0000ac30: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+0000ac40: 6572 6369 732e 666f 726d 6174 5f66 696c  ercis.format_fil
+0000ac50: 655f 636f 6e74 656e 7473 2865 6d70 7479  e_contents(empty
+0000ac60: 2c20 6d6f 6465 3d6d 6f64 652c 2066 6173  , mode=mode, fas
+0000ac70: 743d 4661 6c73 6529 0a20 2020 2020 2020  t=False).       
+0000ac80: 206a 7573 745f 6e6c 203d 2022 5c6e 220a   just_nl = "\n".
+0000ac90: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000aca0: 662e 6173 7365 7274 5261 6973 6573 2863  f.assertRaises(c
+0000acb0: 6572 6369 732e 4e6f 7468 696e 6743 6861  ercis.NothingCha
+0000acc0: 6e67 6564 293a 0a20 2020 2020 2020 2020  nged):.         
+0000acd0: 2020 2063 6572 6369 732e 666f 726d 6174     cercis.format
+0000ace0: 5f66 696c 655f 636f 6e74 656e 7473 286a  _file_contents(j
+0000acf0: 7573 745f 6e6c 2c20 6d6f 6465 3d6d 6f64  ust_nl, mode=mod
+0000ad00: 652c 2066 6173 743d 4661 6c73 6529 0a20  e, fast=False). 
+0000ad10: 2020 2020 2020 2073 616d 6520 3d20 226a         same = "j
+0000ad20: 203d 205b 312c 2032 2c20 335d 5c6e 220a   = [1, 2, 3]\n".
+0000ad30: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000ad40: 662e 6173 7365 7274 5261 6973 6573 2863  f.assertRaises(c
+0000ad50: 6572 6369 732e 4e6f 7468 696e 6743 6861  ercis.NothingCha
+0000ad60: 6e67 6564 293a 0a20 2020 2020 2020 2020  nged):.         
+0000ad70: 2020 2063 6572 6369 732e 666f 726d 6174     cercis.format
+0000ad80: 5f66 696c 655f 636f 6e74 656e 7473 2873  _file_contents(s
+0000ad90: 616d 652c 206d 6f64 653d 6d6f 6465 2c20  ame, mode=mode, 
+0000ada0: 6661 7374 3d46 616c 7365 290a 2020 2020  fast=False).    
+0000adb0: 2020 2020 6469 6666 6572 656e 7420 3d20      different = 
+0000adc0: 226a 203d 205b 312c 322c 335d 220a 2020  "j = [1,2,3]".  
+0000add0: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
+0000ade0: 2073 616d 650a 2020 2020 2020 2020 6163   same.        ac
+0000adf0: 7475 616c 203d 2063 6572 6369 732e 666f  tual = cercis.fo
+0000ae00: 726d 6174 5f66 696c 655f 636f 6e74 656e  rmat_file_conten
+0000ae10: 7473 2864 6966 6665 7265 6e74 2c20 6d6f  ts(different, mo
+0000ae20: 6465 3d6d 6f64 652c 2066 6173 743d 4661  de=mode, fast=Fa
+0000ae30: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
+0000ae40: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+0000ae50: 7065 6374 6564 2c20 6163 7475 616c 290a  pected, actual).
+0000ae60: 2020 2020 2020 2020 696e 7661 6c69 6420          invalid 
+0000ae70: 3d20 2272 6574 7572 6e20 6966 2079 6f75  = "return if you
+0000ae80: 2063 616e 220a 2020 2020 2020 2020 7769   can".        wi
+0000ae90: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+0000aea0: 6973 6573 2863 6572 6369 732e 496e 7661  ises(cercis.Inva
+0000aeb0: 6c69 6449 6e70 7574 2920 6173 2065 3a0a  lidInput) as e:.
+0000aec0: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+0000aed0: 6973 2e66 6f72 6d61 745f 6669 6c65 5f63  is.format_file_c
+0000aee0: 6f6e 7465 6e74 7328 696e 7661 6c69 642c  ontents(invalid,
+0000aef0: 206d 6f64 653d 6d6f 6465 2c20 6661 7374   mode=mode, fast
+0000af00: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+0000af10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000af20: 2873 7472 2865 2e65 7863 6570 7469 6f6e  (str(e.exception
+0000af30: 292c 2022 4361 6e6e 6f74 2070 6172 7365  ), "Cannot parse
+0000af40: 3a20 313a 373a 2072 6574 7572 6e20 6966  : 1:7: return if
+0000af50: 2079 6f75 2063 616e 2229 0a0a 2020 2020   you can")..    
+0000af60: 2020 2020 6d6f 6465 203d 2063 6572 6369      mode = cerci
+0000af70: 732e 4d6f 6465 2870 7265 7669 6577 3d54  s.Mode(preview=T
+0000af80: 7275 6529 0a20 2020 2020 2020 206a 7573  rue).        jus
+0000af90: 745f 6372 6c66 203d 2022 5c72 5c6e 220a  t_crlf = "\r\n".
+0000afa0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000afb0: 662e 6173 7365 7274 5261 6973 6573 2863  f.assertRaises(c
+0000afc0: 6572 6369 732e 4e6f 7468 696e 6743 6861  ercis.NothingCha
+0000afd0: 6e67 6564 293a 0a20 2020 2020 2020 2020  nged):.         
+0000afe0: 2020 2063 6572 6369 732e 666f 726d 6174     cercis.format
+0000aff0: 5f66 696c 655f 636f 6e74 656e 7473 286a  _file_contents(j
+0000b000: 7573 745f 6372 6c66 2c20 6d6f 6465 3d6d  ust_crlf, mode=m
+0000b010: 6f64 652c 2066 6173 743d 4661 6c73 6529  ode, fast=False)
+0000b020: 0a20 2020 2020 2020 206a 7573 745f 7768  .        just_wh
+0000b030: 6974 6573 7061 6365 5f6e 6c20 3d20 225c  itespace_nl = "\
+0000b040: 6e5c 745c 6e20 5c6e 5c74 205c 6e20 5c74  n\t\n \n\t \n \t
+0000b050: 5c6e 5c6e 220a 2020 2020 2020 2020 6163  \n\n".        ac
+0000b060: 7475 616c 203d 2063 6572 6369 732e 666f  tual = cercis.fo
+0000b070: 726d 6174 5f66 696c 655f 636f 6e74 656e  rmat_file_conten
+0000b080: 7473 286a 7573 745f 7768 6974 6573 7061  ts(just_whitespa
+0000b090: 6365 5f6e 6c2c 206d 6f64 653d 6d6f 6465  ce_nl, mode=mode
+0000b0a0: 2c20 6661 7374 3d46 616c 7365 290a 2020  , fast=False).  
+0000b0b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000b0c0: 7445 7175 616c 2822 5c6e 222c 2061 6374  tEqual("\n", act
+0000b0d0: 7561 6c29 0a20 2020 2020 2020 206a 7573  ual).        jus
+0000b0e0: 745f 7768 6974 6573 7061 6365 5f63 726c  t_whitespace_crl
+0000b0f0: 6620 3d20 225c 725c 6e5c 745c 725c 6e20  f = "\r\n\t\r\n 
+0000b100: 5c72 5c6e 5c74 205c 725c 6e20 5c74 5c72  \r\n\t \r\n \t\r
+0000b110: 5c6e 5c72 5c6e 220a 2020 2020 2020 2020  \n\r\n".        
+0000b120: 6163 7475 616c 203d 2063 6572 6369 732e  actual = cercis.
+0000b130: 666f 726d 6174 5f66 696c 655f 636f 6e74  format_file_cont
+0000b140: 656e 7473 280a 2020 2020 2020 2020 2020  ents(.          
+0000b150: 2020 6a75 7374 5f77 6869 7465 7370 6163    just_whitespac
+0000b160: 655f 6372 6c66 2c20 6d6f 6465 3d6d 6f64  e_crlf, mode=mod
+0000b170: 652c 2066 6173 743d 4661 6c73 650a 2020  e, fast=False.  
+0000b180: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000b190: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000b1a0: 2822 5c72 5c6e 222c 2061 6374 7561 6c29  ("\r\n", actual)
+0000b1b0: 0a0a 2020 2020 6465 6620 7465 7374 5f65  ..    def test_e
+0000b1c0: 6e64 6d61 726b 6572 2873 656c 6629 202d  ndmarker(self) -
+0000b1d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000b1e0: 6e20 3d20 6365 7263 6973 2e6c 6962 3274  n = cercis.lib2t
+0000b1f0: 6f33 5f70 6172 7365 2822 5c6e 2229 0a20  o3_parse("\n"). 
+0000b200: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000b210: 7274 4571 7561 6c28 6e2e 7479 7065 2c20  rtEqual(n.type, 
+0000b220: 6365 7263 6973 2e73 796d 732e 6669 6c65  cercis.syms.file
+0000b230: 5f69 6e70 7574 290a 2020 2020 2020 2020  _input).        
+0000b240: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000b250: 286c 656e 286e 2e63 6869 6c64 7265 6e29  (len(n.children)
+0000b260: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+0000b270: 662e 6173 7365 7274 4571 7561 6c28 6e2e  f.assertEqual(n.
+0000b280: 6368 696c 6472 656e 5b30 5d2e 7479 7065  children[0].type
+0000b290: 2c20 6365 7263 6973 2e74 6f6b 656e 2e45  , cercis.token.E
+0000b2a0: 4e44 4d41 524b 4552 290a 0a20 2020 2040  NDMARKER)..    @
+0000b2b0: 7079 7465 7374 2e6d 6172 6b2e 696e 636f  pytest.mark.inco
+0000b2c0: 6d70 6174 6962 6c65 5f77 6974 685f 6d79  mpatible_with_my
+0000b2d0: 7079 630a 2020 2020 4075 6e69 7474 6573  pyc.    @unittes
+0000b2e0: 742e 736b 6970 4966 286f 732e 656e 7669  t.skipIf(os.envi
+0000b2f0: 726f 6e2e 6765 7428 2253 4b49 505f 4153  ron.get("SKIP_AS
+0000b300: 545f 5052 494e 5422 292c 2022 7573 6572  T_PRINT"), "user
+0000b310: 2073 6574 2053 4b49 505f 4153 545f 5052   set SKIP_AST_PR
+0000b320: 494e 5422 290a 2020 2020 6465 6620 7465  INT").    def te
+0000b330: 7374 5f61 7373 6572 7446 6f72 6d61 7445  st_assertFormatE
+0000b340: 7175 616c 2873 656c 6629 202d 3e20 4e6f  qual(self) -> No
+0000b350: 6e65 3a0a 2020 2020 2020 2020 6f75 745f  ne:.        out_
+0000b360: 6c69 6e65 7320 3d20 5b5d 0a20 2020 2020  lines = [].     
+0000b370: 2020 2065 7272 5f6c 696e 6573 203d 205b     err_lines = [
+0000b380: 5d0a 0a20 2020 2020 2020 2064 6566 206f  ]..        def o
+0000b390: 7574 286d 7367 3a20 7374 722c 202a 2a6b  ut(msg: str, **k
+0000b3a0: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
+0000b3b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000b3c0: 206f 7574 5f6c 696e 6573 2e61 7070 656e   out_lines.appen
+0000b3d0: 6428 6d73 6729 0a0a 2020 2020 2020 2020  d(msg)..        
+0000b3e0: 6465 6620 6572 7228 6d73 673a 2073 7472  def err(msg: str
+0000b3f0: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
+0000b400: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000b410: 2020 2020 2020 6572 725f 6c69 6e65 732e        err_lines.
+0000b420: 6170 7065 6e64 286d 7367 290a 0a20 2020  append(msg)..   
+0000b430: 2020 2020 2077 6974 6820 7061 7463 6828       with patch(
+0000b440: 2263 6572 6369 732e 6f75 7470 7574 2e5f  "cercis.output._
+0000b450: 6f75 7422 2c20 6f75 7429 2c20 7061 7463  out", out), patc
+0000b460: 6828 2263 6572 6369 732e 6f75 7470 7574  h("cercis.output
+0000b470: 2e5f 6572 7222 2c20 6572 7229 3a0a 2020  ._err", err):.  
+0000b480: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+0000b490: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+0000b4a0: 2841 7373 6572 7469 6f6e 4572 726f 7229  (AssertionError)
+0000b4b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b4c0: 2020 7365 6c66 2e61 7373 6572 7446 6f72    self.assertFor
+0000b4d0: 6d61 7445 7175 616c 2822 6a20 3d20 5b31  matEqual("j = [1
+0000b4e0: 2c20 322c 2033 5d22 2c20 226a 203d 205b  , 2, 3]", "j = [
+0000b4f0: 312c 2032 2c20 332c 5d22 290a 0a20 2020  1, 2, 3,]")..   
+0000b500: 2020 2020 206f 7574 5f73 7472 203d 2022       out_str = "
+0000b510: 222e 6a6f 696e 286f 7574 5f6c 696e 6573  ".join(out_lines
+0000b520: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000b530: 7373 6572 7449 6e28 2245 7870 6563 7465  ssertIn("Expecte
+0000b540: 6420 7472 6565 3a22 2c20 6f75 745f 7374  d tree:", out_st
+0000b550: 7229 0a20 2020 2020 2020 2073 656c 662e  r).        self.
+0000b560: 6173 7365 7274 496e 2822 4163 7475 616c  assertIn("Actual
+0000b570: 2074 7265 653a 222c 206f 7574 5f73 7472   tree:", out_str
+0000b580: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000b590: 7373 6572 7445 7175 616c 2822 222e 6a6f  ssertEqual("".jo
+0000b5a0: 696e 2865 7272 5f6c 696e 6573 292c 2022  in(err_lines), "
+0000b5b0: 2229 0a0a 2020 2020 4065 7665 6e74 5f6c  ")..    @event_l
+0000b5c0: 6f6f 7028 290a 2020 2020 4070 6174 6368  oop().    @patch
+0000b5d0: 2822 636f 6e63 7572 7265 6e74 2e66 7574  ("concurrent.fut
+0000b5e0: 7572 6573 2e50 726f 6365 7373 506f 6f6c  ures.ProcessPool
+0000b5f0: 4578 6563 7574 6f72 222c 204d 6167 6963  Executor", Magic
+0000b600: 4d6f 636b 2873 6964 655f 6566 6665 6374  Mock(side_effect
+0000b610: 3d4f 5345 7272 6f72 2929 0a20 2020 2064  =OSError)).    d
+0000b620: 6566 2074 6573 745f 776f 726b 735f 696e  ef test_works_in
+0000b630: 5f6d 6f6e 6f5f 7072 6f63 6573 735f 6f6e  _mono_process_on
+0000b640: 6c79 5f65 6e76 6972 6f6e 6d65 6e74 2873  ly_environment(s
+0000b650: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000b660: 2020 2020 2020 7769 7468 2063 6163 6865        with cache
+0000b670: 5f64 6972 2829 2061 7320 776f 726b 7370  _dir() as worksp
+0000b680: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
+0000b690: 2066 6f72 2066 2069 6e20 5b0a 2020 2020   for f in [.    
+0000b6a0: 2020 2020 2020 2020 2020 2020 2877 6f72              (wor
+0000b6b0: 6b73 7061 6365 202f 2022 6f6e 652e 7079  kspace / "one.py
+0000b6c0: 2229 2e72 6573 6f6c 7665 2829 2c0a 2020  ").resolve(),.  
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2877                (w
+0000b6e0: 6f72 6b73 7061 6365 202f 2022 7477 6f2e  orkspace / "two.
+0000b6f0: 7079 2229 2e72 6573 6f6c 7665 2829 2c0a  py").resolve(),.
+0000b700: 2020 2020 2020 2020 2020 2020 5d3a 0a20              ]:. 
+0000b710: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b720: 2e77 7269 7465 5f74 6578 7428 2770 7269  .write_text('pri
+0000b730: 6e74 2822 6865 6c6c 6f22 295c 6e27 290a  nt("hello")\n').
+0000b740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b750: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
+0000b760: 7228 776f 726b 7370 6163 6529 5d29 0a0a  r(workspace)])..
+0000b770: 2020 2020 4065 7665 6e74 5f6c 6f6f 7028      @event_loop(
+0000b780: 290a 2020 2020 6465 6620 7465 7374 5f63  ).    def test_c
+0000b790: 6865 636b 5f64 6966 665f 7573 655f 746f  heck_diff_use_to
+0000b7a0: 6765 7468 6572 2873 656c 6629 202d 3e20  gether(self) -> 
+0000b7b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7371  None:.        sq
+0000b7c0: 203d 2022 2d2d 7369 6e67 6c65 2d71 756f   = "--single-quo
+0000b7d0: 7465 3d46 616c 7365 220a 2020 2020 2020  te=False".      
+0000b7e0: 2020 6c6c 203d 2022 2d2d 6c69 6e65 2d6c    ll = "--line-l
+0000b7f0: 656e 6774 683d 3838 220a 2020 2020 2020  ength=88".      
+0000b800: 2020 7769 7468 2063 6163 6865 5f64 6972    with cache_dir
+0000b810: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000b820: 2320 4669 6c65 7320 7768 6963 6820 7769  # Files which wi
+0000b830: 6c6c 2062 6520 7265 666f 726d 6174 7465  ll be reformatte
+0000b840: 642e 0a20 2020 2020 2020 2020 2020 2073  d..            s
+0000b850: 7263 3120 3d20 6765 745f 6361 7365 5f70  rc1 = get_case_p
+0000b860: 6174 6828 226d 6973 6365 6c6c 616e 656f  ath("miscellaneo
+0000b870: 7573 222c 2022 7374 7269 6e67 5f71 756f  us", "string_quo
+0000b880: 7465 7322 290a 2020 2020 2020 2020 2020  tes").          
+0000b890: 2020 7365 6c66 2e69 6e76 6f6b 6542 6c61    self.invokeBla
+0000b8a0: 636b 285b 7374 7228 7372 6331 292c 2022  ck([str(src1), "
+0000b8b0: 2d2d 6469 6666 222c 2022 2d2d 6368 6563  --diff", "--chec
+0000b8c0: 6b22 2c20 7371 2c20 6c6c 5d2c 2065 7869  k", sq, ll], exi
+0000b8d0: 745f 636f 6465 3d31 290a 2020 2020 2020  t_code=1).      
+0000b8e0: 2020 2020 2020 2320 4669 6c65 7320 7768        # Files wh
+0000b8f0: 6963 6820 7769 6c6c 206e 6f74 2062 6520  ich will not be 
+0000b900: 7265 666f 726d 6174 7465 642e 0a20 2020  reformatted..   
+0000b910: 2020 2020 2020 2020 2073 7263 3220 3d20           src2 = 
+0000b920: 6765 745f 6361 7365 5f70 6174 6828 2273  get_case_path("s
+0000b930: 696d 706c 655f 6361 7365 7322 2c20 2263  imple_cases", "c
+0000b940: 6f6d 706f 7369 7469 6f6e 2229 0a20 2020  omposition").   
+0000b950: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+0000b960: 766f 6b65 426c 6163 6b28 5b73 7472 2873  vokeBlack([str(s
+0000b970: 7263 3229 2c20 222d 2d64 6966 6622 2c20  rc2), "--diff", 
+0000b980: 222d 2d63 6865 636b 222c 2073 712c 206c  "--check", sq, l
+0000b990: 6c5d 290a 2020 2020 2020 2020 2020 2020  l]).            
+0000b9a0: 2320 4d75 6c74 6920 6669 6c65 2063 6f6d  # Multi file com
+0000b9b0: 6d61 6e64 2e0a 2020 2020 2020 2020 2020  mand..          
+0000b9c0: 2020 7365 6c66 2e69 6e76 6f6b 6542 6c61    self.invokeBla
+0000b9d0: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
+0000b9e0: 2020 2020 5b73 7472 2873 7263 3129 2c20      [str(src1), 
+0000b9f0: 7374 7228 7372 6332 292c 2022 2d2d 6469  str(src2), "--di
+0000ba00: 6666 222c 2022 2d2d 6368 6563 6b22 2c20  ff", "--check", 
+0000ba10: 7371 2c20 6c6c 5d2c 0a20 2020 2020 2020  sq, ll],.       
+0000ba20: 2020 2020 2020 2020 2065 7869 745f 636f           exit_co
+0000ba30: 6465 3d31 2c0a 2020 2020 2020 2020 2020  de=1,.          
+0000ba40: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+0000ba50: 745f 6e6f 5f73 7263 5f66 6169 6c73 2873  t_no_src_fails(s
+0000ba60: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000ba70: 2020 2020 2020 7769 7468 2063 6163 6865        with cache
+0000ba80: 5f64 6972 2829 3a0a 2020 2020 2020 2020  _dir():.        
+0000ba90: 2020 2020 7365 6c66 2e69 6e76 6f6b 6542      self.invokeB
+0000baa0: 6c61 636b 285b 5d2c 2065 7869 745f 636f  lack([], exit_co
+0000bab0: 6465 3d31 290a 0a20 2020 2064 6566 2074  de=1)..    def t
+0000bac0: 6573 745f 7372 635f 616e 645f 636f 6465  est_src_and_code
+0000bad0: 5f66 6169 6c73 2873 656c 6629 202d 3e20  _fails(self) -> 
+0000bae0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7769  None:.        wi
+0000baf0: 7468 2063 6163 6865 5f64 6972 2829 3a0a  th cache_dir():.
+0000bb00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000bb10: 2e69 6e76 6f6b 6542 6c61 636b 285b 222e  .invokeBlack([".
+0000bb20: 222c 2022 2d63 222c 2022 3022 5d2c 2065  ", "-c", "0"], e
+0000bb30: 7869 745f 636f 6465 3d31 290a 0a20 2020  xit_code=1)..   
+0000bb40: 2064 6566 2074 6573 745f 6272 6f6b 656e   def test_broken
+0000bb50: 5f73 796d 6c69 6e6b 2873 656c 6629 202d  _symlink(self) -
+0000bb60: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000bb70: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
+0000bb80: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
+0000bb90: 2020 2020 2020 2020 2020 2073 796d 6c69             symli
+0000bba0: 6e6b 203d 2077 6f72 6b73 7061 6365 202f  nk = workspace /
+0000bbb0: 2022 6272 6f6b 656e 5f6c 696e 6b2e 7079   "broken_link.py
+0000bbc0: 220a 2020 2020 2020 2020 2020 2020 7472  ".            tr
+0000bbd0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0000bbe0: 2020 2073 796d 6c69 6e6b 2e73 796d 6c69     symlink.symli
+0000bbf0: 6e6b 5f74 6f28 226e 6f6e 6578 6973 7465  nk_to("nonexiste
+0000bc00: 6e74 2e70 7922 290a 2020 2020 2020 2020  nt.py").        
+0000bc10: 2020 2020 6578 6365 7074 2028 4f53 4572      except (OSEr
+0000bc20: 726f 722c 204e 6f74 496d 706c 656d 656e  ror, NotImplemen
+0000bc30: 7465 6445 7272 6f72 2920 6173 2065 3a0a  tedError) as e:.
+0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc50: 7365 6c66 2e73 6b69 7054 6573 7428 6622  self.skipTest(f"
+0000bc60: 4361 6e27 7420 6372 6561 7465 2073 796d  Can't create sym
+0000bc70: 6c69 6e6b 733a 207b 657d 2229 0a20 2020  links: {e}").   
+0000bc80: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+0000bc90: 766f 6b65 426c 6163 6b28 5b73 7472 2877  vokeBlack([str(w
+0000bca0: 6f72 6b73 7061 6365 2e72 6573 6f6c 7665  orkspace.resolve
+0000bcb0: 2829 295d 290a 0a20 2020 2064 6566 2074  ())])..    def t
+0000bcc0: 6573 745f 7369 6e67 6c65 5f66 696c 655f  est_single_file_
+0000bcd0: 666f 7263 655f 7079 6928 7365 6c66 2920  force_pyi(self) 
+0000bce0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000bcf0: 2070 7969 5f6d 6f64 6520 3d20 7265 706c   pyi_mode = repl
+0000bd00: 6163 6528 4445 4641 554c 545f 4d4f 4445  ace(DEFAULT_MODE
+0000bd10: 2c20 6973 5f70 7969 3d54 7275 6529 0a20  , is_pyi=True). 
+0000bd20: 2020 2020 2020 2063 6f6e 7465 6e74 732c         contents,
+0000bd30: 2065 7870 6563 7465 6420 3d20 7265 6164   expected = read
+0000bd40: 5f64 6174 6128 226d 6973 6365 6c6c 616e  _data("miscellan
+0000bd50: 656f 7573 222c 2022 666f 7263 655f 7079  eous", "force_py
+0000bd60: 6922 290a 2020 2020 2020 2020 7769 7468  i").        with
+0000bd70: 2063 6163 6865 5f64 6972 2829 2061 7320   cache_dir() as 
+0000bd80: 776f 726b 7370 6163 653a 0a20 2020 2020  workspace:.     
+0000bd90: 2020 2020 2020 2070 6174 6820 3d20 2877         path = (w
+0000bda0: 6f72 6b73 7061 6365 202f 2022 6669 6c65  orkspace / "file
+0000bdb0: 2e70 7922 292e 7265 736f 6c76 6528 290a  .py").resolve().
+0000bdc0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000bdd0: 206f 7065 6e28 7061 7468 2c20 2277 2229   open(path, "w")
+0000bde0: 2061 7320 6668 3a0a 2020 2020 2020 2020   as fh:.        
+0000bdf0: 2020 2020 2020 2020 6668 2e77 7269 7465          fh.write
+0000be00: 2863 6f6e 7465 6e74 7329 0a20 2020 2020  (contents).     
+0000be10: 2020 2020 2020 2073 656c 662e 696e 766f         self.invo
+0000be20: 6b65 426c 6163 6b28 5b73 7472 2870 6174  keBlack([str(pat
+0000be30: 6829 2c20 222d 2d70 7969 225d 290a 2020  h), "--pyi"]).  
+0000be40: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+0000be50: 7065 6e28 7061 7468 2c20 2272 2229 2061  pen(path, "r") a
+0000be60: 7320 6668 3a0a 2020 2020 2020 2020 2020  s fh:.          
+0000be70: 2020 2020 2020 6163 7475 616c 203d 2066        actual = f
+0000be80: 682e 7265 6164 2829 0a20 2020 2020 2020  h.read().       
+0000be90: 2020 2020 2023 2076 6572 6966 7920 6361       # verify ca
+0000bea0: 6368 6520 7769 7468 202d 2d70 7969 2069  che with --pyi i
+0000beb0: 7320 7365 7061 7261 7465 0a20 2020 2020  s separate.     
+0000bec0: 2020 2020 2020 2070 7969 5f63 6163 6865         pyi_cache
+0000bed0: 203d 2063 6572 6369 732e 7265 6164 5f63   = cercis.read_c
+0000bee0: 6163 6865 2870 7969 5f6d 6f64 6529 0a20  ache(pyi_mode). 
+0000bef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000bf00: 6173 7365 7274 496e 2873 7472 2870 6174  assertIn(str(pat
+0000bf10: 6829 2c20 7079 695f 6361 6368 6529 0a20  h), pyi_cache). 
+0000bf20: 2020 2020 2020 2020 2020 206e 6f72 6d61             norma
+0000bf30: 6c5f 6361 6368 6520 3d20 6365 7263 6973  l_cache = cercis
+0000bf40: 2e72 6561 645f 6361 6368 6528 4445 4641  .read_cache(DEFA
+0000bf50: 554c 545f 4d4f 4445 290a 2020 2020 2020  ULT_MODE).      
+0000bf60: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000bf70: 744e 6f74 496e 2873 7472 2870 6174 6829  tNotIn(str(path)
+0000bf80: 2c20 6e6f 726d 616c 5f63 6163 6865 290a  , normal_cache).
+0000bf90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000bfa0: 6572 7446 6f72 6d61 7445 7175 616c 2865  ertFormatEqual(e
+0000bfb0: 7870 6563 7465 642c 2061 6374 7561 6c29  xpected, actual)
+0000bfc0: 0a20 2020 2020 2020 2063 6572 6369 732e  .        cercis.
+0000bfd0: 6173 7365 7274 5f65 7175 6976 616c 656e  assert_equivalen
+0000bfe0: 7428 636f 6e74 656e 7473 2c20 6163 7475  t(contents, actu
+0000bff0: 616c 290a 2020 2020 2020 2020 6365 7263  al).        cerc
+0000c000: 6973 2e61 7373 6572 745f 7374 6162 6c65  is.assert_stable
+0000c010: 2863 6f6e 7465 6e74 732c 2061 6374 7561  (contents, actua
+0000c020: 6c2c 2070 7969 5f6d 6f64 6529 0a0a 2020  l, pyi_mode)..  
+0000c030: 2020 4065 7665 6e74 5f6c 6f6f 7028 290a    @event_loop().
+0000c040: 2020 2020 6465 6620 7465 7374 5f6d 756c      def test_mul
+0000c050: 7469 5f66 696c 655f 666f 7263 655f 7079  ti_file_force_py
+0000c060: 6928 7365 6c66 2920 2d3e 204e 6f6e 653a  i(self) -> None:
+0000c070: 0a20 2020 2020 2020 2072 6567 5f6d 6f64  .        reg_mod
+0000c080: 6520 3d20 4445 4641 554c 545f 4d4f 4445  e = DEFAULT_MODE
+0000c090: 0a20 2020 2020 2020 2070 7969 5f6d 6f64  .        pyi_mod
+0000c0a0: 6520 3d20 7265 706c 6163 6528 4445 4641  e = replace(DEFA
+0000c0b0: 554c 545f 4d4f 4445 2c20 6973 5f70 7969  ULT_MODE, is_pyi
+0000c0c0: 3d54 7275 6529 0a20 2020 2020 2020 2063  =True).        c
+0000c0d0: 6f6e 7465 6e74 732c 2065 7870 6563 7465  ontents, expecte
+0000c0e0: 6420 3d20 7265 6164 5f64 6174 6128 226d  d = read_data("m
+0000c0f0: 6973 6365 6c6c 616e 656f 7573 222c 2022  iscellaneous", "
+0000c100: 666f 7263 655f 7079 6922 290a 2020 2020  force_pyi").    
+0000c110: 2020 2020 7769 7468 2063 6163 6865 5f64      with cache_d
+0000c120: 6972 2829 2061 7320 776f 726b 7370 6163  ir() as workspac
+0000c130: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+0000c140: 6174 6873 203d 205b 0a20 2020 2020 2020  aths = [.       
+0000c150: 2020 2020 2020 2020 2028 776f 726b 7370           (worksp
+0000c160: 6163 6520 2f20 2266 696c 6531 2e70 7922  ace / "file1.py"
+0000c170: 292e 7265 736f 6c76 6528 292c 0a20 2020  ).resolve(),.   
+0000c180: 2020 2020 2020 2020 2020 2020 2028 776f               (wo
+0000c190: 726b 7370 6163 6520 2f20 2266 696c 6532  rkspace / "file2
+0000c1a0: 2e70 7922 292e 7265 736f 6c76 6528 292c  .py").resolve(),
+0000c1b0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+0000c1c0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+0000c1d0: 6174 6820 696e 2070 6174 6873 3a0a 2020  ath in paths:.  
+0000c1e0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+0000c1f0: 7468 206f 7065 6e28 7061 7468 2c20 2277  th open(path, "w
+0000c200: 2229 2061 7320 6668 3a0a 2020 2020 2020  ") as fh:.      
+0000c210: 2020 2020 2020 2020 2020 2020 2020 6668                fh
+0000c220: 2e77 7269 7465 2863 6f6e 7465 6e74 7329  .write(contents)
+0000c230: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c240: 662e 696e 766f 6b65 426c 6163 6b28 5b73  f.invokeBlack([s
+0000c250: 7472 2870 2920 666f 7220 7020 696e 2070  tr(p) for p in p
+0000c260: 6174 6873 5d20 2b20 5b22 2d2d 7079 6922  aths] + ["--pyi"
+0000c270: 5d29 0a20 2020 2020 2020 2020 2020 2066  ]).            f
+0000c280: 6f72 2070 6174 6820 696e 2070 6174 6873  or path in paths
+0000c290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c2a0: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
+0000c2b0: 2c20 2272 2229 2061 7320 6668 3a0a 2020  , "r") as fh:.  
+0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2d0: 2020 6163 7475 616c 203d 2066 682e 7265    actual = fh.re
+0000c2e0: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
+0000c2f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000c300: 4571 7561 6c28 6163 7475 616c 2c20 6578  Equal(actual, ex
+0000c310: 7065 6374 6564 290a 2020 2020 2020 2020  pected).        
+0000c320: 2020 2020 2320 7665 7269 6679 2063 6163      # verify cac
+0000c330: 6865 2077 6974 6820 2d2d 7079 6920 6973  he with --pyi is
+0000c340: 2073 6570 6172 6174 650a 2020 2020 2020   separate.      
+0000c350: 2020 2020 2020 7079 695f 6361 6368 6520        pyi_cache 
+0000c360: 3d20 6365 7263 6973 2e72 6561 645f 6361  = cercis.read_ca
+0000c370: 6368 6528 7079 695f 6d6f 6465 290a 2020  che(pyi_mode).  
+0000c380: 2020 2020 2020 2020 2020 6e6f 726d 616c            normal
+0000c390: 5f63 6163 6865 203d 2063 6572 6369 732e  _cache = cercis.
+0000c3a0: 7265 6164 5f63 6163 6865 2872 6567 5f6d  read_cache(reg_m
+0000c3b0: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
+0000c3c0: 2066 6f72 2070 6174 6820 696e 2070 6174   for path in pat
+0000c3d0: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
+0000c3e0: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
+0000c3f0: 6e28 7374 7228 7061 7468 292c 2070 7969  n(str(path), pyi
+0000c400: 5f63 6163 6865 290a 2020 2020 2020 2020  _cache).        
+0000c410: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000c420: 6572 744e 6f74 496e 2873 7472 2870 6174  ertNotIn(str(pat
+0000c430: 6829 2c20 6e6f 726d 616c 5f63 6163 6865  h), normal_cache
+0000c440: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000c450: 7069 7065 5f66 6f72 6365 5f70 7969 2873  pipe_force_pyi(s
+0000c460: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000c470: 2020 2020 2020 736f 7572 6365 2c20 6578        source, ex
+0000c480: 7065 6374 6564 203d 2072 6561 645f 6461  pected = read_da
+0000c490: 7461 2822 6d69 7363 656c 6c61 6e65 6f75  ta("miscellaneou
+0000c4a0: 7322 2c20 2266 6f72 6365 5f70 7969 2229  s", "force_pyi")
+0000c4b0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000c4c0: 3d20 436c 6952 756e 6e65 7228 292e 696e  = CliRunner().in
+0000c4d0: 766f 6b65 280a 2020 2020 2020 2020 2020  voke(.          
+0000c4e0: 2020 6365 7263 6973 2e6d 6169 6e2c 205b    cercis.main, [
+0000c4f0: 222d 222c 2022 2d71 222c 2022 2d2d 7079  "-", "-q", "--py
+0000c500: 6922 5d2c 2069 6e70 7574 3d42 7974 6573  i"], input=Bytes
+0000c510: 494f 2873 6f75 7263 652e 656e 636f 6465  IO(source.encode
+0000c520: 2822 7574 6638 2229 290a 2020 2020 2020  ("utf8")).      
+0000c530: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+0000c540: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0000c550: 756c 742e 6578 6974 5f63 6f64 652c 2030  ult.exit_code, 0
+0000c560: 290a 2020 2020 2020 2020 6163 7475 616c  ).        actual
+0000c570: 203d 2072 6573 756c 742e 6f75 7470 7574   = result.output
+0000c580: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000c590: 7365 7274 466f 726d 6174 4571 7561 6c28  sertFormatEqual(
+0000c5a0: 6163 7475 616c 2c20 6578 7065 6374 6564  actual, expected
+0000c5b0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000c5c0: 7369 6e67 6c65 5f66 696c 655f 666f 7263  single_file_forc
+0000c5d0: 655f 7079 3336 2873 656c 6629 202d 3e20  e_py36(self) -> 
+0000c5e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7265  None:.        re
+0000c5f0: 675f 6d6f 6465 203d 2044 4546 4155 4c54  g_mode = DEFAULT
+0000c600: 5f4d 4f44 450a 2020 2020 2020 2020 7079  _MODE.        py
+0000c610: 3336 5f6d 6f64 6520 3d20 7265 706c 6163  36_mode = replac
+0000c620: 6528 4445 4641 554c 545f 4d4f 4445 2c20  e(DEFAULT_MODE, 
+0000c630: 7461 7267 6574 5f76 6572 7369 6f6e 733d  target_versions=
+0000c640: 5059 3336 5f56 4552 5349 4f4e 5329 0a20  PY36_VERSIONS). 
+0000c650: 2020 2020 2020 2073 6f75 7263 652c 2065         source, e
+0000c660: 7870 6563 7465 6420 3d20 7265 6164 5f64  xpected = read_d
+0000c670: 6174 6128 226d 6973 6365 6c6c 616e 656f  ata("miscellaneo
+0000c680: 7573 222c 2022 666f 7263 655f 7079 3336  us", "force_py36
+0000c690: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
+0000c6a0: 6361 6368 655f 6469 7228 2920 6173 2077  cache_dir() as w
+0000c6b0: 6f72 6b73 7061 6365 3a0a 2020 2020 2020  orkspace:.      
+0000c6c0: 2020 2020 2020 7061 7468 203d 2028 776f        path = (wo
+0000c6d0: 726b 7370 6163 6520 2f20 2266 696c 652e  rkspace / "file.
+0000c6e0: 7079 2229 2e72 6573 6f6c 7665 2829 0a20  py").resolve(). 
+0000c6f0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000c700: 6f70 656e 2870 6174 682c 2022 7722 2920  open(path, "w") 
+0000c710: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
+0000c720: 2020 2020 2020 2066 682e 7772 6974 6528         fh.write(
+0000c730: 736f 7572 6365 290a 2020 2020 2020 2020  source).        
+0000c740: 2020 2020 7365 6c66 2e69 6e76 6f6b 6542      self.invokeB
+0000c750: 6c61 636b 285b 7374 7228 7061 7468 292c  lack([str(path),
+0000c760: 202a 5059 3336 5f41 5247 535d 290a 2020   *PY36_ARGS]).  
+0000c770: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+0000c780: 7065 6e28 7061 7468 2c20 2272 2229 2061  pen(path, "r") a
+0000c790: 7320 6668 3a0a 2020 2020 2020 2020 2020  s fh:.          
+0000c7a0: 2020 2020 2020 6163 7475 616c 203d 2066        actual = f
+0000c7b0: 682e 7265 6164 2829 0a20 2020 2020 2020  h.read().       
+0000c7c0: 2020 2020 2023 2076 6572 6966 7920 6361       # verify ca
+0000c7d0: 6368 6520 7769 7468 202d 2d74 6172 6765  che with --targe
+0000c7e0: 742d 7665 7273 696f 6e20 6973 2073 6570  t-version is sep
+0000c7f0: 6172 6174 650a 2020 2020 2020 2020 2020  arate.          
+0000c800: 2020 7079 3336 5f63 6163 6865 203d 2063    py36_cache = c
+0000c810: 6572 6369 732e 7265 6164 5f63 6163 6865  ercis.read_cache
+0000c820: 2870 7933 365f 6d6f 6465 290a 2020 2020  (py36_mode).    
+0000c830: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000c840: 6572 7449 6e28 7374 7228 7061 7468 292c  ertIn(str(path),
+0000c850: 2070 7933 365f 6361 6368 6529 0a20 2020   py36_cache).   
+0000c860: 2020 2020 2020 2020 206e 6f72 6d61 6c5f           normal_
+0000c870: 6361 6368 6520 3d20 6365 7263 6973 2e72  cache = cercis.r
+0000c880: 6561 645f 6361 6368 6528 7265 675f 6d6f  ead_cache(reg_mo
+0000c890: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
+0000c8a0: 7365 6c66 2e61 7373 6572 744e 6f74 496e  self.assertNotIn
+0000c8b0: 2873 7472 2870 6174 6829 2c20 6e6f 726d  (str(path), norm
+0000c8c0: 616c 5f63 6163 6865 290a 2020 2020 2020  al_cache).      
+0000c8d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000c8e0: 616c 2861 6374 7561 6c2c 2065 7870 6563  al(actual, expec
+0000c8f0: 7465 6429 0a0a 2020 2020 4065 7665 6e74  ted)..    @event
+0000c900: 5f6c 6f6f 7028 290a 2020 2020 6465 6620  _loop().    def 
+0000c910: 7465 7374 5f6d 756c 7469 5f66 696c 655f  test_multi_file_
+0000c920: 666f 7263 655f 7079 3336 2873 656c 6629  force_py36(self)
+0000c930: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000c940: 2020 7265 675f 6d6f 6465 203d 2044 4546    reg_mode = DEF
+0000c950: 4155 4c54 5f4d 4f44 450a 2020 2020 2020  AULT_MODE.      
+0000c960: 2020 7079 3336 5f6d 6f64 6520 3d20 7265    py36_mode = re
+0000c970: 706c 6163 6528 4445 4641 554c 545f 4d4f  place(DEFAULT_MO
+0000c980: 4445 2c20 7461 7267 6574 5f76 6572 7369  DE, target_versi
+0000c990: 6f6e 733d 5059 3336 5f56 4552 5349 4f4e  ons=PY36_VERSION
+0000c9a0: 5329 0a20 2020 2020 2020 2073 6f75 7263  S).        sourc
+0000c9b0: 652c 2065 7870 6563 7465 6420 3d20 7265  e, expected = re
+0000c9c0: 6164 5f64 6174 6128 226d 6973 6365 6c6c  ad_data("miscell
+0000c9d0: 616e 656f 7573 222c 2022 666f 7263 655f  aneous", "force_
+0000c9e0: 7079 3336 2229 0a20 2020 2020 2020 2077  py36").        w
+0000c9f0: 6974 6820 6361 6368 655f 6469 7228 2920  ith cache_dir() 
+0000ca00: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
+0000ca10: 2020 2020 2020 2020 2020 7061 7468 7320            paths 
+0000ca20: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+0000ca30: 2020 2020 2877 6f72 6b73 7061 6365 202f      (workspace /
+0000ca40: 2022 6669 6c65 312e 7079 2229 2e72 6573   "file1.py").res
+0000ca50: 6f6c 7665 2829 2c0a 2020 2020 2020 2020  olve(),.        
+0000ca60: 2020 2020 2020 2020 2877 6f72 6b73 7061          (workspa
+0000ca70: 6365 202f 2022 6669 6c65 322e 7079 2229  ce / "file2.py")
+0000ca80: 2e72 6573 6f6c 7665 2829 2c0a 2020 2020  .resolve(),.    
+0000ca90: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0000caa0: 2020 2020 2020 666f 7220 7061 7468 2069        for path i
+0000cab0: 6e20 7061 7468 733a 0a20 2020 2020 2020  n paths:.       
+0000cac0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+0000cad0: 656e 2870 6174 682c 2022 7722 2920 6173  en(path, "w") as
+0000cae0: 2066 683a 0a20 2020 2020 2020 2020 2020   fh:.           
+0000caf0: 2020 2020 2020 2020 2066 682e 7772 6974           fh.writ
+0000cb00: 6528 736f 7572 6365 290a 2020 2020 2020  e(source).      
+0000cb10: 2020 2020 2020 7365 6c66 2e69 6e76 6f6b        self.invok
+0000cb20: 6542 6c61 636b 285b 7374 7228 7029 2066  eBlack([str(p) f
+0000cb30: 6f72 2070 2069 6e20 7061 7468 735d 202b  or p in paths] +
+0000cb40: 2050 5933 365f 4152 4753 290a 2020 2020   PY36_ARGS).    
+0000cb50: 2020 2020 2020 2020 666f 7220 7061 7468          for path
+0000cb60: 2069 6e20 7061 7468 733a 0a20 2020 2020   in paths:.     
+0000cb70: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000cb80: 6f70 656e 2870 6174 682c 2022 7222 2920  open(path, "r") 
+0000cb90: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
+0000cba0: 2020 2020 2020 2020 2020 2061 6374 7561             actua
+0000cbb0: 6c20 3d20 6668 2e72 6561 6428 290a 2020  l = fh.read().  
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cbd0: 6c66 2e61 7373 6572 7445 7175 616c 2861  lf.assertEqual(a
+0000cbe0: 6374 7561 6c2c 2065 7870 6563 7465 6429  ctual, expected)
+0000cbf0: 0a20 2020 2020 2020 2020 2020 2023 2076  .            # v
+0000cc00: 6572 6966 7920 6361 6368 6520 7769 7468  erify cache with
+0000cc10: 202d 2d74 6172 6765 742d 7665 7273 696f   --target-versio
+0000cc20: 6e20 6973 2073 6570 6172 6174 650a 2020  n is separate.  
+0000cc30: 2020 2020 2020 2020 2020 7079 695f 6361            pyi_ca
+0000cc40: 6368 6520 3d20 6365 7263 6973 2e72 6561  che = cercis.rea
+0000cc50: 645f 6361 6368 6528 7079 3336 5f6d 6f64  d_cache(py36_mod
+0000cc60: 6529 0a20 2020 2020 2020 2020 2020 206e  e).            n
+0000cc70: 6f72 6d61 6c5f 6361 6368 6520 3d20 6365  ormal_cache = ce
+0000cc80: 7263 6973 2e72 6561 645f 6361 6368 6528  rcis.read_cache(
+0000cc90: 7265 675f 6d6f 6465 290a 2020 2020 2020  reg_mode).      
+0000cca0: 2020 2020 2020 666f 7220 7061 7468 2069        for path i
+0000ccb0: 6e20 7061 7468 733a 0a20 2020 2020 2020  n paths:.       
+0000ccc0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000ccd0: 7365 7274 496e 2873 7472 2870 6174 6829  sertIn(str(path)
+0000cce0: 2c20 7079 695f 6361 6368 6529 0a20 2020  , pyi_cache).   
+0000ccf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000cd00: 662e 6173 7365 7274 4e6f 7449 6e28 7374  f.assertNotIn(st
+0000cd10: 7228 7061 7468 292c 206e 6f72 6d61 6c5f  r(path), normal_
+0000cd20: 6361 6368 6529 0a0a 2020 2020 6465 6620  cache)..    def 
+0000cd30: 7465 7374 5f70 6970 655f 666f 7263 655f  test_pipe_force_
+0000cd40: 7079 3336 2873 656c 6629 202d 3e20 4e6f  py36(self) -> No
+0000cd50: 6e65 3a0a 2020 2020 2020 2020 736f 7572  ne:.        sour
+0000cd60: 6365 2c20 6578 7065 6374 6564 203d 2072  ce, expected = r
+0000cd70: 6561 645f 6461 7461 2822 6d69 7363 656c  ead_data("miscel
+0000cd80: 6c61 6e65 6f75 7322 2c20 2266 6f72 6365  laneous", "force
+0000cd90: 5f70 7933 3622 290a 2020 2020 2020 2020  _py36").        
+0000cda0: 7265 7375 6c74 203d 2043 6c69 5275 6e6e  result = CliRunn
+0000cdb0: 6572 2829 2e69 6e76 6f6b 6528 0a20 2020  er().invoke(.   
+0000cdc0: 2020 2020 2020 2020 2063 6572 6369 732e           cercis.
+0000cdd0: 6d61 696e 2c0a 2020 2020 2020 2020 2020  main,.          
+0000cde0: 2020 5b22 2d22 2c20 222d 7122 2c20 222d    ["-", "-q", "-
+0000cdf0: 2d74 6172 6765 742d 7665 7273 696f 6e3d  -target-version=
+0000ce00: 7079 3336 225d 2c0a 2020 2020 2020 2020  py36"],.        
+0000ce10: 2020 2020 696e 7075 743d 4279 7465 7349      input=BytesI
+0000ce20: 4f28 736f 7572 6365 2e65 6e63 6f64 6528  O(source.encode(
+0000ce30: 2275 7466 3822 2929 2c0a 2020 2020 2020  "utf8")),.      
+0000ce40: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+0000ce50: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0000ce60: 756c 742e 6578 6974 5f63 6f64 652c 2030  ult.exit_code, 0
+0000ce70: 290a 2020 2020 2020 2020 6163 7475 616c  ).        actual
+0000ce80: 203d 2072 6573 756c 742e 6f75 7470 7574   = result.output
+0000ce90: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000cea0: 7365 7274 466f 726d 6174 4571 7561 6c28  sertFormatEqual(
+0000ceb0: 6163 7475 616c 2c20 6578 7065 6374 6564  actual, expected
+0000cec0: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+0000ced0: 6172 6b2e 696e 636f 6d70 6174 6962 6c65  ark.incompatible
+0000cee0: 5f77 6974 685f 6d79 7079 630a 2020 2020  _with_mypyc.    
+0000cef0: 6465 6620 7465 7374 5f72 6566 6f72 6d61  def test_reforma
+0000cf00: 745f 6f6e 655f 7769 7468 5f73 7464 696e  t_one_with_stdin
+0000cf10: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000cf20: 2020 2020 2020 2020 7769 7468 2070 6174          with pat
+0000cf30: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
+0000cf40: 2263 6572 6369 732e 666f 726d 6174 5f73  "cercis.format_s
+0000cf50: 7464 696e 5f74 6f5f 7374 646f 7574 222c  tdin_to_stdout",
+0000cf60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000cf70: 7572 6e5f 7661 6c75 653d 6c61 6d62 6461  urn_value=lambda
+0000cf80: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+0000cf90: 3a20 6365 7263 6973 2e43 6861 6e67 6564  : cercis.Changed
+0000cfa0: 2e59 4553 2c0a 2020 2020 2020 2020 2920  .YES,.        ) 
+0000cfb0: 6173 2066 7374 733a 0a20 2020 2020 2020  as fsts:.       
+0000cfc0: 2020 2020 2072 6570 6f72 7420 3d20 4d61       report = Ma
+0000cfd0: 6769 634d 6f63 6b28 290a 2020 2020 2020  gicMock().      
+0000cfe0: 2020 2020 2020 7061 7468 203d 2050 6174        path = Pat
+0000cff0: 6828 222d 2229 0a20 2020 2020 2020 2020  h("-").         
+0000d000: 2020 2063 6572 6369 732e 7265 666f 726d     cercis.reform
+0000d010: 6174 5f6f 6e65 280a 2020 2020 2020 2020  at_one(.        
+0000d020: 2020 2020 2020 2020 7061 7468 2c0a 2020          path,.  
+0000d030: 2020 2020 2020 2020 2020 2020 2020 6661                fa
+0000d040: 7374 3d54 7275 652c 0a20 2020 2020 2020  st=True,.       
+0000d050: 2020 2020 2020 2020 2077 7269 7465 5f62           write_b
+0000d060: 6163 6b3d 6365 7263 6973 2e57 7269 7465  ack=cercis.Write
+0000d070: 4261 636b 2e59 4553 2c0a 2020 2020 2020  Back.YES,.      
+0000d080: 2020 2020 2020 2020 2020 6d6f 6465 3d44            mode=D
+0000d090: 4546 4155 4c54 5f4d 4f44 452c 0a20 2020  EFAULT_MODE,.   
+0000d0a0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+0000d0b0: 6f72 743d 7265 706f 7274 2c0a 2020 2020  ort=report,.    
+0000d0c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d0d0: 2020 2020 2020 6673 7473 2e61 7373 6572        fsts.asser
+0000d0e0: 745f 6361 6c6c 6564 5f6f 6e63 6528 290a  t_called_once().
+0000d0f0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+0000d100: 7274 2e64 6f6e 652e 6173 7365 7274 5f63  rt.done.assert_c
+0000d110: 616c 6c65 645f 7769 7468 2870 6174 682c  alled_with(path,
+0000d120: 2063 6572 6369 732e 4368 616e 6765 642e   cercis.Changed.
+0000d130: 5945 5329 0a0a 2020 2020 4070 7974 6573  YES)..    @pytes
+0000d140: 742e 6d61 726b 2e69 6e63 6f6d 7061 7469  t.mark.incompati
+0000d150: 626c 655f 7769 7468 5f6d 7970 7963 0a20  ble_with_mypyc. 
+0000d160: 2020 2064 6566 2074 6573 745f 7265 666f     def test_refo
+0000d170: 726d 6174 5f6f 6e65 5f77 6974 685f 7374  rmat_one_with_st
+0000d180: 6469 6e5f 6669 6c65 6e61 6d65 2873 656c  din_filename(sel
+0000d190: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000d1a0: 2020 2020 7769 7468 2070 6174 6368 280a      with patch(.
+0000d1b0: 2020 2020 2020 2020 2020 2020 2263 6572              "cer
+0000d1c0: 6369 732e 666f 726d 6174 5f73 7464 696e  cis.format_stdin
+0000d1d0: 5f74 6f5f 7374 646f 7574 222c 0a20 2020  _to_stdout",.   
+0000d1e0: 2020 2020 2020 2020 2072 6574 7572 6e5f           return_
+0000d1f0: 7661 6c75 653d 6c61 6d62 6461 202a 6172  value=lambda *ar
+0000d200: 6773 2c20 2a2a 6b77 6172 6773 3a20 6365  gs, **kwargs: ce
+0000d210: 7263 6973 2e43 6861 6e67 6564 2e59 4553  rcis.Changed.YES
+0000d220: 2c0a 2020 2020 2020 2020 2920 6173 2066  ,.        ) as f
+0000d230: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
+0000d240: 2072 6570 6f72 7420 3d20 4d61 6769 634d   report = MagicM
+0000d250: 6f63 6b28 290a 2020 2020 2020 2020 2020  ock().          
+0000d260: 2020 7020 3d20 2266 6f6f 2e70 7922 0a20    p = "foo.py". 
+0000d270: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+0000d280: 3d20 5061 7468 2866 225f 5f42 4c41 434b  = Path(f"__BLACK
+0000d290: 5f53 5444 494e 5f46 494c 454e 414d 455f  _STDIN_FILENAME_
+0000d2a0: 5f7b 707d 2229 0a20 2020 2020 2020 2020  _{p}").         
+0000d2b0: 2020 2065 7870 6563 7465 6420 3d20 5061     expected = Pa
+0000d2c0: 7468 2870 290a 2020 2020 2020 2020 2020  th(p).          
+0000d2d0: 2020 6365 7263 6973 2e72 6566 6f72 6d61    cercis.reforma
+0000d2e0: 745f 6f6e 6528 0a20 2020 2020 2020 2020  t_one(.         
+0000d2f0: 2020 2020 2020 2070 6174 682c 0a20 2020         path,.   
+0000d300: 2020 2020 2020 2020 2020 2020 2066 6173               fas
+0000d310: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
+0000d320: 2020 2020 2020 2020 7772 6974 655f 6261          write_ba
+0000d330: 636b 3d63 6572 6369 732e 5772 6974 6542  ck=cercis.WriteB
+0000d340: 6163 6b2e 5945 532c 0a20 2020 2020 2020  ack.YES,.       
+0000d350: 2020 2020 2020 2020 206d 6f64 653d 4445           mode=DE
+0000d360: 4641 554c 545f 4d4f 4445 2c0a 2020 2020  FAULT_MODE,.    
+0000d370: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+0000d380: 7274 3d72 6570 6f72 742c 0a20 2020 2020  rt=report,.     
+0000d390: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d3a0: 2020 2020 2066 7374 732e 6173 7365 7274       fsts.assert
+0000d3b0: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+0000d3c0: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
+0000d3d0: 2020 2066 6173 743d 5472 7565 2c20 7772     fast=True, wr
+0000d3e0: 6974 655f 6261 636b 3d63 6572 6369 732e  ite_back=cercis.
+0000d3f0: 5772 6974 6542 6163 6b2e 5945 532c 206d  WriteBack.YES, m
+0000d400: 6f64 653d 4445 4641 554c 545f 4d4f 4445  ode=DEFAULT_MODE
+0000d410: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d420: 2020 2020 2020 2020 2020 2023 205f 5f42             # __B
+0000d430: 4c41 434b 5f53 5444 494e 5f46 494c 454e  LACK_STDIN_FILEN
+0000d440: 414d 455f 5f20 7368 6f75 6c64 2068 6176  AME__ should hav
+0000d450: 6520 6265 656e 2073 7472 6970 7065 640a  e been stripped.
+0000d460: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+0000d470: 7274 2e64 6f6e 652e 6173 7365 7274 5f63  rt.done.assert_c
+0000d480: 616c 6c65 645f 7769 7468 2865 7870 6563  alled_with(expec
+0000d490: 7465 642c 2063 6572 6369 732e 4368 616e  ted, cercis.Chan
+0000d4a0: 6765 642e 5945 5329 0a0a 2020 2020 4070  ged.YES)..    @p
+0000d4b0: 7974 6573 742e 6d61 726b 2e69 6e63 6f6d  ytest.mark.incom
+0000d4c0: 7061 7469 626c 655f 7769 7468 5f6d 7970  patible_with_myp
+0000d4d0: 7963 0a20 2020 2064 6566 2074 6573 745f  yc.    def test_
+0000d4e0: 7265 666f 726d 6174 5f6f 6e65 5f77 6974  reformat_one_wit
+0000d4f0: 685f 7374 6469 6e5f 6669 6c65 6e61 6d65  h_stdin_filename
+0000d500: 5f70 7969 2873 656c 6629 202d 3e20 4e6f  _pyi(self) -> No
+0000d510: 6e65 3a0a 2020 2020 2020 2020 7769 7468  ne:.        with
+0000d520: 2070 6174 6368 280a 2020 2020 2020 2020   patch(.        
+0000d530: 2020 2020 2263 6572 6369 732e 666f 726d      "cercis.form
+0000d540: 6174 5f73 7464 696e 5f74 6f5f 7374 646f  at_stdin_to_stdo
+0000d550: 7574 222c 0a20 2020 2020 2020 2020 2020  ut",.           
+0000d560: 2072 6574 7572 6e5f 7661 6c75 653d 6c61   return_value=la
+0000d570: 6d62 6461 202a 6172 6773 2c20 2a2a 6b77  mbda *args, **kw
+0000d580: 6172 6773 3a20 6365 7263 6973 2e43 6861  args: cercis.Cha
+0000d590: 6e67 6564 2e59 4553 2c0a 2020 2020 2020  nged.YES,.      
+0000d5a0: 2020 2920 6173 2066 7374 733a 0a20 2020    ) as fsts:.   
+0000d5b0: 2020 2020 2020 2020 2072 6570 6f72 7420           report 
+0000d5c0: 3d20 4d61 6769 634d 6f63 6b28 290a 2020  = MagicMock().  
+0000d5d0: 2020 2020 2020 2020 2020 7020 3d20 2266            p = "f
+0000d5e0: 6f6f 2e70 7969 220a 2020 2020 2020 2020  oo.pyi".        
+0000d5f0: 2020 2020 7061 7468 203d 2050 6174 6828      path = Path(
+0000d600: 6622 5f5f 424c 4143 4b5f 5354 4449 4e5f  f"__BLACK_STDIN_
+0000d610: 4649 4c45 4e41 4d45 5f5f 7b70 7d22 290a  FILENAME__{p}").
+0000d620: 2020 2020 2020 2020 2020 2020 6578 7065              expe
+0000d630: 6374 6564 203d 2050 6174 6828 7029 0a20  cted = Path(p). 
+0000d640: 2020 2020 2020 2020 2020 2063 6572 6369             cerci
+0000d650: 732e 7265 666f 726d 6174 5f6f 6e65 280a  s.reformat_one(.
+0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d670: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000d680: 2020 2020 2020 6661 7374 3d54 7275 652c        fast=True,
+0000d690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d6a0: 2077 7269 7465 5f62 6163 6b3d 6365 7263   write_back=cerc
+0000d6b0: 6973 2e57 7269 7465 4261 636b 2e59 4553  is.WriteBack.YES
+0000d6c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000d6d0: 2020 6d6f 6465 3d44 4546 4155 4c54 5f4d    mode=DEFAULT_M
+0000d6e0: 4f44 452c 0a20 2020 2020 2020 2020 2020  ODE,.           
+0000d6f0: 2020 2020 2072 6570 6f72 743d 7265 706f       report=repo
+0000d700: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
+0000d710: 290a 2020 2020 2020 2020 2020 2020 6673  ).            fs
+0000d720: 7473 2e61 7373 6572 745f 6361 6c6c 6564  ts.assert_called
+0000d730: 5f6f 6e63 655f 7769 7468 280a 2020 2020  _once_with(.    
+0000d740: 2020 2020 2020 2020 2020 2020 6661 7374              fast
+0000d750: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+0000d760: 2020 2020 2020 2077 7269 7465 5f62 6163         write_bac
+0000d770: 6b3d 6365 7263 6973 2e57 7269 7465 4261  k=cercis.WriteBa
+0000d780: 636b 2e59 4553 2c0a 2020 2020 2020 2020  ck.YES,.        
+0000d790: 2020 2020 2020 2020 6d6f 6465 3d72 6570          mode=rep
+0000d7a0: 6c61 6365 2844 4546 4155 4c54 5f4d 4f44  lace(DEFAULT_MOD
+0000d7b0: 452c 2069 735f 7079 693d 5472 7565 292c  E, is_pyi=True),
+0000d7c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d7d0: 2020 2020 2020 2020 2020 2023 205f 5f42             # __B
+0000d7e0: 4c41 434b 5f53 5444 494e 5f46 494c 454e  LACK_STDIN_FILEN
+0000d7f0: 414d 455f 5f20 7368 6f75 6c64 2068 6176  AME__ should hav
+0000d800: 6520 6265 656e 2073 7472 6970 7065 640a  e been stripped.
+0000d810: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+0000d820: 7274 2e64 6f6e 652e 6173 7365 7274 5f63  rt.done.assert_c
+0000d830: 616c 6c65 645f 7769 7468 2865 7870 6563  alled_with(expec
+0000d840: 7465 642c 2063 6572 6369 732e 4368 616e  ted, cercis.Chan
+0000d850: 6765 642e 5945 5329 0a0a 2020 2020 4070  ged.YES)..    @p
+0000d860: 7974 6573 742e 6d61 726b 2e69 6e63 6f6d  ytest.mark.incom
+0000d870: 7061 7469 626c 655f 7769 7468 5f6d 7970  patible_with_myp
+0000d880: 7963 0a20 2020 2064 6566 2074 6573 745f  yc.    def test_
+0000d890: 7265 666f 726d 6174 5f6f 6e65 5f77 6974  reformat_one_wit
+0000d8a0: 685f 7374 6469 6e5f 6669 6c65 6e61 6d65  h_stdin_filename
+0000d8b0: 5f69 7079 6e62 2873 656c 6629 202d 3e20  _ipynb(self) -> 
+0000d8c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7769  None:.        wi
+0000d8d0: 7468 2070 6174 6368 280a 2020 2020 2020  th patch(.      
+0000d8e0: 2020 2020 2020 2263 6572 6369 732e 666f        "cercis.fo
+0000d8f0: 726d 6174 5f73 7464 696e 5f74 6f5f 7374  rmat_stdin_to_st
+0000d900: 646f 7574 222c 0a20 2020 2020 2020 2020  dout",.         
+0000d910: 2020 2072 6574 7572 6e5f 7661 6c75 653d     return_value=
+0000d920: 6c61 6d62 6461 202a 6172 6773 2c20 2a2a  lambda *args, **
+0000d930: 6b77 6172 6773 3a20 6365 7263 6973 2e43  kwargs: cercis.C
+0000d940: 6861 6e67 6564 2e59 4553 2c0a 2020 2020  hanged.YES,.    
+0000d950: 2020 2020 2920 6173 2066 7374 733a 0a20      ) as fsts:. 
+0000d960: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
+0000d970: 7420 3d20 4d61 6769 634d 6f63 6b28 290a  t = MagicMock().
+0000d980: 2020 2020 2020 2020 2020 2020 7020 3d20              p = 
+0000d990: 2266 6f6f 2e69 7079 6e62 220a 2020 2020  "foo.ipynb".    
+0000d9a0: 2020 2020 2020 2020 7061 7468 203d 2050          path = P
+0000d9b0: 6174 6828 6622 5f5f 424c 4143 4b5f 5354  ath(f"__BLACK_ST
+0000d9c0: 4449 4e5f 4649 4c45 4e41 4d45 5f5f 7b70  DIN_FILENAME__{p
+0000d9d0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0000d9e0: 6578 7065 6374 6564 203d 2050 6174 6828  expected = Path(
+0000d9f0: 7029 0a20 2020 2020 2020 2020 2020 2063  p).            c
+0000da00: 6572 6369 732e 7265 666f 726d 6174 5f6f  ercis.reformat_o
+0000da10: 6e65 280a 2020 2020 2020 2020 2020 2020  ne(.            
+0000da20: 2020 2020 7061 7468 2c0a 2020 2020 2020      path,.      
+0000da30: 2020 2020 2020 2020 2020 6661 7374 3d54            fast=T
+0000da40: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0000da50: 2020 2020 2077 7269 7465 5f62 6163 6b3d       write_back=
+0000da60: 6365 7263 6973 2e57 7269 7465 4261 636b  cercis.WriteBack
+0000da70: 2e59 4553 2c0a 2020 2020 2020 2020 2020  .YES,.          
+0000da80: 2020 2020 2020 6d6f 6465 3d44 4546 4155        mode=DEFAU
+0000da90: 4c54 5f4d 4f44 452c 0a20 2020 2020 2020  LT_MODE,.       
+0000daa0: 2020 2020 2020 2020 2072 6570 6f72 743d           report=
+0000dab0: 7265 706f 7274 2c0a 2020 2020 2020 2020  report,.        
+0000dac0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000dad0: 2020 6673 7473 2e61 7373 6572 745f 6361    fsts.assert_ca
+0000dae0: 6c6c 6564 5f6f 6e63 655f 7769 7468 280a  lled_once_with(.
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 6661 7374 3d54 7275 652c 0a20 2020 2020  fast=True,.     
+0000db10: 2020 2020 2020 2020 2020 2077 7269 7465             write
+0000db20: 5f62 6163 6b3d 6365 7263 6973 2e57 7269  _back=cercis.Wri
+0000db30: 7465 4261 636b 2e59 4553 2c0a 2020 2020  teBack.YES,.    
+0000db40: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0000db50: 3d72 6570 6c61 6365 2844 4546 4155 4c54  =replace(DEFAULT
+0000db60: 5f4d 4f44 452c 2069 735f 6970 796e 623d  _MODE, is_ipynb=
+0000db70: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+0000db80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000db90: 2023 205f 5f42 4c41 434b 5f53 5444 494e   # __BLACK_STDIN
+0000dba0: 5f46 494c 454e 414d 455f 5f20 7368 6f75  _FILENAME__ shou
+0000dbb0: 6c64 2068 6176 6520 6265 656e 2073 7472  ld have been str
+0000dbc0: 6970 7065 640a 2020 2020 2020 2020 2020  ipped.          
+0000dbd0: 2020 7265 706f 7274 2e64 6f6e 652e 6173    report.done.as
+0000dbe0: 7365 7274 5f63 616c 6c65 645f 7769 7468  sert_called_with
+0000dbf0: 2865 7870 6563 7465 642c 2063 6572 6369  (expected, cerci
+0000dc00: 732e 4368 616e 6765 642e 5945 5329 0a0a  s.Changed.YES)..
+0000dc10: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0000dc20: 2e69 6e63 6f6d 7061 7469 626c 655f 7769  .incompatible_wi
+0000dc30: 7468 5f6d 7970 7963 0a20 2020 2064 6566  th_mypyc.    def
+0000dc40: 2074 6573 745f 7265 666f 726d 6174 5f6f   test_reformat_o
+0000dc50: 6e65 5f77 6974 685f 7374 6469 6e5f 616e  ne_with_stdin_an
+0000dc60: 645f 6578 6973 7469 6e67 5f70 6174 6828  d_existing_path(
+0000dc70: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000dc80: 2020 2020 2020 2077 6974 6820 7061 7463         with patc
+0000dc90: 6828 0a20 2020 2020 2020 2020 2020 2022  h(.            "
+0000dca0: 6365 7263 6973 2e66 6f72 6d61 745f 7374  cercis.format_st
+0000dcb0: 6469 6e5f 746f 5f73 7464 6f75 7422 2c0a  din_to_stdout",.
+0000dcc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000dcd0: 726e 5f76 616c 7565 3d6c 616d 6264 6120  rn_value=lambda 
+0000dce0: 2a61 7267 732c 202a 2a6b 7761 7267 733a  *args, **kwargs:
+0000dcf0: 2063 6572 6369 732e 4368 616e 6765 642e   cercis.Changed.
+0000dd00: 5945 532c 0a20 2020 2020 2020 2029 2061  YES,.        ) a
+0000dd10: 7320 6673 7473 3a0a 2020 2020 2020 2020  s fsts:.        
+0000dd20: 2020 2020 7265 706f 7274 203d 204d 6167      report = Mag
+0000dd30: 6963 4d6f 636b 2829 0a20 2020 2020 2020  icMock().       
+0000dd40: 2020 2020 2023 2045 7665 6e20 7769 7468       # Even with
+0000dd50: 2061 6e20 6578 6973 7469 6e67 2066 696c   an existing fil
+0000dd60: 652c 2073 696e 6365 2077 6520 6172 6520  e, since we are 
+0000dd70: 666f 7263 696e 6720 7374 6469 6e2c 2063  forcing stdin, c
+0000dd80: 6572 6369 730a 2020 2020 2020 2020 2020  ercis.          
+0000dd90: 2020 2320 7368 6f75 6c64 206f 7574 7075    # should outpu
+0000dda0: 7420 746f 2073 7464 6f75 7420 616e 6420  t to stdout and 
+0000ddb0: 6e6f 7420 6d6f 6469 6679 2074 6865 2066  not modify the f
+0000ddc0: 696c 6520 696e 706c 6163 650a 2020 2020  ile inplace.    
+0000ddd0: 2020 2020 2020 2020 7020 3d20 5448 4953          p = THIS
+0000dde0: 5f44 4952 202f 2022 6461 7461 2220 2f20  _DIR / "data" / 
+0000ddf0: 2273 696d 706c 655f 6361 7365 7322 202f  "simple_cases" /
+0000de00: 2022 636f 6c6c 6563 7469 6f6e 732e 7079   "collections.py
+0000de10: 220a 2020 2020 2020 2020 2020 2020 2320  ".            # 
+0000de20: 4d61 6b65 2073 7572 6520 6973 5f66 696c  Make sure is_fil
+0000de30: 6520 6163 7475 616c 6c79 2072 6574 7572  e actually retur
+0000de40: 6e73 2054 7275 650a 2020 2020 2020 2020  ns True.        
+0000de50: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0000de60: 7275 6528 702e 6973 5f66 696c 6528 2929  rue(p.is_file())
+0000de70: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+0000de80: 6820 3d20 5061 7468 2866 225f 5f42 4c41  h = Path(f"__BLA
+0000de90: 434b 5f53 5444 494e 5f46 494c 454e 414d  CK_STDIN_FILENAM
+0000dea0: 455f 5f7b 707d 2229 0a20 2020 2020 2020  E__{p}").       
+0000deb0: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+0000dec0: 5061 7468 2870 290a 2020 2020 2020 2020  Path(p).        
+0000ded0: 2020 2020 6365 7263 6973 2e72 6566 6f72      cercis.refor
+0000dee0: 6d61 745f 6f6e 6528 0a20 2020 2020 2020  mat_one(.       
+0000def0: 2020 2020 2020 2020 2070 6174 682c 0a20           path,. 
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000df10: 6173 743d 5472 7565 2c0a 2020 2020 2020  ast=True,.      
+0000df20: 2020 2020 2020 2020 2020 7772 6974 655f            write_
+0000df30: 6261 636b 3d63 6572 6369 732e 5772 6974  back=cercis.Writ
+0000df40: 6542 6163 6b2e 5945 532c 0a20 2020 2020  eBack.YES,.     
+0000df50: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
+0000df60: 4445 4641 554c 545f 4d4f 4445 2c0a 2020  DEFAULT_MODE,.  
+0000df70: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000df80: 706f 7274 3d72 6570 6f72 742c 0a20 2020  port=report,.   
+0000df90: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000dfa0: 2020 2020 2020 2066 7374 732e 6173 7365         fsts.asse
+0000dfb0: 7274 5f63 616c 6c65 645f 6f6e 6365 2829  rt_called_once()
+0000dfc0: 0a20 2020 2020 2020 2020 2020 2023 205f  .            # _
+0000dfd0: 5f42 4c41 434b 5f53 5444 494e 5f46 494c  _BLACK_STDIN_FIL
+0000dfe0: 454e 414d 455f 5f20 7368 6f75 6c64 2068  ENAME__ should h
+0000dff0: 6176 6520 6265 656e 2073 7472 6970 7065  ave been strippe
+0000e000: 640a 2020 2020 2020 2020 2020 2020 7265  d.            re
+0000e010: 706f 7274 2e64 6f6e 652e 6173 7365 7274  port.done.assert
+0000e020: 5f63 616c 6c65 645f 7769 7468 2865 7870  _called_with(exp
+0000e030: 6563 7465 642c 2063 6572 6369 732e 4368  ected, cercis.Ch
+0000e040: 616e 6765 642e 5945 5329 0a0a 2020 2020  anged.YES)..    
+0000e050: 6465 6620 7465 7374 5f72 6566 6f72 6d61  def test_reforma
+0000e060: 745f 6f6e 655f 7769 7468 5f73 7464 696e  t_one_with_stdin
+0000e070: 5f65 6d70 7479 2873 656c 6629 202d 3e20  _empty(self) -> 
+0000e080: 4e6f 6e65 3a0a 2020 2020 2020 2020 6361  None:.        ca
+0000e090: 7365 7320 3d20 5b0a 2020 2020 2020 2020  ses = [.        
+0000e0a0: 2020 2020 2822 222c 2022 2229 2c0a 2020      ("", ""),.  
+0000e0b0: 2020 2020 2020 2020 2020 2822 5c6e 222c            ("\n",
+0000e0c0: 2022 5c6e 2229 2c0a 2020 2020 2020 2020   "\n"),.        
+0000e0d0: 2020 2020 2822 5c72 5c6e 222c 2022 5c72      ("\r\n", "\r
+0000e0e0: 5c6e 2229 2c0a 2020 2020 2020 2020 2020  \n"),.          
+0000e0f0: 2020 2822 205c 7422 2c20 2222 292c 0a20    (" \t", ""),. 
+0000e100: 2020 2020 2020 2020 2020 2028 2220 5c74             (" \t
+0000e110: 5c6e 5c74 2022 2c20 225c 6e22 292c 0a20  \n\t ", "\n"),. 
+0000e120: 2020 2020 2020 2020 2020 2028 2220 5c74             (" \t
+0000e130: 5c72 5c6e 5c74 2022 2c20 225c 725c 6e22  \r\n\t ", "\r\n"
+0000e140: 292c 0a20 2020 2020 2020 205d 0a0a 2020  ),.        ]..  
+0000e150: 2020 2020 2020 6465 6620 5f6e 6577 5f77        def _new_w
+0000e160: 7261 7070 6572 280a 2020 2020 2020 2020  rapper(.        
+0000e170: 2020 2020 2020 2020 6f75 7470 7574 3a20          output: 
+0000e180: 696f 2e53 7472 696e 6749 4f2c 2069 6f5f  io.StringIO, io_
+0000e190: 5465 7874 494f 5772 6170 7065 723a 2054  TextIOWrapper: T
+0000e1a0: 7970 655b 696f 2e54 6578 7449 4f57 7261  ype[io.TextIOWra
+0000e1b0: 7070 6572 5d0a 2020 2020 2020 2020 2920  pper].        ) 
+0000e1c0: 2d3e 2043 616c 6c61 626c 655b 5b41 6e79  -> Callable[[Any
+0000e1d0: 2c20 416e 795d 2c20 696f 2e54 6578 7449  , Any], io.TextI
+0000e1e0: 4f57 7261 7070 6572 5d3a 0a20 2020 2020  OWrapper]:.     
+0000e1f0: 2020 2020 2020 2064 6566 2067 6574 5f6f         def get_o
+0000e200: 7574 7075 7428 2a61 7267 733a 2041 6e79  utput(*args: Any
+0000e210: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
+0000e220: 202d 3e20 696f 2e54 6578 7449 4f57 7261   -> io.TextIOWra
+0000e230: 7070 6572 3a0a 2020 2020 2020 2020 2020  pper:.          
+0000e240: 2020 2020 2020 6966 2061 7267 7320 3d3d        if args ==
+0000e250: 2028 7379 732e 7374 646f 7574 2e62 7566   (sys.stdout.buf
+0000e260: 6665 722c 293a 0a20 2020 2020 2020 2020  fer,):.         
+0000e270: 2020 2020 2020 2020 2020 2023 2049 7427             # It'
+0000e280: 7320 6066 6f72 6d61 745f 7374 6469 6e5f  s `format_stdin_
+0000e290: 746f 5f73 7464 6f75 7428 2960 2063 616c  to_stdout()` cal
+0000e2a0: 6c69 6e67 2060 696f 2e54 6578 7449 4f57  ling `io.TextIOW
+0000e2b0: 7261 7070 6572 2829 602c 0a20 2020 2020  rapper()`,.     
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000e2d0: 2072 6574 7572 6e20 6f75 7220 6d6f 636b   return our mock
+0000e2e0: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+0000e2f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000e300: 7572 6e20 6f75 7470 7574 0a20 2020 2020  urn output.     
+0000e310: 2020 2020 2020 2020 2020 2023 2049 7427             # It'
+0000e320: 7320 736f 6d65 7468 696e 6720 656c 7365  s something else
+0000e330: 2028 692e 652e 2060 6465 636f 6465 5f62   (i.e. `decode_b
+0000e340: 7974 6573 2829 6029 2063 616c 6c69 6e67  ytes()`) calling
+0000e350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e360: 2023 2060 696f 2e54 6578 7449 4f57 7261   # `io.TextIOWra
+0000e370: 7070 6572 2829 602c 2070 6173 7320 7468  pper()`, pass th
+0000e380: 726f 7567 6820 746f 2074 6865 206f 7269  rough to the ori
+0000e390: 6769 6e61 6c20 696d 706c 656d 656e 7461  ginal implementa
+0000e3a0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+0000e3b0: 2020 2020 2020 2320 5365 6520 6469 7363        # See disc
+0000e3c0: 7573 7369 6f6e 2069 6e20 6874 7470 733a  ussion in https:
+0000e3d0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
+0000e3e0: 2f62 6c61 636b 2f70 756c 6c2f 3234 3839  /black/pull/2489
+0000e3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e400: 2072 6574 7572 6e20 696f 5f54 6578 7449   return io_TextI
+0000e410: 4f57 7261 7070 6572 282a 6172 6773 2c20  OWrapper(*args, 
+0000e420: 2a2a 6b77 6172 6773 290a 0a20 2020 2020  **kwargs)..     
+0000e430: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
+0000e440: 745f 6f75 7470 7574 0a0a 2020 2020 2020  t_output..      
+0000e450: 2020 6d6f 6465 203d 2063 6572 6369 732e    mode = cercis.
+0000e460: 4d6f 6465 2870 7265 7669 6577 3d54 7275  Mode(preview=Tru
+0000e470: 6529 0a20 2020 2020 2020 2066 6f72 2063  e).        for c
+0000e480: 6f6e 7465 6e74 2c20 6578 7065 6374 6564  ontent, expected
+0000e490: 2069 6e20 6361 7365 733a 0a20 2020 2020   in cases:.     
+0000e4a0: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
+0000e4b0: 696f 2e53 7472 696e 6749 4f28 290a 2020  io.StringIO().  
+0000e4c0: 2020 2020 2020 2020 2020 696f 5f54 6578            io_Tex
+0000e4d0: 7449 4f57 7261 7070 6572 203d 2069 6f2e  tIOWrapper = io.
+0000e4e0: 5465 7874 494f 5772 6170 7065 720a 0a20  TextIOWrapper.. 
+0000e4f0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000e500: 7061 7463 6828 2269 6f2e 5465 7874 494f  patch("io.TextIO
+0000e510: 5772 6170 7065 7222 2c20 5f6e 6577 5f77  Wrapper", _new_w
+0000e520: 7261 7070 6572 286f 7574 7075 742c 2069  rapper(output, i
+0000e530: 6f5f 5465 7874 494f 5772 6170 7065 7229  o_TextIOWrapper)
+0000e540: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000e550: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000e560: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+0000e570: 6973 2e66 6f72 6d61 745f 7374 6469 6e5f  is.format_stdin_
+0000e580: 746f 5f73 7464 6f75 7428 0a20 2020 2020  to_stdout(.     
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5a0: 2020 2066 6173 743d 5472 7565 2c0a 2020     fast=True,.  
+0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5c0: 2020 2020 2020 636f 6e74 656e 743d 636f        content=co
+0000e5d0: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000e5f0: 7269 7465 5f62 6163 6b3d 6365 7263 6973  rite_back=cercis
+0000e600: 2e57 7269 7465 4261 636b 2e59 4553 2c0a  .WriteBack.YES,.
+0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e620: 2020 2020 2020 2020 6d6f 6465 3d6d 6f64          mode=mod
+0000e630: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000e640: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000e650: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0000e660: 696f 2e55 6e73 7570 706f 7274 6564 4f70  io.UnsupportedOp
+0000e670: 6572 6174 696f 6e3a 0a20 2020 2020 2020  eration:.       
+0000e680: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+0000e690: 7320 2023 2053 7472 696e 6749 4f20 646f  s  # StringIO do
+0000e6a0: 6573 206e 6f74 2073 7570 706f 7274 2064  es not support d
+0000e6b0: 6574 6163 680a 2020 2020 2020 2020 2020  etach.          
+0000e6c0: 2020 2020 2020 6173 7365 7274 206f 7574        assert out
+0000e6d0: 7075 742e 6765 7476 616c 7565 2829 203d  put.getvalue() =
+0000e6e0: 3d20 6578 7065 6374 6564 0a0a 2020 2020  = expected..    
+0000e6f0: 2020 2020 2320 416e 2065 6d70 7479 2073      # An empty s
+0000e700: 7472 696e 6720 6973 2074 6865 206f 6e6c  tring is the onl
+0000e710: 7920 7465 7374 2063 6173 6520 666f 7220  y test case for 
+0000e720: 6070 7265 7669 6577 3d46 616c 7365 600a  `preview=False`.
+0000e730: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+0000e740: 2069 6f2e 5374 7269 6e67 494f 2829 0a20   io.StringIO(). 
+0000e750: 2020 2020 2020 2069 6f5f 5465 7874 494f         io_TextIO
+0000e760: 5772 6170 7065 7220 3d20 696f 2e54 6578  Wrapper = io.Tex
+0000e770: 7449 4f57 7261 7070 6572 0a20 2020 2020  tIOWrapper.     
+0000e780: 2020 2077 6974 6820 7061 7463 6828 2269     with patch("i
+0000e790: 6f2e 5465 7874 494f 5772 6170 7065 7222  o.TextIOWrapper"
+0000e7a0: 2c20 5f6e 6577 5f77 7261 7070 6572 286f  , _new_wrapper(o
+0000e7b0: 7574 7075 742c 2069 6f5f 5465 7874 494f  utput, io_TextIO
+0000e7c0: 5772 6170 7065 7229 293a 0a20 2020 2020  Wrapper)):.     
+0000e7d0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000e7e0: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+0000e7f0: 6973 2e66 6f72 6d61 745f 7374 6469 6e5f  is.format_stdin_
+0000e800: 746f 5f73 7464 6f75 7428 0a20 2020 2020  to_stdout(.     
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e820: 6173 743d 5472 7565 2c0a 2020 2020 2020  ast=True,.      
+0000e830: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000e840: 6e74 656e 743d 2222 2c0a 2020 2020 2020  ntent="",.      
+0000e850: 2020 2020 2020 2020 2020 2020 2020 7772                wr
+0000e860: 6974 655f 6261 636b 3d63 6572 6369 732e  ite_back=cercis.
+0000e870: 5772 6974 6542 6163 6b2e 5945 532c 0a20  WriteBack.YES,. 
+0000e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e890: 2020 206d 6f64 653d 4445 4641 554c 545f     mode=DEFAULT_
+0000e8a0: 4d4f 4445 2c0a 2020 2020 2020 2020 2020  MODE,.          
+0000e8b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000e8c0: 2020 2020 6578 6365 7074 2069 6f2e 556e      except io.Un
+0000e8d0: 7375 7070 6f72 7465 644f 7065 7261 7469  supportedOperati
+0000e8e0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+0000e8f0: 2020 2020 7061 7373 2020 2320 5374 7269      pass  # Stri
+0000e900: 6e67 494f 2064 6f65 7320 6e6f 7420 7375  ngIO does not su
+0000e910: 7070 6f72 7420 6465 7461 6368 0a20 2020  pport detach.   
+0000e920: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000e930: 6f75 7470 7574 2e67 6574 7661 6c75 6528  output.getvalue(
+0000e940: 2920 3d3d 2022 220a 0a20 2020 2064 6566  ) == ""..    def
+0000e950: 2074 6573 745f 696e 7661 6c69 645f 636c   test_invalid_cl
+0000e960: 695f 7265 6765 7828 7365 6c66 2920 2d3e  i_regex(self) ->
+0000e970: 204e 6f6e 653a 0a20 2020 2020 2020 2066   None:.        f
+0000e980: 6f72 206f 7074 696f 6e20 696e 205b 222d  or option in ["-
+0000e990: 2d69 6e63 6c75 6465 222c 2022 2d2d 6578  -include", "--ex
+0000e9a0: 636c 7564 6522 2c20 222d 2d65 7874 656e  clude", "--exten
+0000e9b0: 642d 6578 636c 7564 6522 2c20 222d 2d66  d-exclude", "--f
+0000e9c0: 6f72 6365 2d65 7863 6c75 6465 225d 3a0a  orce-exclude"]:.
+0000e9d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e9e0: 2e69 6e76 6f6b 6542 6c61 636b 285b 222d  .invokeBlack(["-
+0000e9f0: 222c 206f 7074 696f 6e2c 2022 2a2a 2829  ", option, "**()
+0000ea00: 2821 212a 2922 5d2c 2065 7869 745f 636f  (!!*)"], exit_co
+0000ea10: 6465 3d32 290a 0a20 2020 2064 6566 2074  de=2)..    def t
+0000ea20: 6573 745f 7265 7175 6972 6564 5f76 6572  est_required_ver
+0000ea30: 7369 6f6e 5f6d 6174 6368 6573 5f76 6572  sion_matches_ver
+0000ea40: 7369 6f6e 2873 656c 6629 202d 3e20 4e6f  sion(self) -> No
+0000ea50: 6e65 3a0a 2020 2020 2020 2020 7365 6c66  ne:.        self
+0000ea60: 2e69 6e76 6f6b 6542 6c61 636b 280a 2020  .invokeBlack(.  
+0000ea70: 2020 2020 2020 2020 2020 5b22 2d2d 7265            ["--re
+0000ea80: 7175 6972 6564 2d76 6572 7369 6f6e 222c  quired-version",
+0000ea90: 2063 6572 6369 732e 5f5f 7665 7273 696f   cercis.__versio
+0000eaa0: 6e5f 5f2c 2022 2d63 222c 2022 3022 5d2c  n__, "-c", "0"],
+0000eab0: 0a20 2020 2020 2020 2020 2020 2065 7869  .            exi
+0000eac0: 745f 636f 6465 3d30 2c0a 2020 2020 2020  t_code=0,.      
+0000ead0: 2020 2020 2020 6967 6e6f 7265 5f63 6f6e        ignore_con
+0000eae0: 6669 673d 5472 7565 2c0a 2020 2020 2020  fig=True,.      
+0000eaf0: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+0000eb00: 745f 7265 7175 6972 6564 5f76 6572 7369  t_required_versi
+0000eb10: 6f6e 5f6d 6174 6368 6573 5f70 6172 7469  on_matches_parti
+0000eb20: 616c 5f76 6572 7369 6f6e 2873 656c 6629  al_version(self)
+0000eb30: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000eb40: 2020 7365 6c66 2e69 6e76 6f6b 6542 6c61    self.invokeBla
+0000eb50: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
+0000eb60: 5b22 2d2d 7265 7175 6972 6564 2d76 6572  ["--required-ver
+0000eb70: 7369 6f6e 222c 2063 6572 6369 732e 5f5f  sion", cercis.__
+0000eb80: 7665 7273 696f 6e5f 5f2e 7370 6c69 7428  version__.split(
+0000eb90: 222e 2229 5b30 5d2c 2022 2d63 222c 2022  ".")[0], "-c", "
+0000eba0: 3022 5d2c 0a20 2020 2020 2020 2020 2020  0"],.           
+0000ebb0: 2065 7869 745f 636f 6465 3d30 2c0a 2020   exit_code=0,.  
+0000ebc0: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
+0000ebd0: 5f63 6f6e 6669 673d 5472 7565 2c0a 2020  _config=True,.  
+0000ebe0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000ebf0: 2074 6573 745f 7265 7175 6972 6564 5f76   test_required_v
+0000ec00: 6572 7369 6f6e 5f64 6f65 735f 6e6f 745f  ersion_does_not_
+0000ec10: 6d61 7463 685f 6f6e 5f6d 696e 6f72 5f76  match_on_minor_v
+0000ec20: 6572 7369 6f6e 2873 656c 6629 202d 3e20  ersion(self) -> 
+0000ec30: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
+0000ec40: 6c66 2e69 6e76 6f6b 6542 6c61 636b 280a  lf.invokeBlack(.
+0000ec50: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+0000ec60: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+0000ec70: 2d72 6571 7569 7265 642d 7665 7273 696f  -required-versio
+0000ec80: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+0000ec90: 2020 2020 6365 7263 6973 2e5f 5f76 6572      cercis.__ver
+0000eca0: 7369 6f6e 5f5f 2e73 706c 6974 2822 2e22  sion__.split("."
+0000ecb0: 295b 305d 202b 2022 2e39 3939 222c 0a20  )[0] + ".999",. 
+0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000ecd0: 2d63 222c 0a20 2020 2020 2020 2020 2020  -c",.           
+0000ece0: 2020 2020 2022 3022 2c0a 2020 2020 2020       "0",.      
+0000ecf0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+0000ed00: 2020 2020 2065 7869 745f 636f 6465 3d31       exit_code=1
+0000ed10: 2c0a 2020 2020 2020 2020 2020 2020 6967  ,.            ig
+0000ed20: 6e6f 7265 5f63 6f6e 6669 673d 5472 7565  nore_config=True
+0000ed30: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000ed40: 2064 6566 2074 6573 745f 7265 7175 6972   def test_requir
+0000ed50: 6564 5f76 6572 7369 6f6e 5f64 6f65 735f  ed_version_does_
+0000ed60: 6e6f 745f 6d61 7463 685f 7665 7273 696f  not_match_versio
+0000ed70: 6e28 7365 6c66 2920 2d3e 204e 6f6e 653a  n(self) -> None:
+0000ed80: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000ed90: 3d20 426c 6163 6b52 756e 6e65 7228 292e  = BlackRunner().
+0000eda0: 696e 766f 6b65 280a 2020 2020 2020 2020  invoke(.        
+0000edb0: 2020 2020 6365 7263 6973 2e6d 6169 6e2c      cercis.main,
+0000edc0: 0a20 2020 2020 2020 2020 2020 205b 222d  .            ["-
+0000edd0: 2d72 6571 7569 7265 642d 7665 7273 696f  -required-versio
+0000ede0: 6e22 2c20 2232 302e 3939 6222 2c20 222d  n", "20.99b", "-
+0000edf0: 6322 2c20 2230 225d 2c0a 2020 2020 2020  c", "0"],.      
+0000ee00: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+0000ee10: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0000ee20: 756c 742e 6578 6974 5f63 6f64 652c 2031  ult.exit_code, 1
+0000ee30: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000ee40: 7373 6572 7449 6e28 2272 6571 7569 7265  ssertIn("require
+0000ee50: 6420 7665 7273 696f 6e22 2c20 7265 7375  d version", resu
+0000ee60: 6c74 2e73 7464 6572 7229 0a0a 2020 2020  lt.stderr)..    
+0000ee70: 6465 6620 7465 7374 5f70 7265 7365 7276  def test_preserv
+0000ee80: 6573 5f6c 696e 655f 656e 6469 6e67 7328  es_line_endings(
+0000ee90: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000eea0: 2020 2020 2020 2077 6974 6820 5465 6d70         with Temp
+0000eeb0: 6f72 6172 7944 6972 6563 746f 7279 2829  oraryDirectory()
+0000eec0: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
+0000eed0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+0000eee0: 6669 6c65 203d 2050 6174 6828 776f 726b  file = Path(work
+0000eef0: 7370 6163 6529 202f 2022 7465 7374 2e70  space) / "test.p
+0000ef00: 7922 0a20 2020 2020 2020 2020 2020 2066  y".            f
+0000ef10: 6f72 206e 6c20 696e 205b 225c 6e22 2c20  or nl in ["\n", 
+0000ef20: 225c 725c 6e22 5d3a 0a20 2020 2020 2020  "\r\n"]:.       
+0000ef30: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+0000ef40: 7320 3d20 6e6c 2e6a 6f69 6e28 5b22 6465  s = nl.join(["de
+0000ef50: 6620 6628 2020 293a 222c 2022 2020 2020  f f(  ):", "    
+0000ef60: 7061 7373 225d 290a 2020 2020 2020 2020  pass"]).        
+0000ef70: 2020 2020 2020 2020 7465 7374 5f66 696c          test_fil
+0000ef80: 652e 7772 6974 655f 6279 7465 7328 636f  e.write_bytes(co
+0000ef90: 6e74 656e 7473 2e65 6e63 6f64 6528 2929  ntents.encode())
+0000efa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000efb0: 2066 6628 7465 7374 5f66 696c 652c 2077   ff(test_file, w
+0000efc0: 7269 7465 5f62 6163 6b3d 6365 7263 6973  rite_back=cercis
+0000efd0: 2e57 7269 7465 4261 636b 2e59 4553 290a  .WriteBack.YES).
 0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eff0: 6365 7263 6973 2e6d 6169 6e2c 205b 222d  cercis.main, ["-
-0000f000: 222c 2022 2d2d 6661 7374 225d 2c20 696e  ", "--fast"], in
-0000f010: 7075 743d 4279 7465 7349 4f28 636f 6e74  put=BytesIO(cont
-0000f020: 656e 7473 2e65 6e63 6f64 6528 2275 7466  ents.encode("utf
-0000f030: 3822 2929 0a20 2020 2020 2020 2020 2020  8")).           
-0000f040: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-0000f050: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000f060: 7265 7375 6c74 2e65 7869 745f 636f 6465  result.exit_code
-0000f070: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
-0000f080: 206f 7574 7075 7420 3d20 7265 7375 6c74   output = result
-0000f090: 2e73 7464 6f75 745f 6279 7465 730a 2020  .stdout_bytes.  
-0000f0a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000f0b0: 7373 6572 7449 6e28 6e6c 2e65 6e63 6f64  ssertIn(nl.encod
-0000f0c0: 6528 2275 7466 3822 292c 206f 7574 7075  e("utf8"), outpu
-0000f0d0: 7429 0a20 2020 2020 2020 2020 2020 2069  t).            i
-0000f0e0: 6620 6e6c 203d 3d20 225c 6e22 3a0a 2020  f nl == "\n":.  
-0000f0f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f100: 6c66 2e61 7373 6572 744e 6f74 496e 2862  lf.assertNotIn(b
-0000f110: 225c 725c 6e22 2c20 6f75 7470 7574 290a  "\r\n", output).
-0000f120: 0a20 2020 2064 6566 2074 6573 745f 6e6f  .    def test_no
-0000f130: 726d 616c 697a 655f 6c69 6e65 5f65 6e64  rmalize_line_end
-0000f140: 696e 6773 2873 656c 6629 202d 3e20 4e6f  ings(self) -> No
-0000f150: 6e65 3a0a 2020 2020 2020 2020 7769 7468  ne:.        with
-0000f160: 2054 656d 706f 7261 7279 4469 7265 6374   TemporaryDirect
-0000f170: 6f72 7928 2920 6173 2077 6f72 6b73 7061  ory() as workspa
-0000f180: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-0000f190: 7465 7374 5f66 696c 6520 3d20 5061 7468  test_file = Path
-0000f1a0: 2877 6f72 6b73 7061 6365 2920 2f20 2274  (workspace) / "t
-0000f1b0: 6573 742e 7079 220a 2020 2020 2020 2020  est.py".        
-0000f1c0: 2020 2020 666f 7220 6461 7461 2c20 6578      for data, ex
-0000f1d0: 7065 6374 6564 2069 6e20 280a 2020 2020  pected in (.    
-0000f1e0: 2020 2020 2020 2020 2020 2020 2862 2263              (b"c
-0000f1f0: 5c72 5c6e 635c 6e20 222c 2062 2263 5c72  \r\nc\n ", b"c\r
-0000f200: 5c6e 635c 725c 6e22 292c 0a20 2020 2020  \nc\r\n"),.     
-0000f210: 2020 2020 2020 2020 2020 2028 6222 6c5c             (b"l\
-0000f220: 6e6c 5c72 5c6e 2022 2c20 6222 6c5c 6e6c  nl\r\n ", b"l\nl
-0000f230: 5c6e 2229 2c0a 2020 2020 2020 2020 2020  \n"),.          
-0000f240: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0000f250: 2020 2020 2074 6573 745f 6669 6c65 2e77       test_file.w
-0000f260: 7269 7465 5f62 7974 6573 2864 6174 6129  rite_bytes(data)
-0000f270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f280: 2066 6628 7465 7374 5f66 696c 652c 2077   ff(test_file, w
-0000f290: 7269 7465 5f62 6163 6b3d 6365 7263 6973  rite_back=cercis
-0000f2a0: 2e57 7269 7465 4261 636b 2e59 4553 290a  .WriteBack.YES).
-0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000f2d0: 2874 6573 745f 6669 6c65 2e72 6561 645f  (test_file.read_
-0000f2e0: 6279 7465 7328 292c 2065 7870 6563 7465  bytes(), expecte
-0000f2f0: 6429 0a0a 2020 2020 6465 6620 7465 7374  d)..    def test
-0000f300: 5f61 7373 6572 745f 6571 7569 7661 6c65  _assert_equivale
-0000f310: 6e74 5f64 6966 6665 7265 6e74 5f61 7374  nt_different_ast
-0000f320: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-0000f330: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000f340: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-0000f350: 4173 7365 7274 696f 6e45 7272 6f72 293a  AssertionError):
-0000f360: 0a20 2020 2020 2020 2020 2020 2063 6572  .            cer
-0000f370: 6369 732e 6173 7365 7274 5f65 7175 6976  cis.assert_equiv
-0000f380: 616c 656e 7428 227b 7d22 2c20 224e 6f6e  alent("{}", "Non
-0000f390: 6522 290a 0a20 2020 2064 6566 2074 6573  e")..    def tes
-0000f3a0: 745f 7368 6868 5f63 6c69 636b 2873 656c  t_shhh_click(sel
-0000f3b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000f3c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000f3d0: 2020 2020 2066 726f 6d20 636c 6963 6b20       from click 
-0000f3e0: 696d 706f 7274 205f 756e 6963 6f64 6566  import _unicodef
-0000f3f0: 756e 2020 2320 7479 7065 3a20 6967 6e6f  un  # type: igno
-0000f400: 7265 0a20 2020 2020 2020 2065 7863 6570  re.        excep
-0000f410: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
-0000f420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f430: 736b 6970 5465 7374 2822 496e 636f 6d70  skipTest("Incomp
-0000f440: 6174 6962 6c65 2043 6c69 636b 2076 6572  atible Click ver
-0000f450: 7369 6f6e 2229 0a0a 2020 2020 2020 2020  sion")..        
-0000f460: 6966 206e 6f74 2068 6173 6174 7472 285f  if not hasattr(_
-0000f470: 756e 6963 6f64 6566 756e 2c20 225f 7665  unicodefun, "_ve
-0000f480: 7269 6679 5f70 7974 686f 6e5f 656e 7622  rify_python_env"
-0000f490: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000f4a0: 656c 662e 736b 6970 5465 7374 2822 496e  elf.skipTest("In
-0000f4b0: 636f 6d70 6174 6962 6c65 2043 6c69 636b  compatible Click
-0000f4c0: 2076 6572 7369 6f6e 2229 0a0a 2020 2020   version")..    
-0000f4d0: 2020 2020 2320 4669 7273 742c 206c 6574      # First, let
-0000f4e0: 2773 2073 6565 2069 6620 436c 6963 6b20  's see if Click 
-0000f4f0: 6973 2063 7261 7368 696e 6720 7769 7468  is crashing with
-0000f500: 2061 2070 7265 6665 7272 6564 2041 5343   a preferred ASC
-0000f510: 4949 2063 6861 7273 6574 2e0a 2020 2020  II charset..    
-0000f520: 2020 2020 7769 7468 2070 6174 6368 2822      with patch("
-0000f530: 6c6f 6361 6c65 2e67 6574 7072 6566 6572  locale.getprefer
-0000f540: 7265 6465 6e63 6f64 696e 6722 2920 6173  redencoding") as
-0000f550: 2067 7065 3a0a 2020 2020 2020 2020 2020   gpe:.          
-0000f560: 2020 6770 652e 7265 7475 726e 5f76 616c    gpe.return_val
-0000f570: 7565 203d 2022 4153 4349 4922 0a20 2020  ue = "ASCII".   
-0000f580: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-0000f590: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-0000f5a0: 5275 6e74 696d 6545 7272 6f72 293a 0a20  RuntimeError):. 
-0000f5b0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-0000f5c0: 756e 6963 6f64 6566 756e 2e5f 7665 7269  unicodefun._veri
-0000f5d0: 6679 5f70 7974 686f 6e5f 656e 7628 290a  fy_python_env().
-0000f5e0: 2020 2020 2020 2020 2320 4e6f 772c 206c          # Now, l
-0000f5f0: 6574 2773 2073 696c 656e 6365 2043 6c69  et's silence Cli
-0000f600: 636b 2e2e 2e0a 2020 2020 2020 2020 6365  ck....        ce
-0000f610: 7263 6973 2e70 6174 6368 5f63 6c69 636b  rcis.patch_click
-0000f620: 2829 0a20 2020 2020 2020 2023 202e 2e2e  ().        # ...
-0000f630: 616e 6420 636f 6e66 6972 6d20 6974 2773  and confirm it's
-0000f640: 2073 696c 656e 742e 0a20 2020 2020 2020   silent..       
-0000f650: 2077 6974 6820 7061 7463 6828 226c 6f63   with patch("loc
-0000f660: 616c 652e 6765 7470 7265 6665 7272 6564  ale.getpreferred
-0000f670: 656e 636f 6469 6e67 2229 2061 7320 6770  encoding") as gp
-0000f680: 653a 0a20 2020 2020 2020 2020 2020 2067  e:.            g
-0000f690: 7065 2e72 6574 7572 6e5f 7661 6c75 6520  pe.return_value 
-0000f6a0: 3d20 2241 5343 4949 220a 2020 2020 2020  = "ASCII".      
-0000f6b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000f6c0: 2020 2020 2020 2020 2020 205f 756e 6963             _unic
-0000f6d0: 6f64 6566 756e 2e5f 7665 7269 6679 5f70  odefun._verify_p
-0000f6e0: 7974 686f 6e5f 656e 7628 290a 2020 2020  ython_env().    
-0000f6f0: 2020 2020 2020 2020 6578 6365 7074 2052          except R
-0000f700: 756e 7469 6d65 4572 726f 7220 6173 2072  untimeError as r
-0000f710: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000f720: 2020 2073 656c 662e 6661 696c 2866 2260     self.fail(f"`
-0000f730: 7061 7463 685f 636c 6963 6b28 2960 2066  patch_click()` f
-0000f740: 6169 6c65 642c 2065 7863 6570 7469 6f6e  ailed, exception
-0000f750: 2073 7469 6c6c 2072 6169 7365 643a 207b   still raised: {
-0000f760: 7265 7d22 290a 0a20 2020 2064 6566 2074  re}")..    def t
-0000f770: 6573 745f 726f 6f74 5f6c 6f67 6765 725f  est_root_logger_
-0000f780: 6e6f 745f 7573 6564 5f64 6972 6563 746c  not_used_directl
-0000f790: 7928 7365 6c66 2920 2d3e 204e 6f6e 653a  y(self) -> None:
-0000f7a0: 0a20 2020 2020 2020 2064 6566 2066 6169  .        def fai
-0000f7b0: 6c28 2a61 7267 733a 2041 6e79 2c20 2a2a  l(*args: Any, **
-0000f7c0: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
-0000f7d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000f7e0: 2020 7365 6c66 2e66 6169 6c28 2252 6563    self.fail("Rec
-0000f7f0: 6f72 6420 6372 6561 7465 6420 7769 7468  ord created with
-0000f800: 2072 6f6f 7420 6c6f 6767 6572 2229 0a0a   root logger")..
-0000f810: 2020 2020 2020 2020 7769 7468 2070 6174          with pat
-0000f820: 6368 2e6d 756c 7469 706c 6528 0a20 2020  ch.multiple(.   
-0000f830: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
-0000f840: 2e72 6f6f 742c 0a20 2020 2020 2020 2020  .root,.         
-0000f850: 2020 2064 6562 7567 3d66 6169 6c2c 0a20     debug=fail,. 
-0000f860: 2020 2020 2020 2020 2020 2069 6e66 6f3d             info=
-0000f870: 6661 696c 2c0a 2020 2020 2020 2020 2020  fail,.          
-0000f880: 2020 7761 726e 696e 673d 6661 696c 2c0a    warning=fail,.
-0000f890: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-0000f8a0: 723d 6661 696c 2c0a 2020 2020 2020 2020  r=fail,.        
-0000f8b0: 2020 2020 6372 6974 6963 616c 3d66 6169      critical=fai
-0000f8c0: 6c2c 0a20 2020 2020 2020 2020 2020 206c  l,.            l
-0000f8d0: 6f67 3d66 6169 6c2c 0a20 2020 2020 2020  og=fail,.       
-0000f8e0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000f8f0: 6666 2854 4849 535f 4449 5220 2f20 2275  ff(THIS_DIR / "u
-0000f900: 7469 6c2e 7079 2229 0a0a 2020 2020 6465  til.py")..    de
-0000f910: 6620 7465 7374 5f69 6e76 616c 6964 5f63  f test_invalid_c
-0000f920: 6f6e 6669 675f 7265 7475 726e 5f63 6f64  onfig_return_cod
-0000f930: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-0000f940: 0a20 2020 2020 2020 2074 6d70 5f66 696c  .        tmp_fil
-0000f950: 6520 3d20 5061 7468 2863 6572 6369 732e  e = Path(cercis.
-0000f960: 6475 6d70 5f74 6f5f 6669 6c65 2829 290a  dump_to_file()).
-0000f970: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000f980: 2020 2020 2020 2020 2074 6d70 5f63 6f6e           tmp_con
-0000f990: 6669 6720 3d20 5061 7468 2863 6572 6369  fig = Path(cerci
-0000f9a0: 732e 6475 6d70 5f74 6f5f 6669 6c65 2829  s.dump_to_file()
-0000f9b0: 290a 2020 2020 2020 2020 2020 2020 746d  ).            tm
-0000f9c0: 705f 636f 6e66 6967 2e75 6e6c 696e 6b28  p_config.unlink(
-0000f9d0: 290a 2020 2020 2020 2020 2020 2020 6172  ).            ar
-0000f9e0: 6773 203d 205b 222d 2d63 6f6e 6669 6722  gs = ["--config"
-0000f9f0: 2c20 7374 7228 746d 705f 636f 6e66 6967  , str(tmp_config
-0000fa00: 292c 2073 7472 2874 6d70 5f66 696c 6529  ), str(tmp_file)
-0000fa10: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
-0000fa20: 6c66 2e69 6e76 6f6b 6542 6c61 636b 2861  lf.invokeBlack(a
-0000fa30: 7267 732c 2065 7869 745f 636f 6465 3d32  rgs, exit_code=2
-0000fa40: 2c20 6967 6e6f 7265 5f63 6f6e 6669 673d  , ignore_config=
-0000fa50: 4661 6c73 6529 0a20 2020 2020 2020 2066  False).        f
-0000fa60: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-0000fa70: 2020 2020 746d 705f 6669 6c65 2e75 6e6c      tmp_file.unl
-0000fa80: 696e 6b28 290a 0a20 2020 2064 6566 2074  ink()..    def t
-0000fa90: 6573 745f 7061 7273 655f 7079 7072 6f6a  est_parse_pyproj
-0000faa0: 6563 745f 746f 6d6c 2873 656c 6629 202d  ect_toml(self) -
-0000fab0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000fac0: 7465 7374 5f74 6f6d 6c5f 6669 6c65 203d  test_toml_file =
-0000fad0: 2054 4849 535f 4449 5220 2f20 2274 6573   THIS_DIR / "tes
-0000fae0: 742e 746f 6d6c 220a 2020 2020 2020 2020  t.toml".        
-0000faf0: 636f 6e66 6967 203d 2063 6572 6369 732e  config = cercis.
-0000fb00: 7061 7273 655f 7079 7072 6f6a 6563 745f  parse_pyproject_
-0000fb10: 746f 6d6c 2873 7472 2874 6573 745f 746f  toml(str(test_to
-0000fb20: 6d6c 5f66 696c 6529 290a 2020 2020 2020  ml_file)).      
-0000fb30: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000fb40: 616c 2863 6f6e 6669 675b 2276 6572 626f  al(config["verbo
-0000fb50: 7365 225d 2c20 3129 0a20 2020 2020 2020  se"], 1).       
-0000fb60: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000fb70: 6c28 636f 6e66 6967 5b22 6368 6563 6b22  l(config["check"
-0000fb80: 5d2c 2022 6e6f 2229 0a20 2020 2020 2020  ], "no").       
-0000fb90: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000fba0: 6c28 636f 6e66 6967 5b22 6469 6666 225d  l(config["diff"]
-0000fbb0: 2c20 2279 2229 0a20 2020 2020 2020 2073  , "y").        s
-0000fbc0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000fbd0: 636f 6e66 6967 5b22 636f 6c6f 7222 5d2c  config["color"],
-0000fbe0: 2054 7275 6529 0a20 2020 2020 2020 2073   True).        s
-0000fbf0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000fc00: 636f 6e66 6967 5b22 6c69 6e65 5f6c 656e  config["line_len
-0000fc10: 6774 6822 5d2c 2037 3929 0a20 2020 2020  gth"], 79).     
-0000fc20: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000fc30: 7561 6c28 636f 6e66 6967 5b22 7461 7267  ual(config["targ
-0000fc40: 6574 5f76 6572 7369 6f6e 225d 2c20 5b22  et_version"], ["
-0000fc50: 7079 3336 222c 2022 7079 3337 222c 2022  py36", "py37", "
-0000fc60: 7079 3338 225d 290a 2020 2020 2020 2020  py38"]).        
-0000fc70: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000fc80: 2863 6f6e 6669 675b 2270 7974 686f 6e5f  (config["python_
-0000fc90: 6365 6c6c 5f6d 6167 6963 7322 5d2c 205b  cell_magics"], [
-0000fca0: 2263 7573 746f 6d31 222c 2022 6375 7374  "custom1", "cust
-0000fcb0: 6f6d 3222 5d29 0a20 2020 2020 2020 2073  om2"]).        s
-0000fcc0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000fcd0: 636f 6e66 6967 5b22 6578 636c 7564 6522  config["exclude"
-0000fce0: 5d2c 2072 225c 2e70 7969 3f24 2229 0a20  ], r"\.pyi?$"). 
-0000fcf0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000fd00: 7274 4571 7561 6c28 636f 6e66 6967 5b22  rtEqual(config["
-0000fd10: 696e 636c 7564 6522 5d2c 2072 225c 2e70  include"], r"\.p
-0000fd20: 793f 2422 290a 0a20 2020 2064 6566 2074  y?$")..    def t
-0000fd30: 6573 745f 7061 7273 655f 7079 7072 6f6a  est_parse_pyproj
-0000fd40: 6563 745f 746f 6d6c 5f70 726f 6a65 6374  ect_toml_project
-0000fd50: 5f6d 6574 6164 6174 6128 7365 6c66 2920  _metadata(self) 
-0000fd60: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000fd70: 2066 6f72 2074 6573 745f 746f 6d6c 2c20   for test_toml, 
-0000fd80: 6578 7065 6374 6564 2069 6e20 5b0a 2020  expected in [.  
-0000fd90: 2020 2020 2020 2020 2020 2822 6f6e 6c79            ("only
-0000fda0: 5f62 6c61 636b 5f70 7970 726f 6a65 6374  _black_pyproject
-0000fdb0: 2e74 6f6d 6c22 2c20 5b22 7079 3331 3022  .toml", ["py310"
-0000fdc0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-0000fdd0: 2822 6f6e 6c79 5f6d 6574 6164 6174 615f  ("only_metadata_
-0000fde0: 7079 7072 6f6a 6563 742e 746f 6d6c 222c  pyproject.toml",
-0000fdf0: 205b 2270 7933 3722 2c20 2270 7933 3822   ["py37", "py38"
-0000fe00: 2c20 2270 7933 3922 2c20 2270 7933 3130  , "py39", "py310
-0000fe10: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
-0000fe20: 2028 226e 6569 7468 6572 5f70 7970 726f   ("neither_pypro
-0000fe30: 6a65 6374 2e74 6f6d 6c22 2c20 4e6f 6e65  ject.toml", None
-0000fe40: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0000fe50: 2262 6f74 685f 7079 7072 6f6a 6563 742e  "both_pyproject.
-0000fe60: 746f 6d6c 222c 205b 2270 7933 3130 225d  toml", ["py310"]
-0000fe70: 292c 0a20 2020 2020 2020 205d 3a0a 2020  ),.        ]:.  
-0000fe80: 2020 2020 2020 2020 2020 7465 7374 5f74            test_t
-0000fe90: 6f6d 6c5f 6669 6c65 203d 2054 4849 535f  oml_file = THIS_
-0000fea0: 4449 5220 2f20 2264 6174 6122 202f 2022  DIR / "data" / "
-0000feb0: 7072 6f6a 6563 745f 6d65 7461 6461 7461  project_metadata
-0000fec0: 2220 2f20 7465 7374 5f74 6f6d 6c0a 2020  " / test_toml.  
-0000fed0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000fee0: 203d 2063 6572 6369 732e 7061 7273 655f   = cercis.parse_
-0000fef0: 7079 7072 6f6a 6563 745f 746f 6d6c 2873  pyproject_toml(s
-0000ff00: 7472 2874 6573 745f 746f 6d6c 5f66 696c  tr(test_toml_fil
-0000ff10: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-0000ff20: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000ff30: 2863 6f6e 6669 672e 6765 7428 2274 6172  (config.get("tar
-0000ff40: 6765 745f 7665 7273 696f 6e22 292c 2065  get_version"), e
-0000ff50: 7870 6563 7465 6429 0a0a 2020 2020 6465  xpected)..    de
-0000ff60: 6620 7465 7374 5f69 6e66 6572 5f74 6172  f test_infer_tar
-0000ff70: 6765 745f 7665 7273 696f 6e28 7365 6c66  get_version(self
-0000ff80: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000ff90: 2020 2066 6f72 2076 6572 7369 6f6e 2c20     for version, 
-0000ffa0: 6578 7065 6374 6564 2069 6e20 5b0a 2020  expected in [.  
-0000ffb0: 2020 2020 2020 2020 2020 2822 332e 3622            ("3.6"
-0000ffc0: 2c20 5b54 6172 6765 7456 6572 7369 6f6e  , [TargetVersion
-0000ffd0: 2e50 5933 365d 292c 0a20 2020 2020 2020  .PY36]),.       
-0000ffe0: 2020 2020 2028 2233 2e31 312e 3072 6331       ("3.11.0rc1
-0000fff0: 222c 205b 5461 7267 6574 5665 7273 696f  ", [TargetVersio
-00010000: 6e2e 5059 3331 315d 292c 0a20 2020 2020  n.PY311]),.     
-00010010: 2020 2020 2020 2028 223e 3d33 2e31 3022         (">=3.10"
-00010020: 2c20 5b54 6172 6765 7456 6572 7369 6f6e  , [TargetVersion
-00010030: 2e50 5933 3130 2c20 5461 7267 6574 5665  .PY310, TargetVe
-00010040: 7273 696f 6e2e 5059 3331 315d 292c 0a20  rsion.PY311]),. 
-00010050: 2020 2020 2020 2020 2020 2028 223e 3d33             (">=3
-00010060: 2e31 302e 3622 2c20 5b54 6172 6765 7456  .10.6", [TargetV
-00010070: 6572 7369 6f6e 2e50 5933 3130 2c20 5461  ersion.PY310, Ta
-00010080: 7267 6574 5665 7273 696f 6e2e 5059 3331  rgetVersion.PY31
-00010090: 315d 292c 0a20 2020 2020 2020 2020 2020  1]),.           
-000100a0: 2028 223c 332e 3622 2c20 5b54 6172 6765   ("<3.6", [Targe
-000100b0: 7456 6572 7369 6f6e 2e50 5933 332c 2054  tVersion.PY33, T
-000100c0: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
-000100d0: 342c 2054 6172 6765 7456 6572 7369 6f6e  4, TargetVersion
-000100e0: 2e50 5933 355d 292c 0a20 2020 2020 2020  .PY35]),.       
-000100f0: 2020 2020 2028 223e 332e 372c 3c33 2e31       (">3.7,<3.1
-00010100: 3022 2c20 5b54 6172 6765 7456 6572 7369  0", [TargetVersi
-00010110: 6f6e 2e50 5933 382c 2054 6172 6765 7456  on.PY38, TargetV
-00010120: 6572 7369 6f6e 2e50 5933 395d 292c 0a20  ersion.PY39]),. 
-00010130: 2020 2020 2020 2020 2020 2028 223e 332e             (">3.
-00010140: 372c 213d 332e 382c 213d 332e 3922 2c20  7,!=3.8,!=3.9", 
-00010150: 5b54 6172 6765 7456 6572 7369 6f6e 2e50  [TargetVersion.P
-00010160: 5933 3130 2c20 5461 7267 6574 5665 7273  Y310, TargetVers
-00010170: 696f 6e2e 5059 3331 315d 292c 0a20 2020  ion.PY311]),.   
-00010180: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-00010190: 2020 2020 2020 2020 2020 2022 3e20 332e             "> 3.
-000101a0: 392e 342c 2021 3d20 332e 3130 2e33 222c  9.4, != 3.10.3",
-000101b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101c0: 205b 5461 7267 6574 5665 7273 696f 6e2e   [TargetVersion.
-000101d0: 5059 3339 2c20 5461 7267 6574 5665 7273  PY39, TargetVers
-000101e0: 696f 6e2e 5059 3331 302c 2054 6172 6765  ion.PY310, Targe
-000101f0: 7456 6572 7369 6f6e 2e50 5933 3131 5d2c  tVersion.PY311],
-00010200: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00010210: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-00010220: 2020 2020 2020 2020 2020 2020 2020 2221                "!
-00010230: 3d33 2e33 2c21 3d33 2e34 222c 0a20 2020  =3.3,!=3.4",.   
-00010240: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2054 6172 6765 7456 6572 7369 6f6e     TargetVersion
-00010270: 2e50 5933 352c 0a20 2020 2020 2020 2020  .PY35,.         
-00010280: 2020 2020 2020 2020 2020 2054 6172 6765             Targe
-00010290: 7456 6572 7369 6f6e 2e50 5933 362c 0a20  tVersion.PY36,. 
-000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102b0: 2020 2054 6172 6765 7456 6572 7369 6f6e     TargetVersion
-000102c0: 2e50 5933 372c 0a20 2020 2020 2020 2020  .PY37,.         
-000102d0: 2020 2020 2020 2020 2020 2054 6172 6765             Targe
-000102e0: 7456 6572 7369 6f6e 2e50 5933 382c 0a20  tVersion.PY38,. 
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 2054 6172 6765 7456 6572 7369 6f6e     TargetVersion
-00010310: 2e50 5933 392c 0a20 2020 2020 2020 2020  .PY39,.         
-00010320: 2020 2020 2020 2020 2020 2054 6172 6765             Targe
-00010330: 7456 6572 7369 6f6e 2e50 5933 3130 2c0a  tVersion.PY310,.
-00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010350: 2020 2020 5461 7267 6574 5665 7273 696f      TargetVersio
-00010360: 6e2e 5059 3331 312c 0a20 2020 2020 2020  n.PY311,.       
-00010370: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00010380: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00010390: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-000103a0: 2020 2020 2020 2020 2022 3d3d 332e 2a22           "==3.*"
-000103b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000103c0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000103d0: 2020 2020 2020 2020 5461 7267 6574 5665          TargetVe
-000103e0: 7273 696f 6e2e 5059 3333 2c0a 2020 2020  rsion.PY33,.    
-000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010400: 5461 7267 6574 5665 7273 696f 6e2e 5059  TargetVersion.PY
-00010410: 3334 2c0a 2020 2020 2020 2020 2020 2020  34,.            
-00010420: 2020 2020 2020 2020 5461 7267 6574 5665          TargetVe
-00010430: 7273 696f 6e2e 5059 3335 2c0a 2020 2020  rsion.PY35,.    
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 5461 7267 6574 5665 7273 696f 6e2e 5059  TargetVersion.PY
-00010460: 3336 2c0a 2020 2020 2020 2020 2020 2020  36,.            
-00010470: 2020 2020 2020 2020 5461 7267 6574 5665          TargetVe
-00010480: 7273 696f 6e2e 5059 3337 2c0a 2020 2020  rsion.PY37,.    
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 5461 7267 6574 5665 7273 696f 6e2e 5059  TargetVersion.PY
-000104b0: 3338 2c0a 2020 2020 2020 2020 2020 2020  38,.            
-000104c0: 2020 2020 2020 2020 5461 7267 6574 5665          TargetVe
-000104d0: 7273 696f 6e2e 5059 3339 2c0a 2020 2020  rsion.PY39,.    
-000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104f0: 5461 7267 6574 5665 7273 696f 6e2e 5059  TargetVersion.PY
-00010500: 3331 302c 0a20 2020 2020 2020 2020 2020  310,.           
-00010510: 2020 2020 2020 2020 2054 6172 6765 7456           TargetV
-00010520: 6572 7369 6f6e 2e50 5933 3131 2c0a 2020  ersion.PY311,.  
-00010530: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00010540: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00010550: 2020 2020 2020 2020 2020 2020 2822 3d3d              ("==
-00010560: 332e 382e 2a22 2c20 5b54 6172 6765 7456  3.8.*", [TargetV
-00010570: 6572 7369 6f6e 2e50 5933 385d 292c 0a20  ersion.PY38]),. 
-00010580: 2020 2020 2020 2020 2020 2028 4e6f 6e65             (None
-00010590: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
-000105a0: 2020 2020 2028 2222 2c20 4e6f 6e65 292c       ("", None),
-000105b0: 0a20 2020 2020 2020 2020 2020 2028 2269  .            ("i
-000105c0: 6e76 616c 6964 222c 204e 6f6e 6529 2c0a  nvalid", None),.
-000105d0: 2020 2020 2020 2020 2020 2020 2822 3d3d              ("==
-000105e0: 696e 7661 6c69 6422 2c20 4e6f 6e65 292c  invalid", None),
-000105f0: 0a20 2020 2020 2020 2020 2020 2028 223e  .            (">
-00010600: 332e 392c 213d 696e 7661 6c69 6422 2c20  3.9,!=invalid", 
-00010610: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
-00010620: 2020 2028 2233 222c 204e 6f6e 6529 2c0a     ("3", None),.
-00010630: 2020 2020 2020 2020 2020 2020 2822 332e              ("3.
-00010640: 3222 2c20 4e6f 6e65 292c 0a20 2020 2020  2", None),.     
-00010650: 2020 2020 2020 2028 2232 2e37 2e31 3822         ("2.7.18"
-00010660: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
-00010670: 2020 2020 2028 223d 3d32 2e37 222c 204e       ("==2.7", N
-00010680: 6f6e 6529 2c0a 2020 2020 2020 2020 2020  one),.          
-00010690: 2020 2822 3e33 2e31 302c 3c33 2e31 3122    (">3.10,<3.11"
-000106a0: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
-000106b0: 205d 3a0a 2020 2020 2020 2020 2020 2020   ]:.            
-000106c0: 7465 7374 5f74 6f6d 6c20 3d20 7b22 7072  test_toml = {"pr
-000106d0: 6f6a 6563 7422 3a20 7b22 7265 7175 6972  oject": {"requir
-000106e0: 6573 2d70 7974 686f 6e22 3a20 7665 7273  es-python": vers
-000106f0: 696f 6e7d 7d0a 2020 2020 2020 2020 2020  ion}}.          
-00010700: 2020 7265 7375 6c74 203d 2063 6572 6369    result = cerci
-00010710: 732e 6669 6c65 732e 696e 6665 725f 7461  s.files.infer_ta
-00010720: 7267 6574 5f76 6572 7369 6f6e 2874 6573  rget_version(tes
-00010730: 745f 746f 6d6c 290a 2020 2020 2020 2020  t_toml).        
-00010740: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00010750: 7175 616c 2872 6573 756c 742c 2065 7870  qual(result, exp
-00010760: 6563 7465 6429 0a0a 2020 2020 6465 6620  ected)..    def 
-00010770: 7465 7374 5f72 6561 645f 7079 7072 6f6a  test_read_pyproj
-00010780: 6563 745f 746f 6d6c 2873 656c 6629 202d  ect_toml(self) -
-00010790: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000107a0: 7465 7374 5f74 6f6d 6c5f 6669 6c65 203d  test_toml_file =
-000107b0: 2054 4849 535f 4449 5220 2f20 2274 6573   THIS_DIR / "tes
-000107c0: 742e 746f 6d6c 220a 2020 2020 2020 2020  t.toml".        
-000107d0: 6661 6b65 5f63 7478 203d 2046 616b 6543  fake_ctx = FakeC
-000107e0: 6f6e 7465 7874 2829 0a20 2020 2020 2020  ontext().       
-000107f0: 2063 6572 6369 732e 7265 6164 5f70 7970   cercis.read_pyp
-00010800: 726f 6a65 6374 5f74 6f6d 6c28 6661 6b65  roject_toml(fake
-00010810: 5f63 7478 2c20 4661 6b65 5061 7261 6d65  _ctx, FakeParame
-00010820: 7465 7228 292c 2073 7472 2874 6573 745f  ter(), str(test_
-00010830: 746f 6d6c 5f66 696c 6529 290a 2020 2020  toml_file)).    
-00010840: 2020 2020 636f 6e66 6967 203d 2066 616b      config = fak
-00010850: 655f 6374 782e 6465 6661 756c 745f 6d61  e_ctx.default_ma
-00010860: 700a 2020 2020 2020 2020 7365 6c66 2e61  p.        self.a
-00010870: 7373 6572 7445 7175 616c 2863 6f6e 6669  ssertEqual(confi
-00010880: 675b 2276 6572 626f 7365 225d 2c20 2231  g["verbose"], "1
-00010890: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000108a0: 6173 7365 7274 4571 7561 6c28 636f 6e66  assertEqual(conf
-000108b0: 6967 5b22 6368 6563 6b22 5d2c 2022 6e6f  ig["check"], "no
-000108c0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000108d0: 6173 7365 7274 4571 7561 6c28 636f 6e66  assertEqual(conf
-000108e0: 6967 5b22 6469 6666 225d 2c20 2279 2229  ig["diff"], "y")
-000108f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00010900: 7365 7274 4571 7561 6c28 636f 6e66 6967  sertEqual(config
-00010910: 5b22 636f 6c6f 7222 5d2c 2022 5472 7565  ["color"], "True
-00010920: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00010930: 6173 7365 7274 4571 7561 6c28 636f 6e66  assertEqual(conf
-00010940: 6967 5b22 6c69 6e65 5f6c 656e 6774 6822  ig["line_length"
-00010950: 5d2c 2022 3739 2229 0a20 2020 2020 2020  ], "79").       
-00010960: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00010970: 6c28 636f 6e66 6967 5b22 7461 7267 6574  l(config["target
-00010980: 5f76 6572 7369 6f6e 225d 2c20 5b22 7079  _version"], ["py
-00010990: 3336 222c 2022 7079 3337 222c 2022 7079  36", "py37", "py
-000109a0: 3338 225d 290a 2020 2020 2020 2020 7365  38"]).        se
-000109b0: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
-000109c0: 6f6e 6669 675b 2265 7863 6c75 6465 225d  onfig["exclude"]
-000109d0: 2c20 7222 5c2e 7079 693f 2422 290a 2020  , r"\.pyi?$").  
-000109e0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000109f0: 7445 7175 616c 2863 6f6e 6669 675b 2269  tEqual(config["i
-00010a00: 6e63 6c75 6465 225d 2c20 7222 5c2e 7079  nclude"], r"\.py
-00010a10: 3f24 2229 0a0a 2020 2020 4070 7974 6573  ?$")..    @pytes
-00010a20: 742e 6d61 726b 2e69 6e63 6f6d 7061 7469  t.mark.incompati
-00010a30: 626c 655f 7769 7468 5f6d 7970 7963 0a20  ble_with_mypyc. 
-00010a40: 2020 2064 6566 2074 6573 745f 6669 6e64     def test_find
-00010a50: 5f70 726f 6a65 6374 5f72 6f6f 7428 7365  _project_root(se
-00010a60: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00010a70: 2020 2020 2077 6974 6820 5465 6d70 6f72       with Tempor
-00010a80: 6172 7944 6972 6563 746f 7279 2829 2061  aryDirectory() a
-00010a90: 7320 776f 726b 7370 6163 653a 0a20 2020  s workspace:.   
-00010aa0: 2020 2020 2020 2020 2072 6f6f 7420 3d20           root = 
-00010ab0: 5061 7468 2877 6f72 6b73 7061 6365 290a  Path(workspace).
-00010ac0: 2020 2020 2020 2020 2020 2020 7465 7374              test
-00010ad0: 5f64 6972 203d 2072 6f6f 7420 2f20 2274  _dir = root / "t
-00010ae0: 6573 7422 0a20 2020 2020 2020 2020 2020  est".           
-00010af0: 2074 6573 745f 6469 722e 6d6b 6469 7228   test_dir.mkdir(
-00010b00: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00010b10: 7263 5f64 6972 203d 2072 6f6f 7420 2f20  rc_dir = root / 
-00010b20: 2273 7263 220a 2020 2020 2020 2020 2020  "src".          
-00010b30: 2020 7372 635f 6469 722e 6d6b 6469 7228    src_dir.mkdir(
-00010b40: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00010b50: 6f6f 745f 7079 7072 6f6a 6563 7420 3d20  oot_pyproject = 
-00010b60: 726f 6f74 202f 2022 7079 7072 6f6a 6563  root / "pyprojec
-00010b70: 742e 746f 6d6c 220a 2020 2020 2020 2020  t.toml".        
-00010b80: 2020 2020 726f 6f74 5f70 7970 726f 6a65      root_pyproje
-00010b90: 6374 2e74 6f75 6368 2829 0a20 2020 2020  ct.touch().     
-00010ba0: 2020 2020 2020 2073 7263 5f70 7970 726f         src_pypro
-00010bb0: 6a65 6374 203d 2073 7263 5f64 6972 202f  ject = src_dir /
-00010bc0: 2022 7079 7072 6f6a 6563 742e 746f 6d6c   "pyproject.toml
-00010bd0: 220a 2020 2020 2020 2020 2020 2020 7372  ".            sr
-00010be0: 635f 7079 7072 6f6a 6563 742e 746f 7563  c_pyproject.touc
-00010bf0: 6828 290a 2020 2020 2020 2020 2020 2020  h().            
-00010c00: 7372 635f 7079 7468 6f6e 203d 2073 7263  src_python = src
-00010c10: 5f64 6972 202f 2022 666f 6f2e 7079 220a  _dir / "foo.py".
-00010c20: 2020 2020 2020 2020 2020 2020 7372 635f              src_
-00010c30: 7079 7468 6f6e 2e74 6f75 6368 2829 0a0a  python.touch()..
-00010c40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010c50: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
-00010c60: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00010c70: 7263 6973 2e66 696e 645f 7072 6f6a 6563  rcis.find_projec
-00010c80: 745f 726f 6f74 2828 7372 635f 6469 722c  t_root((src_dir,
-00010c90: 2074 6573 745f 6469 7229 292c 0a20 2020   test_dir)),.   
-00010ca0: 2020 2020 2020 2020 2020 2020 2028 726f               (ro
-00010cb0: 6f74 2e72 6573 6f6c 7665 2829 2c20 2270  ot.resolve(), "p
-00010cc0: 7970 726f 6a65 6374 2e74 6f6d 6c22 292c  yproject.toml"),
-00010cd0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00010ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010cf0: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00010d00: 2020 2020 2020 2020 2020 2020 2063 6572               cer
-00010d10: 6369 732e 6669 6e64 5f70 726f 6a65 6374  cis.find_project
-00010d20: 5f72 6f6f 7428 2873 7263 5f64 6972 2c29  _root((src_dir,)
-00010d30: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00010d40: 2020 2028 7372 635f 6469 722e 7265 736f     (src_dir.reso
-00010d50: 6c76 6528 292c 2022 7079 7072 6f6a 6563  lve(), "pyprojec
-00010d60: 742e 746f 6d6c 2229 2c0a 2020 2020 2020  t.toml"),.      
-00010d70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010d80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00010d90: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-00010da0: 2020 2020 2020 6365 7263 6973 2e66 696e        cercis.fin
-00010db0: 645f 7072 6f6a 6563 745f 726f 6f74 2828  d_project_root((
-00010dc0: 7372 635f 7079 7468 6f6e 2c29 292c 0a20  src_python,)),. 
-00010dd0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00010de0: 7372 635f 6469 722e 7265 736f 6c76 6528  src_dir.resolve(
-00010df0: 292c 2022 7079 7072 6f6a 6563 742e 746f  ), "pyproject.to
-00010e00: 6d6c 2229 2c0a 2020 2020 2020 2020 2020  ml"),.          
-00010e10: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00010e20: 2077 6974 6820 6368 616e 6765 5f64 6972   with change_dir
-00010e30: 6563 746f 7279 2874 6573 745f 6469 7229  ectory(test_dir)
-00010e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010e50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00010e60: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00010e70: 2020 2020 2020 2020 6365 7263 6973 2e66          cercis.f
-00010e80: 696e 645f 7072 6f6a 6563 745f 726f 6f74  ind_project_root
-00010e90: 2828 222d 222c 292c 2073 7464 696e 5f66  (("-",), stdin_f
-00010ea0: 696c 656e 616d 653d 222e 2e2f 7372 632f  ilename="../src/
-00010eb0: 612e 7079 2229 2c0a 2020 2020 2020 2020  a.py"),.        
-00010ec0: 2020 2020 2020 2020 2020 2020 2873 7263              (src
-00010ed0: 5f64 6972 2e72 6573 6f6c 7665 2829 2c20  _dir.resolve(), 
-00010ee0: 2270 7970 726f 6a65 6374 2e74 6f6d 6c22  "pyproject.toml"
-00010ef0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00010f00: 2020 2029 0a0a 2020 2020 4070 6174 6368     )..    @patch
-00010f10: 280a 2020 2020 2020 2020 2263 6572 6369  (.        "cerci
-00010f20: 732e 6669 6c65 732e 6669 6e64 5f75 7365  s.files.find_use
-00010f30: 725f 7079 7072 6f6a 6563 745f 746f 6d6c  r_pyproject_toml
-00010f40: 222c 0a20 2020 2029 0a20 2020 2064 6566  ",.    ).    def
-00010f50: 2074 6573 745f 6669 6e64 5f70 7970 726f   test_find_pypro
-00010f60: 6a65 6374 5f74 6f6d 6c28 7365 6c66 2c20  ject_toml(self, 
-00010f70: 6669 6e64 5f75 7365 725f 7079 7072 6f6a  find_user_pyproj
-00010f80: 6563 745f 746f 6d6c 3a20 4d61 6769 634d  ect_toml: MagicM
-00010f90: 6f63 6b29 202d 3e20 4e6f 6e65 3a0a 2020  ock) -> None:.  
-00010fa0: 2020 2020 2020 6669 6e64 5f75 7365 725f        find_user_
-00010fb0: 7079 7072 6f6a 6563 745f 746f 6d6c 2e73  pyproject_toml.s
-00010fc0: 6964 655f 6566 6665 6374 203d 2052 756e  ide_effect = Run
-00010fd0: 7469 6d65 4572 726f 7228 290a 0a20 2020  timeError()..   
-00010fe0: 2020 2020 2077 6974 6820 7265 6469 7265       with redire
-00010ff0: 6374 5f73 7464 6572 7228 696f 2e53 7472  ct_stderr(io.Str
-00011000: 696e 6749 4f28 2929 2061 7320 7374 6465  ingIO()) as stde
-00011010: 7272 3a0a 2020 2020 2020 2020 2020 2020  rr:.            
-00011020: 7265 7375 6c74 203d 2063 6572 6369 732e  result = cercis.
-00011030: 6669 6c65 732e 6669 6e64 5f70 7970 726f  files.find_pypro
-00011040: 6a65 6374 5f74 6f6d 6c28 0a20 2020 2020  ject_toml(.     
-00011050: 2020 2020 2020 2020 2020 2070 6174 685f             path_
-00011060: 7365 6172 6368 5f73 7461 7274 3d28 7374  search_start=(st
-00011070: 7228 5061 7468 2e63 7764 2829 2e72 6f6f  r(Path.cwd().roo
-00011080: 7429 2c29 0a20 2020 2020 2020 2020 2020  t),).           
-00011090: 2029 0a0a 2020 2020 2020 2020 6173 7365   )..        asse
-000110a0: 7274 2072 6573 756c 7420 6973 204e 6f6e  rt result is Non
-000110b0: 650a 2020 2020 2020 2020 6572 7220 3d20  e.        err = 
-000110c0: 7374 6465 7272 2e67 6574 7661 6c75 6528  stderr.getvalue(
-000110d0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-000110e0: 2022 4967 6e6f 7269 6e67 2075 7365 7220   "Ignoring user 
-000110f0: 636f 6e66 6967 7572 6174 696f 6e22 2069  configuration" i
-00011100: 6e20 6572 720a 0a20 2020 2040 7061 7463  n err..    @patc
-00011110: 6828 0a20 2020 2020 2020 2022 6365 7263  h(.        "cerc
-00011120: 6973 2e66 696c 6573 2e66 696e 645f 7573  is.files.find_us
-00011130: 6572 5f70 7970 726f 6a65 6374 5f74 6f6d  er_pyproject_tom
-00011140: 6c22 2c0a 2020 2020 2020 2020 6365 7263  l",.        cerc
-00011150: 6973 2e66 696c 6573 2e66 696e 645f 7573  is.files.find_us
-00011160: 6572 5f70 7970 726f 6a65 6374 5f74 6f6d  er_pyproject_tom
-00011170: 6c2e 5f5f 7772 6170 7065 645f 5f2c 0a20  l.__wrapped__,. 
-00011180: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
-00011190: 745f 6669 6e64 5f75 7365 725f 7079 7072  t_find_user_pypr
-000111a0: 6f6a 6563 745f 746f 6d6c 5f6c 696e 7578  oject_toml_linux
-000111b0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000111c0: 2020 2020 2020 2020 6966 2073 7973 7465          if syste
-000111d0: 6d28 2920 3d3d 2022 5769 6e64 6f77 7322  m() == "Windows"
-000111e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000111f0: 7475 726e 0a0a 2020 2020 2020 2020 2320  turn..        # 
-00011200: 5465 7374 2069 6620 5844 475f 434f 4e46  Test if XDG_CONF
-00011210: 4947 5f48 4f4d 4520 6973 2063 6865 636b  IG_HOME is check
-00011220: 6564 0a20 2020 2020 2020 2077 6974 6820  ed.        with 
-00011230: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
-00011240: 7279 2829 2061 7320 776f 726b 7370 6163  ry() as workspac
-00011250: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00011260: 6d70 5f75 7365 725f 636f 6e66 6967 203d  mp_user_config =
-00011270: 2050 6174 6828 776f 726b 7370 6163 6529   Path(workspace)
-00011280: 202f 2022 6365 7263 6973 220a 2020 2020   / "cercis".    
-00011290: 2020 2020 2020 2020 7769 7468 2070 6174          with pat
-000112a0: 6368 2e64 6963 7428 226f 732e 656e 7669  ch.dict("os.envi
-000112b0: 726f 6e22 2c20 7b22 5844 475f 434f 4e46  ron", {"XDG_CONF
-000112c0: 4947 5f48 4f4d 4522 3a20 776f 726b 7370  IG_HOME": worksp
-000112d0: 6163 657d 293a 0a20 2020 2020 2020 2020  ace}):.         
-000112e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000112f0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
-00011300: 2020 2020 2020 2020 2020 2020 2063 6572               cer
-00011310: 6369 732e 6669 6c65 732e 6669 6e64 5f75  cis.files.find_u
-00011320: 7365 725f 7079 7072 6f6a 6563 745f 746f  ser_pyproject_to
-00011330: 6d6c 2829 2c20 746d 705f 7573 6572 5f63  ml(), tmp_user_c
-00011340: 6f6e 6669 672e 7265 736f 6c76 6528 290a  onfig.resolve().
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 290a 0a20 2020 2020 2020 2023 2054 6573  )..        # Tes
-00011370: 7420 6661 6c6c 6261 636b 2066 6f72 2058  t fallback for X
-00011380: 4447 5f43 4f4e 4649 475f 484f 4d45 0a20  DG_CONFIG_HOME. 
-00011390: 2020 2020 2020 2077 6974 6820 7061 7463         with patc
-000113a0: 682e 6469 6374 2822 6f73 2e65 6e76 6972  h.dict("os.envir
-000113b0: 6f6e 2229 3a0a 2020 2020 2020 2020 2020  on"):.          
-000113c0: 2020 6f73 2e65 6e76 6972 6f6e 2e70 6f70    os.environ.pop
-000113d0: 2822 5844 475f 434f 4e46 4947 5f48 4f4d  ("XDG_CONFIG_HOM
-000113e0: 4522 2c20 4e6f 6e65 290a 2020 2020 2020  E", None).      
-000113f0: 2020 2020 2020 6661 6c6c 6261 636b 5f75        fallback_u
-00011400: 7365 725f 636f 6e66 6967 203d 2050 6174  ser_config = Pat
-00011410: 6828 227e 2f2e 636f 6e66 6967 2229 2e65  h("~/.config").e
-00011420: 7870 616e 6475 7365 7228 2920 2f20 2263  xpanduser() / "c
-00011430: 6572 6369 7322 0a20 2020 2020 2020 2020  ercis".         
-00011440: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00011450: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
-00011460: 2020 2020 2063 6572 6369 732e 6669 6c65       cercis.file
-00011470: 732e 6669 6e64 5f75 7365 725f 7079 7072  s.find_user_pypr
-00011480: 6f6a 6563 745f 746f 6d6c 2829 2c20 6661  oject_toml(), fa
-00011490: 6c6c 6261 636b 5f75 7365 725f 636f 6e66  llback_user_conf
-000114a0: 6967 2e72 6573 6f6c 7665 2829 0a20 2020  ig.resolve().   
-000114b0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-000114c0: 6465 6620 7465 7374 5f66 696e 645f 7573  def test_find_us
-000114d0: 6572 5f70 7970 726f 6a65 6374 5f74 6f6d  er_pyproject_tom
-000114e0: 6c5f 7769 6e64 6f77 7328 7365 6c66 2920  l_windows(self) 
-000114f0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00011500: 2069 6620 7379 7374 656d 2829 2021 3d20   if system() != 
-00011510: 2257 696e 646f 7773 223a 0a20 2020 2020  "Windows":.     
-00011520: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-00011530: 2020 2020 2020 2075 7365 725f 636f 6e66         user_conf
-00011540: 6967 5f70 6174 6820 3d20 5061 7468 2e68  ig_path = Path.h
-00011550: 6f6d 6528 2920 2f20 222e 6365 7263 6973  ome() / ".cercis
-00011560: 220a 2020 2020 2020 2020 7365 6c66 2e61  ".        self.a
-00011570: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00011580: 2020 2020 2020 2020 6365 7263 6973 2e66          cercis.f
-00011590: 696c 6573 2e66 696e 645f 7573 6572 5f70  iles.find_user_p
-000115a0: 7970 726f 6a65 6374 5f74 6f6d 6c28 292c  yproject_toml(),
-000115b0: 2075 7365 725f 636f 6e66 6967 5f70 6174   user_config_pat
-000115c0: 682e 7265 736f 6c76 6528 290a 2020 2020  h.resolve().    
-000115d0: 2020 2020 290a 0a20 2020 2064 6566 2074      )..    def t
-000115e0: 6573 745f 6270 6f5f 3333 3636 305f 776f  est_bpo_33660_wo
-000115f0: 726b 6172 6f75 6e64 2873 656c 6629 202d  rkaround(self) -
-00011600: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00011610: 6966 2073 7973 7465 6d28 2920 3d3d 2022  if system() == "
-00011620: 5769 6e64 6f77 7322 3a0a 2020 2020 2020  Windows":.      
-00011630: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-00011640: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00011650: 6275 6773 2e70 7974 686f 6e2e 6f72 672f  bugs.python.org/
-00011660: 6973 7375 6533 3336 3630 0a20 2020 2020  issue33660.     
-00011670: 2020 2072 6f6f 7420 3d20 5061 7468 2822     root = Path("
-00011680: 2f22 290a 2020 2020 2020 2020 7769 7468  /").        with
-00011690: 2063 6861 6e67 655f 6469 7265 6374 6f72   change_director
-000116a0: 7928 726f 6f74 293a 0a20 2020 2020 2020  y(root):.       
-000116b0: 2020 2020 2070 6174 6820 3d20 5061 7468       path = Path
-000116c0: 2822 776f 726b 7370 6163 6522 2920 2f20  ("workspace") / 
-000116d0: 2270 726f 6a65 6374 220a 2020 2020 2020  "project".      
-000116e0: 2020 2020 2020 7265 706f 7274 203d 2063        report = c
-000116f0: 6572 6369 732e 5265 706f 7274 2876 6572  ercis.Report(ver
-00011700: 626f 7365 3d54 7275 6529 0a20 2020 2020  bose=True).     
-00011710: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
-00011720: 645f 7061 7468 203d 2063 6572 6369 732e  d_path = cercis.
-00011730: 6e6f 726d 616c 697a 655f 7061 7468 5f6d  normalize_path_m
-00011740: 6179 6265 5f69 676e 6f72 6528 7061 7468  aybe_ignore(path
-00011750: 2c20 726f 6f74 2c20 7265 706f 7274 290a  , root, report).
-00011760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011770: 2e61 7373 6572 7445 7175 616c 286e 6f72  .assertEqual(nor
-00011780: 6d61 6c69 7a65 645f 7061 7468 2c20 2277  malized_path, "w
-00011790: 6f72 6b73 7061 6365 2f70 726f 6a65 6374  orkspace/project
-000117a0: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
-000117b0: 5f6e 6f72 6d61 6c69 7a65 5f70 6174 685f  _normalize_path_
-000117c0: 6967 6e6f 7265 5f77 696e 646f 7773 5f6a  ignore_windows_j
-000117d0: 756e 6374 696f 6e73 5f6f 7574 7369 6465  unctions_outside
-000117e0: 5f6f 665f 726f 6f74 2873 656c 6629 202d  _of_root(self) -
-000117f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00011800: 6966 2073 7973 7465 6d28 2920 213d 2022  if system() != "
-00011810: 5769 6e64 6f77 7322 3a0a 2020 2020 2020  Windows":.      
-00011820: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-00011830: 2020 2020 2020 7769 7468 2054 656d 706f        with Tempo
-00011840: 7261 7279 4469 7265 6374 6f72 7928 2920  raryDirectory() 
-00011850: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
-00011860: 2020 2020 2020 2020 2020 726f 6f74 203d            root =
-00011870: 2050 6174 6828 776f 726b 7370 6163 6529   Path(workspace)
-00011880: 0a20 2020 2020 2020 2020 2020 206a 756e  .            jun
-00011890: 6374 696f 6e5f 6469 7220 3d20 726f 6f74  ction_dir = root
-000118a0: 202f 2022 6a75 6e63 7469 6f6e 220a 2020   / "junction".  
-000118b0: 2020 2020 2020 2020 2020 6a75 6e63 7469            juncti
-000118c0: 6f6e 5f74 6172 6765 745f 6f75 7473 6964  on_target_outsid
-000118d0: 655f 6f66 5f72 6f6f 7420 3d20 726f 6f74  e_of_root = root
-000118e0: 202f 2022 2e2e 220a 2020 2020 2020 2020   / "..".        
-000118f0: 2020 2020 6f73 2e73 7973 7465 6d28 6622      os.system(f"
-00011900: 6d6b 6c69 6e6b 202f 4a20 7b6a 756e 6374  mklink /J {junct
-00011910: 696f 6e5f 6469 727d 207b 6a75 6e63 7469  ion_dir} {juncti
-00011920: 6f6e 5f74 6172 6765 745f 6f75 7473 6964  on_target_outsid
-00011930: 655f 6f66 5f72 6f6f 747d 2229 0a0a 2020  e_of_root}")..  
-00011940: 2020 2020 2020 2020 2020 7265 706f 7274            report
-00011950: 203d 2063 6572 6369 732e 5265 706f 7274   = cercis.Report
-00011960: 2876 6572 626f 7365 3d54 7275 6529 0a20  (verbose=True). 
-00011970: 2020 2020 2020 2020 2020 206e 6f72 6d61             norma
-00011980: 6c69 7a65 645f 7061 7468 203d 2063 6572  lized_path = cer
-00011990: 6369 732e 6e6f 726d 616c 697a 655f 7061  cis.normalize_pa
-000119a0: 7468 5f6d 6179 6265 5f69 676e 6f72 6528  th_maybe_ignore(
-000119b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119c0: 206a 756e 6374 696f 6e5f 6469 722c 2072   junction_dir, r
-000119d0: 6f6f 742c 2072 6570 6f72 740a 2020 2020  oot, report.    
-000119e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000119f0: 2020 2020 2020 2320 4d61 6e75 616c 6c79        # Manually
-00011a00: 2064 656c 6574 6520 666f 7220 5079 7468   delete for Pyth
-00011a10: 6f6e 203c 2033 2e38 0a20 2020 2020 2020  on < 3.8.       
-00011a20: 2020 2020 206f 732e 7379 7374 656d 2866       os.system(f
-00011a30: 2272 6d64 6972 207b 6a75 6e63 7469 6f6e  "rmdir {junction
-00011a40: 5f64 6972 7d22 290a 0a20 2020 2020 2020  _dir}")..       
-00011a50: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00011a60: 4571 7561 6c28 6e6f 726d 616c 697a 6564  Equal(normalized
-00011a70: 5f70 6174 682c 204e 6f6e 6529 0a0a 2020  _path, None)..  
-00011a80: 2020 6465 6620 7465 7374 5f6e 6577 6c69    def test_newli
-00011a90: 6e65 5f63 6f6d 6d65 6e74 5f69 6e74 6572  ne_comment_inter
-00011aa0: 6163 7469 6f6e 2873 656c 6629 202d 3e20  action(self) -> 
-00011ab0: 4e6f 6e65 3a0a 2020 2020 2020 2020 736f  None:.        so
-00011ac0: 7572 6365 203d 2022 636c 6173 7320 413a  urce = "class A:
-00011ad0: 5c5c 5c72 5c6e 2320 7479 7065 3a20 6967  \\\r\n# type: ig
-00011ae0: 6e6f 7265 5c6e 2070 6173 735c 6e22 0a20  nore\n pass\n". 
-00011af0: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
-00011b00: 6365 7263 6973 2e66 6f72 6d61 745f 7374  cercis.format_st
-00011b10: 7228 736f 7572 6365 2c20 6d6f 6465 3d44  r(source, mode=D
-00011b20: 4546 4155 4c54 5f4d 4f44 4529 0a20 2020  EFAULT_MODE).   
-00011b30: 2020 2020 2063 6572 6369 732e 6173 7365       cercis.asse
-00011b40: 7274 5f73 7461 626c 6528 736f 7572 6365  rt_stable(source
-00011b50: 2c20 6f75 7470 7574 2c20 6d6f 6465 3d44  , output, mode=D
-00011b60: 4546 4155 4c54 5f4d 4f44 4529 0a0a 2020  EFAULT_MODE)..  
-00011b70: 2020 6465 6620 7465 7374 5f62 706f 5f32    def test_bpo_2
-00011b80: 3134 325f 776f 726b 6172 6f75 6e64 2873  142_workaround(s
-00011b90: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00011ba0: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00011bb0: 6275 6773 2e70 7974 686f 6e2e 6f72 672f  bugs.python.org/
-00011bc0: 6973 7375 6532 3134 320a 0a20 2020 2020  issue2142..     
-00011bd0: 2020 2073 6f75 7263 652c 205f 203d 2072     source, _ = r
-00011be0: 6561 645f 6461 7461 2822 6d69 7363 656c  ead_data("miscel
-00011bf0: 6c61 6e65 6f75 7322 2c20 226d 6973 7369  laneous", "missi
-00011c00: 6e67 5f66 696e 616c 5f6e 6577 6c69 6e65  ng_final_newline
-00011c10: 2229 0a20 2020 2020 2020 2023 2072 6561  ").        # rea
-00011c20: 645f 6461 7461 2061 6464 7320 6120 7472  d_data adds a tr
-00011c30: 6169 6c69 6e67 206e 6577 6c69 6e65 0a20  ailing newline. 
-00011c40: 2020 2020 2020 2073 6f75 7263 6520 3d20         source = 
-00011c50: 736f 7572 6365 2e72 7374 7269 7028 290a  source.rstrip().
-00011c60: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00011c70: 2c20 5f20 3d20 7265 6164 5f64 6174 6128  , _ = read_data(
-00011c80: 226d 6973 6365 6c6c 616e 656f 7573 222c  "miscellaneous",
-00011c90: 2022 6d69 7373 696e 675f 6669 6e61 6c5f   "missing_final_
-00011ca0: 6e65 776c 696e 652e 6469 6666 2229 0a20  newline.diff"). 
-00011cb0: 2020 2020 2020 2074 6d70 5f66 696c 6520         tmp_file 
-00011cc0: 3d20 5061 7468 2863 6572 6369 732e 6475  = Path(cercis.du
-00011cd0: 6d70 5f74 6f5f 6669 6c65 2873 6f75 7263  mp_to_file(sourc
-00011ce0: 652c 2065 6e73 7572 655f 6669 6e61 6c5f  e, ensure_final_
-00011cf0: 6e65 776c 696e 653d 4661 6c73 6529 290a  newline=False)).
-00011d00: 2020 2020 2020 2020 6469 6666 5f68 6561          diff_hea
-00011d10: 6465 7220 3d20 7265 2e63 6f6d 7069 6c65  der = re.compile
-00011d20: 280a 2020 2020 2020 2020 2020 2020 7266  (.            rf
-00011d30: 227b 7265 2e65 7363 6170 6528 7374 7228  "{re.escape(str(
-00011d40: 746d 705f 6669 6c65 2929 7d5c 745c 645c  tmp_file))}\t\d\
-00011d50: 645c 645c 642d 5c64 5c64 2d5c 645c 6420  d\d\d-\d\d-\d\d 
-00011d60: 220a 2020 2020 2020 2020 2020 2020 7222  ".            r"
-00011d70: 5c64 5c64 3a5c 645c 643a 5c64 5c64 5c2e  \d\d:\d\d:\d\d\.
-00011d80: 5c64 5c64 5c64 5c64 5c64 5c64 205c 2b5c  \d\d\d\d\d\d \+\
-00011d90: 645c 645c 645c 6422 0a20 2020 2020 2020  d\d\d\d".       
-00011da0: 2029 0a20 2020 2020 2020 2074 7279 3a0a   ).        try:.
-00011db0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00011dc0: 6c74 203d 2042 6c61 636b 5275 6e6e 6572  lt = BlackRunner
-00011dd0: 2829 2e69 6e76 6f6b 6528 6365 7263 6973  ().invoke(cercis
-00011de0: 2e6d 6169 6e2c 205b 222d 2d64 6966 6622  .main, ["--diff"
-00011df0: 2c20 7374 7228 746d 705f 6669 6c65 295d  , str(tmp_file)]
-00011e00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00011e10: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00011e20: 6573 756c 742e 6578 6974 5f63 6f64 652c  esult.exit_code,
-00011e30: 2030 290a 2020 2020 2020 2020 6669 6e61   0).        fina
-00011e40: 6c6c 793a 0a20 2020 2020 2020 2020 2020  lly:.           
-00011e50: 206f 732e 756e 6c69 6e6b 2874 6d70 5f66   os.unlink(tmp_f
-00011e60: 696c 6529 0a20 2020 2020 2020 2061 6374  ile).        act
-00011e70: 7561 6c20 3d20 7265 7375 6c74 2e6f 7574  ual = result.out
-00011e80: 7075 740a 2020 2020 2020 2020 6163 7475  put.        actu
-00011e90: 616c 203d 2064 6966 665f 6865 6164 6572  al = diff_header
-00011ea0: 2e73 7562 2844 4554 4552 4d49 4e49 5354  .sub(DETERMINIST
-00011eb0: 4943 5f48 4541 4445 522c 2061 6374 7561  IC_HEADER, actua
-00011ec0: 6c29 0a20 2020 2020 2020 2073 656c 662e  l).        self.
-00011ed0: 6173 7365 7274 4571 7561 6c28 6163 7475  assertEqual(actu
-00011ee0: 616c 2c20 6578 7065 6374 6564 290a 0a20  al, expected).. 
-00011ef0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00011f00: 0a20 2020 2064 6566 2063 6f6d 7061 7265  .    def compare
-00011f10: 5f72 6573 756c 7473 280a 2020 2020 2020  _results(.      
-00011f20: 2020 2020 2020 7265 7375 6c74 3a20 636c        result: cl
-00011f30: 6963 6b2e 7465 7374 696e 672e 5265 7375  ick.testing.Resu
-00011f40: 6c74 2c20 6578 7065 6374 6564 5f76 616c  lt, expected_val
-00011f50: 7565 3a20 7374 722c 2065 7870 6563 7465  ue: str, expecte
-00011f60: 645f 6578 6974 5f63 6f64 653a 2069 6e74  d_exit_code: int
-00011f70: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
-00011f80: 2020 2020 2020 2020 2222 2248 656c 7065          """Helpe
-00011f90: 7220 6d65 7468 6f64 2074 6f20 7465 7374  r method to test
-00011fa0: 2074 6865 2076 616c 7565 2061 6e64 2065   the value and e
-00011fb0: 7869 7420 636f 6465 206f 6620 6120 636c  xit code of a cl
-00011fc0: 6963 6b20 5265 7375 6c74 2e22 2222 0a20  ick Result.""". 
-00011fd0: 2020 2020 2020 2061 7373 6572 7420 280a         assert (.
-00011fe0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00011ff0: 6c74 2e6f 7574 7075 7420 3d3d 2065 7870  lt.output == exp
-00012000: 6563 7465 645f 7661 6c75 650a 2020 2020  ected_value.    
-00012010: 2020 2020 292c 2022 5468 6520 6f75 7470      ), "The outp
-00012020: 7574 2064 6964 206e 6f74 206d 6174 6368  ut did not match
-00012030: 2074 6865 2065 7870 6563 7465 6420 7661   the expected va
-00012040: 6c75 652e 220a 2020 2020 2020 2020 6173  lue.".        as
-00012050: 7365 7274 2072 6573 756c 742e 6578 6974  sert result.exit
-00012060: 5f63 6f64 6520 3d3d 2065 7870 6563 7465  _code == expecte
-00012070: 645f 6578 6974 5f63 6f64 652c 2022 5468  d_exit_code, "Th
-00012080: 6520 6578 6974 2063 6f64 6520 6973 2069  e exit code is i
-00012090: 6e63 6f72 7265 6374 2e22 0a0a 2020 2020  ncorrect."..    
-000120a0: 6465 6620 7465 7374 5f63 6f64 655f 6f70  def test_code_op
-000120b0: 7469 6f6e 2873 656c 6629 202d 3e20 4e6f  tion(self) -> No
-000120c0: 6e65 3a0a 2020 2020 2020 2020 2222 2254  ne:.        """T
-000120d0: 6573 7420 7468 6520 636f 6465 206f 7074  est the code opt
-000120e0: 696f 6e20 7769 7468 206e 6f20 6368 616e  ion with no chan
-000120f0: 6765 732e 2222 220a 2020 2020 2020 2020  ges.""".        
-00012100: 636f 6465 203d 2022 7072 696e 7428 2748  code = "print('H
-00012110: 656c 6c6f 2077 6f72 6c64 2729 5c6e 220a  ello world')\n".
-00012120: 2020 2020 2020 2020 6172 6773 203d 205b          args = [
-00012130: 222d 2d63 6f64 6522 2c20 636f 6465 2c20  "--code", code, 
-00012140: 222d 2d73 696e 676c 652d 7175 6f74 653d  "--single-quote=
-00012150: 5472 7565 225d 0a20 2020 2020 2020 2072  True"].        r
-00012160: 6573 756c 7420 3d20 436c 6952 756e 6e65  esult = CliRunne
-00012170: 7228 292e 696e 766f 6b65 2863 6572 6369  r().invoke(cerci
-00012180: 732e 6d61 696e 2c20 6172 6773 290a 0a20  s.main, args).. 
-00012190: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
-000121a0: 6172 655f 7265 7375 6c74 7328 7265 7375  are_results(resu
-000121b0: 6c74 2c20 636f 6465 2c20 3029 0a0a 2020  lt, code, 0)..  
-000121c0: 2020 6465 6620 7465 7374 5f63 6f64 655f    def test_code_
-000121d0: 6f70 7469 6f6e 5f63 6861 6e67 6564 2873  option_changed(s
-000121e0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-000121f0: 2020 2020 2020 2222 2254 6573 7420 7468        """Test th
-00012200: 6520 636f 6465 206f 7074 696f 6e20 7768  e code option wh
-00012210: 656e 2063 6861 6e67 6573 2061 7265 2072  en changes are r
-00012220: 6571 7569 7265 642e 2222 220a 2020 2020  equired.""".    
-00012230: 2020 2020 636f 6465 203d 2027 7072 696e      code = 'prin
-00012240: 7428 2268 656c 6c6f 2077 6f72 6c64 2229  t("hello world")
-00012250: 270a 2020 2020 2020 2020 666f 726d 6174  '.        format
-00012260: 7465 6420 3d20 6365 7263 6973 2e66 6f72  ted = cercis.for
-00012270: 6d61 745f 7374 7228 636f 6465 2c20 6d6f  mat_str(code, mo
-00012280: 6465 3d44 4546 4155 4c54 5f4d 4f44 4529  de=DEFAULT_MODE)
-00012290: 0a0a 2020 2020 2020 2020 6172 6773 203d  ..        args =
-000122a0: 205b 222d 2d63 6f64 6522 2c20 636f 6465   ["--code", code
-000122b0: 2c20 222d 2d73 696e 676c 652d 7175 6f74  , "--single-quot
-000122c0: 653d 5472 7565 225d 0a20 2020 2020 2020  e=True"].       
-000122d0: 2072 6573 756c 7420 3d20 436c 6952 756e   result = CliRun
-000122e0: 6e65 7228 292e 696e 766f 6b65 2863 6572  ner().invoke(cer
-000122f0: 6369 732e 6d61 696e 2c20 6172 6773 290a  cis.main, args).
-00012300: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00012310: 6d70 6172 655f 7265 7375 6c74 7328 7265  mpare_results(re
-00012320: 7375 6c74 2c20 666f 726d 6174 7465 642c  sult, formatted,
-00012330: 2030 290a 0a20 2020 2064 6566 2074 6573   0)..    def tes
-00012340: 745f 636f 6465 5f6f 7074 696f 6e5f 6368  t_code_option_ch
-00012350: 6563 6b28 7365 6c66 2920 2d3e 204e 6f6e  eck(self) -> Non
-00012360: 653a 0a20 2020 2020 2020 2022 2222 5465  e:.        """Te
-00012370: 7374 2074 6865 2063 6f64 6520 6f70 7469  st the code opti
-00012380: 6f6e 2077 6865 6e20 6368 6563 6b20 6973  on when check is
-00012390: 2070 6173 7365 642e 2222 220a 2020 2020   passed.""".    
-000123a0: 2020 2020 6172 6773 203d 205b 222d 2d63      args = ["--c
-000123b0: 6865 636b 222c 2022 2d2d 636f 6465 222c  heck", "--code",
-000123c0: 2027 7072 696e 7428 2248 656c 6c6f 2077   'print("Hello w
-000123d0: 6f72 6c64 2229 5c6e 275d 0a20 2020 2020  orld")\n'].     
-000123e0: 2020 2072 6573 756c 7420 3d20 436c 6952     result = CliR
-000123f0: 756e 6e65 7228 292e 696e 766f 6b65 2863  unner().invoke(c
-00012400: 6572 6369 732e 6d61 696e 2c20 6172 6773  ercis.main, args
-00012410: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00012420: 6f6d 7061 7265 5f72 6573 756c 7473 2872  ompare_results(r
-00012430: 6573 756c 742c 2022 222c 2030 290a 0a20  esult, "", 0).. 
-00012440: 2020 2064 6566 2074 6573 745f 636f 6465     def test_code
-00012450: 5f6f 7074 696f 6e5f 6368 6563 6b5f 6368  _option_check_ch
-00012460: 616e 6765 6428 7365 6c66 2920 2d3e 204e  anged(self) -> N
-00012470: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00012480: 5465 7374 2074 6865 2063 6f64 6520 6f70  Test the code op
-00012490: 7469 6f6e 2077 6865 6e20 6368 616e 6765  tion when change
-000124a0: 7320 6172 6520 7265 7175 6972 6564 2c20  s are required, 
-000124b0: 616e 6420 6368 6563 6b20 6973 2070 6173  and check is pas
-000124c0: 7365 642e 2222 220a 2020 2020 2020 2020  sed.""".        
-000124d0: 6172 6773 203d 205b 222d 2d63 6865 636b  args = ["--check
-000124e0: 222c 2022 2d2d 636f 6465 222c 2022 7072  ", "--code", "pr
-000124f0: 696e 7428 2768 656c 6c6f 2077 6f72 6c64  int('hello world
-00012500: 2729 225d 0a20 2020 2020 2020 2072 6573  ')"].        res
-00012510: 756c 7420 3d20 436c 6952 756e 6e65 7228  ult = CliRunner(
-00012520: 292e 696e 766f 6b65 2863 6572 6369 732e  ).invoke(cercis.
-00012530: 6d61 696e 2c20 6172 6773 290a 2020 2020  main, args).    
-00012540: 2020 2020 7365 6c66 2e63 6f6d 7061 7265      self.compare
-00012550: 5f72 6573 756c 7473 2872 6573 756c 742c  _results(result,
-00012560: 2022 222c 2031 290a 0a20 2020 2064 6566   "", 1)..    def
-00012570: 2074 6573 745f 636f 6465 5f6f 7074 696f   test_code_optio
-00012580: 6e5f 6469 6666 2873 656c 6629 202d 3e20  n_diff(self) -> 
-00012590: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000125a0: 2254 6573 7420 7468 6520 636f 6465 206f  "Test the code o
-000125b0: 7074 696f 6e20 7768 656e 2064 6966 6620  ption when diff 
-000125c0: 6973 2070 6173 7365 642e 2222 220a 2020  is passed.""".  
-000125d0: 2020 2020 2020 636f 6465 203d 2027 7072        code = 'pr
-000125e0: 696e 7428 2268 656c 6c6f 2077 6f72 6c64  int("hello world
-000125f0: 2229 270a 2020 2020 2020 2020 666f 726d  ")'.        form
-00012600: 6174 7465 6420 3d20 6365 7263 6973 2e66  atted = cercis.f
-00012610: 6f72 6d61 745f 7374 7228 636f 6465 2c20  ormat_str(code, 
-00012620: 6d6f 6465 3d44 4546 4155 4c54 5f4d 4f44  mode=DEFAULT_MOD
-00012630: 4529 0a20 2020 2020 2020 2072 6573 756c  E).        resul
-00012640: 745f 6469 6666 203d 2064 6966 6628 636f  t_diff = diff(co
-00012650: 6465 2c20 666f 726d 6174 7465 642c 2022  de, formatted, "
-00012660: 5354 4449 4e22 2c20 2253 5444 4f55 5422  STDIN", "STDOUT"
-00012670: 290a 0a20 2020 2020 2020 2061 7267 7320  )..        args 
-00012680: 3d20 5b22 2d2d 6469 6666 222c 2022 2d2d  = ["--diff", "--
-00012690: 636f 6465 222c 2063 6f64 652c 2022 2d2d  code", code, "--
-000126a0: 7369 6e67 6c65 2d71 756f 7465 3d54 7275  single-quote=Tru
-000126b0: 6522 5d0a 2020 2020 2020 2020 7265 7375  e"].        resu
-000126c0: 6c74 203d 2043 6c69 5275 6e6e 6572 2829  lt = CliRunner()
-000126d0: 2e69 6e76 6f6b 6528 6365 7263 6973 2e6d  .invoke(cercis.m
-000126e0: 6169 6e2c 2061 7267 7329 0a0a 2020 2020  ain, args)..    
-000126f0: 2020 2020 2320 5265 6d6f 7665 2074 696d      # Remove tim
-00012700: 6520 6672 6f6d 2064 6966 660a 2020 2020  e from diff.    
-00012710: 2020 2020 6f75 7470 7574 203d 2044 4946      output = DIF
-00012720: 465f 5449 4d45 2e73 7562 2822 222c 2072  F_TIME.sub("", r
-00012730: 6573 756c 742e 6f75 7470 7574 290a 0a20  esult.output).. 
-00012740: 2020 2020 2020 2061 7373 6572 7420 6f75         assert ou
-00012750: 7470 7574 203d 3d20 7265 7375 6c74 5f64  tput == result_d
-00012760: 6966 662c 2022 5468 6520 6f75 7470 7574  iff, "The output
-00012770: 2064 6964 206e 6f74 206d 6174 6368 2074   did not match t
-00012780: 6865 2065 7870 6563 7465 6420 7661 6c75  he expected valu
-00012790: 652e 220a 2020 2020 2020 2020 6173 7365  e.".        asse
-000127a0: 7274 2072 6573 756c 742e 6578 6974 5f63  rt result.exit_c
-000127b0: 6f64 6520 3d3d 2030 2c20 2254 6865 2065  ode == 0, "The e
-000127c0: 7869 7420 636f 6465 2069 7320 696e 636f  xit code is inco
-000127d0: 7272 6563 742e 220a 0a20 2020 2064 6566  rrect."..    def
-000127e0: 2074 6573 745f 636f 6465 5f6f 7074 696f   test_code_optio
-000127f0: 6e5f 636f 6c6f 725f 6469 6666 2873 656c  n_color_diff(sel
-00012800: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00012810: 2020 2020 2222 2254 6573 7420 7468 6520      """Test the 
-00012820: 636f 6465 206f 7074 696f 6e20 7768 656e  code option when
-00012830: 2063 6f6c 6f72 2061 6e64 2064 6966 6620   color and diff 
-00012840: 6172 6520 7061 7373 6564 2e22 2222 0a20  are passed.""". 
-00012850: 2020 2020 2020 2063 6f64 6520 3d20 2770         code = 'p
-00012860: 7269 6e74 2822 6865 6c6c 6f20 776f 726c  rint("hello worl
-00012870: 6422 2927 0a20 2020 2020 2020 2066 6f72  d")'.        for
-00012880: 6d61 7474 6564 203d 2063 6572 6369 732e  matted = cercis.
-00012890: 666f 726d 6174 5f73 7472 2863 6f64 652c  format_str(code,
-000128a0: 206d 6f64 653d 4445 4641 554c 545f 4d4f   mode=DEFAULT_MO
-000128b0: 4445 290a 0a20 2020 2020 2020 2072 6573  DE)..        res
-000128c0: 756c 745f 6469 6666 203d 2064 6966 6628  ult_diff = diff(
-000128d0: 636f 6465 2c20 666f 726d 6174 7465 642c  code, formatted,
-000128e0: 2022 5354 4449 4e22 2c20 2253 5444 4f55   "STDIN", "STDOU
-000128f0: 5422 290a 2020 2020 2020 2020 7265 7375  T").        resu
-00012900: 6c74 5f64 6966 6620 3d20 636f 6c6f 725f  lt_diff = color_
-00012910: 6469 6666 2872 6573 756c 745f 6469 6666  diff(result_diff
-00012920: 290a 0a20 2020 2020 2020 2061 7267 7320  )..        args 
-00012930: 3d20 5b22 2d2d 6469 6666 222c 2022 2d2d  = ["--diff", "--
-00012940: 636f 6c6f 7222 2c20 222d 2d63 6f64 6522  color", "--code"
-00012950: 2c20 636f 6465 2c20 222d 2d73 696e 676c  , code, "--singl
-00012960: 652d 7175 6f74 653d 5472 7565 225d 0a20  e-quote=True"]. 
-00012970: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00012980: 436c 6952 756e 6e65 7228 292e 696e 766f  CliRunner().invo
-00012990: 6b65 2863 6572 6369 732e 6d61 696e 2c20  ke(cercis.main, 
-000129a0: 6172 6773 290a 0a20 2020 2020 2020 2023  args)..        #
-000129b0: 2052 656d 6f76 6520 7469 6d65 2066 726f   Remove time fro
-000129c0: 6d20 6469 6666 0a20 2020 2020 2020 206f  m diff.        o
-000129d0: 7574 7075 7420 3d20 4449 4646 5f54 494d  utput = DIFF_TIM
-000129e0: 452e 7375 6228 2222 2c20 7265 7375 6c74  E.sub("", result
-000129f0: 2e6f 7574 7075 7429 0a0a 2020 2020 2020  .output)..      
-00012a00: 2020 6173 7365 7274 206f 7574 7075 7420    assert output 
-00012a10: 3d3d 2072 6573 756c 745f 6469 6666 2c20  == result_diff, 
-00012a20: 2254 6865 206f 7574 7075 7420 6469 6420  "The output did 
-00012a30: 6e6f 7420 6d61 7463 6820 7468 6520 6578  not match the ex
-00012a40: 7065 6374 6564 2076 616c 7565 2e22 0a20  pected value.". 
-00012a50: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
-00012a60: 7375 6c74 2e65 7869 745f 636f 6465 203d  sult.exit_code =
-00012a70: 3d20 302c 2022 5468 6520 6578 6974 2063  = 0, "The exit c
-00012a80: 6f64 6520 6973 2069 6e63 6f72 7265 6374  ode is incorrect
-00012a90: 2e22 0a0a 2020 2020 4070 7974 6573 742e  ."..    @pytest.
-00012aa0: 6d61 726b 2e69 6e63 6f6d 7061 7469 626c  mark.incompatibl
-00012ab0: 655f 7769 7468 5f6d 7970 7963 0a20 2020  e_with_mypyc.   
-00012ac0: 2064 6566 2074 6573 745f 636f 6465 5f6f   def test_code_o
-00012ad0: 7074 696f 6e5f 7361 6665 2873 656c 6629  ption_safe(self)
-00012ae0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00012af0: 2020 2222 2254 6573 7420 7468 6174 2074    """Test that t
-00012b00: 6865 2063 6f64 6520 6f70 7469 6f6e 2074  he code option t
-00012b10: 6872 6f77 7320 616e 2065 7272 6f72 2077  hrows an error w
-00012b20: 6865 6e20 7468 6520 7361 6e69 7479 2063  hen the sanity c
-00012b30: 6865 636b 7320 6661 696c 2e22 2222 0a20  hecks fail.""". 
-00012b40: 2020 2020 2020 2023 2050 6174 6368 2063         # Patch c
-00012b50: 6572 6369 732e 6173 7365 7274 5f65 7175  ercis.assert_equ
-00012b60: 6976 616c 656e 7420 746f 2065 6e73 7572  ivalent to ensur
-00012b70: 6520 7468 6520 7361 6e69 7479 2063 6865  e the sanity che
-00012b80: 636b 7320 6661 696c 0a20 2020 2020 2020  cks fail.       
-00012b90: 2077 6974 6820 7061 7463 682e 6f62 6a65   with patch.obje
-00012ba0: 6374 2863 6572 6369 732c 2022 6173 7365  ct(cercis, "asse
-00012bb0: 7274 5f65 7175 6976 616c 656e 7422 2c20  rt_equivalent", 
-00012bc0: 7369 6465 5f65 6666 6563 743d 4173 7365  side_effect=Asse
-00012bd0: 7274 696f 6e45 7272 6f72 293a 0a20 2020  rtionError):.   
-00012be0: 2020 2020 2020 2020 2063 6f64 6520 3d20           code = 
-00012bf0: 2770 7269 6e74 2822 4865 6c6c 6f20 776f  'print("Hello wo
-00012c00: 726c 6422 2927 0a20 2020 2020 2020 2020  rld")'.         
-00012c10: 2020 2065 7272 6f72 5f6d 7367 203d 2066     error_msg = f
-00012c20: 227b 636f 6465 7d5c 6e65 7272 6f72 3a20  "{code}\nerror: 
-00012c30: 6361 6e6e 6f74 2066 6f72 6d61 7420 3c73  cannot format <s
-00012c40: 7472 696e 673e 3a20 5c6e 220a 0a20 2020  tring>: \n"..   
-00012c50: 2020 2020 2020 2020 2061 7267 7320 3d20           args = 
-00012c60: 5b22 2d2d 7361 6665 222c 2022 2d2d 636f  ["--safe", "--co
-00012c70: 6465 222c 2063 6f64 655d 0a20 2020 2020  de", code].     
-00012c80: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00012c90: 436c 6952 756e 6e65 7228 292e 696e 766f  CliRunner().invo
-00012ca0: 6b65 2863 6572 6369 732e 6d61 696e 2c20  ke(cercis.main, 
-00012cb0: 6172 6773 290a 0a20 2020 2020 2020 2020  args)..         
-00012cc0: 2020 2073 656c 662e 636f 6d70 6172 655f     self.compare_
-00012cd0: 7265 7375 6c74 7328 7265 7375 6c74 2c20  results(result, 
-00012ce0: 6572 726f 725f 6d73 672c 2031 3233 290a  error_msg, 123).
-00012cf0: 0a20 2020 2064 6566 2074 6573 745f 636f  .    def test_co
-00012d00: 6465 5f6f 7074 696f 6e5f 6661 7374 2873  de_option_fast(s
-00012d10: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00012d20: 2020 2020 2020 2222 2254 6573 7420 7468        """Test th
-00012d30: 6174 2074 6865 2063 6f64 6520 6f70 7469  at the code opti
-00012d40: 6f6e 2069 676e 6f72 6573 2065 7272 6f72  on ignores error
-00012d50: 7320 7768 656e 2074 6865 2073 616e 6974  s when the sanit
-00012d60: 7920 6368 6563 6b73 2066 6169 6c2e 2222  y checks fail.""
-00012d70: 220a 2020 2020 2020 2020 2320 5061 7463  ".        # Patc
-00012d80: 6820 6365 7263 6973 2e61 7373 6572 745f  h cercis.assert_
-00012d90: 6571 7569 7661 6c65 6e74 2074 6f20 656e  equivalent to en
-00012da0: 7375 7265 2074 6865 2073 616e 6974 7920  sure the sanity 
-00012db0: 6368 6563 6b73 2066 6169 6c0a 2020 2020  checks fail.    
-00012dc0: 2020 2020 7769 7468 2070 6174 6368 2e6f      with patch.o
-00012dd0: 626a 6563 7428 6365 7263 6973 2c20 2261  bject(cercis, "a
-00012de0: 7373 6572 745f 6571 7569 7661 6c65 6e74  ssert_equivalent
-00012df0: 222c 2073 6964 655f 6566 6665 6374 3d41  ", side_effect=A
-00012e00: 7373 6572 7469 6f6e 4572 726f 7229 3a0a  ssertionError):.
-00012e10: 2020 2020 2020 2020 2020 2020 636f 6465              code
-00012e20: 203d 2022 7072 696e 7428 2748 656c 6c6f   = "print('Hello
-00012e30: 2077 6f72 6c64 2729 220a 2020 2020 2020   world')".      
-00012e40: 2020 2020 2020 666f 726d 6174 7465 6420        formatted 
-00012e50: 3d20 6365 7263 6973 2e66 6f72 6d61 745f  = cercis.format_
-00012e60: 7374 7228 636f 6465 2c20 6d6f 6465 3d44  str(code, mode=D
-00012e70: 4546 4155 4c54 5f4d 4f44 4529 0a0a 2020  EFAULT_MODE)..  
-00012e80: 2020 2020 2020 2020 2020 6172 6773 203d            args =
-00012e90: 205b 222d 2d66 6173 7422 2c20 222d 2d63   ["--fast", "--c
-00012ea0: 6f64 6522 2c20 636f 6465 2c20 222d 2d73  ode", code, "--s
-00012eb0: 696e 676c 652d 7175 6f74 653d 5472 7565  ingle-quote=True
-00012ec0: 225d 0a20 2020 2020 2020 2020 2020 2072  "].            r
-00012ed0: 6573 756c 7420 3d20 436c 6952 756e 6e65  esult = CliRunne
-00012ee0: 7228 292e 696e 766f 6b65 2863 6572 6369  r().invoke(cerci
-00012ef0: 732e 6d61 696e 2c20 6172 6773 290a 0a20  s.main, args).. 
-00012f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012f10: 636f 6d70 6172 655f 7265 7375 6c74 7328  compare_results(
-00012f20: 7265 7375 6c74 2c20 666f 726d 6174 7465  result, formatte
-00012f30: 642c 2030 290a 0a20 2020 2040 7079 7465  d, 0)..    @pyte
-00012f40: 7374 2e6d 6172 6b2e 696e 636f 6d70 6174  st.mark.incompat
-00012f50: 6962 6c65 5f77 6974 685f 6d79 7079 630a  ible_with_mypyc.
-00012f60: 2020 2020 6465 6620 7465 7374 5f63 6f64      def test_cod
-00012f70: 655f 6f70 7469 6f6e 5f63 6f6e 6669 6728  e_option_config(
-00012f80: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00012f90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012fa0: 2020 2054 6573 7420 7468 6174 2074 6865     Test that the
-00012fb0: 2063 6f64 6520 6f70 7469 6f6e 2066 696e   code option fin
-00012fc0: 6473 2074 6865 2070 7970 726f 6a65 6374  ds the pyproject
-00012fd0: 2e74 6f6d 6c20 696e 2074 6865 2063 7572  .toml in the cur
-00012fe0: 7265 6e74 2064 6972 6563 746f 7279 2e0a  rent directory..
-00012ff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013000: 2020 2020 7769 7468 2070 6174 6368 2e6f      with patch.o
-00013010: 626a 6563 7428 6365 7263 6973 2c20 2270  bject(cercis, "p
-00013020: 6172 7365 5f70 7970 726f 6a65 6374 5f74  arse_pyproject_t
-00013030: 6f6d 6c22 2c20 7265 7475 726e 5f76 616c  oml", return_val
-00013040: 7565 3d7b 7d29 2061 7320 7061 7273 653a  ue={}) as parse:
-00013050: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-00013060: 7320 3d20 5b22 2d2d 636f 6465 222c 2022  s = ["--code", "
-00013070: 7072 696e 7422 5d0a 2020 2020 2020 2020  print"].        
-00013080: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
-00013090: 6520 6f6e 6c79 2064 6972 6563 746f 7279  e only directory
-000130a0: 206b 6e6f 776e 2074 6f20 636f 6e74 6169   known to contai
-000130b0: 6e20 6120 7079 7072 6f6a 6563 742e 746f  n a pyproject.to
-000130c0: 6d6c 0a20 2020 2020 2020 2020 2020 2077  ml.            w
-000130d0: 6974 6820 6368 616e 6765 5f64 6972 6563  ith change_direc
-000130e0: 746f 7279 2850 524f 4a45 4354 5f52 4f4f  tory(PROJECT_ROO
-000130f0: 5429 3a0a 2020 2020 2020 2020 2020 2020  T):.            
-00013100: 2020 2020 436c 6952 756e 6e65 7228 292e      CliRunner().
-00013110: 696e 766f 6b65 2863 6572 6369 732e 6d61  invoke(cercis.ma
-00013120: 696e 2c20 6172 6773 290a 2020 2020 2020  in, args).      
-00013130: 2020 2020 2020 2020 2020 7079 7072 6f6a            pyproj
-00013140: 6563 745f 7061 7468 203d 2050 6174 6828  ect_path = Path(
-00013150: 5061 7468 2e63 7764 2829 2c20 2270 7970  Path.cwd(), "pyp
-00013160: 726f 6a65 6374 2e74 6f6d 6c22 292e 7265  roject.toml").re
-00013170: 736f 6c76 6528 290a 0a20 2020 2020 2020  solve()..       
-00013180: 2020 2020 2061 7373 6572 7420 280a 2020       assert (.  
-00013190: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-000131a0: 6e28 7061 7273 652e 6d6f 636b 5f63 616c  n(parse.mock_cal
-000131b0: 6c73 2920 3e3d 2031 0a20 2020 2020 2020  ls) >= 1.       
-000131c0: 2020 2020 2029 2c20 2245 7870 6563 7465       ), "Expecte
-000131d0: 6420 636f 6e66 6967 2070 6172 7365 2074  d config parse t
-000131e0: 6f20 6265 2063 616c 6c65 6420 7769 7468  o be called with
-000131f0: 2074 6865 2063 7572 7265 6e74 2064 6972   the current dir
-00013200: 6563 746f 7279 2e22 0a0a 2020 2020 2020  ectory."..      
-00013210: 2020 2020 2020 5f2c 2063 616c 6c5f 6172        _, call_ar
-00013220: 6773 2c20 5f20 3d20 7061 7273 652e 6d6f  gs, _ = parse.mo
-00013230: 636b 5f63 616c 6c73 5b30 5d0a 2020 2020  ck_calls[0].    
-00013240: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
-00013250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013260: 2063 616c 6c5f 6172 6773 5b30 5d2e 6c6f   call_args[0].lo
-00013270: 7765 7228 2920 3d3d 2073 7472 2870 7970  wer() == str(pyp
-00013280: 726f 6a65 6374 5f70 6174 6829 2e6c 6f77  roject_path).low
-00013290: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-000132a0: 2029 2c20 2249 6e63 6f72 7265 6374 2063   ), "Incorrect c
-000132b0: 6f6e 6669 6720 6c6f 6164 6564 2e22 0a0a  onfig loaded."..
-000132c0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-000132d0: 2e69 6e63 6f6d 7061 7469 626c 655f 7769  .incompatible_wi
-000132e0: 7468 5f6d 7970 7963 0a20 2020 2064 6566  th_mypyc.    def
-000132f0: 2074 6573 745f 636f 6465 5f6f 7074 696f   test_code_optio
-00013300: 6e5f 7061 7265 6e74 5f63 6f6e 6669 6728  n_parent_config(
-00013310: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00013320: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013330: 2020 2054 6573 7420 7468 6174 2074 6865     Test that the
-00013340: 2063 6f64 6520 6f70 7469 6f6e 2066 696e   code option fin
-00013350: 6473 2074 6865 2070 7970 726f 6a65 6374  ds the pyproject
-00013360: 2e74 6f6d 6c20 696e 2074 6865 2070 6172  .toml in the par
-00013370: 656e 7420 6469 7265 6374 6f72 792e 0a20  ent directory.. 
-00013380: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013390: 2020 2077 6974 6820 7061 7463 682e 6f62     with patch.ob
-000133a0: 6a65 6374 2863 6572 6369 732c 2022 7061  ject(cercis, "pa
-000133b0: 7273 655f 7079 7072 6f6a 6563 745f 746f  rse_pyproject_to
-000133c0: 6d6c 222c 2072 6574 7572 6e5f 7661 6c75  ml", return_valu
-000133d0: 653d 7b7d 2920 6173 2070 6172 7365 3a0a  e={}) as parse:.
-000133e0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-000133f0: 2063 6861 6e67 655f 6469 7265 6374 6f72   change_director
-00013400: 7928 5448 4953 5f44 4952 293a 0a20 2020  y(THIS_DIR):.   
-00013410: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00013420: 7320 3d20 5b22 2d2d 636f 6465 222c 2022  s = ["--code", "
-00013430: 7072 696e 7422 5d0a 2020 2020 2020 2020  print"].        
-00013440: 2020 2020 2020 2020 436c 6952 756e 6e65          CliRunne
-00013450: 7228 292e 696e 766f 6b65 2863 6572 6369  r().invoke(cerci
-00013460: 732e 6d61 696e 2c20 6172 6773 290a 0a20  s.main, args).. 
-00013470: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00013480: 7970 726f 6a65 6374 5f70 6174 6820 3d20  yproject_path = 
-00013490: 5061 7468 2850 6174 6828 292e 6377 6428  Path(Path().cwd(
-000134a0: 292e 7061 7265 6e74 2c20 2270 7970 726f  ).parent, "pypro
-000134b0: 6a65 6374 2e74 6f6d 6c22 292e 7265 736f  ject.toml").reso
-000134c0: 6c76 6528 290a 2020 2020 2020 2020 2020  lve().          
-000134d0: 2020 2020 2020 6173 7365 7274 2028 0a20        assert (. 
-000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134f0: 2020 206c 656e 2870 6172 7365 2e6d 6f63     len(parse.moc
-00013500: 6b5f 6361 6c6c 7329 203e 3d20 310a 2020  k_calls) >= 1.  
-00013510: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-00013520: 2022 4578 7065 6374 6564 2063 6f6e 6669   "Expected confi
-00013530: 6720 7061 7273 6520 746f 2062 6520 6361  g parse to be ca
-00013540: 6c6c 6564 2077 6974 6820 7468 6520 6375  lled with the cu
-00013550: 7272 656e 7420 6469 7265 6374 6f72 792e  rrent directory.
-00013560: 220a 0a20 2020 2020 2020 2020 2020 2020  "..             
-00013570: 2020 205f 2c20 6361 6c6c 5f61 7267 732c     _, call_args,
-00013580: 205f 203d 2070 6172 7365 2e6d 6f63 6b5f   _ = parse.mock_
-00013590: 6361 6c6c 735b 305d 0a20 2020 2020 2020  calls[0].       
-000135a0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000135b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000135c0: 2020 2020 2020 6361 6c6c 5f61 7267 735b        call_args[
-000135d0: 305d 2e6c 6f77 6572 2829 203d 3d20 7374  0].lower() == st
-000135e0: 7228 7079 7072 6f6a 6563 745f 7061 7468  r(pyproject_path
-000135f0: 292e 6c6f 7765 7228 290a 2020 2020 2020  ).lower().      
-00013600: 2020 2020 2020 2020 2020 292c 2022 496e            ), "In
-00013610: 636f 7272 6563 7420 636f 6e66 6967 206c  correct config l
-00013620: 6f61 6465 642e 220a 0a20 2020 2064 6566  oaded."..    def
-00013630: 2074 6573 745f 666f 725f 6861 6e64 6c65   test_for_handle
-00013640: 645f 756e 6578 7065 6374 6564 5f65 6f66  d_unexpected_eof
-00013650: 5f65 7272 6f72 2873 656c 6629 202d 3e20  _error(self) -> 
-00013660: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00013670: 220a 2020 2020 2020 2020 5465 7374 2074  ".        Test t
-00013680: 6861 7420 616e 2075 6e65 7870 6563 7465  hat an unexpecte
-00013690: 6420 454f 4620 5379 6e74 6178 4572 726f  d EOF SyntaxErro
-000136a0: 7220 6973 206e 6963 656c 7920 7072 6573  r is nicely pres
-000136b0: 656e 7465 642e 0a20 2020 2020 2020 2022  ented..        "
-000136c0: 2222 0a20 2020 2020 2020 2077 6974 6820  "".        with 
-000136d0: 7079 7465 7374 2e72 6169 7365 7328 6365  pytest.raises(ce
-000136e0: 7263 6973 2e70 6172 7369 6e67 2e49 6e76  rcis.parsing.Inv
-000136f0: 616c 6964 496e 7075 7429 2061 7320 6578  alidInput) as ex
-00013700: 635f 696e 666f 3a0a 2020 2020 2020 2020  c_info:.        
-00013710: 2020 2020 6365 7263 6973 2e6c 6962 3274      cercis.lib2t
-00013720: 6f33 5f70 6172 7365 2822 7072 696e 7428  o3_parse("print(
-00013730: 222c 207b 7d29 0a0a 2020 2020 2020 2020  ", {})..        
-00013740: 6578 635f 696e 666f 2e6d 6174 6368 2822  exc_info.match("
-00013750: 4361 6e6e 6f74 2070 6172 7365 3a20 323a  Cannot parse: 2:
-00013760: 303a 2045 4f46 2069 6e20 6d75 6c74 692d  0: EOF in multi-
-00013770: 6c69 6e65 2073 7461 7465 6d65 6e74 2229  line statement")
-00013780: 0a0a 2020 2020 6465 6620 7465 7374 5f65  ..    def test_e
-00013790: 7175 6976 616c 656e 6379 5f61 7374 5f70  quivalency_ast_p
-000137a0: 6172 7365 5f66 6169 6c75 7265 5f69 6e63  arse_failure_inc
-000137b0: 6c75 6465 735f 6572 726f 7228 7365 6c66  ludes_error(self
-000137c0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000137d0: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-000137e0: 6169 7365 7328 4173 7365 7274 696f 6e45  aises(AssertionE
-000137f0: 7272 6f72 2920 6173 2065 7272 3a0a 2020  rror) as err:.  
-00013800: 2020 2020 2020 2020 2020 6365 7263 6973            cercis
-00013810: 2e61 7373 6572 745f 6571 7569 7661 6c65  .assert_equivale
-00013820: 6e74 2822 61c2 abc2 bb61 2020 3d20 3122  nt("a....a  = 1"
-00013830: 2c20 2261 c2ab c2bb 6120 203d 2031 2229  , "a....a  = 1")
-00013840: 0a0a 2020 2020 2020 2020 6572 722e 6d61  ..        err.ma
-00013850: 7463 6828 222d 2d73 6166 6522 290a 2020  tch("--safe").  
-00013860: 2020 2020 2020 2320 556e 666f 7274 756e        # Unfortun
-00013870: 6174 656c 7920 7468 6520 5379 6e74 6178  ately the Syntax
-00013880: 4572 726f 7220 6d65 7373 6167 6520 6861  Error message ha
-00013890: 7320 6368 616e 6765 6420 696e 206e 6577  s changed in new
-000138a0: 6572 2076 6572 7369 6f6e 7320 736f 2077  er versions so w
-000138b0: 650a 2020 2020 2020 2020 2320 6361 6e27  e.        # can'
-000138c0: 7420 6d61 7463 6820 6974 2064 6972 6563  t match it direc
-000138d0: 746c 792e 0a20 2020 2020 2020 2065 7272  tly..        err
-000138e0: 2e6d 6174 6368 2822 696e 7661 6c69 6420  .match("invalid 
-000138f0: 6368 6172 6163 7465 7222 290a 2020 2020  character").    
-00013900: 2020 2020 6572 722e 6d61 7463 6828 7222      err.match(r"
-00013910: 5c28 3c75 6e6b 6e6f 776e 3e2c 206c 696e  \(<unknown>, lin
-00013920: 6520 315c 2922 290a 0a0a 636c 6173 7320  e 1\)")...class 
-00013930: 5465 7374 4361 6368 696e 673a 0a20 2020  TestCaching:.   
-00013940: 2064 6566 2074 6573 745f 6765 745f 6361   def test_get_ca
-00013950: 6368 655f 6469 7228 0a20 2020 2020 2020  che_dir(.       
-00013960: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00013970: 2020 2020 2020 2074 6d70 5f70 6174 683a         tmp_path:
-00013980: 2050 6174 682c 0a20 2020 2020 2020 2020   Path,.         
-00013990: 2020 206d 6f6e 6b65 7970 6174 6368 3a20     monkeypatch: 
-000139a0: 7079 7465 7374 2e4d 6f6e 6b65 7950 6174  pytest.MonkeyPat
-000139b0: 6368 2c0a 2020 2020 2920 2d3e 204e 6f6e  ch,.    ) -> Non
-000139c0: 653a 0a20 2020 2020 2020 2023 2043 7265  e:.        # Cre
-000139d0: 6174 6520 6d75 6c74 6970 6c65 2063 6163  ate multiple cac
-000139e0: 6865 2064 6972 6563 746f 7269 6573 0a20  he directories. 
-000139f0: 2020 2020 2020 2077 6f72 6b73 7061 6365         workspace
-00013a00: 3120 3d20 746d 705f 7061 7468 202f 2022  1 = tmp_path / "
-00013a10: 7773 3122 0a20 2020 2020 2020 2077 6f72  ws1".        wor
-00013a20: 6b73 7061 6365 312e 6d6b 6469 7228 290a  kspace1.mkdir().
-00013a30: 2020 2020 2020 2020 776f 726b 7370 6163          workspac
-00013a40: 6532 203d 2074 6d70 5f70 6174 6820 2f20  e2 = tmp_path / 
-00013a50: 2277 7332 220a 2020 2020 2020 2020 776f  "ws2".        wo
-00013a60: 726b 7370 6163 6532 2e6d 6b64 6972 2829  rkspace2.mkdir()
-00013a70: 0a0a 2020 2020 2020 2020 2320 466f 7263  ..        # Forc
-00013a80: 6520 7573 6572 5f63 6163 6865 5f64 6972  e user_cache_dir
-00013a90: 2074 6f20 7573 6520 7468 6520 7465 6d70   to use the temp
-00013aa0: 6f72 6172 7920 6469 7265 6374 6f72 7920  orary directory 
-00013ab0: 666f 7220 6561 7369 6572 2061 7373 6572  for easier asser
-00013ac0: 7469 6f6e 730a 2020 2020 2020 2020 7061  tions.        pa
-00013ad0: 7463 685f 7573 6572 5f63 6163 6865 5f64  tch_user_cache_d
-00013ae0: 6972 203d 2070 6174 6368 280a 2020 2020  ir = patch(.    
-00013af0: 2020 2020 2020 2020 7461 7267 6574 3d22          target="
-00013b00: 6365 7263 6973 2e63 6163 6865 2e75 7365  cercis.cache.use
-00013b10: 725f 6361 6368 655f 6469 7222 2c0a 2020  r_cache_dir",.  
-00013b20: 2020 2020 2020 2020 2020 6175 746f 7370            autosp
-00013b30: 6563 3d54 7275 652c 0a20 2020 2020 2020  ec=True,.       
-00013b40: 2020 2020 2072 6574 7572 6e5f 7661 6c75       return_valu
-00013b50: 653d 7374 7228 776f 726b 7370 6163 6531  e=str(workspace1
-00013b60: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
-00013b70: 2020 2020 2020 2320 4966 2042 4c41 434b        # If BLACK
-00013b80: 5f43 4143 4845 5f44 4952 2069 7320 6e6f  _CACHE_DIR is no
-00013b90: 7420 7365 742c 2075 7365 2075 7365 725f  t set, use user_
-00013ba0: 6361 6368 655f 6469 720a 2020 2020 2020  cache_dir.      
-00013bb0: 2020 6d6f 6e6b 6579 7061 7463 682e 6465    monkeypatch.de
-00013bc0: 6c65 6e76 2822 424c 4143 4b5f 4341 4348  lenv("BLACK_CACH
-00013bd0: 455f 4449 5222 2c20 7261 6973 696e 673d  E_DIR", raising=
-00013be0: 4661 6c73 6529 0a20 2020 2020 2020 2077  False).        w
-00013bf0: 6974 6820 7061 7463 685f 7573 6572 5f63  ith patch_user_c
-00013c00: 6163 6865 5f64 6972 3a0a 2020 2020 2020  ache_dir:.      
-00013c10: 2020 2020 2020 6173 7365 7274 2067 6574        assert get
-00013c20: 5f63 6163 6865 5f64 6972 2829 203d 3d20  _cache_dir() == 
-00013c30: 776f 726b 7370 6163 6531 0a0a 2020 2020  workspace1..    
-00013c40: 2020 2020 2320 4966 2069 7420 6973 2073      # If it is s
-00013c50: 6574 2c20 7573 6520 7468 6520 7061 7468  et, use the path
-00013c60: 2070 726f 7669 6465 6420 696e 2074 6865   provided in the
-00013c70: 2065 6e76 2076 6172 2e0a 2020 2020 2020   env var..      
-00013c80: 2020 6d6f 6e6b 6579 7061 7463 682e 7365    monkeypatch.se
-00013c90: 7465 6e76 2822 424c 4143 4b5f 4341 4348  tenv("BLACK_CACH
-00013ca0: 455f 4449 5222 2c20 7374 7228 776f 726b  E_DIR", str(work
-00013cb0: 7370 6163 6532 2929 0a20 2020 2020 2020  space2)).       
-00013cc0: 2061 7373 6572 7420 6765 745f 6361 6368   assert get_cach
-00013cd0: 655f 6469 7228 2920 3d3d 2077 6f72 6b73  e_dir() == works
-00013ce0: 7061 6365 320a 0a20 2020 2064 6566 2074  pace2..    def t
-00013cf0: 6573 745f 6361 6368 655f 6272 6f6b 656e  est_cache_broken
-00013d00: 5f66 696c 6528 7365 6c66 2920 2d3e 204e  _file(self) -> N
-00013d10: 6f6e 653a 0a20 2020 2020 2020 206d 6f64  one:.        mod
-00013d20: 6520 3d20 4445 4641 554c 545f 4d4f 4445  e = DEFAULT_MODE
-00013d30: 0a20 2020 2020 2020 2077 6974 6820 6361  .        with ca
-00013d40: 6368 655f 6469 7228 2920 6173 2077 6f72  che_dir() as wor
-00013d50: 6b73 7061 6365 3a0a 2020 2020 2020 2020  kspace:.        
-00013d60: 2020 2020 6361 6368 655f 6669 6c65 203d      cache_file =
-00013d70: 2067 6574 5f63 6163 6865 5f66 696c 6528   get_cache_file(
-00013d80: 6d6f 6465 290a 2020 2020 2020 2020 2020  mode).          
-00013d90: 2020 6361 6368 655f 6669 6c65 2e77 7269    cache_file.wri
-00013da0: 7465 5f74 6578 7428 2274 6869 7320 6973  te_text("this is
-00013db0: 206e 6f74 2061 2070 6963 6b6c 6522 290a   not a pickle").
-00013dc0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00013dd0: 7274 2063 6572 6369 732e 7265 6164 5f63  rt cercis.read_c
-00013de0: 6163 6865 286d 6f64 6529 203d 3d20 7b7d  ache(mode) == {}
-00013df0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-00013e00: 203d 2028 776f 726b 7370 6163 6520 2f20   = (workspace / 
-00013e10: 2274 6573 742e 7079 2229 2e72 6573 6f6c  "test.py").resol
-00013e20: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
-00013e30: 2073 7263 2e77 7269 7465 5f74 6578 7428   src.write_text(
-00013e40: 2270 7269 6e74 2827 6865 6c6c 6f27 2922  "print('hello')"
-00013e50: 290a 2020 2020 2020 2020 2020 2020 696e  ).            in
-00013e60: 766f 6b65 426c 6163 6b28 5b73 7472 2873  vokeBlack([str(s
-00013e70: 7263 295d 290a 2020 2020 2020 2020 2020  rc)]).          
-00013e80: 2020 6361 6368 6520 3d20 6365 7263 6973    cache = cercis
-00013e90: 2e72 6561 645f 6361 6368 6528 6d6f 6465  .read_cache(mode
-00013ea0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-00013eb0: 7365 7274 2073 7472 2873 7263 2920 696e  sert str(src) in
-00013ec0: 2063 6163 6865 0a0a 2020 2020 6465 6620   cache..    def 
-00013ed0: 7465 7374 5f63 6163 6865 5f73 696e 676c  test_cache_singl
-00013ee0: 655f 6669 6c65 5f61 6c72 6561 6479 5f63  e_file_already_c
-00013ef0: 6163 6865 6428 7365 6c66 2920 2d3e 204e  ached(self) -> N
-00013f00: 6f6e 653a 0a20 2020 2020 2020 206d 6f64  one:.        mod
-00013f10: 6520 3d20 4445 4641 554c 545f 4d4f 4445  e = DEFAULT_MODE
-00013f20: 0a20 2020 2020 2020 2077 6974 6820 6361  .        with ca
-00013f30: 6368 655f 6469 7228 2920 6173 2077 6f72  che_dir() as wor
-00013f40: 6b73 7061 6365 3a0a 2020 2020 2020 2020  kspace:.        
-00013f50: 2020 2020 7372 6320 3d20 2877 6f72 6b73      src = (works
-00013f60: 7061 6365 202f 2022 7465 7374 2e70 7922  pace / "test.py"
-00013f70: 292e 7265 736f 6c76 6528 290a 2020 2020  ).resolve().    
-00013f80: 2020 2020 2020 2020 7372 632e 7772 6974          src.writ
-00013f90: 655f 7465 7874 2822 7072 696e 7428 2768  e_text("print('h
-00013fa0: 656c 6c6f 2729 2229 0a20 2020 2020 2020  ello')").       
-00013fb0: 2020 2020 2063 6572 6369 732e 7772 6974       cercis.writ
-00013fc0: 655f 6361 6368 6528 7b7d 2c20 5b73 7263  e_cache({}, [src
-00013fd0: 5d2c 206d 6f64 6529 0a20 2020 2020 2020  ], mode).       
-00013fe0: 2020 2020 2069 6e76 6f6b 6542 6c61 636b       invokeBlack
-00013ff0: 285b 7374 7228 7372 6329 5d29 0a20 2020  ([str(src)]).   
-00014000: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00014010: 7372 632e 7265 6164 5f74 6578 7428 2920  src.read_text() 
-00014020: 3d3d 2022 7072 696e 7428 2768 656c 6c6f  == "print('hello
-00014030: 2729 220a 0a20 2020 2040 6576 656e 745f  ')"..    @event_
-00014040: 6c6f 6f70 2829 0a20 2020 2064 6566 2074  loop().    def t
-00014050: 6573 745f 6361 6368 655f 6d75 6c74 6970  est_cache_multip
-00014060: 6c65 5f66 696c 6573 2873 656c 6629 202d  le_files(self) -
-00014070: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00014080: 6d6f 6465 203d 2044 4546 4155 4c54 5f4d  mode = DEFAULT_M
-00014090: 4f44 450a 2020 2020 2020 2020 7769 7468  ODE.        with
-000140a0: 2063 6163 6865 5f64 6972 2829 2061 7320   cache_dir() as 
-000140b0: 776f 726b 7370 6163 652c 2070 6174 6368  workspace, patch
-000140c0: 280a 2020 2020 2020 2020 2020 2020 2263  (.            "c
-000140d0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-000140e0: 732e 5072 6f63 6573 7350 6f6f 6c45 7865  s.ProcessPoolExe
-000140f0: 6375 746f 7222 2c20 6e65 773d 5468 7265  cutor", new=Thre
-00014100: 6164 506f 6f6c 4578 6563 7574 6f72 0a20  adPoolExecutor. 
-00014110: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00014120: 2020 2020 2020 6f6e 6520 3d20 2877 6f72        one = (wor
-00014130: 6b73 7061 6365 202f 2022 6f6e 652e 7079  kspace / "one.py
-00014140: 2229 2e72 6573 6f6c 7665 2829 0a20 2020  ").resolve().   
-00014150: 2020 2020 2020 2020 2077 6974 6820 6f6e           with on
-00014160: 652e 6f70 656e 2822 7722 2920 6173 2066  e.open("w") as f
-00014170: 6f62 6a3a 0a20 2020 2020 2020 2020 2020  obj:.           
-00014180: 2020 2020 2066 6f62 6a2e 7772 6974 6528       fobj.write(
-00014190: 2270 7269 6e74 2827 6865 6c6c 6f27 2922  "print('hello')"
-000141a0: 290a 2020 2020 2020 2020 2020 2020 7477  ).            tw
-000141b0: 6f20 3d20 2877 6f72 6b73 7061 6365 202f  o = (workspace /
-000141c0: 2022 7477 6f2e 7079 2229 2e72 6573 6f6c   "two.py").resol
-000141d0: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
-000141e0: 2077 6974 6820 7477 6f2e 6f70 656e 2822   with two.open("
-000141f0: 7722 2920 6173 2066 6f62 6a3a 0a20 2020  w") as fobj:.   
-00014200: 2020 2020 2020 2020 2020 2020 2066 6f62               fob
-00014210: 6a2e 7772 6974 6528 2270 7269 6e74 2827  j.write("print('
-00014220: 6865 6c6c 6f27 2922 290a 2020 2020 2020  hello')").      
-00014230: 2020 2020 2020 6365 7263 6973 2e77 7269        cercis.wri
-00014240: 7465 5f63 6163 6865 287b 7d2c 205b 6f6e  te_cache({}, [on
-00014250: 655d 2c20 6d6f 6465 290a 2020 2020 2020  e], mode).      
-00014260: 2020 2020 2020 696e 766f 6b65 426c 6163        invokeBlac
-00014270: 6b28 5b73 7472 2877 6f72 6b73 7061 6365  k([str(workspace
-00014280: 292c 2022 2d2d 7369 6e67 6c65 2d71 756f  ), "--single-quo
-00014290: 7465 3d46 616c 7365 225d 290a 2020 2020  te=False"]).    
-000142a0: 2020 2020 2020 2020 7769 7468 206f 6e65          with one
-000142b0: 2e6f 7065 6e28 2272 2229 2061 7320 666f  .open("r") as fo
-000142c0: 626a 3a0a 2020 2020 2020 2020 2020 2020  bj:.            
-000142d0: 2020 2020 6173 7365 7274 2066 6f62 6a2e      assert fobj.
-000142e0: 7265 6164 2829 203d 3d20 2270 7269 6e74  read() == "print
-000142f0: 2827 6865 6c6c 6f27 2922 0a20 2020 2020  ('hello')".     
-00014300: 2020 2020 2020 2077 6974 6820 7477 6f2e         with two.
-00014310: 6f70 656e 2822 7222 2920 6173 2066 6f62  open("r") as fob
-00014320: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
-00014330: 2020 2061 7373 6572 7420 666f 626a 2e72     assert fobj.r
-00014340: 6561 6428 2920 3d3d 2027 7072 696e 7428  ead() == 'print(
-00014350: 2268 656c 6c6f 2229 5c6e 270a 2020 2020  "hello")\n'.    
-00014360: 2020 2020 2020 2020 6361 6368 6520 3d20          cache = 
-00014370: 6365 7263 6973 2e72 6561 645f 6361 6368  cercis.read_cach
-00014380: 6528 6d6f 6465 290a 2020 2020 2020 2020  e(mode).        
-00014390: 2020 2020 6173 7365 7274 2073 7472 286f      assert str(o
-000143a0: 6e65 2920 696e 2063 6163 6865 0a20 2020  ne) in cache.   
-000143b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000143c0: 7374 7228 7477 6f29 2069 6e20 6361 6368  str(two) in cach
-000143d0: 650a 0a20 2020 2040 7079 7465 7374 2e6d  e..    @pytest.m
-000143e0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
-000143f0: 2263 6f6c 6f72 222c 205b 4661 6c73 652c  "color", [False,
-00014400: 2054 7275 655d 2c20 6964 733d 5b22 6e6f   True], ids=["no
-00014410: 2d63 6f6c 6f72 222c 2022 7769 7468 2d63  -color", "with-c
-00014420: 6f6c 6f72 225d 290a 2020 2020 6465 6620  olor"]).    def 
-00014430: 7465 7374 5f6e 6f5f 6361 6368 655f 7768  test_no_cache_wh
-00014440: 656e 5f77 7269 7465 6261 636b 5f64 6966  en_writeback_dif
-00014450: 6628 7365 6c66 2c20 636f 6c6f 723a 2062  f(self, color: b
-00014460: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
-00014470: 2020 2020 2020 6d6f 6465 203d 2044 4546        mode = DEF
-00014480: 4155 4c54 5f4d 4f44 450a 2020 2020 2020  AULT_MODE.      
-00014490: 2020 7769 7468 2063 6163 6865 5f64 6972    with cache_dir
-000144a0: 2829 2061 7320 776f 726b 7370 6163 653a  () as workspace:
-000144b0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-000144c0: 203d 2028 776f 726b 7370 6163 6520 2f20   = (workspace / 
-000144d0: 2274 6573 742e 7079 2229 2e72 6573 6f6c  "test.py").resol
-000144e0: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
-000144f0: 2077 6974 6820 7372 632e 6f70 656e 2822   with src.open("
-00014500: 7722 2920 6173 2066 6f62 6a3a 0a20 2020  w") as fobj:.   
-00014510: 2020 2020 2020 2020 2020 2020 2066 6f62               fob
-00014520: 6a2e 7772 6974 6528 2270 7269 6e74 2827  j.write("print('
-00014530: 6865 6c6c 6f27 2922 290a 2020 2020 2020  hello')").      
-00014540: 2020 2020 2020 7769 7468 2070 6174 6368        with patch
-00014550: 2822 6365 7263 6973 2e72 6561 645f 6361  ("cercis.read_ca
-00014560: 6368 6522 2920 6173 2072 6561 645f 6361  che") as read_ca
-00014570: 6368 652c 2070 6174 6368 280a 2020 2020  che, patch(.    
-00014580: 2020 2020 2020 2020 2020 2020 2263 6572              "cer
-00014590: 6369 732e 7772 6974 655f 6361 6368 6522  cis.write_cache"
-000145a0: 0a20 2020 2020 2020 2020 2020 2029 2061  .            ) a
-000145b0: 7320 7772 6974 655f 6361 6368 653a 0a20  s write_cache:. 
-000145c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000145d0: 6d64 203d 205b 7374 7228 7372 6329 2c20  md = [str(src), 
-000145e0: 222d 2d64 6966 6622 5d0a 2020 2020 2020  "--diff"].      
-000145f0: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
-00014600: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00014610: 2020 2020 2020 2020 636d 642e 6170 7065          cmd.appe
-00014620: 6e64 2822 2d2d 636f 6c6f 7222 290a 2020  nd("--color").  
-00014630: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00014640: 766f 6b65 426c 6163 6b28 636d 6429 0a20  vokeBlack(cmd). 
-00014650: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00014660: 6163 6865 5f66 696c 6520 3d20 6765 745f  ache_file = get_
-00014670: 6361 6368 655f 6669 6c65 286d 6f64 6529  cache_file(mode)
-00014680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014690: 2061 7373 6572 7420 6361 6368 655f 6669   assert cache_fi
-000146a0: 6c65 2e65 7869 7374 7328 2920 6973 2046  le.exists() is F
-000146b0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-000146c0: 2020 2020 2077 7269 7465 5f63 6163 6865       write_cache
-000146d0: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-000146e0: 6564 2829 0a20 2020 2020 2020 2020 2020  ed().           
-000146f0: 2020 2020 2072 6561 645f 6361 6368 652e       read_cache.
-00014700: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
-00014710: 6428 290a 0a20 2020 2040 7079 7465 7374  d()..    @pytest
-00014720: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-00014730: 6528 2263 6f6c 6f72 222c 205b 4661 6c73  e("color", [Fals
-00014740: 652c 2054 7275 655d 2c20 6964 733d 5b22  e, True], ids=["
-00014750: 6e6f 2d63 6f6c 6f72 222c 2022 7769 7468  no-color", "with
-00014760: 2d63 6f6c 6f72 225d 290a 2020 2020 4065  -color"]).    @e
-00014770: 7665 6e74 5f6c 6f6f 7028 290a 2020 2020  vent_loop().    
-00014780: 6465 6620 7465 7374 5f6f 7574 7075 745f  def test_output_
-00014790: 6c6f 636b 696e 675f 7768 656e 5f77 7269  locking_when_wri
-000147a0: 7465 6261 636b 5f64 6966 6628 7365 6c66  teback_diff(self
-000147b0: 2c20 636f 6c6f 723a 2062 6f6f 6c29 202d  , color: bool) -
-000147c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000147d0: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
-000147e0: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
-000147f0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-00014800: 6167 2069 6e20 7261 6e67 6528 302c 2034  ag in range(0, 4
-00014810: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014820: 2020 2073 7263 203d 2028 776f 726b 7370     src = (worksp
-00014830: 6163 6520 2f20 6622 7465 7374 7b74 6167  ace / f"test{tag
-00014840: 7d2e 7079 2229 2e72 6573 6f6c 7665 2829  }.py").resolve()
-00014850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014860: 2077 6974 6820 7372 632e 6f70 656e 2822   with src.open("
-00014870: 7722 2920 6173 2066 6f62 6a3a 0a20 2020  w") as fobj:.   
-00014880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014890: 2066 6f62 6a2e 7772 6974 6528 2270 7269   fobj.write("pri
-000148a0: 6e74 2827 6865 6c6c 6f27 2922 290a 2020  nt('hello')").  
-000148b0: 2020 2020 2020 2020 2020 7769 7468 2070            with p
-000148c0: 6174 6368 280a 2020 2020 2020 2020 2020  atch(.          
-000148d0: 2020 2020 2020 2263 6572 6369 732e 636f        "cercis.co
-000148e0: 6e63 7572 7265 6e63 792e 4d61 6e61 6765  ncurrency.Manage
-000148f0: 7222 2c20 7772 6170 733d 6d75 6c74 6970  r", wraps=multip
-00014900: 726f 6365 7373 696e 672e 4d61 6e61 6765  rocessing.Manage
-00014910: 720a 2020 2020 2020 2020 2020 2020 2920  r.            ) 
-00014920: 6173 206d 6772 3a0a 2020 2020 2020 2020  as mgr:.        
-00014930: 2020 2020 2020 2020 636d 6420 3d20 5b22          cmd = ["
-00014940: 2d2d 6469 6666 222c 2073 7472 2877 6f72  --diff", str(wor
-00014950: 6b73 7061 6365 295d 0a20 2020 2020 2020  kspace)].       
-00014960: 2020 2020 2020 2020 2069 6620 636f 6c6f           if colo
-00014970: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00014980: 2020 2020 2020 2063 6d64 2e61 7070 656e         cmd.appen
-00014990: 6428 222d 2d63 6f6c 6f72 2229 0a20 2020  d("--color").   
-000149a0: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
-000149b0: 6f6b 6542 6c61 636b 2863 6d64 2c20 6578  okeBlack(cmd, ex
-000149c0: 6974 5f63 6f64 653d 3029 0a20 2020 2020  it_code=0).     
-000149d0: 2020 2020 2020 2020 2020 2023 2074 6869             # thi
-000149e0: 7320 6973 6e27 7420 7175 6974 6520 646f  s isn't quite do
-000149f0: 696e 6720 7768 6174 2077 6520 7761 6e74  ing what we want
-00014a00: 2c20 6275 7420 6966 2069 7420 5f69 736e  , but if it _isn
-00014a10: 2774 5f0a 2020 2020 2020 2020 2020 2020  't_.            
-00014a20: 2020 2020 2320 6361 6c6c 6564 2074 6865      # called the
-00014a30: 6e20 7765 2063 616e 6e6f 7420 6265 2075  n we cannot be u
-00014a40: 7369 6e67 2074 6865 206c 6f63 6b20 6974  sing the lock it
-00014a50: 2070 726f 7669 6465 730a 2020 2020 2020   provides.      
-00014a60: 2020 2020 2020 2020 2020 6d67 722e 6173            mgr.as
-00014a70: 7365 7274 5f63 616c 6c65 6428 290a 0a20  sert_called().. 
-00014a80: 2020 2064 6566 2074 6573 745f 6e6f 5f63     def test_no_c
-00014a90: 6163 6865 5f77 6865 6e5f 7374 6469 6e28  ache_when_stdin(
-00014aa0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00014ab0: 2020 2020 2020 206d 6f64 6520 3d20 4445         mode = DE
-00014ac0: 4641 554c 545f 4d4f 4445 0a20 2020 2020  FAULT_MODE.     
-00014ad0: 2020 2077 6974 6820 6361 6368 655f 6469     with cache_di
-00014ae0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
-00014af0: 2072 6573 756c 7420 3d20 436c 6952 756e   result = CliRun
-00014b00: 6e65 7228 292e 696e 766f 6b65 280a 2020  ner().invoke(.  
-00014b10: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00014b20: 7263 6973 2e6d 6169 6e2c 205b 222d 225d  rcis.main, ["-"]
-00014b30: 2c20 696e 7075 743d 4279 7465 7349 4f28  , input=BytesIO(
-00014b40: 6222 7072 696e 7428 2768 656c 6c6f 2729  b"print('hello')
-00014b50: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
-00014b60: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00014b70: 6572 7420 6e6f 7420 7265 7375 6c74 2e65  ert not result.e
-00014b80: 7869 745f 636f 6465 0a20 2020 2020 2020  xit_code.       
-00014b90: 2020 2020 2063 6163 6865 5f66 696c 6520       cache_file 
-00014ba0: 3d20 6765 745f 6361 6368 655f 6669 6c65  = get_cache_file
-00014bb0: 286d 6f64 6529 0a20 2020 2020 2020 2020  (mode).         
-00014bc0: 2020 2061 7373 6572 7420 6e6f 7420 6361     assert not ca
-00014bd0: 6368 655f 6669 6c65 2e65 7869 7374 7328  che_file.exists(
-00014be0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00014bf0: 7265 6164 5f63 6163 6865 5f6e 6f5f 6361  read_cache_no_ca
-00014c00: 6368 6566 696c 6528 7365 6c66 2920 2d3e  chefile(self) ->
-00014c10: 204e 6f6e 653a 0a20 2020 2020 2020 206d   None:.        m
-00014c20: 6f64 6520 3d20 4445 4641 554c 545f 4d4f  ode = DEFAULT_MO
-00014c30: 4445 0a20 2020 2020 2020 2077 6974 6820  DE.        with 
-00014c40: 6361 6368 655f 6469 7228 293a 0a20 2020  cache_dir():.   
-00014c50: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00014c60: 6365 7263 6973 2e72 6561 645f 6361 6368  cercis.read_cach
-00014c70: 6528 6d6f 6465 2920 3d3d 207b 7d0a 0a20  e(mode) == {}.. 
-00014c80: 2020 2064 6566 2074 6573 745f 7772 6974     def test_writ
-00014c90: 655f 6361 6368 655f 7265 6164 5f63 6163  e_cache_read_cac
-00014ca0: 6865 2873 656c 6629 202d 3e20 4e6f 6e65  he(self) -> None
-00014cb0: 3a0a 2020 2020 2020 2020 6d6f 6465 203d  :.        mode =
-00014cc0: 2044 4546 4155 4c54 5f4d 4f44 450a 2020   DEFAULT_MODE.  
-00014cd0: 2020 2020 2020 7769 7468 2063 6163 6865        with cache
-00014ce0: 5f64 6972 2829 2061 7320 776f 726b 7370  _dir() as worksp
-00014cf0: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
-00014d00: 2073 7263 203d 2028 776f 726b 7370 6163   src = (workspac
-00014d10: 6520 2f20 2274 6573 742e 7079 2229 2e72  e / "test.py").r
-00014d20: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
-00014d30: 2020 2020 2073 7263 2e74 6f75 6368 2829       src.touch()
-00014d40: 0a20 2020 2020 2020 2020 2020 2063 6572  .            cer
-00014d50: 6369 732e 7772 6974 655f 6361 6368 6528  cis.write_cache(
-00014d60: 7b7d 2c20 5b73 7263 5d2c 206d 6f64 6529  {}, [src], mode)
-00014d70: 0a20 2020 2020 2020 2020 2020 2063 6163  .            cac
-00014d80: 6865 203d 2063 6572 6369 732e 7265 6164  he = cercis.read
-00014d90: 5f63 6163 6865 286d 6f64 6529 0a20 2020  _cache(mode).   
-00014da0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00014db0: 7374 7228 7372 6329 2069 6e20 6361 6368  str(src) in cach
-00014dc0: 650a 2020 2020 2020 2020 2020 2020 6173  e.            as
-00014dd0: 7365 7274 2063 6163 6865 5b73 7472 2873  sert cache[str(s
-00014de0: 7263 295d 203d 3d20 6365 7263 6973 2e67  rc)] == cercis.g
-00014df0: 6574 5f63 6163 6865 5f69 6e66 6f28 7372  et_cache_info(sr
-00014e00: 6329 0a0a 2020 2020 6465 6620 7465 7374  c)..    def test
-00014e10: 5f66 696c 7465 725f 6361 6368 6564 2873  _filter_cached(s
-00014e20: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00014e30: 2020 2020 2020 7769 7468 2054 656d 706f        with Tempo
-00014e40: 7261 7279 4469 7265 6374 6f72 7928 2920  raryDirectory() 
-00014e50: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
-00014e60: 2020 2020 2020 2020 2020 7061 7468 203d            path =
-00014e70: 2050 6174 6828 776f 726b 7370 6163 6529   Path(workspace)
-00014e80: 0a20 2020 2020 2020 2020 2020 2075 6e63  .            unc
-00014e90: 6163 6865 6420 3d20 2870 6174 6820 2f20  ached = (path / 
-00014ea0: 2275 6e63 6163 6865 6422 292e 7265 736f  "uncached").reso
-00014eb0: 6c76 6528 290a 2020 2020 2020 2020 2020  lve().          
-00014ec0: 2020 6361 6368 6564 203d 2028 7061 7468    cached = (path
-00014ed0: 202f 2022 6361 6368 6564 2229 2e72 6573   / "cached").res
-00014ee0: 6f6c 7665 2829 0a20 2020 2020 2020 2020  olve().         
-00014ef0: 2020 2063 6163 6865 645f 6275 745f 6368     cached_but_ch
-00014f00: 616e 6765 6420 3d20 2870 6174 6820 2f20  anged = (path / 
-00014f10: 2263 6861 6e67 6564 2229 2e72 6573 6f6c  "changed").resol
-00014f20: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
-00014f30: 2075 6e63 6163 6865 642e 746f 7563 6828   uncached.touch(
-00014f40: 290a 2020 2020 2020 2020 2020 2020 6361  ).            ca
-00014f50: 6368 6564 2e74 6f75 6368 2829 0a20 2020  ched.touch().   
-00014f60: 2020 2020 2020 2020 2063 6163 6865 645f           cached_
-00014f70: 6275 745f 6368 616e 6765 642e 746f 7563  but_changed.touc
-00014f80: 6828 290a 2020 2020 2020 2020 2020 2020  h().            
-00014f90: 6361 6368 6520 3d20 7b0a 2020 2020 2020  cache = {.      
-00014fa0: 2020 2020 2020 2020 2020 7374 7228 6361            str(ca
-00014fb0: 6368 6564 293a 2063 6572 6369 732e 6765  ched): cercis.ge
-00014fc0: 745f 6361 6368 655f 696e 666f 2863 6163  t_cache_info(cac
-00014fd0: 6865 6429 2c0a 2020 2020 2020 2020 2020  hed),.          
-00014fe0: 2020 2020 2020 7374 7228 6361 6368 6564        str(cached
-00014ff0: 5f62 7574 5f63 6861 6e67 6564 293a 2028  _but_changed): (
-00015000: 302e 302c 2030 292c 0a20 2020 2020 2020  0.0, 0),.       
-00015010: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00015020: 2020 2074 6f64 6f2c 2064 6f6e 6520 3d20     todo, done = 
-00015030: 6365 7263 6973 2e63 6163 6865 2e66 696c  cercis.cache.fil
-00015040: 7465 725f 6361 6368 6564 280a 2020 2020  ter_cached(.    
-00015050: 2020 2020 2020 2020 2020 2020 6361 6368              cach
-00015060: 652c 207b 756e 6361 6368 6564 2c20 6361  e, {uncached, ca
-00015070: 6368 6564 2c20 6361 6368 6564 5f62 7574  ched, cached_but
-00015080: 5f63 6861 6e67 6564 7d0a 2020 2020 2020  _changed}.      
-00015090: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000150a0: 2020 2020 6173 7365 7274 2074 6f64 6f20      assert todo 
-000150b0: 3d3d 207b 756e 6361 6368 6564 2c20 6361  == {uncached, ca
-000150c0: 6368 6564 5f62 7574 5f63 6861 6e67 6564  ched_but_changed
-000150d0: 7d0a 2020 2020 2020 2020 2020 2020 6173  }.            as
-000150e0: 7365 7274 2064 6f6e 6520 3d3d 207b 6361  sert done == {ca
-000150f0: 6368 6564 7d0a 0a20 2020 2064 6566 2074  ched}..    def t
-00015100: 6573 745f 7772 6974 655f 6361 6368 655f  est_write_cache_
-00015110: 6372 6561 7465 735f 6469 7265 6374 6f72  creates_director
-00015120: 795f 6966 5f6e 6565 6465 6428 7365 6c66  y_if_needed(self
-00015130: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00015140: 2020 206d 6f64 6520 3d20 4445 4641 554c     mode = DEFAUL
-00015150: 545f 4d4f 4445 0a20 2020 2020 2020 2077  T_MODE.        w
-00015160: 6974 6820 6361 6368 655f 6469 7228 6578  ith cache_dir(ex
-00015170: 6973 7473 3d46 616c 7365 2920 6173 2077  ists=False) as w
-00015180: 6f72 6b73 7061 6365 3a0a 2020 2020 2020  orkspace:.      
-00015190: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
-000151a0: 2077 6f72 6b73 7061 6365 2e65 7869 7374   workspace.exist
-000151b0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-000151c0: 6365 7263 6973 2e77 7269 7465 5f63 6163  cercis.write_cac
-000151d0: 6865 287b 7d2c 205b 5d2c 206d 6f64 6529  he({}, [], mode)
-000151e0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-000151f0: 6572 7420 776f 726b 7370 6163 652e 6578  ert workspace.ex
-00015200: 6973 7473 2829 0a0a 2020 2020 4065 7665  ists()..    @eve
-00015210: 6e74 5f6c 6f6f 7028 290a 2020 2020 6465  nt_loop().    de
-00015220: 6620 7465 7374 5f66 6169 6c65 645f 666f  f test_failed_fo
-00015230: 726d 6174 7469 6e67 5f64 6f65 735f 6e6f  rmatting_does_no
-00015240: 745f 6765 745f 6361 6368 6564 2873 656c  t_get_cached(sel
-00015250: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00015260: 2020 2020 6d6f 6465 203d 2044 4546 4155      mode = DEFAU
-00015270: 4c54 5f4d 4f44 450a 2020 2020 2020 2020  LT_MODE.        
-00015280: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
-00015290: 2061 7320 776f 726b 7370 6163 652c 2070   as workspace, p
-000152a0: 6174 6368 280a 2020 2020 2020 2020 2020  atch(.          
-000152b0: 2020 2263 6f6e 6375 7272 656e 742e 6675    "concurrent.fu
-000152c0: 7475 7265 732e 5072 6f63 6573 7350 6f6f  tures.ProcessPoo
-000152d0: 6c45 7865 6375 746f 7222 2c20 6e65 773d  lExecutor", new=
-000152e0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
-000152f0: 6f72 0a20 2020 2020 2020 2029 3a0a 2020  or.        ):.  
-00015300: 2020 2020 2020 2020 2020 6661 696c 696e            failin
-00015310: 6720 3d20 2877 6f72 6b73 7061 6365 202f  g = (workspace /
-00015320: 2022 6661 696c 696e 672e 7079 2229 2e72   "failing.py").r
-00015330: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
-00015340: 2020 2020 2077 6974 6820 6661 696c 696e       with failin
-00015350: 672e 6f70 656e 2822 7722 2920 6173 2066  g.open("w") as f
-00015360: 6f62 6a3a 0a20 2020 2020 2020 2020 2020  obj:.           
-00015370: 2020 2020 2066 6f62 6a2e 7772 6974 6528       fobj.write(
-00015380: 226e 6f74 2061 6374 7561 6c6c 7920 7079  "not actually py
-00015390: 7468 6f6e 2229 0a20 2020 2020 2020 2020  thon").         
-000153a0: 2020 2063 6c65 616e 203d 2028 776f 726b     clean = (work
-000153b0: 7370 6163 6520 2f20 2263 6c65 616e 2e70  space / "clean.p
-000153c0: 7922 292e 7265 736f 6c76 6528 290a 2020  y").resolve().  
-000153d0: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-000153e0: 6c65 616e 2e6f 7065 6e28 2277 2229 2061  lean.open("w") a
-000153f0: 7320 666f 626a 3a0a 2020 2020 2020 2020  s fobj:.        
-00015400: 2020 2020 2020 2020 666f 626a 2e77 7269          fobj.wri
-00015410: 7465 2827 7072 696e 7428 2268 656c 6c6f  te('print("hello
-00015420: 2229 5c6e 2729 0a20 2020 2020 2020 2020  ")\n').         
-00015430: 2020 2069 6e76 6f6b 6542 6c61 636b 285b     invokeBlack([
-00015440: 7374 7228 776f 726b 7370 6163 6529 5d2c  str(workspace)],
-00015450: 2065 7869 745f 636f 6465 3d31 3233 290a   exit_code=123).
-00015460: 2020 2020 2020 2020 2020 2020 6361 6368              cach
-00015470: 6520 3d20 6365 7263 6973 2e72 6561 645f  e = cercis.read_
-00015480: 6361 6368 6528 6d6f 6465 290a 2020 2020  cache(mode).    
-00015490: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-000154a0: 7472 2866 6169 6c69 6e67 2920 6e6f 7420  tr(failing) not 
-000154b0: 696e 2063 6163 6865 0a20 2020 2020 2020  in cache.       
-000154c0: 2020 2020 2061 7373 6572 7420 7374 7228       assert str(
-000154d0: 636c 6561 6e29 2069 6e20 6361 6368 650a  clean) in cache.
-000154e0: 0a20 2020 2064 6566 2074 6573 745f 7772  .    def test_wr
-000154f0: 6974 655f 6361 6368 655f 7772 6974 655f  ite_cache_write_
-00015500: 6661 696c 2873 656c 6629 202d 3e20 4e6f  fail(self) -> No
-00015510: 6e65 3a0a 2020 2020 2020 2020 6d6f 6465  ne:.        mode
-00015520: 203d 2044 4546 4155 4c54 5f4d 4f44 450a   = DEFAULT_MODE.
-00015530: 2020 2020 2020 2020 7769 7468 2063 6163          with cac
-00015540: 6865 5f64 6972 2829 2c20 7061 7463 682e  he_dir(), patch.
-00015550: 6f62 6a65 6374 2850 6174 682c 2022 6f70  object(Path, "op
-00015560: 656e 2229 2061 7320 6d6f 636b 3a0a 2020  en") as mock:.  
-00015570: 2020 2020 2020 2020 2020 6d6f 636b 2e73            mock.s
-00015580: 6964 655f 6566 6665 6374 203d 204f 5345  ide_effect = OSE
-00015590: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
-000155a0: 2063 6572 6369 732e 7772 6974 655f 6361   cercis.write_ca
-000155b0: 6368 6528 7b7d 2c20 5b5d 2c20 6d6f 6465  che({}, [], mode
-000155c0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-000155d0: 7265 6164 5f63 6163 6865 5f6c 696e 655f  read_cache_line_
-000155e0: 6c65 6e67 7468 7328 7365 6c66 2920 2d3e  lengths(self) ->
-000155f0: 204e 6f6e 653a 0a20 2020 2020 2020 206d   None:.        m
-00015600: 6f64 6520 3d20 4445 4641 554c 545f 4d4f  ode = DEFAULT_MO
-00015610: 4445 0a20 2020 2020 2020 2073 686f 7274  DE.        short
-00015620: 5f6d 6f64 6520 3d20 7265 706c 6163 6528  _mode = replace(
-00015630: 4445 4641 554c 545f 4d4f 4445 2c20 6c69  DEFAULT_MODE, li
-00015640: 6e65 5f6c 656e 6774 683d 3129 0a20 2020  ne_length=1).   
-00015650: 2020 2020 2077 6974 6820 6361 6368 655f       with cache_
-00015660: 6469 7228 2920 6173 2077 6f72 6b73 7061  dir() as workspa
-00015670: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-00015680: 7061 7468 203d 2028 776f 726b 7370 6163  path = (workspac
-00015690: 6520 2f20 2266 696c 652e 7079 2229 2e72  e / "file.py").r
-000156a0: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
-000156b0: 2020 2020 2070 6174 682e 746f 7563 6828       path.touch(
-000156c0: 290a 2020 2020 2020 2020 2020 2020 6365  ).            ce
-000156d0: 7263 6973 2e77 7269 7465 5f63 6163 6865  rcis.write_cache
-000156e0: 287b 7d2c 205b 7061 7468 5d2c 206d 6f64  ({}, [path], mod
-000156f0: 6529 0a20 2020 2020 2020 2020 2020 206f  e).            o
-00015700: 6e65 203d 2063 6572 6369 732e 7265 6164  ne = cercis.read
-00015710: 5f63 6163 6865 286d 6f64 6529 0a20 2020  _cache(mode).   
-00015720: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00015730: 7374 7228 7061 7468 2920 696e 206f 6e65  str(path) in one
-00015740: 0a20 2020 2020 2020 2020 2020 2074 776f  .            two
-00015750: 203d 2063 6572 6369 732e 7265 6164 5f63   = cercis.read_c
-00015760: 6163 6865 2873 686f 7274 5f6d 6f64 6529  ache(short_mode)
-00015770: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00015780: 6572 7420 7374 7228 7061 7468 2920 6e6f  ert str(path) no
-00015790: 7420 696e 2074 776f 0a0a 0a64 6566 2061  t in two...def a
-000157a0: 7373 6572 745f 636f 6c6c 6563 7465 645f  ssert_collected_
-000157b0: 736f 7572 6365 7328 0a20 2020 2020 2020  sources(.       
-000157c0: 2073 7263 3a20 5365 7175 656e 6365 5b55   src: Sequence[U
-000157d0: 6e69 6f6e 5b73 7472 2c20 5061 7468 5d5d  nion[str, Path]]
-000157e0: 2c0a 2020 2020 2020 2020 6578 7065 6374  ,.        expect
-000157f0: 6564 3a20 5365 7175 656e 6365 5b55 6e69  ed: Sequence[Uni
-00015800: 6f6e 5b73 7472 2c20 5061 7468 5d5d 2c0a  on[str, Path]],.
-00015810: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-00015820: 2020 2063 7478 3a20 4f70 7469 6f6e 616c     ctx: Optional
-00015830: 5b46 616b 6543 6f6e 7465 7874 5d20 3d20  [FakeContext] = 
-00015840: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
-00015850: 636c 7564 653a 204f 7074 696f 6e61 6c5b  clude: Optional[
-00015860: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00015870: 2020 2020 2069 6e63 6c75 6465 3a20 4f70       include: Op
-00015880: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00015890: 6e65 2c0a 2020 2020 2020 2020 6578 7465  ne,.        exte
-000158a0: 6e64 5f65 7863 6c75 6465 3a20 4f70 7469  nd_exclude: Opti
-000158b0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-000158c0: 2c0a 2020 2020 2020 2020 666f 7263 655f  ,.        force_
-000158d0: 6578 636c 7564 653a 204f 7074 696f 6e61  exclude: Optiona
-000158e0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-000158f0: 2020 2020 2020 2073 7464 696e 5f66 696c         stdin_fil
-00015900: 656e 616d 653a 204f 7074 696f 6e61 6c5b  ename: Optional[
-00015910: 7374 725d 203d 204e 6f6e 652c 0a29 202d  str] = None,.) -
-00015920: 3e20 4e6f 6e65 3a0a 2020 2020 6773 5f73  > None:.    gs_s
-00015930: 7263 203d 2074 7570 6c65 2873 7472 2850  rc = tuple(str(P
-00015940: 6174 6828 7329 2920 666f 7220 7320 696e  ath(s)) for s in
-00015950: 2073 7263 290a 2020 2020 6773 5f65 7870   src).    gs_exp
-00015960: 6563 7465 6420 3d20 5b50 6174 6828 7329  ected = [Path(s)
-00015970: 2066 6f72 2073 2069 6e20 6578 7065 6374   for s in expect
-00015980: 6564 5d0a 2020 2020 6773 5f65 7863 6c75  ed].    gs_exclu
-00015990: 6465 203d 204e 6f6e 6520 6966 2065 7863  de = None if exc
-000159a0: 6c75 6465 2069 7320 4e6f 6e65 2065 6c73  lude is None els
-000159b0: 6520 636f 6d70 696c 655f 7061 7474 6572  e compile_patter
-000159c0: 6e28 6578 636c 7564 6529 0a20 2020 2067  n(exclude).    g
-000159d0: 735f 696e 636c 7564 6520 3d20 4445 4641  s_include = DEFA
-000159e0: 554c 545f 494e 434c 5544 4520 6966 2069  ULT_INCLUDE if i
-000159f0: 6e63 6c75 6465 2069 7320 4e6f 6e65 2065  nclude is None e
-00015a00: 6c73 6520 636f 6d70 696c 655f 7061 7474  lse compile_patt
-00015a10: 6572 6e28 696e 636c 7564 6529 0a20 2020  ern(include).   
-00015a20: 2067 735f 6578 7465 6e64 5f65 7863 6c75   gs_extend_exclu
-00015a30: 6465 203d 2028 0a20 2020 2020 2020 204e  de = (.        N
-00015a40: 6f6e 6520 6966 2065 7874 656e 645f 6578  one if extend_ex
-00015a50: 636c 7564 6520 6973 204e 6f6e 6520 656c  clude is None el
-00015a60: 7365 2063 6f6d 7069 6c65 5f70 6174 7465  se compile_patte
-00015a70: 726e 2865 7874 656e 645f 6578 636c 7564  rn(extend_exclud
-00015a80: 6529 0a20 2020 2029 0a20 2020 2067 735f  e).    ).    gs_
-00015a90: 666f 7263 655f 6578 636c 7564 6520 3d20  force_exclude = 
-00015aa0: 4e6f 6e65 2069 6620 666f 7263 655f 6578  None if force_ex
-00015ab0: 636c 7564 6520 6973 204e 6f6e 6520 656c  clude is None el
-00015ac0: 7365 2063 6f6d 7069 6c65 5f70 6174 7465  se compile_patte
-00015ad0: 726e 2866 6f72 6365 5f65 7863 6c75 6465  rn(force_exclude
-00015ae0: 290a 2020 2020 636f 6c6c 6563 7465 6420  ).    collected 
-00015af0: 3d20 6365 7263 6973 2e67 6574 5f73 6f75  = cercis.get_sou
-00015b00: 7263 6573 280a 2020 2020 2020 2020 6374  rces(.        ct
-00015b10: 783d 6374 7820 6f72 2046 616b 6543 6f6e  x=ctx or FakeCon
-00015b20: 7465 7874 2829 2c0a 2020 2020 2020 2020  text(),.        
-00015b30: 7372 633d 6773 5f73 7263 2c0a 2020 2020  src=gs_src,.    
-00015b40: 2020 2020 7175 6965 743d 4661 6c73 652c      quiet=False,
-00015b50: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
-00015b60: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00015b70: 696e 636c 7564 653d 6773 5f69 6e63 6c75  include=gs_inclu
-00015b80: 6465 2c0a 2020 2020 2020 2020 6578 636c  de,.        excl
-00015b90: 7564 653d 6773 5f65 7863 6c75 6465 2c0a  ude=gs_exclude,.
-00015ba0: 2020 2020 2020 2020 6578 7465 6e64 5f65          extend_e
-00015bb0: 7863 6c75 6465 3d67 735f 6578 7465 6e64  xclude=gs_extend
-00015bc0: 5f65 7863 6c75 6465 2c0a 2020 2020 2020  _exclude,.      
-00015bd0: 2020 666f 7263 655f 6578 636c 7564 653d    force_exclude=
-00015be0: 6773 5f66 6f72 6365 5f65 7863 6c75 6465  gs_force_exclude
-00015bf0: 2c0a 2020 2020 2020 2020 7265 706f 7274  ,.        report
-00015c00: 3d63 6572 6369 732e 5265 706f 7274 2829  =cercis.Report()
-00015c10: 2c0a 2020 2020 2020 2020 7374 6469 6e5f  ,.        stdin_
-00015c20: 6669 6c65 6e61 6d65 3d73 7464 696e 5f66  filename=stdin_f
-00015c30: 696c 656e 616d 652c 0a20 2020 2029 0a20  ilename,.    ). 
-00015c40: 2020 2061 7373 6572 7420 736f 7274 6564     assert sorted
-00015c50: 2863 6f6c 6c65 6374 6564 2920 3d3d 2073  (collected) == s
-00015c60: 6f72 7465 6428 6773 5f65 7870 6563 7465  orted(gs_expecte
-00015c70: 6429 0a0a 0a63 6c61 7373 2054 6573 7446  d)...class TestF
-00015c80: 696c 6543 6f6c 6c65 6374 696f 6e3a 0a20  ileCollection:. 
-00015c90: 2020 2064 6566 2074 6573 745f 696e 636c     def test_incl
-00015ca0: 7564 655f 6578 636c 7564 6528 7365 6c66  ude_exclude(self
-00015cb0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00015cc0: 2020 2070 6174 6820 3d20 5448 4953 5f44     path = THIS_D
-00015cd0: 4952 202f 2022 6461 7461 2220 2f20 2269  IR / "data" / "i
-00015ce0: 6e63 6c75 6465 5f65 7863 6c75 6465 5f74  nclude_exclude_t
-00015cf0: 6573 7473 220a 2020 2020 2020 2020 7372  ests".        sr
-00015d00: 6320 3d20 5b70 6174 685d 0a20 2020 2020  c = [path].     
-00015d10: 2020 2065 7870 6563 7465 6420 3d20 5b0a     expected = [.
-00015d20: 2020 2020 2020 2020 2020 2020 5061 7468              Path
-00015d30: 2870 6174 6820 2f20 2262 2f64 6f6e 745f  (path / "b/dont_
-00015d40: 6578 636c 7564 652f 612e 7079 2229 2c0a  exclude/a.py"),.
-00015d50: 2020 2020 2020 2020 2020 2020 5061 7468              Path
-00015d60: 2870 6174 6820 2f20 2262 2f64 6f6e 745f  (path / "b/dont_
-00015d70: 6578 636c 7564 652f 612e 7079 6922 292c  exclude/a.pyi"),
-00015d80: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-00015d90: 2020 2061 7373 6572 745f 636f 6c6c 6563     assert_collec
-00015da0: 7465 645f 736f 7572 6365 7328 0a20 2020  ted_sources(.   
-00015db0: 2020 2020 2020 2020 2073 7263 2c0a 2020           src,.  
-00015dc0: 2020 2020 2020 2020 2020 6578 7065 6374            expect
-00015dd0: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
-00015de0: 696e 636c 7564 653d 7222 5c2e 7079 693f  include=r"\.pyi?
-00015df0: 2422 2c0a 2020 2020 2020 2020 2020 2020  $",.            
-00015e00: 6578 636c 7564 653d 7222 2f65 7863 6c75  exclude=r"/exclu
-00015e10: 6465 2f7c 2f5c 2e64 6566 696e 6974 656c  de/|/\.definitel
-00015e20: 795f 6578 636c 7564 652f 222c 0a20 2020  y_exclude/",.   
-00015e30: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00015e40: 7465 7374 5f67 6974 6967 6e6f 7265 5f75  test_gitignore_u
-00015e50: 7365 645f 6173 5f64 6566 6175 6c74 2873  sed_as_default(s
-00015e60: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00015e70: 2020 2020 2020 6261 7365 203d 2050 6174        base = Pat
-00015e80: 6828 4441 5441 5f44 4952 202f 2022 696e  h(DATA_DIR / "in
-00015e90: 636c 7564 655f 6578 636c 7564 655f 7465  clude_exclude_te
-00015ea0: 7374 7322 290a 2020 2020 2020 2020 6578  sts").        ex
-00015eb0: 7065 6374 6564 203d 205b 0a20 2020 2020  pected = [.     
-00015ec0: 2020 2020 2020 2062 6173 6520 2f20 2262         base / "b
-00015ed0: 2f2e 6465 6669 6e69 7465 6c79 5f65 7863  /.definitely_exc
-00015ee0: 6c75 6465 2f61 2e70 7922 2c0a 2020 2020  lude/a.py",.    
-00015ef0: 2020 2020 2020 2020 6261 7365 202f 2022          base / "
-00015f00: 622f 2e64 6566 696e 6974 656c 795f 6578  b/.definitely_ex
-00015f10: 636c 7564 652f 612e 7079 6922 2c0a 2020  clude/a.pyi",.  
-00015f20: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00015f30: 7372 6320 3d20 5b62 6173 6520 2f20 2262  src = [base / "b
-00015f40: 2f22 5d0a 2020 2020 2020 2020 6374 7820  /"].        ctx 
-00015f50: 3d20 4661 6b65 436f 6e74 6578 7428 290a  = FakeContext().
-00015f60: 2020 2020 2020 2020 6374 782e 6f62 6a5b          ctx.obj[
-00015f70: 2272 6f6f 7422 5d20 3d20 6261 7365 0a20  "root"] = base. 
-00015f80: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
-00015f90: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
-00015fa0: 7372 632c 2065 7870 6563 7465 642c 2063  src, expected, c
-00015fb0: 7478 3d63 7478 2c20 6578 7465 6e64 5f65  tx=ctx, extend_e
-00015fc0: 7863 6c75 6465 3d72 222f 6578 636c 7564  xclude=r"/exclud
-00015fd0: 652f 2229 0a0a 2020 2020 6465 6620 7465  e/")..    def te
-00015fe0: 7374 5f67 6974 6967 6e6f 7265 5f75 7365  st_gitignore_use
-00015ff0: 645f 6f6e 5f6d 756c 7469 706c 655f 736f  d_on_multiple_so
-00016000: 7572 6365 7328 7365 6c66 2920 2d3e 204e  urces(self) -> N
-00016010: 6f6e 653a 0a20 2020 2020 2020 2072 6f6f  one:.        roo
-00016020: 7420 3d20 5061 7468 2844 4154 415f 4449  t = Path(DATA_DI
-00016030: 5220 2f20 2267 6974 6967 6e6f 7265 5f75  R / "gitignore_u
-00016040: 7365 645f 6f6e 5f6d 756c 7469 706c 655f  sed_on_multiple_
-00016050: 736f 7572 6365 7322 290a 2020 2020 2020  sources").      
-00016060: 2020 6578 7065 6374 6564 203d 205b 0a20    expected = [. 
-00016070: 2020 2020 2020 2020 2020 2072 6f6f 7420             root 
-00016080: 2f20 2264 6972 3122 202f 2022 622e 7079  / "dir1" / "b.py
-00016090: 222c 0a20 2020 2020 2020 2020 2020 2072  ",.            r
-000160a0: 6f6f 7420 2f20 2264 6972 3222 202f 2022  oot / "dir2" / "
-000160b0: 622e 7079 222c 0a20 2020 2020 2020 205d  b.py",.        ]
-000160c0: 0a20 2020 2020 2020 2063 7478 203d 2046  .        ctx = F
-000160d0: 616b 6543 6f6e 7465 7874 2829 0a20 2020  akeContext().   
-000160e0: 2020 2020 2063 7478 2e6f 626a 5b22 726f       ctx.obj["ro
-000160f0: 6f74 225d 203d 2072 6f6f 740a 2020 2020  ot"] = root.    
-00016100: 2020 2020 7372 6320 3d20 5b72 6f6f 7420      src = [root 
-00016110: 2f20 2264 6972 3122 2c20 726f 6f74 202f  / "dir1", root /
-00016120: 2022 6469 7232 225d 0a20 2020 2020 2020   "dir2"].       
-00016130: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
-00016140: 645f 736f 7572 6365 7328 7372 632c 2065  d_sources(src, e
-00016150: 7870 6563 7465 642c 2063 7478 3d63 7478  xpected, ctx=ctx
-00016160: 290a 0a20 2020 2040 7061 7463 6828 2263  )..    @patch("c
-00016170: 6572 6369 732e 6669 6e64 5f70 726f 6a65  ercis.find_proje
-00016180: 6374 5f72 6f6f 7422 2c20 6c61 6d62 6461  ct_root", lambda
-00016190: 202a 6172 6773 3a20 2854 4849 535f 4449   *args: (THIS_DI
-000161a0: 522e 7265 736f 6c76 6528 292c 204e 6f6e  R.resolve(), Non
-000161b0: 6529 290a 2020 2020 6465 6620 7465 7374  e)).    def test
-000161c0: 5f65 7863 6c75 6465 5f66 6f72 5f69 7373  _exclude_for_iss
-000161d0: 7565 5f31 3537 3228 7365 6c66 2920 2d3e  ue_1572(self) ->
-000161e0: 204e 6f6e 653a 0a20 2020 2020 2020 2023   None:.        #
-000161f0: 2045 7863 6c75 6465 2073 686f 756c 646e   Exclude shouldn
-00016200: 2774 2074 6f75 6368 2066 696c 6573 2074  't touch files t
-00016210: 6861 7420 7765 7265 2065 7870 6c69 6369  hat were explici
-00016220: 746c 7920 6769 7665 6e20 746f 2042 6c61  tly given to Bla
-00016230: 636b 2074 6872 6f75 6768 2074 6865 0a20  ck through the. 
-00016240: 2020 2020 2020 2023 2043 4c49 2e20 4578         # CLI. Ex
-00016250: 636c 7564 6520 6973 2073 7570 706f 7365  clude is suppose
-00016260: 6420 746f 206f 6e6c 7920 6170 706c 7920  d to only apply 
-00016270: 746f 2074 6865 2072 6563 7572 7369 7665  to the recursive
-00016280: 2064 6973 636f 7665 7279 206f 6620 6669   discovery of fi
-00016290: 6c65 732e 0a20 2020 2020 2020 2023 2068  les..        # h
-000162a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000162b0: 6d2f 7073 662f 626c 6163 6b2f 6973 7375  m/psf/black/issu
-000162c0: 6573 2f31 3537 320a 2020 2020 2020 2020  es/1572.        
-000162d0: 7061 7468 203d 2044 4154 415f 4449 5220  path = DATA_DIR 
-000162e0: 2f20 2269 6e63 6c75 6465 5f65 7863 6c75  / "include_exclu
-000162f0: 6465 5f74 6573 7473 220a 2020 2020 2020  de_tests".      
-00016300: 2020 7372 6320 3d20 5b70 6174 6820 2f20    src = [path / 
-00016310: 2262 2f65 7863 6c75 6465 2f61 2e70 7922  "b/exclude/a.py"
-00016320: 5d0a 2020 2020 2020 2020 6578 7065 6374  ].        expect
-00016330: 6564 203d 205b 7061 7468 202f 2022 622f  ed = [path / "b/
-00016340: 6578 636c 7564 652f 612e 7079 225d 0a20  exclude/a.py"]. 
-00016350: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
-00016360: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
-00016370: 7372 632c 2065 7870 6563 7465 642c 2069  src, expected, i
-00016380: 6e63 6c75 6465 3d22 222c 2065 7863 6c75  nclude="", exclu
-00016390: 6465 3d72 222f 6578 636c 7564 652f 7c61  de=r"/exclude/|a
-000163a0: 5c2e 7079 2229 0a0a 2020 2020 6465 6620  \.py")..    def 
-000163b0: 7465 7374 5f67 6974 6967 6e6f 7265 5f65  test_gitignore_e
-000163c0: 7863 6c75 6465 2873 656c 6629 202d 3e20  xclude(self) -> 
-000163d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
-000163e0: 7468 203d 2054 4849 535f 4449 5220 2f20  th = THIS_DIR / 
-000163f0: 2264 6174 6122 202f 2022 696e 636c 7564  "data" / "includ
-00016400: 655f 6578 636c 7564 655f 7465 7374 7322  e_exclude_tests"
-00016410: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
-00016420: 203d 2072 652e 636f 6d70 696c 6528 7222   = re.compile(r"
-00016430: 5c2e 7079 693f 2422 290a 2020 2020 2020  \.pyi?$").      
-00016440: 2020 6578 636c 7564 6520 3d20 7265 2e63    exclude = re.c
-00016450: 6f6d 7069 6c65 2872 2222 290a 2020 2020  ompile(r"").    
-00016460: 2020 2020 7265 706f 7274 203d 2063 6572      report = cer
-00016470: 6369 732e 5265 706f 7274 2829 0a20 2020  cis.Report().   
-00016480: 2020 2020 2067 6974 6967 6e6f 7265 203d       gitignore =
-00016490: 2050 6174 6853 7065 632e 6672 6f6d 5f6c   PathSpec.from_l
-000164a0: 696e 6573 280a 2020 2020 2020 2020 2020  ines(.          
-000164b0: 2020 2267 6974 7769 6c64 6d61 7463 6822    "gitwildmatch"
-000164c0: 2c20 5b22 6578 636c 7564 652f 222c 2022  , ["exclude/", "
-000164d0: 2e64 6566 696e 6974 656c 795f 6578 636c  .definitely_excl
-000164e0: 7564 6522 5d0a 2020 2020 2020 2020 290a  ude"].        ).
-000164f0: 2020 2020 2020 2020 736f 7572 6365 733a          sources:
-00016500: 204c 6973 745b 5061 7468 5d20 3d20 5b5d   List[Path] = []
-00016510: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-00016520: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
-00016530: 2020 5061 7468 2870 6174 6820 2f20 2262    Path(path / "b
-00016540: 2f64 6f6e 745f 6578 636c 7564 652f 612e  /dont_exclude/a.
-00016550: 7079 2229 2c0a 2020 2020 2020 2020 2020  py"),.          
-00016560: 2020 5061 7468 2870 6174 6820 2f20 2262    Path(path / "b
-00016570: 2f64 6f6e 745f 6578 636c 7564 652f 612e  /dont_exclude/a.
-00016580: 7079 6922 292c 0a20 2020 2020 2020 205d  pyi"),.        ]
-00016590: 0a20 2020 2020 2020 2074 6869 735f 6162  .        this_ab
-000165a0: 7320 3d20 5448 4953 5f44 4952 2e72 6573  s = THIS_DIR.res
-000165b0: 6f6c 7665 2829 0a20 2020 2020 2020 2073  olve().        s
-000165c0: 6f75 7263 6573 2e65 7874 656e 6428 0a20  ources.extend(. 
-000165d0: 2020 2020 2020 2020 2020 2063 6572 6369             cerci
-000165e0: 732e 6765 6e5f 7079 7468 6f6e 5f66 696c  s.gen_python_fil
-000165f0: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-00016600: 2020 2020 7061 7468 2e69 7465 7264 6972      path.iterdir
-00016610: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00016620: 2020 2020 7468 6973 5f61 6273 2c0a 2020      this_abs,.  
-00016630: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00016640: 636c 7564 652c 0a20 2020 2020 2020 2020  clude,.         
-00016650: 2020 2020 2020 2065 7863 6c75 6465 2c0a         exclude,.
-00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016670: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00016680: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
-00016690: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-000166a0: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
-000166b0: 2020 2020 7b70 6174 683a 2067 6974 6967      {path: gitig
-000166c0: 6e6f 7265 7d2c 0a20 2020 2020 2020 2020  nore},.         
-000166d0: 2020 2020 2020 2076 6572 626f 7365 3d46         verbose=F
-000166e0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000166f0: 2020 2020 2020 7175 6965 743d 4661 6c73        quiet=Fals
-00016700: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-00016710: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00016720: 2020 2061 7373 6572 7420 736f 7274 6564     assert sorted
-00016730: 2865 7870 6563 7465 6429 203d 3d20 736f  (expected) == so
-00016740: 7274 6564 2873 6f75 7263 6573 290a 0a20  rted(sources).. 
-00016750: 2020 2064 6566 2074 6573 745f 6e65 7374     def test_nest
-00016760: 6564 5f67 6974 6967 6e6f 7265 2873 656c  ed_gitignore(sel
-00016770: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00016780: 2020 2020 7061 7468 203d 2050 6174 6828      path = Path(
-00016790: 5448 4953 5f44 4952 202f 2022 6461 7461  THIS_DIR / "data
-000167a0: 2220 2f20 226e 6573 7465 645f 6769 7469  " / "nested_giti
-000167b0: 676e 6f72 655f 7465 7374 7322 290a 2020  gnore_tests").  
-000167c0: 2020 2020 2020 696e 636c 7564 6520 3d20        include = 
-000167d0: 7265 2e63 6f6d 7069 6c65 2872 225c 2e70  re.compile(r"\.p
-000167e0: 7969 3f24 2229 0a20 2020 2020 2020 2065  yi?$").        e
-000167f0: 7863 6c75 6465 203d 2072 652e 636f 6d70  xclude = re.comp
-00016800: 696c 6528 7222 2229 0a20 2020 2020 2020  ile(r"").       
-00016810: 2072 6f6f 745f 6769 7469 676e 6f72 6520   root_gitignore 
-00016820: 3d20 6365 7263 6973 2e66 696c 6573 2e67  = cercis.files.g
-00016830: 6574 5f67 6974 6967 6e6f 7265 2870 6174  et_gitignore(pat
-00016840: 6829 0a20 2020 2020 2020 2072 6570 6f72  h).        repor
-00016850: 7420 3d20 6365 7263 6973 2e52 6570 6f72  t = cercis.Repor
-00016860: 7428 290a 2020 2020 2020 2020 6578 7065  t().        expe
-00016870: 6374 6564 3a20 4c69 7374 5b50 6174 685d  cted: List[Path]
-00016880: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00016890: 2050 6174 6828 7061 7468 202f 2022 782e   Path(path / "x.
-000168a0: 7079 2229 2c0a 2020 2020 2020 2020 2020  py"),.          
-000168b0: 2020 5061 7468 2870 6174 6820 2f20 2272    Path(path / "r
-000168c0: 6f6f 742f 622e 7079 2229 2c0a 2020 2020  oot/b.py"),.    
-000168d0: 2020 2020 2020 2020 5061 7468 2870 6174          Path(pat
-000168e0: 6820 2f20 2272 6f6f 742f 632e 7079 2229  h / "root/c.py")
-000168f0: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
-00016900: 7468 2870 6174 6820 2f20 2272 6f6f 742f  th(path / "root/
-00016910: 6368 696c 642f 632e 7079 2229 2c0a 2020  child/c.py"),.  
-00016920: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00016930: 7468 6973 5f61 6273 203d 2054 4849 535f  this_abs = THIS_
-00016940: 4449 522e 7265 736f 6c76 6528 290a 2020  DIR.resolve().  
-00016950: 2020 2020 2020 736f 7572 6365 7320 3d20        sources = 
-00016960: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
-00016970: 2020 6365 7263 6973 2e67 656e 5f70 7974    cercis.gen_pyt
-00016980: 686f 6e5f 6669 6c65 7328 0a20 2020 2020  hon_files(.     
-00016990: 2020 2020 2020 2020 2020 2070 6174 682e             path.
-000169a0: 6974 6572 6469 7228 292c 0a20 2020 2020  iterdir(),.     
-000169b0: 2020 2020 2020 2020 2020 2074 6869 735f             this_
-000169c0: 6162 732c 0a20 2020 2020 2020 2020 2020  abs,.           
-000169d0: 2020 2020 2069 6e63 6c75 6465 2c0a 2020       include,.  
-000169e0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000169f0: 636c 7564 652c 0a20 2020 2020 2020 2020  clude,.         
-00016a00: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
-00016a10: 2020 2020 2020 2020 2020 2020 204e 6f6e               Non
-00016a20: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00016a30: 2020 2072 6570 6f72 742c 0a20 2020 2020     report,.     
-00016a40: 2020 2020 2020 2020 2020 207b 7061 7468             {path
-00016a50: 3a20 726f 6f74 5f67 6974 6967 6e6f 7265  : root_gitignore
-00016a60: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00016a70: 2020 2076 6572 626f 7365 3d46 616c 7365     verbose=False
-00016a80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016a90: 2020 7175 6965 743d 4661 6c73 652c 0a20    quiet=False,. 
-00016aa0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00016ab0: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
-00016ac0: 7373 6572 7420 736f 7274 6564 2865 7870  ssert sorted(exp
-00016ad0: 6563 7465 6429 203d 3d20 736f 7274 6564  ected) == sorted
-00016ae0: 2873 6f75 7263 6573 290a 0a20 2020 2064  (sources)..    d
-00016af0: 6566 2074 6573 745f 6e65 7374 6564 5f67  ef test_nested_g
-00016b00: 6974 6967 6e6f 7265 5f64 6972 6563 746c  itignore_directl
-00016b10: 795f 696e 5f73 6f75 7263 655f 6469 7265  y_in_source_dire
-00016b20: 6374 6f72 7928 7365 6c66 2920 2d3e 204e  ctory(self) -> N
-00016b30: 6f6e 653a 0a20 2020 2020 2020 2023 2068  one:.        # h
-00016b40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00016b50: 6d2f 7073 662f 626c 6163 6b2f 6973 7375  m/psf/black/issu
-00016b60: 6573 2f32 3539 380a 2020 2020 2020 2020  es/2598.        
-00016b70: 7061 7468 203d 2050 6174 6828 4441 5441  path = Path(DATA
-00016b80: 5f44 4952 202f 2022 6e65 7374 6564 5f67  _DIR / "nested_g
-00016b90: 6974 6967 6e6f 7265 5f74 6573 7473 2229  itignore_tests")
-00016ba0: 0a20 2020 2020 2020 2073 7263 203d 2050  .        src = P
-00016bb0: 6174 6828 7061 7468 202f 2022 726f 6f74  ath(path / "root
-00016bc0: 2220 2f20 2263 6869 6c64 2229 0a20 2020  " / "child").   
-00016bd0: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
-00016be0: 5b73 7263 202f 2022 612e 7079 222c 2073  [src / "a.py", s
-00016bf0: 7263 202f 2022 632e 7079 225d 0a20 2020  rc / "c.py"].   
-00016c00: 2020 2020 2061 7373 6572 745f 636f 6c6c       assert_coll
-00016c10: 6563 7465 645f 736f 7572 6365 7328 5b73  ected_sources([s
-00016c20: 7263 5d2c 2065 7870 6563 7465 6429 0a0a  rc], expected)..
-00016c30: 2020 2020 6465 6620 7465 7374 5f69 6e76      def test_inv
-00016c40: 616c 6964 5f67 6974 6967 6e6f 7265 2873  alid_gitignore(s
-00016c50: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00016c60: 2020 2020 2020 7061 7468 203d 2054 4849        path = THI
-00016c70: 535f 4449 5220 2f20 2264 6174 6122 202f  S_DIR / "data" /
-00016c80: 2022 696e 7661 6c69 645f 6769 7469 676e   "invalid_gitign
-00016c90: 6f72 655f 7465 7374 7322 0a20 2020 2020  ore_tests".     
-00016ca0: 2020 2065 6d70 7479 5f63 6f6e 6669 6720     empty_config 
-00016cb0: 3d20 7061 7468 202f 2022 7079 7072 6f6a  = path / "pyproj
-00016cc0: 6563 742e 746f 6d6c 220a 2020 2020 2020  ect.toml".      
-00016cd0: 2020 7265 7375 6c74 203d 2042 6c61 636b    result = Black
-00016ce0: 5275 6e6e 6572 2829 2e69 6e76 6f6b 6528  Runner().invoke(
-00016cf0: 0a20 2020 2020 2020 2020 2020 2063 6572  .            cer
-00016d00: 6369 732e 6d61 696e 2c20 5b22 2d2d 7665  cis.main, ["--ve
-00016d10: 7262 6f73 6522 2c20 222d 2d63 6f6e 6669  rbose", "--confi
-00016d20: 6722 2c20 7374 7228 656d 7074 795f 636f  g", str(empty_co
-00016d30: 6e66 6967 292c 2073 7472 2870 6174 6829  nfig), str(path)
-00016d40: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
-00016d50: 2020 2020 6173 7365 7274 2072 6573 756c      assert resul
-00016d60: 742e 6578 6974 5f63 6f64 6520 3d3d 2031  t.exit_code == 1
-00016d70: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00016d80: 7265 7375 6c74 2e73 7464 6572 725f 6279  result.stderr_by
-00016d90: 7465 7320 6973 206e 6f74 204e 6f6e 650a  tes is not None.
-00016da0: 0a20 2020 2020 2020 2067 6974 6967 6e6f  .        gitigno
-00016db0: 7265 203d 2070 6174 6820 2f20 222e 6769  re = path / ".gi
-00016dc0: 7469 676e 6f72 6522 0a20 2020 2020 2020  tignore".       
-00016dd0: 2061 7373 6572 7420 6622 436f 756c 6420   assert f"Could 
-00016de0: 6e6f 7420 7061 7273 6520 7b67 6974 6967  not parse {gitig
-00016df0: 6e6f 7265 7d22 2069 6e20 7265 7375 6c74  nore}" in result
-00016e00: 2e73 7464 6572 725f 6279 7465 732e 6465  .stderr_bytes.de
-00016e10: 636f 6465 2829 0a0a 2020 2020 6465 6620  code()..    def 
-00016e20: 7465 7374 5f69 6e76 616c 6964 5f6e 6573  test_invalid_nes
-00016e30: 7465 645f 6769 7469 676e 6f72 6528 7365  ted_gitignore(se
-00016e40: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00016e50: 2020 2020 2070 6174 6820 3d20 5448 4953       path = THIS
-00016e60: 5f44 4952 202f 2022 6461 7461 2220 2f20  _DIR / "data" / 
-00016e70: 2269 6e76 616c 6964 5f6e 6573 7465 645f  "invalid_nested_
-00016e80: 6769 7469 676e 6f72 655f 7465 7374 7322  gitignore_tests"
-00016e90: 0a20 2020 2020 2020 2065 6d70 7479 5f63  .        empty_c
-00016ea0: 6f6e 6669 6720 3d20 7061 7468 202f 2022  onfig = path / "
-00016eb0: 7079 7072 6f6a 6563 742e 746f 6d6c 220a  pyproject.toml".
-00016ec0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00016ed0: 2042 6c61 636b 5275 6e6e 6572 2829 2e69   BlackRunner().i
-00016ee0: 6e76 6f6b 6528 0a20 2020 2020 2020 2020  nvoke(.         
-00016ef0: 2020 2063 6572 6369 732e 6d61 696e 2c20     cercis.main, 
-00016f00: 5b22 2d2d 7665 7262 6f73 6522 2c20 222d  ["--verbose", "-
-00016f10: 2d63 6f6e 6669 6722 2c20 7374 7228 656d  -config", str(em
-00016f20: 7074 795f 636f 6e66 6967 292c 2073 7472  pty_config), str
-00016f30: 2870 6174 6829 5d0a 2020 2020 2020 2020  (path)].        
-00016f40: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-00016f50: 2072 6573 756c 742e 6578 6974 5f63 6f64   result.exit_cod
-00016f60: 6520 3d3d 2031 0a20 2020 2020 2020 2061  e == 1.        a
-00016f70: 7373 6572 7420 7265 7375 6c74 2e73 7464  ssert result.std
-00016f80: 6572 725f 6279 7465 7320 6973 206e 6f74  err_bytes is not
-00016f90: 204e 6f6e 650a 0a20 2020 2020 2020 2067   None..        g
-00016fa0: 6974 6967 6e6f 7265 203d 2070 6174 6820  itignore = path 
-00016fb0: 2f20 2261 2220 2f20 222e 6769 7469 676e  / "a" / ".gitign
-00016fc0: 6f72 6522 0a20 2020 2020 2020 2061 7373  ore".        ass
-00016fd0: 6572 7420 6622 436f 756c 6420 6e6f 7420  ert f"Could not 
-00016fe0: 7061 7273 6520 7b67 6974 6967 6e6f 7265  parse {gitignore
-00016ff0: 7d22 2069 6e20 7265 7375 6c74 2e73 7464  }" in result.std
-00017000: 6572 725f 6279 7465 732e 6465 636f 6465  err_bytes.decode
-00017010: 2829 0a0a 2020 2020 6465 6620 7465 7374  ()..    def test
-00017020: 5f67 6974 6967 6e6f 7265 5f74 6861 745f  _gitignore_that_
-00017030: 6967 6e6f 7265 735f 7375 6266 6f6c 6465  ignores_subfolde
-00017040: 7273 2873 656c 6629 202d 3e20 4e6f 6e65  rs(self) -> None
-00017050: 3a0a 2020 2020 2020 2020 2320 4966 2067  :.        # If g
-00017060: 6974 6967 6e6f 7265 2077 6974 6820 2a2f  itignore with */
-00017070: 2a20 6973 2069 6e20 726f 6f74 0a20 2020  * is in root.   
-00017080: 2020 2020 2072 6f6f 7420 3d20 5061 7468       root = Path
-00017090: 2844 4154 415f 4449 5220 2f20 2269 676e  (DATA_DIR / "ign
-000170a0: 6f72 655f 7375 6266 6f6c 6465 7273 5f67  ore_subfolders_g
-000170b0: 6974 6967 6e6f 7265 5f74 6573 7473 2220  itignore_tests" 
-000170c0: 2f20 2273 7562 6469 7222 290a 2020 2020  / "subdir").    
-000170d0: 2020 2020 6578 7065 6374 6564 203d 205b      expected = [
-000170e0: 726f 6f74 202f 2022 622e 7079 225d 0a20  root / "b.py"]. 
-000170f0: 2020 2020 2020 2063 7478 203d 2046 616b         ctx = Fak
-00017100: 6543 6f6e 7465 7874 2829 0a20 2020 2020  eContext().     
-00017110: 2020 2063 7478 2e6f 626a 5b22 726f 6f74     ctx.obj["root
-00017120: 225d 203d 2072 6f6f 740a 2020 2020 2020  "] = root.      
-00017130: 2020 6173 7365 7274 5f63 6f6c 6c65 6374    assert_collect
-00017140: 6564 5f73 6f75 7263 6573 285b 726f 6f74  ed_sources([root
-00017150: 5d2c 2065 7870 6563 7465 642c 2063 7478  ], expected, ctx
-00017160: 3d63 7478 290a 0a20 2020 2020 2020 2023  =ctx)..        #
-00017170: 2049 6620 2e67 6974 6967 6e6f 7265 2077   If .gitignore w
-00017180: 6974 6820 2a2f 2a20 6973 206e 6573 7465  ith */* is neste
-00017190: 640a 2020 2020 2020 2020 726f 6f74 203d  d.        root =
-000171a0: 2050 6174 6828 4441 5441 5f44 4952 202f   Path(DATA_DIR /
-000171b0: 2022 6967 6e6f 7265 5f73 7562 666f 6c64   "ignore_subfold
-000171c0: 6572 735f 6769 7469 676e 6f72 655f 7465  ers_gitignore_te
-000171d0: 7374 7322 290a 2020 2020 2020 2020 6578  sts").        ex
-000171e0: 7065 6374 6564 203d 205b 0a20 2020 2020  pected = [.     
-000171f0: 2020 2020 2020 2072 6f6f 7420 2f20 2261         root / "a
-00017200: 2e70 7922 2c0a 2020 2020 2020 2020 2020  .py",.          
-00017210: 2020 726f 6f74 202f 2022 7375 6264 6972    root / "subdir
-00017220: 2220 2f20 2262 2e70 7922 2c0a 2020 2020  " / "b.py",.    
-00017230: 2020 2020 5d0a 2020 2020 2020 2020 6374      ].        ct
-00017240: 7820 3d20 4661 6b65 436f 6e74 6578 7428  x = FakeContext(
-00017250: 290a 2020 2020 2020 2020 6374 782e 6f62  ).        ctx.ob
-00017260: 6a5b 2272 6f6f 7422 5d20 3d20 726f 6f74  j["root"] = root
-00017270: 0a20 2020 2020 2020 2061 7373 6572 745f  .        assert_
-00017280: 636f 6c6c 6563 7465 645f 736f 7572 6365  collected_source
-00017290: 7328 5b72 6f6f 745d 2c20 6578 7065 6374  s([root], expect
-000172a0: 6564 2c20 6374 783d 6374 7829 0a0a 2020  ed, ctx=ctx)..  
-000172b0: 2020 2020 2020 2320 4966 2063 6f6d 6d61        # If comma
-000172c0: 6e64 2069 7320 6578 6563 7574 6564 2066  nd is executed f
-000172d0: 726f 6d20 6f75 7465 7220 6469 720a 2020  rom outer dir.  
-000172e0: 2020 2020 2020 726f 6f74 203d 2050 6174        root = Pat
-000172f0: 6828 4441 5441 5f44 4952 202f 2022 6967  h(DATA_DIR / "ig
-00017300: 6e6f 7265 5f73 7562 666f 6c64 6572 735f  nore_subfolders_
-00017310: 6769 7469 676e 6f72 655f 7465 7374 7322  gitignore_tests"
-00017320: 290a 2020 2020 2020 2020 7461 7267 6574  ).        target
-00017330: 203d 2072 6f6f 7420 2f20 2273 7562 6469   = root / "subdi
-00017340: 7222 0a20 2020 2020 2020 2065 7870 6563  r".        expec
-00017350: 7465 6420 3d20 5b74 6172 6765 7420 2f20  ted = [target / 
-00017360: 2262 2e70 7922 5d0a 2020 2020 2020 2020  "b.py"].        
-00017370: 6374 7820 3d20 4661 6b65 436f 6e74 6578  ctx = FakeContex
-00017380: 7428 290a 2020 2020 2020 2020 6374 782e  t().        ctx.
-00017390: 6f62 6a5b 2272 6f6f 7422 5d20 3d20 726f  obj["root"] = ro
-000173a0: 6f74 0a20 2020 2020 2020 2061 7373 6572  ot.        asser
-000173b0: 745f 636f 6c6c 6563 7465 645f 736f 7572  t_collected_sour
-000173c0: 6365 7328 5b74 6172 6765 745d 2c20 6578  ces([target], ex
-000173d0: 7065 6374 6564 2c20 6374 783d 6374 7829  pected, ctx=ctx)
-000173e0: 0a0a 2020 2020 6465 6620 7465 7374 5f65  ..    def test_e
-000173f0: 6d70 7479 5f69 6e63 6c75 6465 2873 656c  mpty_include(sel
-00017400: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00017410: 2020 2020 7061 7468 203d 2044 4154 415f      path = DATA_
-00017420: 4449 5220 2f20 2269 6e63 6c75 6465 5f65  DIR / "include_e
-00017430: 7863 6c75 6465 5f74 6573 7473 220a 2020  xclude_tests".  
-00017440: 2020 2020 2020 7372 6320 3d20 5b70 6174        src = [pat
-00017450: 685d 0a20 2020 2020 2020 2065 7870 6563  h].        expec
-00017460: 7465 6420 3d20 5b0a 2020 2020 2020 2020  ted = [.        
-00017470: 2020 2020 5061 7468 2870 6174 6820 2f20      Path(path / 
-00017480: 2262 2f65 7863 6c75 6465 2f61 2e70 6965  "b/exclude/a.pie
-00017490: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-000174a0: 5061 7468 2870 6174 6820 2f20 2262 2f65  Path(path / "b/e
-000174b0: 7863 6c75 6465 2f61 2e70 7922 292c 0a20  xclude/a.py"),. 
-000174c0: 2020 2020 2020 2020 2020 2050 6174 6828             Path(
-000174d0: 7061 7468 202f 2022 622f 6578 636c 7564  path / "b/exclud
-000174e0: 652f 612e 7079 6922 292c 0a20 2020 2020  e/a.pyi"),.     
-000174f0: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
-00017500: 202f 2022 622f 646f 6e74 5f65 7863 6c75   / "b/dont_exclu
-00017510: 6465 2f61 2e70 6965 2229 2c0a 2020 2020  de/a.pie"),.    
-00017520: 2020 2020 2020 2020 5061 7468 2870 6174          Path(pat
-00017530: 6820 2f20 2262 2f64 6f6e 745f 6578 636c  h / "b/dont_excl
-00017540: 7564 652f 612e 7079 2229 2c0a 2020 2020  ude/a.py"),.    
-00017550: 2020 2020 2020 2020 5061 7468 2870 6174          Path(pat
-00017560: 6820 2f20 2262 2f64 6f6e 745f 6578 636c  h / "b/dont_excl
-00017570: 7564 652f 612e 7079 6922 292c 0a20 2020  ude/a.pyi"),.   
-00017580: 2020 2020 2020 2020 2050 6174 6828 7061           Path(pa
-00017590: 7468 202f 2022 622f 2e64 6566 696e 6974  th / "b/.definit
-000175a0: 656c 795f 6578 636c 7564 652f 612e 7069  ely_exclude/a.pi
-000175b0: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
-000175c0: 2050 6174 6828 7061 7468 202f 2022 622f   Path(path / "b/
-000175d0: 2e64 6566 696e 6974 656c 795f 6578 636c  .definitely_excl
-000175e0: 7564 652f 612e 7079 2229 2c0a 2020 2020  ude/a.py"),.    
-000175f0: 2020 2020 2020 2020 5061 7468 2870 6174          Path(pat
-00017600: 6820 2f20 2262 2f2e 6465 6669 6e69 7465  h / "b/.definite
-00017610: 6c79 5f65 7863 6c75 6465 2f61 2e70 7969  ly_exclude/a.pyi
-00017620: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00017630: 5061 7468 2870 6174 6820 2f20 222e 6769  Path(path / ".gi
-00017640: 7469 676e 6f72 6522 292c 0a20 2020 2020  tignore"),.     
-00017650: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
-00017660: 202f 2022 7079 7072 6f6a 6563 742e 746f   / "pyproject.to
-00017670: 6d6c 2229 2c0a 2020 2020 2020 2020 5d0a  ml"),.        ].
-00017680: 2020 2020 2020 2020 2320 5365 7474 696e          # Settin
-00017690: 6720 6578 636c 7564 6520 6578 706c 6963  g exclude explic
-000176a0: 6974 6c79 2074 6f20 616e 2065 6d70 7479  itly to an empty
-000176b0: 2073 7472 696e 6720 746f 2062 6c6f 636b   string to block
-000176c0: 202e 6769 7469 676e 6f72 6520 7573 6167   .gitignore usag
-000176d0: 652e 0a20 2020 2020 2020 2061 7373 6572  e..        asser
-000176e0: 745f 636f 6c6c 6563 7465 645f 736f 7572  t_collected_sour
-000176f0: 6365 7328 7372 632c 2065 7870 6563 7465  ces(src, expecte
-00017700: 642c 2069 6e63 6c75 6465 3d22 222c 2065  d, include="", e
-00017710: 7863 6c75 6465 3d22 2229 0a0a 2020 2020  xclude="")..    
-00017720: 6465 6620 7465 7374 5f65 7874 656e 645f  def test_extend_
-00017730: 6578 636c 7564 6528 7365 6c66 2920 2d3e  exclude(self) ->
-00017740: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00017750: 6174 6820 3d20 4441 5441 5f44 4952 202f  ath = DATA_DIR /
-00017760: 2022 696e 636c 7564 655f 6578 636c 7564   "include_exclud
-00017770: 655f 7465 7374 7322 0a20 2020 2020 2020  e_tests".       
-00017780: 2073 7263 203d 205b 7061 7468 5d0a 2020   src = [path].  
-00017790: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
-000177a0: 205b 0a20 2020 2020 2020 2020 2020 2050   [.            P
-000177b0: 6174 6828 7061 7468 202f 2022 622f 6578  ath(path / "b/ex
-000177c0: 636c 7564 652f 612e 7079 2229 2c0a 2020  clude/a.py"),.  
-000177d0: 2020 2020 2020 2020 2020 5061 7468 2870            Path(p
-000177e0: 6174 6820 2f20 2262 2f64 6f6e 745f 6578  ath / "b/dont_ex
-000177f0: 636c 7564 652f 612e 7079 2229 2c0a 2020  clude/a.py"),.  
-00017800: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00017810: 6173 7365 7274 5f63 6f6c 6c65 6374 6564  assert_collected
-00017820: 5f73 6f75 7263 6573 280a 2020 2020 2020  _sources(.      
-00017830: 2020 2020 2020 7372 632c 2065 7870 6563        src, expec
-00017840: 7465 642c 2065 7863 6c75 6465 3d72 225c  ted, exclude=r"\
-00017850: 2e70 7969 2422 2c20 6578 7465 6e64 5f65  .pyi$", extend_e
-00017860: 7863 6c75 6465 3d72 225c 2e64 6566 696e  xclude=r"\.defin
-00017870: 6974 656c 795f 6578 636c 7564 6522 0a20  itely_exclude". 
-00017880: 2020 2020 2020 2029 0a0a 2020 2020 4070         )..    @p
-00017890: 7974 6573 742e 6d61 726b 2e69 6e63 6f6d  ytest.mark.incom
-000178a0: 7061 7469 626c 655f 7769 7468 5f6d 7970  patible_with_myp
-000178b0: 7963 0a20 2020 2064 6566 2074 6573 745f  yc.    def test_
-000178c0: 7379 6d6c 696e 6b5f 6f75 745f 6f66 5f72  symlink_out_of_r
-000178d0: 6f6f 745f 6469 7265 6374 6f72 7928 7365  oot_directory(se
-000178e0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-000178f0: 2020 2020 2070 6174 6820 3d20 4d61 6769       path = Magi
-00017900: 634d 6f63 6b28 290a 2020 2020 2020 2020  cMock().        
-00017910: 726f 6f74 203d 2054 4849 535f 4449 522e  root = THIS_DIR.
-00017920: 7265 736f 6c76 6528 290a 2020 2020 2020  resolve().      
-00017930: 2020 6368 696c 6420 3d20 4d61 6769 634d    child = MagicM
-00017940: 6f63 6b28 290a 2020 2020 2020 2020 696e  ock().        in
-00017950: 636c 7564 6520 3d20 7265 2e63 6f6d 7069  clude = re.compi
-00017960: 6c65 2863 6572 6369 732e 4445 4641 554c  le(cercis.DEFAUL
-00017970: 545f 494e 434c 5544 4553 290a 2020 2020  T_INCLUDES).    
-00017980: 2020 2020 6578 636c 7564 6520 3d20 7265      exclude = re
-00017990: 2e63 6f6d 7069 6c65 2863 6572 6369 732e  .compile(cercis.
-000179a0: 4445 4641 554c 545f 4558 434c 5544 4553  DEFAULT_EXCLUDES
-000179b0: 290a 2020 2020 2020 2020 7265 706f 7274  ).        report
-000179c0: 203d 2063 6572 6369 732e 5265 706f 7274   = cercis.Report
-000179d0: 2829 0a20 2020 2020 2020 2067 6974 6967  ().        gitig
-000179e0: 6e6f 7265 203d 2050 6174 6853 7065 632e  nore = PathSpec.
-000179f0: 6672 6f6d 5f6c 696e 6573 2822 6769 7477  from_lines("gitw
-00017a00: 696c 646d 6174 6368 222c 205b 5d29 0a20  ildmatch", []). 
-00017a10: 2020 2020 2020 2023 2060 6368 696c 6460         # `child`
-00017a20: 2073 686f 756c 6420 6265 6861 7665 206c   should behave l
-00017a30: 696b 6520 6120 7379 6d6c 696e 6b20 7768  ike a symlink wh
-00017a40: 6963 6820 7265 736f 6c76 6564 2070 6174  ich resolved pat
-00017a50: 6820 6973 2063 6c65 6172 6c79 0a20 2020  h is clearly.   
-00017a60: 2020 2020 2023 206f 7574 7369 6465 206f       # outside o
-00017a70: 6620 7468 6520 6072 6f6f 7460 2064 6972  f the `root` dir
-00017a80: 6563 746f 7279 2e0a 2020 2020 2020 2020  ectory..        
-00017a90: 7061 7468 2e69 7465 7264 6972 2e72 6574  path.iterdir.ret
-00017aa0: 7572 6e5f 7661 6c75 6520 3d20 5b63 6869  urn_value = [chi
-00017ab0: 6c64 5d0a 2020 2020 2020 2020 6368 696c  ld].        chil
-00017ac0: 642e 7265 736f 6c76 652e 7265 7475 726e  d.resolve.return
-00017ad0: 5f76 616c 7565 203d 2050 6174 6828 222f  _value = Path("/
-00017ae0: 612f 622f 6322 290a 2020 2020 2020 2020  a/b/c").        
-00017af0: 6368 696c 642e 6173 5f70 6f73 6978 2e72  child.as_posix.r
-00017b00: 6574 7572 6e5f 7661 6c75 6520 3d20 222f  eturn_value = "/
-00017b10: 612f 622f 6322 0a20 2020 2020 2020 2074  a/b/c".        t
-00017b20: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00017b30: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
-00017b40: 2020 2020 2020 6365 7263 6973 2e67 656e        cercis.gen
-00017b50: 5f70 7974 686f 6e5f 6669 6c65 7328 0a20  _python_files(. 
-00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b70: 2020 2070 6174 682e 6974 6572 6469 7228     path.iterdir(
-00017b80: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00017b90: 2020 2020 2020 2072 6f6f 742c 0a20 2020         root,.   
-00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bb0: 2069 6e63 6c75 6465 2c0a 2020 2020 2020   include,.      
-00017bc0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00017bd0: 636c 7564 652c 0a20 2020 2020 2020 2020  clude,.         
-00017be0: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
-00017bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c00: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
-00017c10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017c20: 6570 6f72 742c 0a20 2020 2020 2020 2020  eport,.         
-00017c30: 2020 2020 2020 2020 2020 207b 7061 7468             {path
-00017c40: 3a20 6769 7469 676e 6f72 657d 2c0a 2020  : gitignore},.  
-00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c60: 2020 7665 7262 6f73 653d 4661 6c73 652c    verbose=False,
-00017c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c80: 2020 2020 2071 7569 6574 3d46 616c 7365       quiet=False
-00017c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017ca0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00017cb0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00017cc0: 2056 616c 7565 4572 726f 7220 6173 2076   ValueError as v
-00017cd0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00017ce0: 7974 6573 742e 6661 696c 2866 2260 6765  ytest.fail(f"`ge
-00017cf0: 745f 7079 7468 6f6e 5f66 696c 6573 5f69  t_python_files_i
-00017d00: 6e5f 6469 7228 2960 2066 6169 6c65 643a  n_dir()` failed:
-00017d10: 207b 7665 7d22 290a 2020 2020 2020 2020   {ve}").        
-00017d20: 7061 7468 2e69 7465 7264 6972 2e61 7373  path.iterdir.ass
-00017d30: 6572 745f 6361 6c6c 6564 5f6f 6e63 6528  ert_called_once(
-00017d40: 290a 2020 2020 2020 2020 6368 696c 642e  ).        child.
-00017d50: 7265 736f 6c76 652e 6173 7365 7274 5f63  resolve.assert_c
-00017d60: 616c 6c65 645f 6f6e 6365 2829 0a0a 2020  alled_once()..  
-00017d70: 2020 4070 6174 6368 2822 6365 7263 6973    @patch("cercis
-00017d80: 2e66 696e 645f 7072 6f6a 6563 745f 726f  .find_project_ro
-00017d90: 6f74 222c 206c 616d 6264 6120 2a61 7267  ot", lambda *arg
-00017da0: 733a 2028 5448 4953 5f44 4952 2e72 6573  s: (THIS_DIR.res
-00017db0: 6f6c 7665 2829 2c20 4e6f 6e65 2929 0a20  olve(), None)). 
-00017dc0: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
-00017dd0: 736f 7572 6365 735f 7769 7468 5f73 7464  sources_with_std
-00017de0: 696e 2873 656c 6629 202d 3e20 4e6f 6e65  in(self) -> None
-00017df0: 3a0a 2020 2020 2020 2020 7372 6320 3d20  :.        src = 
-00017e00: 5b22 2d22 5d0a 2020 2020 2020 2020 6578  ["-"].        ex
-00017e10: 7065 6374 6564 203d 205b 222d 225d 0a20  pected = ["-"]. 
-00017e20: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
-00017e30: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
-00017e40: 7372 632c 2065 7870 6563 7465 642c 2069  src, expected, i
-00017e50: 6e63 6c75 6465 3d22 222c 2065 7863 6c75  nclude="", exclu
-00017e60: 6465 3d72 222f 6578 636c 7564 652f 7c61  de=r"/exclude/|a
-00017e70: 5c2e 7079 2229 0a0a 2020 2020 4070 6174  \.py")..    @pat
-00017e80: 6368 2822 6365 7263 6973 2e66 696e 645f  ch("cercis.find_
-00017e90: 7072 6f6a 6563 745f 726f 6f74 222c 206c  project_root", l
-00017ea0: 616d 6264 6120 2a61 7267 733a 2028 5448  ambda *args: (TH
-00017eb0: 4953 5f44 4952 2e72 6573 6f6c 7665 2829  IS_DIR.resolve()
-00017ec0: 2c20 4e6f 6e65 2929 0a20 2020 2064 6566  , None)).    def
-00017ed0: 2074 6573 745f 6765 745f 736f 7572 6365   test_get_source
-00017ee0: 735f 7769 7468 5f73 7464 696e 5f66 696c  s_with_stdin_fil
-00017ef0: 656e 616d 6528 7365 6c66 2920 2d3e 204e  ename(self) -> N
-00017f00: 6f6e 653a 0a20 2020 2020 2020 2073 7263  one:.        src
-00017f10: 203d 205b 222d 225d 0a20 2020 2020 2020   = ["-"].       
-00017f20: 2073 7464 696e 5f66 696c 656e 616d 6520   stdin_filename 
-00017f30: 3d20 7374 7228 5448 4953 5f44 4952 202f  = str(THIS_DIR /
-00017f40: 2022 6461 7461 2f63 6f6c 6c65 6374 696f   "data/collectio
-00017f50: 6e73 2e70 7922 290a 2020 2020 2020 2020  ns.py").        
-00017f60: 6578 7065 6374 6564 203d 205b 6622 5f5f  expected = [f"__
-00017f70: 424c 4143 4b5f 5354 4449 4e5f 4649 4c45  BLACK_STDIN_FILE
-00017f80: 4e41 4d45 5f5f 7b73 7464 696e 5f66 696c  NAME__{stdin_fil
-00017f90: 656e 616d 657d 225d 0a20 2020 2020 2020  ename}"].       
-00017fa0: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
-00017fb0: 645f 736f 7572 6365 7328 0a20 2020 2020  d_sources(.     
-00017fc0: 2020 2020 2020 2073 7263 2c0a 2020 2020         src,.    
-00017fd0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00017fe0: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
-00017ff0: 636c 7564 653d 7222 2f65 7863 6c75 6465  clude=r"/exclude
-00018000: 2f61 5c2e 7079 222c 0a20 2020 2020 2020  /a\.py",.       
-00018010: 2020 2020 2073 7464 696e 5f66 696c 656e       stdin_filen
-00018020: 616d 653d 7374 6469 6e5f 6669 6c65 6e61  ame=stdin_filena
-00018030: 6d65 2c0a 2020 2020 2020 2020 290a 0a20  me,.        ).. 
-00018040: 2020 2040 7061 7463 6828 2263 6572 6369     @patch("cerci
-00018050: 732e 6669 6e64 5f70 726f 6a65 6374 5f72  s.find_project_r
-00018060: 6f6f 7422 2c20 6c61 6d62 6461 202a 6172  oot", lambda *ar
-00018070: 6773 3a20 2854 4849 535f 4449 522e 7265  gs: (THIS_DIR.re
-00018080: 736f 6c76 6528 292c 204e 6f6e 6529 290a  solve(), None)).
-00018090: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
-000180a0: 5f73 6f75 7263 6573 5f77 6974 685f 7374  _sources_with_st
-000180b0: 6469 6e5f 6669 6c65 6e61 6d65 5f61 6e64  din_filename_and
-000180c0: 5f65 7863 6c75 6465 2873 656c 6629 202d  _exclude(self) -
-000180d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000180e0: 2320 4578 636c 7564 6520 7368 6f75 6c64  # Exclude should
-000180f0: 6e27 7420 6578 636c 7564 6520 7374 6469  n't exclude stdi
-00018100: 6e5f 6669 6c65 6e61 6d65 2073 696e 6365  n_filename since
-00018110: 2069 7420 6973 206d 696d 6963 6b69 6e67   it is mimicking
-00018120: 2074 6865 0a20 2020 2020 2020 2023 2066   the.        # f
-00018130: 696c 6520 6265 696e 6720 7061 7373 6564  ile being passed
-00018140: 2064 6972 6563 746c 792e 2054 6869 7320   directly. This 
-00018150: 6973 2074 6865 2073 616d 6520 6173 0a20  is the same as. 
-00018160: 2020 2020 2020 2023 2074 6573 745f 6578         # test_ex
-00018170: 636c 7564 655f 666f 725f 6973 7375 655f  clude_for_issue_
-00018180: 3135 3732 0a20 2020 2020 2020 2070 6174  1572.        pat
-00018190: 6820 3d20 4441 5441 5f44 4952 202f 2022  h = DATA_DIR / "
-000181a0: 696e 636c 7564 655f 6578 636c 7564 655f  include_exclude_
-000181b0: 7465 7374 7322 0a20 2020 2020 2020 2073  tests".        s
-000181c0: 7263 203d 205b 222d 225d 0a20 2020 2020  rc = ["-"].     
-000181d0: 2020 2073 7464 696e 5f66 696c 656e 616d     stdin_filenam
-000181e0: 6520 3d20 7374 7228 7061 7468 202f 2022  e = str(path / "
-000181f0: 622f 6578 636c 7564 652f 612e 7079 2229  b/exclude/a.py")
-00018200: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-00018210: 6420 3d20 5b66 225f 5f42 4c41 434b 5f53  d = [f"__BLACK_S
-00018220: 5444 494e 5f46 494c 454e 414d 455f 5f7b  TDIN_FILENAME__{
-00018230: 7374 6469 6e5f 6669 6c65 6e61 6d65 7d22  stdin_filename}"
-00018240: 5d0a 2020 2020 2020 2020 6173 7365 7274  ].        assert
-00018250: 5f63 6f6c 6c65 6374 6564 5f73 6f75 7263  _collected_sourc
-00018260: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-00018270: 7372 632c 0a20 2020 2020 2020 2020 2020  src,.           
-00018280: 2065 7870 6563 7465 642c 0a20 2020 2020   expected,.     
-00018290: 2020 2020 2020 2065 7863 6c75 6465 3d72         exclude=r
-000182a0: 222f 6578 636c 7564 652f 7c61 5c2e 7079  "/exclude/|a\.py
-000182b0: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-000182c0: 7464 696e 5f66 696c 656e 616d 653d 7374  tdin_filename=st
-000182d0: 6469 6e5f 6669 6c65 6e61 6d65 2c0a 2020  din_filename,.  
-000182e0: 2020 2020 2020 290a 0a20 2020 2040 7061        )..    @pa
-000182f0: 7463 6828 2263 6572 6369 732e 6669 6e64  tch("cercis.find
-00018300: 5f70 726f 6a65 6374 5f72 6f6f 7422 2c20  _project_root", 
-00018310: 6c61 6d62 6461 202a 6172 6773 3a20 2854  lambda *args: (T
-00018320: 4849 535f 4449 522e 7265 736f 6c76 6528  HIS_DIR.resolve(
-00018330: 292c 204e 6f6e 6529 290a 2020 2020 6465  ), None)).    de
-00018340: 6620 7465 7374 5f67 6574 5f73 6f75 7263  f test_get_sourc
-00018350: 6573 5f77 6974 685f 7374 6469 6e5f 6669  es_with_stdin_fi
-00018360: 6c65 6e61 6d65 5f61 6e64 5f65 7874 656e  lename_and_exten
-00018370: 645f 6578 636c 7564 6528 7365 6c66 2920  d_exclude(self) 
-00018380: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00018390: 2023 2045 7874 656e 6420 6578 636c 7564   # Extend exclud
-000183a0: 6520 7368 6f75 6c64 6e27 7420 6578 636c  e shouldn't excl
-000183b0: 7564 6520 7374 6469 6e5f 6669 6c65 6e61  ude stdin_filena
-000183c0: 6d65 2073 696e 6365 2069 7420 6973 206d  me since it is m
-000183d0: 696d 6963 6b69 6e67 2074 6865 0a20 2020  imicking the.   
-000183e0: 2020 2020 2023 2066 696c 6520 6265 696e       # file bein
-000183f0: 6720 7061 7373 6564 2064 6972 6563 746c  g passed directl
-00018400: 792e 2054 6869 7320 6973 2074 6865 2073  y. This is the s
-00018410: 616d 6520 6173 0a20 2020 2020 2020 2023  ame as.        #
-00018420: 2074 6573 745f 6578 636c 7564 655f 666f   test_exclude_fo
-00018430: 725f 6973 7375 655f 3135 3732 0a20 2020  r_issue_1572.   
-00018440: 2020 2020 2073 7263 203d 205b 222d 225d       src = ["-"]
-00018450: 0a20 2020 2020 2020 2070 6174 6820 3d20  .        path = 
-00018460: 5448 4953 5f44 4952 202f 2022 6461 7461  THIS_DIR / "data
-00018470: 2220 2f20 2269 6e63 6c75 6465 5f65 7863  " / "include_exc
-00018480: 6c75 6465 5f74 6573 7473 220a 2020 2020  lude_tests".    
-00018490: 2020 2020 7374 6469 6e5f 6669 6c65 6e61      stdin_filena
-000184a0: 6d65 203d 2073 7472 2870 6174 6820 2f20  me = str(path / 
-000184b0: 2262 2f65 7863 6c75 6465 2f61 2e70 7922  "b/exclude/a.py"
-000184c0: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
-000184d0: 6564 203d 205b 6622 5f5f 424c 4143 4b5f  ed = [f"__BLACK_
-000184e0: 5354 4449 4e5f 4649 4c45 4e41 4d45 5f5f  STDIN_FILENAME__
-000184f0: 7b73 7464 696e 5f66 696c 656e 616d 657d  {stdin_filename}
-00018500: 225d 0a20 2020 2020 2020 2061 7373 6572  "].        asser
-00018510: 745f 636f 6c6c 6563 7465 645f 736f 7572  t_collected_sour
-00018520: 6365 7328 0a20 2020 2020 2020 2020 2020  ces(.           
-00018530: 2073 7263 2c0a 2020 2020 2020 2020 2020   src,.          
-00018540: 2020 6578 7065 6374 6564 2c0a 2020 2020    expected,.    
-00018550: 2020 2020 2020 2020 6578 7465 6e64 5f65          extend_e
-00018560: 7863 6c75 6465 3d72 222f 6578 636c 7564  xclude=r"/exclud
-00018570: 652f 7c61 5c2e 7079 222c 0a20 2020 2020  e/|a\.py",.     
-00018580: 2020 2020 2020 2073 7464 696e 5f66 696c         stdin_fil
-00018590: 656e 616d 653d 7374 6469 6e5f 6669 6c65  ename=stdin_file
-000185a0: 6e61 6d65 2c0a 2020 2020 2020 2020 290a  name,.        ).
-000185b0: 0a20 2020 2040 7061 7463 6828 2263 6572  .    @patch("cer
-000185c0: 6369 732e 6669 6e64 5f70 726f 6a65 6374  cis.find_project
-000185d0: 5f72 6f6f 7422 2c20 6c61 6d62 6461 202a  _root", lambda *
-000185e0: 6172 6773 3a20 2854 4849 535f 4449 522e  args: (THIS_DIR.
-000185f0: 7265 736f 6c76 6528 292c 204e 6f6e 6529  resolve(), None)
-00018600: 290a 2020 2020 6465 6620 7465 7374 5f67  ).    def test_g
-00018610: 6574 5f73 6f75 7263 6573 5f77 6974 685f  et_sources_with_
-00018620: 7374 6469 6e5f 6669 6c65 6e61 6d65 5f61  stdin_filename_a
-00018630: 6e64 5f66 6f72 6365 5f65 7863 6c75 6465  nd_force_exclude
-00018640: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00018650: 2020 2020 2020 2020 2320 466f 7263 6520          # Force 
-00018660: 6578 636c 7564 6520 7368 6f75 6c64 2065  exclude should e
-00018670: 7863 6c75 6465 2074 6865 2066 696c 6520  xclude the file 
-00018680: 7768 656e 2070 6173 7369 6e67 2069 7420  when passing it 
-00018690: 7468 726f 7567 680a 2020 2020 2020 2020  through.        
-000186a0: 2320 7374 6469 6e5f 6669 6c65 6e61 6d65  # stdin_filename
-000186b0: 0a20 2020 2020 2020 2070 6174 6820 3d20  .        path = 
-000186c0: 5448 4953 5f44 4952 202f 2022 6461 7461  THIS_DIR / "data
-000186d0: 2220 2f20 2269 6e63 6c75 6465 5f65 7863  " / "include_exc
-000186e0: 6c75 6465 5f74 6573 7473 220a 2020 2020  lude_tests".    
-000186f0: 2020 2020 7374 6469 6e5f 6669 6c65 6e61      stdin_filena
-00018700: 6d65 203d 2073 7472 2870 6174 6820 2f20  me = str(path / 
-00018710: 2262 2f65 7863 6c75 6465 2f61 2e70 7922  "b/exclude/a.py"
-00018720: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-00018730: 5f63 6f6c 6c65 6374 6564 5f73 6f75 7263  _collected_sourc
-00018740: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-00018750: 7372 633d 5b22 2d22 5d2c 0a20 2020 2020  src=["-"],.     
-00018760: 2020 2020 2020 2065 7870 6563 7465 643d         expected=
-00018770: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-00018780: 666f 7263 655f 6578 636c 7564 653d 7222  force_exclude=r"
-00018790: 2f65 7863 6c75 6465 2f7c 615c 2e70 7922  /exclude/|a\.py"
-000187a0: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
-000187b0: 6469 6e5f 6669 6c65 6e61 6d65 3d73 7464  din_filename=std
-000187c0: 696e 5f66 696c 656e 616d 652c 0a20 2020  in_filename,.   
-000187d0: 2020 2020 2029 0a0a 0a74 7279 3a0a 2020       )...try:.  
-000187e0: 2020 7769 7468 206f 7065 6e28 6365 7263    with open(cerc
-000187f0: 6973 2e5f 5f66 696c 655f 5f2c 2022 7222  is.__file__, "r"
-00018800: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00018810: 3822 2920 6173 205f 6266 3a0a 2020 2020  8") as _bf:.    
-00018820: 2020 2020 626c 6163 6b5f 736f 7572 6365      black_source
-00018830: 5f6c 696e 6573 203d 205f 6266 2e72 6561  _lines = _bf.rea
-00018840: 646c 696e 6573 2829 0a65 7863 6570 7420  dlines().except 
-00018850: 556e 6963 6f64 6544 6563 6f64 6545 7272  UnicodeDecodeErr
-00018860: 6f72 3a0a 2020 2020 6966 206e 6f74 2063  or:.    if not c
-00018870: 6572 6369 732e 434f 4d50 494c 4544 3a0a  ercis.COMPILED:.
-00018880: 2020 2020 2020 2020 7261 6973 650a 0a0a          raise...
-00018890: 6465 6620 7472 6163 6566 756e 6328 0a20  def tracefunc(. 
-000188a0: 2020 2020 2020 2066 7261 6d65 3a20 7479         frame: ty
-000188b0: 7065 732e 4672 616d 6554 7970 652c 2065  pes.FrameType, e
-000188c0: 7665 6e74 3a20 7374 722c 2061 7267 3a20  vent: str, arg: 
-000188d0: 416e 790a 2920 2d3e 2043 616c 6c61 626c  Any.) -> Callabl
-000188e0: 655b 5b74 7970 6573 2e46 7261 6d65 5479  e[[types.FrameTy
-000188f0: 7065 2c20 7374 722c 2041 6e79 5d2c 2041  pe, str, Any], A
-00018900: 6e79 5d3a 0a20 2020 2022 2222 5368 6f77  ny]:.    """Show
-00018910: 2066 756e 6374 696f 6e20 6361 6c6c 7320   function calls 
-00018920: 6066 726f 6d20 6365 7263 6973 2f5f 5f69  `from cercis/__i
-00018930: 6e69 745f 5f2e 7079 6020 6173 2074 6865  nit__.py` as the
-00018940: 7920 6861 7070 656e 2e0a 0a20 2020 2052  y happen...    R
-00018950: 6567 6973 7465 7220 7468 6973 2077 6974  egister this wit
-00018960: 6820 6073 7973 2e73 6574 7472 6163 6528  h `sys.settrace(
-00018970: 2960 2069 6e20 6120 7465 7374 2079 6f75  )` in a test you
-00018980: 2772 6520 6465 6275 6767 696e 672e 0a20  're debugging.. 
-00018990: 2020 2022 2222 0a20 2020 2069 6620 6576     """.    if ev
-000189a0: 656e 7420 213d 2022 6361 6c6c 223a 0a20  ent != "call":. 
-000189b0: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-000189c0: 6163 6566 756e 630a 0a20 2020 2073 7461  acefunc..    sta
-000189d0: 636b 203d 206c 656e 2869 6e73 7065 6374  ck = len(inspect
-000189e0: 2e73 7461 636b 2829 2920 2d20 3139 0a20  .stack()) - 19. 
-000189f0: 2020 2073 7461 636b 202a 3d20 320a 2020     stack *= 2.  
-00018a00: 2020 6669 6c65 6e61 6d65 203d 2066 7261    filename = fra
-00018a10: 6d65 2e66 5f63 6f64 652e 636f 5f66 696c  me.f_code.co_fil
-00018a20: 656e 616d 650a 2020 2020 6c69 6e65 6e6f  ename.    lineno
-00018a30: 203d 2066 7261 6d65 2e66 5f6c 696e 656e   = frame.f_linen
-00018a40: 6f0a 2020 2020 6675 6e63 5f73 6967 5f6c  o.    func_sig_l
-00018a50: 696e 656e 6f20 3d20 6c69 6e65 6e6f 202d  ineno = lineno -
-00018a60: 2031 0a20 2020 2066 756e 636e 616d 6520   1.    funcname 
-00018a70: 3d20 626c 6163 6b5f 736f 7572 6365 5f6c  = black_source_l
-00018a80: 696e 6573 5b66 756e 635f 7369 675f 6c69  ines[func_sig_li
-00018a90: 6e65 6e6f 5d2e 7374 7269 7028 290a 2020  neno].strip().  
-00018aa0: 2020 7768 696c 6520 6675 6e63 6e61 6d65    while funcname
-00018ab0: 2e73 7461 7274 7377 6974 6828 2240 2229  .startswith("@")
-00018ac0: 3a0a 2020 2020 2020 2020 6675 6e63 5f73  :.        func_s
-00018ad0: 6967 5f6c 696e 656e 6f20 2b3d 2031 0a20  ig_lineno += 1. 
-00018ae0: 2020 2020 2020 2066 756e 636e 616d 6520         funcname 
-00018af0: 3d20 626c 6163 6b5f 736f 7572 6365 5f6c  = black_source_l
-00018b00: 696e 6573 5b66 756e 635f 7369 675f 6c69  ines[func_sig_li
-00018b10: 6e65 6e6f 5d2e 7374 7269 7028 290a 2020  neno].strip().  
-00018b20: 2020 6966 2022 6365 7263 6973 2f5f 5f69    if "cercis/__i
-00018b30: 6e69 745f 5f2e 7079 2220 696e 2066 696c  nit__.py" in fil
-00018b40: 656e 616d 653a 0a20 2020 2020 2020 2070  ename:.        p
-00018b50: 7269 6e74 2866 227b 2720 2720 2a20 7374  rint(f"{' ' * st
-00018b60: 6163 6b7d 7b6c 696e 656e 6f7d 3a7b 6675  ack}{lineno}:{fu
-00018b70: 6e63 6e61 6d65 7d22 290a 2020 2020 7265  ncname}").    re
-00018b80: 7475 726e 2074 7261 6365 6675 6e63 0a    turn tracefunc.
+0000eff0: 7570 6461 7465 645f 636f 6e74 656e 7473  updated_contents
+0000f000: 3a20 6279 7465 7320 3d20 7465 7374 5f66  : bytes = test_f
+0000f010: 696c 652e 7265 6164 5f62 7974 6573 2829  ile.read_bytes()
+0000f020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f030: 2073 656c 662e 6173 7365 7274 496e 286e   self.assertIn(n
+0000f040: 6c2e 656e 636f 6465 2829 2c20 7570 6461  l.encode(), upda
+0000f050: 7465 645f 636f 6e74 656e 7473 290a 2020  ted_contents).  
+0000f060: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000f070: 206e 6c20 3d3d 2022 5c6e 223a 0a20 2020   nl == "\n":.   
+0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f090: 2073 656c 662e 6173 7365 7274 4e6f 7449   self.assertNotI
+0000f0a0: 6e28 6222 5c72 5c6e 222c 2075 7064 6174  n(b"\r\n", updat
+0000f0b0: 6564 5f63 6f6e 7465 6e74 7329 0a0a 2020  ed_contents)..  
+0000f0c0: 2020 6465 6620 7465 7374 5f70 7265 7365    def test_prese
+0000f0d0: 7276 6573 5f6c 696e 655f 656e 6469 6e67  rves_line_ending
+0000f0e0: 735f 7669 615f 7374 6469 6e28 7365 6c66  s_via_stdin(self
+0000f0f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000f100: 2020 2066 6f72 206e 6c20 696e 205b 225c     for nl in ["\
+0000f110: 6e22 2c20 225c 725c 6e22 5d3a 0a20 2020  n", "\r\n"]:.   
+0000f120: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+0000f130: 7320 3d20 6e6c 2e6a 6f69 6e28 5b22 6465  s = nl.join(["de
+0000f140: 6620 6628 2020 293a 222c 2022 2020 2020  f f(  ):", "    
+0000f150: 7061 7373 225d 290a 2020 2020 2020 2020  pass"]).        
+0000f160: 2020 2020 7275 6e6e 6572 203d 2042 6c61      runner = Bla
+0000f170: 636b 5275 6e6e 6572 2829 0a20 2020 2020  ckRunner().     
+0000f180: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000f190: 7275 6e6e 6572 2e69 6e76 6f6b 6528 0a20  runner.invoke(. 
+0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f1b0: 6572 6369 732e 6d61 696e 2c20 5b22 2d22  ercis.main, ["-"
+0000f1c0: 2c20 222d 2d66 6173 7422 5d2c 2069 6e70  , "--fast"], inp
+0000f1d0: 7574 3d42 7974 6573 494f 2863 6f6e 7465  ut=BytesIO(conte
+0000f1e0: 6e74 732e 656e 636f 6465 2822 7574 6638  nts.encode("utf8
+0000f1f0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+0000f200: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000f210: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+0000f220: 6573 756c 742e 6578 6974 5f63 6f64 652c  esult.exit_code,
+0000f230: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
+0000f240: 6f75 7470 7574 203d 2072 6573 756c 742e  output = result.
+0000f250: 7374 646f 7574 5f62 7974 6573 0a20 2020  stdout_bytes.   
+0000f260: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000f270: 7365 7274 496e 286e 6c2e 656e 636f 6465  sertIn(nl.encode
+0000f280: 2822 7574 6638 2229 2c20 6f75 7470 7574  ("utf8"), output
+0000f290: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000f2a0: 206e 6c20 3d3d 2022 5c6e 223a 0a20 2020   nl == "\n":.   
+0000f2b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f2c0: 662e 6173 7365 7274 4e6f 7449 6e28 6222  f.assertNotIn(b"
+0000f2d0: 5c72 5c6e 222c 206f 7574 7075 7429 0a0a  \r\n", output)..
+0000f2e0: 2020 2020 6465 6620 7465 7374 5f6e 6f72      def test_nor
+0000f2f0: 6d61 6c69 7a65 5f6c 696e 655f 656e 6469  malize_line_endi
+0000f300: 6e67 7328 7365 6c66 2920 2d3e 204e 6f6e  ngs(self) -> Non
+0000f310: 653a 0a20 2020 2020 2020 2077 6974 6820  e:.        with 
+0000f320: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
+0000f330: 7279 2829 2061 7320 776f 726b 7370 6163  ry() as workspac
+0000f340: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0000f350: 6573 745f 6669 6c65 203d 2050 6174 6828  est_file = Path(
+0000f360: 776f 726b 7370 6163 6529 202f 2022 7465  workspace) / "te
+0000f370: 7374 2e70 7922 0a20 2020 2020 2020 2020  st.py".         
+0000f380: 2020 2066 6f72 2064 6174 612c 2065 7870     for data, exp
+0000f390: 6563 7465 6420 696e 2028 0a20 2020 2020  ected in (.     
+0000f3a0: 2020 2020 2020 2020 2020 2028 6222 635c             (b"c\
+0000f3b0: 725c 6e63 5c6e 2022 2c20 6222 635c 725c  r\nc\n ", b"c\r\
+0000f3c0: 6e63 5c72 5c6e 2229 2c0a 2020 2020 2020  nc\r\n"),.      
+0000f3d0: 2020 2020 2020 2020 2020 2862 226c 5c6e            (b"l\n
+0000f3e0: 6c5c 725c 6e20 222c 2062 226c 5c6e 6c5c  l\r\n ", b"l\nl\
+0000f3f0: 6e22 292c 0a20 2020 2020 2020 2020 2020  n"),.           
+0000f400: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000f410: 2020 2020 7465 7374 5f66 696c 652e 7772      test_file.wr
+0000f420: 6974 655f 6279 7465 7328 6461 7461 290a  ite_bytes(data).
+0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f440: 6666 2874 6573 745f 6669 6c65 2c20 7772  ff(test_file, wr
+0000f450: 6974 655f 6261 636b 3d63 6572 6369 732e  ite_back=cercis.
+0000f460: 5772 6974 6542 6163 6b2e 5945 5329 0a20  WriteBack.YES). 
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f480: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000f490: 7465 7374 5f66 696c 652e 7265 6164 5f62  test_file.read_b
+0000f4a0: 7974 6573 2829 2c20 6578 7065 6374 6564  ytes(), expected
+0000f4b0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000f4c0: 6173 7365 7274 5f65 7175 6976 616c 656e  assert_equivalen
+0000f4d0: 745f 6469 6666 6572 656e 745f 6173 7473  t_different_asts
+0000f4e0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000f4f0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000f500: 662e 6173 7365 7274 5261 6973 6573 2841  f.assertRaises(A
+0000f510: 7373 6572 7469 6f6e 4572 726f 7229 3a0a  ssertionError):.
+0000f520: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+0000f530: 6973 2e61 7373 6572 745f 6571 7569 7661  is.assert_equiva
+0000f540: 6c65 6e74 2822 7b7d 222c 2022 4e6f 6e65  lent("{}", "None
+0000f550: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
+0000f560: 5f73 6868 685f 636c 6963 6b28 7365 6c66  _shhh_click(self
+0000f570: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000f580: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000f590: 2020 2020 6672 6f6d 2063 6c69 636b 2069      from click i
+0000f5a0: 6d70 6f72 7420 5f75 6e69 636f 6465 6675  mport _unicodefu
+0000f5b0: 6e20 2023 2074 7970 653a 2069 676e 6f72  n  # type: ignor
+0000f5c0: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
+0000f5d0: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
+0000f5e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000f5f0: 6b69 7054 6573 7428 2249 6e63 6f6d 7061  kipTest("Incompa
+0000f600: 7469 626c 6520 436c 6963 6b20 7665 7273  tible Click vers
+0000f610: 696f 6e22 290a 0a20 2020 2020 2020 2069  ion")..        i
+0000f620: 6620 6e6f 7420 6861 7361 7474 7228 5f75  f not hasattr(_u
+0000f630: 6e69 636f 6465 6675 6e2c 2022 5f76 6572  nicodefun, "_ver
+0000f640: 6966 795f 7079 7468 6f6e 5f65 6e76 2229  ify_python_env")
+0000f650: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f660: 6c66 2e73 6b69 7054 6573 7428 2249 6e63  lf.skipTest("Inc
+0000f670: 6f6d 7061 7469 626c 6520 436c 6963 6b20  ompatible Click 
+0000f680: 7665 7273 696f 6e22 290a 0a20 2020 2020  version")..     
+0000f690: 2020 2023 2046 6972 7374 2c20 6c65 7427     # First, let'
+0000f6a0: 7320 7365 6520 6966 2043 6c69 636b 2069  s see if Click i
+0000f6b0: 7320 6372 6173 6869 6e67 2077 6974 6820  s crashing with 
+0000f6c0: 6120 7072 6566 6572 7265 6420 4153 4349  a preferred ASCI
+0000f6d0: 4920 6368 6172 7365 742e 0a20 2020 2020  I charset..     
+0000f6e0: 2020 2077 6974 6820 7061 7463 6828 226c     with patch("l
+0000f6f0: 6f63 616c 652e 6765 7470 7265 6665 7272  ocale.getpreferr
+0000f700: 6564 656e 636f 6469 6e67 2229 2061 7320  edencoding") as 
+0000f710: 6770 653a 0a20 2020 2020 2020 2020 2020  gpe:.           
+0000f720: 2067 7065 2e72 6574 7572 6e5f 7661 6c75   gpe.return_valu
+0000f730: 6520 3d20 2241 5343 4949 220a 2020 2020  e = "ASCII".    
+0000f740: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000f750: 662e 6173 7365 7274 5261 6973 6573 2852  f.assertRaises(R
+0000f760: 756e 7469 6d65 4572 726f 7229 3a0a 2020  untimeError):.  
+0000f770: 2020 2020 2020 2020 2020 2020 2020 5f75                _u
+0000f780: 6e69 636f 6465 6675 6e2e 5f76 6572 6966  nicodefun._verif
+0000f790: 795f 7079 7468 6f6e 5f65 6e76 2829 0a20  y_python_env(). 
+0000f7a0: 2020 2020 2020 2023 204e 6f77 2c20 6c65         # Now, le
+0000f7b0: 7427 7320 7369 6c65 6e63 6520 436c 6963  t's silence Clic
+0000f7c0: 6b2e 2e2e 0a20 2020 2020 2020 2063 6572  k....        cer
+0000f7d0: 6369 732e 7061 7463 685f 636c 6963 6b28  cis.patch_click(
+0000f7e0: 290a 2020 2020 2020 2020 2320 2e2e 2e61  ).        # ...a
+0000f7f0: 6e64 2063 6f6e 6669 726d 2069 7427 7320  nd confirm it's 
+0000f800: 7369 6c65 6e74 2e0a 2020 2020 2020 2020  silent..        
+0000f810: 7769 7468 2070 6174 6368 2822 6c6f 6361  with patch("loca
+0000f820: 6c65 2e67 6574 7072 6566 6572 7265 6465  le.getpreferrede
+0000f830: 6e63 6f64 696e 6722 2920 6173 2067 7065  ncoding") as gpe
+0000f840: 3a0a 2020 2020 2020 2020 2020 2020 6770  :.            gp
+0000f850: 652e 7265 7475 726e 5f76 616c 7565 203d  e.return_value =
+0000f860: 2022 4153 4349 4922 0a20 2020 2020 2020   "ASCII".       
+0000f870: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000f880: 2020 2020 2020 2020 2020 5f75 6e69 636f            _unico
+0000f890: 6465 6675 6e2e 5f76 6572 6966 795f 7079  defun._verify_py
+0000f8a0: 7468 6f6e 5f65 6e76 2829 0a20 2020 2020  thon_env().     
+0000f8b0: 2020 2020 2020 2065 7863 6570 7420 5275         except Ru
+0000f8c0: 6e74 696d 6545 7272 6f72 2061 7320 7265  ntimeError as re
+0000f8d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f8e0: 2020 7365 6c66 2e66 6169 6c28 6622 6070    self.fail(f"`p
+0000f8f0: 6174 6368 5f63 6c69 636b 2829 6020 6661  atch_click()` fa
+0000f900: 696c 6564 2c20 6578 6365 7074 696f 6e20  iled, exception 
+0000f910: 7374 696c 6c20 7261 6973 6564 3a20 7b72  still raised: {r
+0000f920: 657d 2229 0a0a 2020 2020 6465 6620 7465  e}")..    def te
+0000f930: 7374 5f72 6f6f 745f 6c6f 6767 6572 5f6e  st_root_logger_n
+0000f940: 6f74 5f75 7365 645f 6469 7265 6374 6c79  ot_used_directly
+0000f950: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000f960: 2020 2020 2020 2020 6465 6620 6661 696c          def fail
+0000f970: 282a 6172 6773 3a20 416e 792c 202a 2a6b  (*args: Any, **k
+0000f980: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
+0000f990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000f9a0: 2073 656c 662e 6661 696c 2822 5265 636f   self.fail("Reco
+0000f9b0: 7264 2063 7265 6174 6564 2077 6974 6820  rd created with 
+0000f9c0: 726f 6f74 206c 6f67 6765 7222 290a 0a20  root logger").. 
+0000f9d0: 2020 2020 2020 2077 6974 6820 7061 7463         with patc
+0000f9e0: 682e 6d75 6c74 6970 6c65 280a 2020 2020  h.multiple(.    
+0000f9f0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+0000fa00: 726f 6f74 2c0a 2020 2020 2020 2020 2020  root,.          
+0000fa10: 2020 6465 6275 673d 6661 696c 2c0a 2020    debug=fail,.  
+0000fa20: 2020 2020 2020 2020 2020 696e 666f 3d66            info=f
+0000fa30: 6169 6c2c 0a20 2020 2020 2020 2020 2020  ail,.           
+0000fa40: 2077 6172 6e69 6e67 3d66 6169 6c2c 0a20   warning=fail,. 
+0000fa50: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+0000fa60: 3d66 6169 6c2c 0a20 2020 2020 2020 2020  =fail,.         
+0000fa70: 2020 2063 7269 7469 6361 6c3d 6661 696c     critical=fail
+0000fa80: 2c0a 2020 2020 2020 2020 2020 2020 6c6f  ,.            lo
+0000fa90: 673d 6661 696c 2c0a 2020 2020 2020 2020  g=fail,.        
+0000faa0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+0000fab0: 6628 5448 4953 5f44 4952 202f 2022 7574  f(THIS_DIR / "ut
+0000fac0: 696c 2e70 7922 290a 0a20 2020 2064 6566  il.py")..    def
+0000fad0: 2074 6573 745f 696e 7661 6c69 645f 636f   test_invalid_co
+0000fae0: 6e66 6967 5f72 6574 7572 6e5f 636f 6465  nfig_return_code
+0000faf0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000fb00: 2020 2020 2020 2020 746d 705f 6669 6c65          tmp_file
+0000fb10: 203d 2050 6174 6828 6365 7263 6973 2e64   = Path(cercis.d
+0000fb20: 756d 705f 746f 5f66 696c 6528 2929 0a20  ump_to_file()). 
+0000fb30: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000fb40: 2020 2020 2020 2020 746d 705f 636f 6e66          tmp_conf
+0000fb50: 6967 203d 2050 6174 6828 6365 7263 6973  ig = Path(cercis
+0000fb60: 2e64 756d 705f 746f 5f66 696c 6528 2929  .dump_to_file())
+0000fb70: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
+0000fb80: 5f63 6f6e 6669 672e 756e 6c69 6e6b 2829  _config.unlink()
+0000fb90: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+0000fba0: 7320 3d20 5b22 2d2d 636f 6e66 6967 222c  s = ["--config",
+0000fbb0: 2073 7472 2874 6d70 5f63 6f6e 6669 6729   str(tmp_config)
+0000fbc0: 2c20 7374 7228 746d 705f 6669 6c65 295d  , str(tmp_file)]
+0000fbd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fbe0: 662e 696e 766f 6b65 426c 6163 6b28 6172  f.invokeBlack(ar
+0000fbf0: 6773 2c20 6578 6974 5f63 6f64 653d 322c  gs, exit_code=2,
+0000fc00: 2069 676e 6f72 655f 636f 6e66 6967 3d46   ignore_config=F
+0000fc10: 616c 7365 290a 2020 2020 2020 2020 6669  alse).        fi
+0000fc20: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+0000fc30: 2020 2074 6d70 5f66 696c 652e 756e 6c69     tmp_file.unli
+0000fc40: 6e6b 2829 0a0a 2020 2020 6465 6620 7465  nk()..    def te
+0000fc50: 7374 5f70 6172 7365 5f70 7970 726f 6a65  st_parse_pyproje
+0000fc60: 6374 5f74 6f6d 6c28 7365 6c66 2920 2d3e  ct_toml(self) ->
+0000fc70: 204e 6f6e 653a 0a20 2020 2020 2020 2074   None:.        t
+0000fc80: 6573 745f 746f 6d6c 5f66 696c 6520 3d20  est_toml_file = 
+0000fc90: 5448 4953 5f44 4952 202f 2022 7465 7374  THIS_DIR / "test
+0000fca0: 2e74 6f6d 6c22 0a20 2020 2020 2020 2063  .toml".        c
+0000fcb0: 6f6e 6669 6720 3d20 6365 7263 6973 2e70  onfig = cercis.p
+0000fcc0: 6172 7365 5f70 7970 726f 6a65 6374 5f74  arse_pyproject_t
+0000fcd0: 6f6d 6c28 7374 7228 7465 7374 5f74 6f6d  oml(str(test_tom
+0000fce0: 6c5f 6669 6c65 2929 0a20 2020 2020 2020  l_file)).       
+0000fcf0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000fd00: 6c28 636f 6e66 6967 5b22 7665 7262 6f73  l(config["verbos
+0000fd10: 6522 5d2c 2031 290a 2020 2020 2020 2020  e"], 1).        
+0000fd20: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000fd30: 2863 6f6e 6669 675b 2263 6865 636b 225d  (config["check"]
+0000fd40: 2c20 226e 6f22 290a 2020 2020 2020 2020  , "no").        
+0000fd50: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000fd60: 2863 6f6e 6669 675b 2264 6966 6622 5d2c  (config["diff"],
+0000fd70: 2022 7922 290a 2020 2020 2020 2020 7365   "y").        se
+0000fd80: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
+0000fd90: 6f6e 6669 675b 2263 6f6c 6f72 225d 2c20  onfig["color"], 
+0000fda0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+0000fdb0: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
+0000fdc0: 6f6e 6669 675b 226c 696e 655f 6c65 6e67  onfig["line_leng
+0000fdd0: 7468 225d 2c20 3739 290a 2020 2020 2020  th"], 79).      
+0000fde0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000fdf0: 616c 2863 6f6e 6669 675b 2274 6172 6765  al(config["targe
+0000fe00: 745f 7665 7273 696f 6e22 5d2c 205b 2270  t_version"], ["p
+0000fe10: 7933 3622 2c20 2270 7933 3722 2c20 2270  y36", "py37", "p
+0000fe20: 7933 3822 5d29 0a20 2020 2020 2020 2073  y38"]).        s
+0000fe30: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000fe40: 636f 6e66 6967 5b22 7079 7468 6f6e 5f63  config["python_c
+0000fe50: 656c 6c5f 6d61 6769 6373 225d 2c20 5b22  ell_magics"], ["
+0000fe60: 6375 7374 6f6d 3122 2c20 2263 7573 746f  custom1", "custo
+0000fe70: 6d32 225d 290a 2020 2020 2020 2020 7365  m2"]).        se
+0000fe80: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
+0000fe90: 6f6e 6669 675b 2265 7863 6c75 6465 225d  onfig["exclude"]
+0000fea0: 2c20 7222 5c2e 7079 693f 2422 290a 2020  , r"\.pyi?$").  
+0000feb0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000fec0: 7445 7175 616c 2863 6f6e 6669 675b 2269  tEqual(config["i
+0000fed0: 6e63 6c75 6465 225d 2c20 7222 5c2e 7079  nclude"], r"\.py
+0000fee0: 3f24 2229 0a0a 2020 2020 6465 6620 7465  ?$")..    def te
+0000fef0: 7374 5f70 6172 7365 5f70 7970 726f 6a65  st_parse_pyproje
+0000ff00: 6374 5f74 6f6d 6c5f 7072 6f6a 6563 745f  ct_toml_project_
+0000ff10: 6d65 7461 6461 7461 2873 656c 6629 202d  metadata(self) -
+0000ff20: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000ff30: 666f 7220 7465 7374 5f74 6f6d 6c2c 2065  for test_toml, e
+0000ff40: 7870 6563 7465 6420 696e 205b 0a20 2020  xpected in [.   
+0000ff50: 2020 2020 2020 2020 2028 226f 6e6c 795f           ("only_
+0000ff60: 626c 6163 6b5f 7079 7072 6f6a 6563 742e  black_pyproject.
+0000ff70: 746f 6d6c 222c 205b 2270 7933 3130 225d  toml", ["py310"]
+0000ff80: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0000ff90: 226f 6e6c 795f 6d65 7461 6461 7461 5f70  "only_metadata_p
+0000ffa0: 7970 726f 6a65 6374 2e74 6f6d 6c22 2c20  yproject.toml", 
+0000ffb0: 5b22 7079 3337 222c 2022 7079 3338 222c  ["py37", "py38",
+0000ffc0: 2022 7079 3339 222c 2022 7079 3331 3022   "py39", "py310"
+0000ffd0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0000ffe0: 2822 6e65 6974 6865 725f 7079 7072 6f6a  ("neither_pyproj
+0000fff0: 6563 742e 746f 6d6c 222c 204e 6f6e 6529  ect.toml", None)
+00010000: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+00010010: 626f 7468 5f70 7970 726f 6a65 6374 2e74  both_pyproject.t
+00010020: 6f6d 6c22 2c20 5b22 7079 3331 3022 5d29  oml", ["py310"])
+00010030: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
+00010040: 2020 2020 2020 2020 2074 6573 745f 746f           test_to
+00010050: 6d6c 5f66 696c 6520 3d20 5448 4953 5f44  ml_file = THIS_D
+00010060: 4952 202f 2022 6461 7461 2220 2f20 2270  IR / "data" / "p
+00010070: 726f 6a65 6374 5f6d 6574 6164 6174 6122  roject_metadata"
+00010080: 202f 2074 6573 745f 746f 6d6c 0a20 2020   / test_toml.   
+00010090: 2020 2020 2020 2020 2063 6f6e 6669 6720           config 
+000100a0: 3d20 6365 7263 6973 2e70 6172 7365 5f70  = cercis.parse_p
+000100b0: 7970 726f 6a65 6374 5f74 6f6d 6c28 7374  yproject_toml(st
+000100c0: 7228 7465 7374 5f74 6f6d 6c5f 6669 6c65  r(test_toml_file
+000100d0: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+000100e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000100f0: 636f 6e66 6967 2e67 6574 2822 7461 7267  config.get("targ
+00010100: 6574 5f76 6572 7369 6f6e 2229 2c20 6578  et_version"), ex
+00010110: 7065 6374 6564 290a 0a20 2020 2064 6566  pected)..    def
+00010120: 2074 6573 745f 696e 6665 725f 7461 7267   test_infer_targ
+00010130: 6574 5f76 6572 7369 6f6e 2873 656c 6629  et_version(self)
+00010140: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00010150: 2020 666f 7220 7665 7273 696f 6e2c 2065    for version, e
+00010160: 7870 6563 7465 6420 696e 205b 0a20 2020  xpected in [.   
+00010170: 2020 2020 2020 2020 2028 2233 2e36 222c           ("3.6",
+00010180: 205b 5461 7267 6574 5665 7273 696f 6e2e   [TargetVersion.
+00010190: 5059 3336 5d29 2c0a 2020 2020 2020 2020  PY36]),.        
+000101a0: 2020 2020 2822 332e 3131 2e30 7263 3122      ("3.11.0rc1"
+000101b0: 2c20 5b54 6172 6765 7456 6572 7369 6f6e  , [TargetVersion
+000101c0: 2e50 5933 3131 5d29 2c0a 2020 2020 2020  .PY311]),.      
+000101d0: 2020 2020 2020 2822 3e3d 332e 3130 222c        (">=3.10",
+000101e0: 205b 5461 7267 6574 5665 7273 696f 6e2e   [TargetVersion.
+000101f0: 5059 3331 302c 2054 6172 6765 7456 6572  PY310, TargetVer
+00010200: 7369 6f6e 2e50 5933 3131 2c20 5461 7267  sion.PY311, Targ
+00010210: 6574 5665 7273 696f 6e2e 5059 3331 325d  etVersion.PY312]
+00010220: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00010230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010240: 2022 3e3d 332e 3130 2e36 222c 0a20 2020   ">=3.10.6",.   
+00010250: 2020 2020 2020 2020 2020 2020 205b 5461               [Ta
+00010260: 7267 6574 5665 7273 696f 6e2e 5059 3331  rgetVersion.PY31
+00010270: 302c 2054 6172 6765 7456 6572 7369 6f6e  0, TargetVersion
+00010280: 2e50 5933 3131 2c20 5461 7267 6574 5665  .PY311, TargetVe
+00010290: 7273 696f 6e2e 5059 3331 325d 2c0a 2020  rsion.PY312],.  
+000102a0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+000102b0: 2020 2020 2020 2020 2028 223c 332e 3622           ("<3.6"
+000102c0: 2c20 5b54 6172 6765 7456 6572 7369 6f6e  , [TargetVersion
+000102d0: 2e50 5933 332c 2054 6172 6765 7456 6572  .PY33, TargetVer
+000102e0: 7369 6f6e 2e50 5933 342c 2054 6172 6765  sion.PY34, Targe
+000102f0: 7456 6572 7369 6f6e 2e50 5933 355d 292c  tVersion.PY35]),
+00010300: 0a20 2020 2020 2020 2020 2020 2028 223e  .            (">
+00010310: 332e 372c 3c33 2e31 3022 2c20 5b54 6172  3.7,<3.10", [Tar
+00010320: 6765 7456 6572 7369 6f6e 2e50 5933 382c  getVersion.PY38,
+00010330: 2054 6172 6765 7456 6572 7369 6f6e 2e50   TargetVersion.P
+00010340: 5933 395d 292c 0a20 2020 2020 2020 2020  Y39]),.         
+00010350: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00010360: 2020 2020 2022 3e33 2e37 2c21 3d33 2e38       ">3.7,!=3.8
+00010370: 2c21 3d33 2e39 222c 0a20 2020 2020 2020  ,!=3.9",.       
+00010380: 2020 2020 2020 2020 205b 5461 7267 6574           [Target
+00010390: 5665 7273 696f 6e2e 5059 3331 302c 2054  Version.PY310, T
+000103a0: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
+000103b0: 3131 2c20 5461 7267 6574 5665 7273 696f  11, TargetVersio
+000103c0: 6e2e 5059 3331 325d 2c0a 2020 2020 2020  n.PY312],.      
+000103d0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+000103e0: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+000103f0: 2020 2020 2020 2022 3e20 332e 392e 342c         "> 3.9.4,
+00010400: 2021 3d20 332e 3130 2e33 222c 0a20 2020   != 3.10.3",.   
+00010410: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 2020 2054 6172 6765 7456 6572 7369 6f6e     TargetVersion
+00010440: 2e50 5933 392c 0a20 2020 2020 2020 2020  .PY39,.         
+00010450: 2020 2020 2020 2020 2020 2054 6172 6765             Targe
+00010460: 7456 6572 7369 6f6e 2e50 5933 3130 2c0a  tVersion.PY310,.
+00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010480: 2020 2020 5461 7267 6574 5665 7273 696f      TargetVersio
+00010490: 6e2e 5059 3331 312c 0a20 2020 2020 2020  n.PY311,.       
+000104a0: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+000104b0: 6765 7456 6572 7369 6f6e 2e50 5933 3132  getVersion.PY312
+000104c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000104d0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+000104e0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+000104f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010500: 2020 2221 3d33 2e33 2c21 3d33 2e34 222c    "!=3.3,!=3.4",
+00010510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010520: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00010530: 2020 2020 2020 2054 6172 6765 7456 6572         TargetVer
+00010540: 7369 6f6e 2e50 5933 352c 0a20 2020 2020  sion.PY35,.     
+00010550: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00010560: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
+00010570: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
+00010580: 2020 2020 2020 2054 6172 6765 7456 6572         TargetVer
+00010590: 7369 6f6e 2e50 5933 372c 0a20 2020 2020  sion.PY37,.     
+000105a0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+000105b0: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
+000105c0: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
+000105d0: 2020 2020 2020 2054 6172 6765 7456 6572         TargetVer
+000105e0: 7369 6f6e 2e50 5933 392c 0a20 2020 2020  sion.PY39,.     
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00010600: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
+00010610: 3130 2c0a 2020 2020 2020 2020 2020 2020  10,.            
+00010620: 2020 2020 2020 2020 5461 7267 6574 5665          TargetVe
+00010630: 7273 696f 6e2e 5059 3331 312c 0a20 2020  rsion.PY311,.   
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 2054 6172 6765 7456 6572 7369 6f6e 2e50   TargetVersion.P
+00010660: 5933 3132 2c0a 2020 2020 2020 2020 2020  Y312,.          
+00010670: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00010680: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00010690: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+000106a0: 2020 2020 2020 223d 3d33 2e2a 222c 0a20        "==3.*",. 
+000106b0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000106c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000106d0: 2020 2020 2054 6172 6765 7456 6572 7369       TargetVersi
+000106e0: 6f6e 2e50 5933 332c 0a20 2020 2020 2020  on.PY33,.       
+000106f0: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+00010700: 6765 7456 6572 7369 6f6e 2e50 5933 342c  getVersion.PY34,
+00010710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010720: 2020 2020 2054 6172 6765 7456 6572 7369       TargetVersi
+00010730: 6f6e 2e50 5933 352c 0a20 2020 2020 2020  on.PY35,.       
+00010740: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+00010750: 6765 7456 6572 7369 6f6e 2e50 5933 362c  getVersion.PY36,
+00010760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010770: 2020 2020 2054 6172 6765 7456 6572 7369       TargetVersi
+00010780: 6f6e 2e50 5933 372c 0a20 2020 2020 2020  on.PY37,.       
+00010790: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+000107a0: 6765 7456 6572 7369 6f6e 2e50 5933 382c  getVersion.PY38,
+000107b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000107c0: 2020 2020 2054 6172 6765 7456 6572 7369       TargetVersi
+000107d0: 6f6e 2e50 5933 392c 0a20 2020 2020 2020  on.PY39,.       
+000107e0: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+000107f0: 6765 7456 6572 7369 6f6e 2e50 5933 3130  getVersion.PY310
+00010800: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010810: 2020 2020 2020 5461 7267 6574 5665 7273        TargetVers
+00010820: 696f 6e2e 5059 3331 312c 0a20 2020 2020  ion.PY311,.     
+00010830: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00010840: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
+00010850: 3132 2c0a 2020 2020 2020 2020 2020 2020  12,.            
+00010860: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00010870: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00010880: 2020 2822 3d3d 332e 382e 2a22 2c20 5b54    ("==3.8.*", [T
+00010890: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
+000108a0: 385d 292c 0a20 2020 2020 2020 2020 2020  8]),.           
+000108b0: 2028 4e6f 6e65 2c20 4e6f 6e65 292c 0a20   (None, None),. 
+000108c0: 2020 2020 2020 2020 2020 2028 2222 2c20             ("", 
+000108d0: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
+000108e0: 2020 2028 2269 6e76 616c 6964 222c 204e     ("invalid", N
+000108f0: 6f6e 6529 2c0a 2020 2020 2020 2020 2020  one),.          
+00010900: 2020 2822 3d3d 696e 7661 6c69 6422 2c20    ("==invalid", 
+00010910: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
+00010920: 2020 2028 223e 332e 392c 213d 696e 7661     (">3.9,!=inva
+00010930: 6c69 6422 2c20 4e6f 6e65 292c 0a20 2020  lid", None),.   
+00010940: 2020 2020 2020 2020 2028 2233 222c 204e           ("3", N
+00010950: 6f6e 6529 2c0a 2020 2020 2020 2020 2020  one),.          
+00010960: 2020 2822 332e 3222 2c20 4e6f 6e65 292c    ("3.2", None),
+00010970: 0a20 2020 2020 2020 2020 2020 2028 2232  .            ("2
+00010980: 2e37 2e31 3822 2c20 4e6f 6e65 292c 0a20  .7.18", None),. 
+00010990: 2020 2020 2020 2020 2020 2028 223d 3d32             ("==2
+000109a0: 2e37 222c 204e 6f6e 6529 2c0a 2020 2020  .7", None),.    
+000109b0: 2020 2020 2020 2020 2822 3e33 2e31 302c          (">3.10,
+000109c0: 3c33 2e31 3122 2c20 4e6f 6e65 292c 0a20  <3.11", None),. 
+000109d0: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
+000109e0: 2020 2020 2020 7465 7374 5f74 6f6d 6c20        test_toml 
+000109f0: 3d20 7b22 7072 6f6a 6563 7422 3a20 7b22  = {"project": {"
+00010a00: 7265 7175 6972 6573 2d70 7974 686f 6e22  requires-python"
+00010a10: 3a20 7665 7273 696f 6e7d 7d0a 2020 2020  : version}}.    
+00010a20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00010a30: 2063 6572 6369 732e 6669 6c65 732e 696e   cercis.files.in
+00010a40: 6665 725f 7461 7267 6574 5f76 6572 7369  fer_target_versi
+00010a50: 6f6e 2874 6573 745f 746f 6d6c 290a 2020  on(test_toml).  
+00010a60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00010a70: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00010a80: 742c 2065 7870 6563 7465 6429 0a0a 2020  t, expected)..  
+00010a90: 2020 6465 6620 7465 7374 5f72 6561 645f    def test_read_
+00010aa0: 7079 7072 6f6a 6563 745f 746f 6d6c 2873  pyproject_toml(s
+00010ab0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00010ac0: 2020 2020 2020 7465 7374 5f74 6f6d 6c5f        test_toml_
+00010ad0: 6669 6c65 203d 2054 4849 535f 4449 5220  file = THIS_DIR 
+00010ae0: 2f20 2274 6573 742e 746f 6d6c 220a 2020  / "test.toml".  
+00010af0: 2020 2020 2020 6661 6b65 5f63 7478 203d        fake_ctx =
+00010b00: 2046 616b 6543 6f6e 7465 7874 2829 0a20   FakeContext(). 
+00010b10: 2020 2020 2020 2063 6572 6369 732e 7265         cercis.re
+00010b20: 6164 5f70 7970 726f 6a65 6374 5f74 6f6d  ad_pyproject_tom
+00010b30: 6c28 6661 6b65 5f63 7478 2c20 4661 6b65  l(fake_ctx, Fake
+00010b40: 5061 7261 6d65 7465 7228 292c 2073 7472  Parameter(), str
+00010b50: 2874 6573 745f 746f 6d6c 5f66 696c 6529  (test_toml_file)
+00010b60: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
+00010b70: 203d 2066 616b 655f 6374 782e 6465 6661   = fake_ctx.defa
+00010b80: 756c 745f 6d61 700a 2020 2020 2020 2020  ult_map.        
+00010b90: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00010ba0: 2863 6f6e 6669 675b 2276 6572 626f 7365  (config["verbose
+00010bb0: 225d 2c20 2231 2229 0a20 2020 2020 2020  "], "1").       
+00010bc0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00010bd0: 6c28 636f 6e66 6967 5b22 6368 6563 6b22  l(config["check"
+00010be0: 5d2c 2022 6e6f 2229 0a20 2020 2020 2020  ], "no").       
+00010bf0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00010c00: 6c28 636f 6e66 6967 5b22 6469 6666 225d  l(config["diff"]
+00010c10: 2c20 2279 2229 0a20 2020 2020 2020 2073  , "y").        s
+00010c20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00010c30: 636f 6e66 6967 5b22 636f 6c6f 7222 5d2c  config["color"],
+00010c40: 2022 5472 7565 2229 0a20 2020 2020 2020   "True").       
+00010c50: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00010c60: 6c28 636f 6e66 6967 5b22 6c69 6e65 5f6c  l(config["line_l
+00010c70: 656e 6774 6822 5d2c 2022 3739 2229 0a20  ength"], "79"). 
+00010c80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010c90: 7274 4571 7561 6c28 636f 6e66 6967 5b22  rtEqual(config["
+00010ca0: 7461 7267 6574 5f76 6572 7369 6f6e 225d  target_version"]
+00010cb0: 2c20 5b22 7079 3336 222c 2022 7079 3337  , ["py36", "py37
+00010cc0: 222c 2022 7079 3338 225d 290a 2020 2020  ", "py38"]).    
+00010cd0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00010ce0: 7175 616c 2863 6f6e 6669 675b 2265 7863  qual(config["exc
+00010cf0: 6c75 6465 225d 2c20 7222 5c2e 7079 693f  lude"], r"\.pyi?
+00010d00: 2422 290a 2020 2020 2020 2020 7365 6c66  $").        self
+00010d10: 2e61 7373 6572 7445 7175 616c 2863 6f6e  .assertEqual(con
+00010d20: 6669 675b 2269 6e63 6c75 6465 225d 2c20  fig["include"], 
+00010d30: 7222 5c2e 7079 3f24 2229 0a0a 2020 2020  r"\.py?$")..    
+00010d40: 4070 7974 6573 742e 6d61 726b 2e69 6e63  @pytest.mark.inc
+00010d50: 6f6d 7061 7469 626c 655f 7769 7468 5f6d  ompatible_with_m
+00010d60: 7970 7963 0a20 2020 2064 6566 2074 6573  ypyc.    def tes
+00010d70: 745f 6669 6e64 5f70 726f 6a65 6374 5f72  t_find_project_r
+00010d80: 6f6f 7428 7365 6c66 2920 2d3e 204e 6f6e  oot(self) -> Non
+00010d90: 653a 0a20 2020 2020 2020 2077 6974 6820  e:.        with 
+00010da0: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
+00010db0: 7279 2829 2061 7320 776f 726b 7370 6163  ry() as workspac
+00010dc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00010dd0: 6f6f 7420 3d20 5061 7468 2877 6f72 6b73  oot = Path(works
+00010de0: 7061 6365 290a 2020 2020 2020 2020 2020  pace).          
+00010df0: 2020 7465 7374 5f64 6972 203d 2072 6f6f    test_dir = roo
+00010e00: 7420 2f20 2274 6573 7422 0a20 2020 2020  t / "test".     
+00010e10: 2020 2020 2020 2074 6573 745f 6469 722e         test_dir.
+00010e20: 6d6b 6469 7228 290a 0a20 2020 2020 2020  mkdir()..       
+00010e30: 2020 2020 2073 7263 5f64 6972 203d 2072       src_dir = r
+00010e40: 6f6f 7420 2f20 2273 7263 220a 2020 2020  oot / "src".    
+00010e50: 2020 2020 2020 2020 7372 635f 6469 722e          src_dir.
+00010e60: 6d6b 6469 7228 290a 0a20 2020 2020 2020  mkdir()..       
+00010e70: 2020 2020 2072 6f6f 745f 7079 7072 6f6a       root_pyproj
+00010e80: 6563 7420 3d20 726f 6f74 202f 2022 7079  ect = root / "py
+00010e90: 7072 6f6a 6563 742e 746f 6d6c 220a 2020  project.toml".  
+00010ea0: 2020 2020 2020 2020 2020 726f 6f74 5f70            root_p
+00010eb0: 7970 726f 6a65 6374 2e74 6f75 6368 2829  yproject.touch()
+00010ec0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
+00010ed0: 5f70 7970 726f 6a65 6374 203d 2073 7263  _pyproject = src
+00010ee0: 5f64 6972 202f 2022 7079 7072 6f6a 6563  _dir / "pyprojec
+00010ef0: 742e 746f 6d6c 220a 2020 2020 2020 2020  t.toml".        
+00010f00: 2020 2020 7372 635f 7079 7072 6f6a 6563      src_pyprojec
+00010f10: 742e 746f 7563 6828 290a 2020 2020 2020  t.touch().      
+00010f20: 2020 2020 2020 7372 635f 7079 7468 6f6e        src_python
+00010f30: 203d 2073 7263 5f64 6972 202f 2022 666f   = src_dir / "fo
+00010f40: 6f2e 7079 220a 2020 2020 2020 2020 2020  o.py".          
+00010f50: 2020 7372 635f 7079 7468 6f6e 2e74 6f75    src_python.tou
+00010f60: 6368 2829 0a0a 2020 2020 2020 2020 2020  ch()..          
+00010f70: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00010f80: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00010f90: 2020 2020 6365 7263 6973 2e66 696e 645f      cercis.find_
+00010fa0: 7072 6f6a 6563 745f 726f 6f74 2828 7372  project_root((sr
+00010fb0: 635f 6469 722c 2074 6573 745f 6469 7229  c_dir, test_dir)
+00010fc0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00010fd0: 2020 2028 726f 6f74 2e72 6573 6f6c 7665     (root.resolve
+00010fe0: 2829 2c20 2270 7970 726f 6a65 6374 2e74  (), "pyproject.t
+00010ff0: 6f6d 6c22 292c 0a20 2020 2020 2020 2020  oml"),.         
+00011000: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00011010: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00011020: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00011030: 2020 2063 6572 6369 732e 6669 6e64 5f70     cercis.find_p
+00011040: 726f 6a65 6374 5f72 6f6f 7428 2873 7263  roject_root((src
+00011050: 5f64 6972 2c29 292c 0a20 2020 2020 2020  _dir,)),.       
+00011060: 2020 2020 2020 2020 2028 7372 635f 6469           (src_di
+00011070: 722e 7265 736f 6c76 6528 292c 2022 7079  r.resolve(), "py
+00011080: 7072 6f6a 6563 742e 746f 6d6c 2229 2c0a  project.toml"),.
+00011090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000110a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000110b0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+000110c0: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+000110d0: 6973 2e66 696e 645f 7072 6f6a 6563 745f  is.find_project_
+000110e0: 726f 6f74 2828 7372 635f 7079 7468 6f6e  root((src_python
+000110f0: 2c29 292c 0a20 2020 2020 2020 2020 2020  ,)),.           
+00011100: 2020 2020 2028 7372 635f 6469 722e 7265       (src_dir.re
+00011110: 736f 6c76 6528 292c 2022 7079 7072 6f6a  solve(), "pyproj
+00011120: 6563 742e 746f 6d6c 2229 2c0a 2020 2020  ect.toml"),.    
+00011130: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00011140: 2020 2020 2020 2077 6974 6820 6368 616e         with chan
+00011150: 6765 5f64 6972 6563 746f 7279 2874 6573  ge_directory(tes
+00011160: 745f 6469 7229 3a0a 2020 2020 2020 2020  t_dir):.        
+00011170: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00011180: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00011190: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+000111a0: 7263 6973 2e66 696e 645f 7072 6f6a 6563  rcis.find_projec
+000111b0: 745f 726f 6f74 2828 222d 222c 292c 2073  t_root(("-",), s
+000111c0: 7464 696e 5f66 696c 656e 616d 653d 222e  tdin_filename=".
+000111d0: 2e2f 7372 632f 612e 7079 2229 2c0a 2020  ./src/a.py"),.  
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 2020 2873 7263 5f64 6972 2e72 6573 6f6c    (src_dir.resol
+00011200: 7665 2829 2c20 2270 7970 726f 6a65 6374  ve(), "pyproject
+00011210: 2e74 6f6d 6c22 292c 0a20 2020 2020 2020  .toml"),.       
+00011220: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00011230: 4070 6174 6368 280a 2020 2020 2020 2020  @patch(.        
+00011240: 2263 6572 6369 732e 6669 6c65 732e 6669  "cercis.files.fi
+00011250: 6e64 5f75 7365 725f 7079 7072 6f6a 6563  nd_user_pyprojec
+00011260: 745f 746f 6d6c 222c 0a20 2020 2029 0a20  t_toml",.    ). 
+00011270: 2020 2064 6566 2074 6573 745f 6669 6e64     def test_find
+00011280: 5f70 7970 726f 6a65 6374 5f74 6f6d 6c28  _pyproject_toml(
+00011290: 7365 6c66 2c20 6669 6e64 5f75 7365 725f  self, find_user_
+000112a0: 7079 7072 6f6a 6563 745f 746f 6d6c 3a20  pyproject_toml: 
+000112b0: 4d61 6769 634d 6f63 6b29 202d 3e20 4e6f  MagicMock) -> No
+000112c0: 6e65 3a0a 2020 2020 2020 2020 6669 6e64  ne:.        find
+000112d0: 5f75 7365 725f 7079 7072 6f6a 6563 745f  _user_pyproject_
+000112e0: 746f 6d6c 2e73 6964 655f 6566 6665 6374  toml.side_effect
+000112f0: 203d 2052 756e 7469 6d65 4572 726f 7228   = RuntimeError(
+00011300: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00011310: 7265 6469 7265 6374 5f73 7464 6572 7228  redirect_stderr(
+00011320: 696f 2e53 7472 696e 6749 4f28 2929 2061  io.StringIO()) a
+00011330: 7320 7374 6465 7272 3a0a 2020 2020 2020  s stderr:.      
+00011340: 2020 2020 2020 7265 7375 6c74 203d 2063        result = c
+00011350: 6572 6369 732e 6669 6c65 732e 6669 6e64  ercis.files.find
+00011360: 5f70 7970 726f 6a65 6374 5f74 6f6d 6c28  _pyproject_toml(
+00011370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011380: 2070 6174 685f 7365 6172 6368 5f73 7461   path_search_sta
+00011390: 7274 3d28 7374 7228 5061 7468 2e63 7764  rt=(str(Path.cwd
+000113a0: 2829 2e72 6f6f 7429 2c29 0a20 2020 2020  ().root),).     
+000113b0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000113c0: 2020 6173 7365 7274 2072 6573 756c 7420    assert result 
+000113d0: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
+000113e0: 6572 7220 3d20 7374 6465 7272 2e67 6574  err = stderr.get
+000113f0: 7661 6c75 6528 290a 2020 2020 2020 2020  value().        
+00011400: 6173 7365 7274 2022 4967 6e6f 7269 6e67  assert "Ignoring
+00011410: 2075 7365 7220 636f 6e66 6967 7572 6174   user configurat
+00011420: 696f 6e22 2069 6e20 6572 720a 0a20 2020  ion" in err..   
+00011430: 2040 7061 7463 6828 0a20 2020 2020 2020   @patch(.       
+00011440: 2022 6365 7263 6973 2e66 696c 6573 2e66   "cercis.files.f
+00011450: 696e 645f 7573 6572 5f70 7970 726f 6a65  ind_user_pyproje
+00011460: 6374 5f74 6f6d 6c22 2c0a 2020 2020 2020  ct_toml",.      
+00011470: 2020 6365 7263 6973 2e66 696c 6573 2e66    cercis.files.f
+00011480: 696e 645f 7573 6572 5f70 7970 726f 6a65  ind_user_pyproje
+00011490: 6374 5f74 6f6d 6c2e 5f5f 7772 6170 7065  ct_toml.__wrappe
+000114a0: 645f 5f2c 0a20 2020 2029 0a20 2020 2064  d__,.    ).    d
+000114b0: 6566 2074 6573 745f 6669 6e64 5f75 7365  ef test_find_use
+000114c0: 725f 7079 7072 6f6a 6563 745f 746f 6d6c  r_pyproject_toml
+000114d0: 5f6c 696e 7578 2873 656c 6629 202d 3e20  _linux(self) -> 
+000114e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
+000114f0: 2073 7973 7465 6d28 2920 3d3d 2022 5769   system() == "Wi
+00011500: 6e64 6f77 7322 3a0a 2020 2020 2020 2020  ndows":.        
+00011510: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00011520: 2020 2020 2320 5465 7374 2069 6620 5844      # Test if XD
+00011530: 475f 434f 4e46 4947 5f48 4f4d 4520 6973  G_CONFIG_HOME is
+00011540: 2063 6865 636b 6564 0a20 2020 2020 2020   checked.       
+00011550: 2077 6974 6820 5465 6d70 6f72 6172 7944   with TemporaryD
+00011560: 6972 6563 746f 7279 2829 2061 7320 776f  irectory() as wo
+00011570: 726b 7370 6163 653a 0a20 2020 2020 2020  rkspace:.       
+00011580: 2020 2020 2074 6d70 5f75 7365 725f 636f       tmp_user_co
+00011590: 6e66 6967 203d 2050 6174 6828 776f 726b  nfig = Path(work
+000115a0: 7370 6163 6529 202f 2022 6365 7263 6973  space) / "cercis
+000115b0: 220a 2020 2020 2020 2020 2020 2020 7769  ".            wi
+000115c0: 7468 2070 6174 6368 2e64 6963 7428 226f  th patch.dict("o
+000115d0: 732e 656e 7669 726f 6e22 2c20 7b22 5844  s.environ", {"XD
+000115e0: 475f 434f 4e46 4947 5f48 4f4d 4522 3a20  G_CONFIG_HOME": 
+000115f0: 776f 726b 7370 6163 657d 293a 0a20 2020  workspace}):.   
+00011600: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011610: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
+00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011630: 2020 2063 6572 6369 732e 6669 6c65 732e     cercis.files.
+00011640: 6669 6e64 5f75 7365 725f 7079 7072 6f6a  find_user_pyproj
+00011650: 6563 745f 746f 6d6c 2829 2c20 746d 705f  ect_toml(), tmp_
+00011660: 7573 6572 5f63 6f6e 6669 672e 7265 736f  user_config.reso
+00011670: 6c76 6528 290a 2020 2020 2020 2020 2020  lve().          
+00011680: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00011690: 2023 2054 6573 7420 6661 6c6c 6261 636b   # Test fallback
+000116a0: 2066 6f72 2058 4447 5f43 4f4e 4649 475f   for XDG_CONFIG_
+000116b0: 484f 4d45 0a20 2020 2020 2020 2077 6974  HOME.        wit
+000116c0: 6820 7061 7463 682e 6469 6374 2822 6f73  h patch.dict("os
+000116d0: 2e65 6e76 6972 6f6e 2229 3a0a 2020 2020  .environ"):.    
+000116e0: 2020 2020 2020 2020 6f73 2e65 6e76 6972          os.envir
+000116f0: 6f6e 2e70 6f70 2822 5844 475f 434f 4e46  on.pop("XDG_CONF
+00011700: 4947 5f48 4f4d 4522 2c20 4e6f 6e65 290a  IG_HOME", None).
+00011710: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
+00011720: 6261 636b 5f75 7365 725f 636f 6e66 6967  back_user_config
+00011730: 203d 2050 6174 6828 227e 2f2e 636f 6e66   = Path("~/.conf
+00011740: 6967 2229 2e65 7870 616e 6475 7365 7228  ig").expanduser(
+00011750: 2920 2f20 2263 6572 6369 7322 0a20 2020  ) / "cercis".   
+00011760: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00011770: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+00011780: 2020 2020 2020 2020 2020 2063 6572 6369             cerci
+00011790: 732e 6669 6c65 732e 6669 6e64 5f75 7365  s.files.find_use
+000117a0: 725f 7079 7072 6f6a 6563 745f 746f 6d6c  r_pyproject_toml
+000117b0: 2829 2c20 6661 6c6c 6261 636b 5f75 7365  (), fallback_use
+000117c0: 725f 636f 6e66 6967 2e72 6573 6f6c 7665  r_config.resolve
+000117d0: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
+000117e0: 0a0a 2020 2020 6465 6620 7465 7374 5f66  ..    def test_f
+000117f0: 696e 645f 7573 6572 5f70 7970 726f 6a65  ind_user_pyproje
+00011800: 6374 5f74 6f6d 6c5f 7769 6e64 6f77 7328  ct_toml_windows(
+00011810: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00011820: 2020 2020 2020 2069 6620 7379 7374 656d         if system
+00011830: 2829 2021 3d20 2257 696e 646f 7773 223a  () != "Windows":
+00011840: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011850: 7572 6e0a 0a20 2020 2020 2020 2075 7365  urn..        use
+00011860: 725f 636f 6e66 6967 5f70 6174 6820 3d20  r_config_path = 
+00011870: 5061 7468 2e68 6f6d 6528 2920 2f20 222e  Path.home() / ".
+00011880: 6365 7263 6973 220a 2020 2020 2020 2020  cercis".        
+00011890: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000118a0: 280a 2020 2020 2020 2020 2020 2020 6365  (.            ce
+000118b0: 7263 6973 2e66 696c 6573 2e66 696e 645f  rcis.files.find_
+000118c0: 7573 6572 5f70 7970 726f 6a65 6374 5f74  user_pyproject_t
+000118d0: 6f6d 6c28 292c 2075 7365 725f 636f 6e66  oml(), user_conf
+000118e0: 6967 5f70 6174 682e 7265 736f 6c76 6528  ig_path.resolve(
+000118f0: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00011900: 2064 6566 2074 6573 745f 6270 6f5f 3333   def test_bpo_33
+00011910: 3636 305f 776f 726b 6172 6f75 6e64 2873  660_workaround(s
+00011920: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00011930: 2020 2020 2020 6966 2073 7973 7465 6d28        if system(
+00011940: 2920 3d3d 2022 5769 6e64 6f77 7322 3a0a  ) == "Windows":.
+00011950: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011960: 726e 0a0a 2020 2020 2020 2020 2320 6874  rn..        # ht
+00011970: 7470 733a 2f2f 6275 6773 2e70 7974 686f  tps://bugs.pytho
+00011980: 6e2e 6f72 672f 6973 7375 6533 3336 3630  n.org/issue33660
+00011990: 0a20 2020 2020 2020 2072 6f6f 7420 3d20  .        root = 
+000119a0: 5061 7468 2822 2f22 290a 2020 2020 2020  Path("/").      
+000119b0: 2020 7769 7468 2063 6861 6e67 655f 6469    with change_di
+000119c0: 7265 6374 6f72 7928 726f 6f74 293a 0a20  rectory(root):. 
+000119d0: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+000119e0: 3d20 5061 7468 2822 776f 726b 7370 6163  = Path("workspac
+000119f0: 6522 2920 2f20 2270 726f 6a65 6374 220a  e") / "project".
+00011a00: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00011a10: 7274 203d 2063 6572 6369 732e 5265 706f  rt = cercis.Repo
+00011a20: 7274 2876 6572 626f 7365 3d54 7275 6529  rt(verbose=True)
+00011a30: 0a20 2020 2020 2020 2020 2020 206e 6f72  .            nor
+00011a40: 6d61 6c69 7a65 645f 7061 7468 203d 2063  malized_path = c
+00011a50: 6572 6369 732e 6e6f 726d 616c 697a 655f  ercis.normalize_
+00011a60: 7061 7468 5f6d 6179 6265 5f69 676e 6f72  path_maybe_ignor
+00011a70: 6528 7061 7468 2c20 726f 6f74 2c20 7265  e(path, root, re
+00011a80: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
+00011a90: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00011aa0: 616c 286e 6f72 6d61 6c69 7a65 645f 7061  al(normalized_pa
+00011ab0: 7468 2c20 2277 6f72 6b73 7061 6365 2f70  th, "workspace/p
+00011ac0: 726f 6a65 6374 2229 0a0a 2020 2020 6465  roject")..    de
+00011ad0: 6620 7465 7374 5f6e 6f72 6d61 6c69 7a65  f test_normalize
+00011ae0: 5f70 6174 685f 6967 6e6f 7265 5f77 696e  _path_ignore_win
+00011af0: 646f 7773 5f6a 756e 6374 696f 6e73 5f6f  dows_junctions_o
+00011b00: 7574 7369 6465 5f6f 665f 726f 6f74 2873  utside_of_root(s
+00011b10: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00011b20: 2020 2020 2020 6966 2073 7973 7465 6d28        if system(
+00011b30: 2920 213d 2022 5769 6e64 6f77 7322 3a0a  ) != "Windows":.
+00011b40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011b50: 726e 0a0a 2020 2020 2020 2020 7769 7468  rn..        with
+00011b60: 2054 656d 706f 7261 7279 4469 7265 6374   TemporaryDirect
+00011b70: 6f72 7928 2920 6173 2077 6f72 6b73 7061  ory() as workspa
+00011b80: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+00011b90: 726f 6f74 203d 2050 6174 6828 776f 726b  root = Path(work
+00011ba0: 7370 6163 6529 0a20 2020 2020 2020 2020  space).         
+00011bb0: 2020 206a 756e 6374 696f 6e5f 6469 7220     junction_dir 
+00011bc0: 3d20 726f 6f74 202f 2022 6a75 6e63 7469  = root / "juncti
+00011bd0: 6f6e 220a 2020 2020 2020 2020 2020 2020  on".            
+00011be0: 6a75 6e63 7469 6f6e 5f74 6172 6765 745f  junction_target_
+00011bf0: 6f75 7473 6964 655f 6f66 5f72 6f6f 7420  outside_of_root 
+00011c00: 3d20 726f 6f74 202f 2022 2e2e 220a 2020  = root / "..".  
+00011c10: 2020 2020 2020 2020 2020 6f73 2e73 7973            os.sys
+00011c20: 7465 6d28 6622 6d6b 6c69 6e6b 202f 4a20  tem(f"mklink /J 
+00011c30: 7b6a 756e 6374 696f 6e5f 6469 727d 207b  {junction_dir} {
+00011c40: 6a75 6e63 7469 6f6e 5f74 6172 6765 745f  junction_target_
+00011c50: 6f75 7473 6964 655f 6f66 5f72 6f6f 747d  outside_of_root}
+00011c60: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+00011c70: 7265 706f 7274 203d 2063 6572 6369 732e  report = cercis.
+00011c80: 5265 706f 7274 2876 6572 626f 7365 3d54  Report(verbose=T
+00011c90: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00011ca0: 206e 6f72 6d61 6c69 7a65 645f 7061 7468   normalized_path
+00011cb0: 203d 2063 6572 6369 732e 6e6f 726d 616c   = cercis.normal
+00011cc0: 697a 655f 7061 7468 5f6d 6179 6265 5f69  ize_path_maybe_i
+00011cd0: 676e 6f72 6528 0a20 2020 2020 2020 2020  gnore(.         
+00011ce0: 2020 2020 2020 206a 756e 6374 696f 6e5f         junction_
+00011cf0: 6469 722c 2072 6f6f 742c 2072 6570 6f72  dir, root, repor
+00011d00: 740a 2020 2020 2020 2020 2020 2020 290a  t.            ).
+00011d10: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
+00011d20: 6e75 616c 6c79 2064 656c 6574 6520 666f  nually delete fo
+00011d30: 7220 5079 7468 6f6e 203c 2033 2e38 0a20  r Python < 3.8. 
+00011d40: 2020 2020 2020 2020 2020 206f 732e 7379             os.sy
+00011d50: 7374 656d 2866 2272 6d64 6972 207b 6a75  stem(f"rmdir {ju
+00011d60: 6e63 7469 6f6e 5f64 6972 7d22 290a 0a20  nction_dir}").. 
+00011d70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011d80: 6173 7365 7274 4571 7561 6c28 6e6f 726d  assertEqual(norm
+00011d90: 616c 697a 6564 5f70 6174 682c 204e 6f6e  alized_path, Non
+00011da0: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
+00011db0: 5f6e 6577 6c69 6e65 5f63 6f6d 6d65 6e74  _newline_comment
+00011dc0: 5f69 6e74 6572 6163 7469 6f6e 2873 656c  _interaction(sel
+00011dd0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00011de0: 2020 2020 736f 7572 6365 203d 2022 636c      source = "cl
+00011df0: 6173 7320 413a 5c5c 5c72 5c6e 2320 7479  ass A:\\\r\n# ty
+00011e00: 7065 3a20 6967 6e6f 7265 5c6e 2070 6173  pe: ignore\n pas
+00011e10: 735c 6e22 0a20 2020 2020 2020 206f 7574  s\n".        out
+00011e20: 7075 7420 3d20 6365 7263 6973 2e66 6f72  put = cercis.for
+00011e30: 6d61 745f 7374 7228 736f 7572 6365 2c20  mat_str(source, 
+00011e40: 6d6f 6465 3d44 4546 4155 4c54 5f4d 4f44  mode=DEFAULT_MOD
+00011e50: 4529 0a20 2020 2020 2020 2063 6572 6369  E).        cerci
+00011e60: 732e 6173 7365 7274 5f73 7461 626c 6528  s.assert_stable(
+00011e70: 736f 7572 6365 2c20 6f75 7470 7574 2c20  source, output, 
+00011e80: 6d6f 6465 3d44 4546 4155 4c54 5f4d 4f44  mode=DEFAULT_MOD
+00011e90: 4529 0a0a 2020 2020 6465 6620 7465 7374  E)..    def test
+00011ea0: 5f62 706f 5f32 3134 325f 776f 726b 6172  _bpo_2142_workar
+00011eb0: 6f75 6e64 2873 656c 6629 202d 3e20 4e6f  ound(self) -> No
+00011ec0: 6e65 3a0a 2020 2020 2020 2020 2320 6874  ne:.        # ht
+00011ed0: 7470 733a 2f2f 6275 6773 2e70 7974 686f  tps://bugs.pytho
+00011ee0: 6e2e 6f72 672f 6973 7375 6532 3134 320a  n.org/issue2142.
+00011ef0: 0a20 2020 2020 2020 2073 6f75 7263 652c  .        source,
+00011f00: 205f 203d 2072 6561 645f 6461 7461 2822   _ = read_data("
+00011f10: 6d69 7363 656c 6c61 6e65 6f75 7322 2c20  miscellaneous", 
+00011f20: 226d 6973 7369 6e67 5f66 696e 616c 5f6e  "missing_final_n
+00011f30: 6577 6c69 6e65 2229 0a20 2020 2020 2020  ewline").       
+00011f40: 2023 2072 6561 645f 6461 7461 2061 6464   # read_data add
+00011f50: 7320 6120 7472 6169 6c69 6e67 206e 6577  s a trailing new
+00011f60: 6c69 6e65 0a20 2020 2020 2020 2073 6f75  line.        sou
+00011f70: 7263 6520 3d20 736f 7572 6365 2e72 7374  rce = source.rst
+00011f80: 7269 7028 290a 2020 2020 2020 2020 6578  rip().        ex
+00011f90: 7065 6374 6564 2c20 5f20 3d20 7265 6164  pected, _ = read
+00011fa0: 5f64 6174 6128 226d 6973 6365 6c6c 616e  _data("miscellan
+00011fb0: 656f 7573 222c 2022 6d69 7373 696e 675f  eous", "missing_
+00011fc0: 6669 6e61 6c5f 6e65 776c 696e 652e 6469  final_newline.di
+00011fd0: 6666 2229 0a20 2020 2020 2020 2074 6d70  ff").        tmp
+00011fe0: 5f66 696c 6520 3d20 5061 7468 2863 6572  _file = Path(cer
+00011ff0: 6369 732e 6475 6d70 5f74 6f5f 6669 6c65  cis.dump_to_file
+00012000: 2873 6f75 7263 652c 2065 6e73 7572 655f  (source, ensure_
+00012010: 6669 6e61 6c5f 6e65 776c 696e 653d 4661  final_newline=Fa
+00012020: 6c73 6529 290a 2020 2020 2020 2020 6469  lse)).        di
+00012030: 6666 5f68 6561 6465 7220 3d20 7265 2e63  ff_header = re.c
+00012040: 6f6d 7069 6c65 280a 2020 2020 2020 2020  ompile(.        
+00012050: 2020 2020 7266 227b 7265 2e65 7363 6170      rf"{re.escap
+00012060: 6528 7374 7228 746d 705f 6669 6c65 2929  e(str(tmp_file))
+00012070: 7d5c 745c 645c 645c 645c 642d 5c64 5c64  }\t\d\d\d\d-\d\d
+00012080: 2d5c 645c 6420 220a 2020 2020 2020 2020  -\d\d ".        
+00012090: 2020 2020 7222 5c64 5c64 3a5c 645c 643a      r"\d\d:\d\d:
+000120a0: 5c64 5c64 5c2e 5c64 5c64 5c64 5c64 5c64  \d\d\.\d\d\d\d\d
+000120b0: 5c64 5c2b 5c64 5c64 3a5c 645c 6422 0a20  \d\+\d\d:\d\d". 
+000120c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000120d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+000120e0: 2020 7265 7375 6c74 203d 2042 6c61 636b    result = Black
+000120f0: 5275 6e6e 6572 2829 2e69 6e76 6f6b 6528  Runner().invoke(
+00012100: 6365 7263 6973 2e6d 6169 6e2c 205b 222d  cercis.main, ["-
+00012110: 2d64 6966 6622 2c20 7374 7228 746d 705f  -diff", str(tmp_
+00012120: 6669 6c65 295d 290a 2020 2020 2020 2020  file)]).        
+00012130: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00012140: 7175 616c 2872 6573 756c 742e 6578 6974  qual(result.exit
+00012150: 5f63 6f64 652c 2030 290a 2020 2020 2020  _code, 0).      
+00012160: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
+00012170: 2020 2020 2020 206f 732e 756e 6c69 6e6b         os.unlink
+00012180: 2874 6d70 5f66 696c 6529 0a20 2020 2020  (tmp_file).     
+00012190: 2020 2061 6374 7561 6c20 3d20 7265 7375     actual = resu
+000121a0: 6c74 2e6f 7574 7075 740a 2020 2020 2020  lt.output.      
+000121b0: 2020 6163 7475 616c 203d 2064 6966 665f    actual = diff_
+000121c0: 6865 6164 6572 2e73 7562 2844 4554 4552  header.sub(DETER
+000121d0: 4d49 4e49 5354 4943 5f48 4541 4445 522c  MINISTIC_HEADER,
+000121e0: 2061 6374 7561 6c29 0a20 2020 2020 2020   actual).       
+000121f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00012200: 6c28 6163 7475 616c 2c20 6578 7065 6374  l(actual, expect
+00012210: 6564 290a 0a20 2020 2040 7374 6174 6963  ed)..    @static
+00012220: 6d65 7468 6f64 0a20 2020 2064 6566 2063  method.    def c
+00012230: 6f6d 7061 7265 5f72 6573 756c 7473 280a  ompare_results(.
+00012240: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00012250: 6c74 3a20 636c 6963 6b2e 7465 7374 696e  lt: click.testin
+00012260: 672e 5265 7375 6c74 2c20 6578 7065 6374  g.Result, expect
+00012270: 6564 5f76 616c 7565 3a20 7374 722c 2065  ed_value: str, e
+00012280: 7870 6563 7465 645f 6578 6974 5f63 6f64  xpected_exit_cod
+00012290: 653a 2069 6e74 0a20 2020 2029 202d 3e20  e: int.    ) -> 
+000122a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000122b0: 2248 656c 7065 7220 6d65 7468 6f64 2074  "Helper method t
+000122c0: 6f20 7465 7374 2074 6865 2076 616c 7565  o test the value
+000122d0: 2061 6e64 2065 7869 7420 636f 6465 206f   and exit code o
+000122e0: 6620 6120 636c 6963 6b20 5265 7375 6c74  f a click Result
+000122f0: 2e22 2222 0a20 2020 2020 2020 2061 7373  .""".        ass
+00012300: 6572 7420 280a 2020 2020 2020 2020 2020  ert (.          
+00012310: 2020 7265 7375 6c74 2e6f 7574 7075 7420    result.output 
+00012320: 3d3d 2065 7870 6563 7465 645f 7661 6c75  == expected_valu
+00012330: 650a 2020 2020 2020 2020 292c 2022 5468  e.        ), "Th
+00012340: 6520 6f75 7470 7574 2064 6964 206e 6f74  e output did not
+00012350: 206d 6174 6368 2074 6865 2065 7870 6563   match the expec
+00012360: 7465 6420 7661 6c75 652e 220a 2020 2020  ted value.".    
+00012370: 2020 2020 6173 7365 7274 2072 6573 756c      assert resul
+00012380: 742e 6578 6974 5f63 6f64 6520 3d3d 2065  t.exit_code == e
+00012390: 7870 6563 7465 645f 6578 6974 5f63 6f64  xpected_exit_cod
+000123a0: 652c 2022 5468 6520 6578 6974 2063 6f64  e, "The exit cod
+000123b0: 6520 6973 2069 6e63 6f72 7265 6374 2e22  e is incorrect."
+000123c0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
+000123d0: 6f64 655f 6f70 7469 6f6e 2873 656c 6629  ode_option(self)
+000123e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000123f0: 2020 2222 2254 6573 7420 7468 6520 636f    """Test the co
+00012400: 6465 206f 7074 696f 6e20 7769 7468 206e  de option with n
+00012410: 6f20 6368 616e 6765 732e 2222 220a 2020  o changes.""".  
+00012420: 2020 2020 2020 636f 6465 203d 2022 7072        code = "pr
+00012430: 696e 7428 2748 656c 6c6f 2077 6f72 6c64  int('Hello world
+00012440: 2729 5c6e 220a 2020 2020 2020 2020 6172  ')\n".        ar
+00012450: 6773 203d 205b 222d 2d63 6f64 6522 2c20  gs = ["--code", 
+00012460: 636f 6465 2c20 222d 2d73 696e 676c 652d  code, "--single-
+00012470: 7175 6f74 653d 5472 7565 225d 0a20 2020  quote=True"].   
+00012480: 2020 2020 2072 6573 756c 7420 3d20 436c       result = Cl
+00012490: 6952 756e 6e65 7228 292e 696e 766f 6b65  iRunner().invoke
+000124a0: 2863 6572 6369 732e 6d61 696e 2c20 6172  (cercis.main, ar
+000124b0: 6773 290a 0a20 2020 2020 2020 2073 656c  gs)..        sel
+000124c0: 662e 636f 6d70 6172 655f 7265 7375 6c74  f.compare_result
+000124d0: 7328 7265 7375 6c74 2c20 636f 6465 2c20  s(result, code, 
+000124e0: 3029 0a0a 2020 2020 6465 6620 7465 7374  0)..    def test
+000124f0: 5f63 6f64 655f 6f70 7469 6f6e 5f63 6861  _code_option_cha
+00012500: 6e67 6564 2873 656c 6629 202d 3e20 4e6f  nged(self) -> No
+00012510: 6e65 3a0a 2020 2020 2020 2020 2222 2254  ne:.        """T
+00012520: 6573 7420 7468 6520 636f 6465 206f 7074  est the code opt
+00012530: 696f 6e20 7768 656e 2063 6861 6e67 6573  ion when changes
+00012540: 2061 7265 2072 6571 7569 7265 642e 2222   are required.""
+00012550: 220a 2020 2020 2020 2020 636f 6465 203d  ".        code =
+00012560: 2027 7072 696e 7428 2268 656c 6c6f 2077   'print("hello w
+00012570: 6f72 6c64 2229 270a 2020 2020 2020 2020  orld")'.        
+00012580: 666f 726d 6174 7465 6420 3d20 6365 7263  formatted = cerc
+00012590: 6973 2e66 6f72 6d61 745f 7374 7228 636f  is.format_str(co
+000125a0: 6465 2c20 6d6f 6465 3d44 4546 4155 4c54  de, mode=DEFAULT
+000125b0: 5f4d 4f44 4529 0a0a 2020 2020 2020 2020  _MODE)..        
+000125c0: 6172 6773 203d 205b 222d 2d63 6f64 6522  args = ["--code"
+000125d0: 2c20 636f 6465 2c20 222d 2d73 696e 676c  , code, "--singl
+000125e0: 652d 7175 6f74 653d 5472 7565 225d 0a20  e-quote=True"]. 
+000125f0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00012600: 436c 6952 756e 6e65 7228 292e 696e 766f  CliRunner().invo
+00012610: 6b65 2863 6572 6369 732e 6d61 696e 2c20  ke(cercis.main, 
+00012620: 6172 6773 290a 0a20 2020 2020 2020 2073  args)..        s
+00012630: 656c 662e 636f 6d70 6172 655f 7265 7375  elf.compare_resu
+00012640: 6c74 7328 7265 7375 6c74 2c20 666f 726d  lts(result, form
+00012650: 6174 7465 642c 2030 290a 0a20 2020 2064  atted, 0)..    d
+00012660: 6566 2074 6573 745f 636f 6465 5f6f 7074  ef test_code_opt
+00012670: 696f 6e5f 6368 6563 6b28 7365 6c66 2920  ion_check(self) 
+00012680: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00012690: 2022 2222 5465 7374 2074 6865 2063 6f64   """Test the cod
+000126a0: 6520 6f70 7469 6f6e 2077 6865 6e20 6368  e option when ch
+000126b0: 6563 6b20 6973 2070 6173 7365 642e 2222  eck is passed.""
+000126c0: 220a 2020 2020 2020 2020 6172 6773 203d  ".        args =
+000126d0: 205b 222d 2d63 6865 636b 222c 2022 2d2d   ["--check", "--
+000126e0: 636f 6465 222c 2027 7072 696e 7428 2248  code", 'print("H
+000126f0: 656c 6c6f 2077 6f72 6c64 2229 5c6e 275d  ello world")\n']
+00012700: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00012710: 3d20 436c 6952 756e 6e65 7228 292e 696e  = CliRunner().in
+00012720: 766f 6b65 2863 6572 6369 732e 6d61 696e  voke(cercis.main
+00012730: 2c20 6172 6773 290a 2020 2020 2020 2020  , args).        
+00012740: 7365 6c66 2e63 6f6d 7061 7265 5f72 6573  self.compare_res
+00012750: 756c 7473 2872 6573 756c 742c 2022 222c  ults(result, "",
+00012760: 2030 290a 0a20 2020 2064 6566 2074 6573   0)..    def tes
+00012770: 745f 636f 6465 5f6f 7074 696f 6e5f 6368  t_code_option_ch
+00012780: 6563 6b5f 6368 616e 6765 6428 7365 6c66  eck_changed(self
+00012790: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000127a0: 2020 2022 2222 5465 7374 2074 6865 2063     """Test the c
+000127b0: 6f64 6520 6f70 7469 6f6e 2077 6865 6e20  ode option when 
+000127c0: 6368 616e 6765 7320 6172 6520 7265 7175  changes are requ
+000127d0: 6972 6564 2c20 616e 6420 6368 6563 6b20  ired, and check 
+000127e0: 6973 2070 6173 7365 642e 2222 220a 2020  is passed.""".  
+000127f0: 2020 2020 2020 6172 6773 203d 205b 222d        args = ["-
+00012800: 2d63 6865 636b 222c 2022 2d2d 636f 6465  -check", "--code
+00012810: 222c 2022 7072 696e 7428 2768 656c 6c6f  ", "print('hello
+00012820: 2077 6f72 6c64 2729 225d 0a20 2020 2020   world')"].     
+00012830: 2020 2072 6573 756c 7420 3d20 436c 6952     result = CliR
+00012840: 756e 6e65 7228 292e 696e 766f 6b65 2863  unner().invoke(c
+00012850: 6572 6369 732e 6d61 696e 2c20 6172 6773  ercis.main, args
+00012860: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00012870: 6f6d 7061 7265 5f72 6573 756c 7473 2872  ompare_results(r
+00012880: 6573 756c 742c 2022 222c 2031 290a 0a20  esult, "", 1).. 
+00012890: 2020 2064 6566 2074 6573 745f 636f 6465     def test_code
+000128a0: 5f6f 7074 696f 6e5f 6469 6666 2873 656c  _option_diff(sel
+000128b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+000128c0: 2020 2020 2222 2254 6573 7420 7468 6520      """Test the 
+000128d0: 636f 6465 206f 7074 696f 6e20 7768 656e  code option when
+000128e0: 2064 6966 6620 6973 2070 6173 7365 642e   diff is passed.
+000128f0: 2222 220a 2020 2020 2020 2020 636f 6465  """.        code
+00012900: 203d 2027 7072 696e 7428 2268 656c 6c6f   = 'print("hello
+00012910: 2077 6f72 6c64 2229 270a 2020 2020 2020   world")'.      
+00012920: 2020 666f 726d 6174 7465 6420 3d20 6365    formatted = ce
+00012930: 7263 6973 2e66 6f72 6d61 745f 7374 7228  rcis.format_str(
+00012940: 636f 6465 2c20 6d6f 6465 3d44 4546 4155  code, mode=DEFAU
+00012950: 4c54 5f4d 4f44 4529 0a20 2020 2020 2020  LT_MODE).       
+00012960: 2072 6573 756c 745f 6469 6666 203d 2064   result_diff = d
+00012970: 6966 6628 636f 6465 2c20 666f 726d 6174  iff(code, format
+00012980: 7465 642c 2022 5354 4449 4e22 2c20 2253  ted, "STDIN", "S
+00012990: 5444 4f55 5422 290a 0a20 2020 2020 2020  TDOUT")..       
+000129a0: 2061 7267 7320 3d20 5b22 2d2d 6469 6666   args = ["--diff
+000129b0: 222c 2022 2d2d 636f 6465 222c 2063 6f64  ", "--code", cod
+000129c0: 652c 2022 2d2d 7369 6e67 6c65 2d71 756f  e, "--single-quo
+000129d0: 7465 3d54 7275 6522 5d0a 2020 2020 2020  te=True"].      
+000129e0: 2020 7265 7375 6c74 203d 2043 6c69 5275    result = CliRu
+000129f0: 6e6e 6572 2829 2e69 6e76 6f6b 6528 6365  nner().invoke(ce
+00012a00: 7263 6973 2e6d 6169 6e2c 2061 7267 7329  rcis.main, args)
+00012a10: 0a0a 2020 2020 2020 2020 2320 5265 6d6f  ..        # Remo
+00012a20: 7665 2074 696d 6520 6672 6f6d 2064 6966  ve time from dif
+00012a30: 660a 2020 2020 2020 2020 6f75 7470 7574  f.        output
+00012a40: 203d 2044 4946 465f 5449 4d45 2e73 7562   = DIFF_TIME.sub
+00012a50: 2822 222c 2072 6573 756c 742e 6f75 7470  ("", result.outp
+00012a60: 7574 290a 0a20 2020 2020 2020 2061 7373  ut)..        ass
+00012a70: 6572 7420 6f75 7470 7574 203d 3d20 7265  ert output == re
+00012a80: 7375 6c74 5f64 6966 662c 2022 5468 6520  sult_diff, "The 
+00012a90: 6f75 7470 7574 2064 6964 206e 6f74 206d  output did not m
+00012aa0: 6174 6368 2074 6865 2065 7870 6563 7465  atch the expecte
+00012ab0: 6420 7661 6c75 652e 220a 2020 2020 2020  d value.".      
+00012ac0: 2020 6173 7365 7274 2072 6573 756c 742e    assert result.
+00012ad0: 6578 6974 5f63 6f64 6520 3d3d 2030 2c20  exit_code == 0, 
+00012ae0: 2254 6865 2065 7869 7420 636f 6465 2069  "The exit code i
+00012af0: 7320 696e 636f 7272 6563 742e 220a 0a20  s incorrect.".. 
+00012b00: 2020 2064 6566 2074 6573 745f 636f 6465     def test_code
+00012b10: 5f6f 7074 696f 6e5f 636f 6c6f 725f 6469  _option_color_di
+00012b20: 6666 2873 656c 6629 202d 3e20 4e6f 6e65  ff(self) -> None
+00012b30: 3a0a 2020 2020 2020 2020 2222 2254 6573  :.        """Tes
+00012b40: 7420 7468 6520 636f 6465 206f 7074 696f  t the code optio
+00012b50: 6e20 7768 656e 2063 6f6c 6f72 2061 6e64  n when color and
+00012b60: 2064 6966 6620 6172 6520 7061 7373 6564   diff are passed
+00012b70: 2e22 2222 0a20 2020 2020 2020 2063 6f64  .""".        cod
+00012b80: 6520 3d20 2770 7269 6e74 2822 6865 6c6c  e = 'print("hell
+00012b90: 6f20 776f 726c 6422 2927 0a20 2020 2020  o world")'.     
+00012ba0: 2020 2066 6f72 6d61 7474 6564 203d 2063     formatted = c
+00012bb0: 6572 6369 732e 666f 726d 6174 5f73 7472  ercis.format_str
+00012bc0: 2863 6f64 652c 206d 6f64 653d 4445 4641  (code, mode=DEFA
+00012bd0: 554c 545f 4d4f 4445 290a 0a20 2020 2020  ULT_MODE)..     
+00012be0: 2020 2072 6573 756c 745f 6469 6666 203d     result_diff =
+00012bf0: 2064 6966 6628 636f 6465 2c20 666f 726d   diff(code, form
+00012c00: 6174 7465 642c 2022 5354 4449 4e22 2c20  atted, "STDIN", 
+00012c10: 2253 5444 4f55 5422 290a 2020 2020 2020  "STDOUT").      
+00012c20: 2020 7265 7375 6c74 5f64 6966 6620 3d20    result_diff = 
+00012c30: 636f 6c6f 725f 6469 6666 2872 6573 756c  color_diff(resul
+00012c40: 745f 6469 6666 290a 0a20 2020 2020 2020  t_diff)..       
+00012c50: 2061 7267 7320 3d20 5b22 2d2d 6469 6666   args = ["--diff
+00012c60: 222c 2022 2d2d 636f 6c6f 7222 2c20 222d  ", "--color", "-
+00012c70: 2d63 6f64 6522 2c20 636f 6465 2c20 222d  -code", code, "-
+00012c80: 2d73 696e 676c 652d 7175 6f74 653d 5472  -single-quote=Tr
+00012c90: 7565 225d 0a20 2020 2020 2020 2072 6573  ue"].        res
+00012ca0: 756c 7420 3d20 436c 6952 756e 6e65 7228  ult = CliRunner(
+00012cb0: 292e 696e 766f 6b65 2863 6572 6369 732e  ).invoke(cercis.
+00012cc0: 6d61 696e 2c20 6172 6773 290a 0a20 2020  main, args)..   
+00012cd0: 2020 2020 2023 2052 656d 6f76 6520 7469       # Remove ti
+00012ce0: 6d65 2066 726f 6d20 6469 6666 0a20 2020  me from diff.   
+00012cf0: 2020 2020 206f 7574 7075 7420 3d20 4449       output = DI
+00012d00: 4646 5f54 494d 452e 7375 6228 2222 2c20  FF_TIME.sub("", 
+00012d10: 7265 7375 6c74 2e6f 7574 7075 7429 0a0a  result.output)..
+00012d20: 2020 2020 2020 2020 6173 7365 7274 206f          assert o
+00012d30: 7574 7075 7420 3d3d 2072 6573 756c 745f  utput == result_
+00012d40: 6469 6666 2c20 2254 6865 206f 7574 7075  diff, "The outpu
+00012d50: 7420 6469 6420 6e6f 7420 6d61 7463 6820  t did not match 
+00012d60: 7468 6520 6578 7065 6374 6564 2076 616c  the expected val
+00012d70: 7565 2e22 0a20 2020 2020 2020 2061 7373  ue.".        ass
+00012d80: 6572 7420 7265 7375 6c74 2e65 7869 745f  ert result.exit_
+00012d90: 636f 6465 203d 3d20 302c 2022 5468 6520  code == 0, "The 
+00012da0: 6578 6974 2063 6f64 6520 6973 2069 6e63  exit code is inc
+00012db0: 6f72 7265 6374 2e22 0a0a 2020 2020 4070  orrect."..    @p
+00012dc0: 7974 6573 742e 6d61 726b 2e69 6e63 6f6d  ytest.mark.incom
+00012dd0: 7061 7469 626c 655f 7769 7468 5f6d 7970  patible_with_myp
+00012de0: 7963 0a20 2020 2064 6566 2074 6573 745f  yc.    def test_
+00012df0: 636f 6465 5f6f 7074 696f 6e5f 7361 6665  code_option_safe
+00012e00: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00012e10: 2020 2020 2020 2020 2222 2254 6573 7420          """Test 
+00012e20: 7468 6174 2074 6865 2063 6f64 6520 6f70  that the code op
+00012e30: 7469 6f6e 2074 6872 6f77 7320 616e 2065  tion throws an e
+00012e40: 7272 6f72 2077 6865 6e20 7468 6520 7361  rror when the sa
+00012e50: 6e69 7479 2063 6865 636b 7320 6661 696c  nity checks fail
+00012e60: 2e22 2222 0a20 2020 2020 2020 2023 2050  .""".        # P
+00012e70: 6174 6368 2063 6572 6369 732e 6173 7365  atch cercis.asse
+00012e80: 7274 5f65 7175 6976 616c 656e 7420 746f  rt_equivalent to
+00012e90: 2065 6e73 7572 6520 7468 6520 7361 6e69   ensure the sani
+00012ea0: 7479 2063 6865 636b 7320 6661 696c 0a20  ty checks fail. 
+00012eb0: 2020 2020 2020 2077 6974 6820 7061 7463         with patc
+00012ec0: 682e 6f62 6a65 6374 2863 6572 6369 732c  h.object(cercis,
+00012ed0: 2022 6173 7365 7274 5f65 7175 6976 616c   "assert_equival
+00012ee0: 656e 7422 2c20 7369 6465 5f65 6666 6563  ent", side_effec
+00012ef0: 743d 4173 7365 7274 696f 6e45 7272 6f72  t=AssertionError
+00012f00: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00012f10: 6f64 6520 3d20 2770 7269 6e74 2822 4865  ode = 'print("He
+00012f20: 6c6c 6f20 776f 726c 6422 2927 0a20 2020  llo world")'.   
+00012f30: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
+00012f40: 7367 203d 2066 227b 636f 6465 7d5c 6e65  sg = f"{code}\ne
+00012f50: 7272 6f72 3a20 6361 6e6e 6f74 2066 6f72  rror: cannot for
+00012f60: 6d61 7420 3c73 7472 696e 673e 3a20 5c6e  mat <string>: \n
+00012f70: 220a 0a20 2020 2020 2020 2020 2020 2061  "..            a
+00012f80: 7267 7320 3d20 5b22 2d2d 7361 6665 222c  rgs = ["--safe",
+00012f90: 2022 2d2d 636f 6465 222c 2063 6f64 655d   "--code", code]
+00012fa0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00012fb0: 756c 7420 3d20 436c 6952 756e 6e65 7228  ult = CliRunner(
+00012fc0: 292e 696e 766f 6b65 2863 6572 6369 732e  ).invoke(cercis.
+00012fd0: 6d61 696e 2c20 6172 6773 290a 0a20 2020  main, args)..   
+00012fe0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00012ff0: 6d70 6172 655f 7265 7375 6c74 7328 7265  mpare_results(re
+00013000: 7375 6c74 2c20 6572 726f 725f 6d73 672c  sult, error_msg,
+00013010: 2031 3233 290a 0a20 2020 2064 6566 2074   123)..    def t
+00013020: 6573 745f 636f 6465 5f6f 7074 696f 6e5f  est_code_option_
+00013030: 6661 7374 2873 656c 6629 202d 3e20 4e6f  fast(self) -> No
+00013040: 6e65 3a0a 2020 2020 2020 2020 2222 2254  ne:.        """T
+00013050: 6573 7420 7468 6174 2074 6865 2063 6f64  est that the cod
+00013060: 6520 6f70 7469 6f6e 2069 676e 6f72 6573  e option ignores
+00013070: 2065 7272 6f72 7320 7768 656e 2074 6865   errors when the
+00013080: 2073 616e 6974 7920 6368 6563 6b73 2066   sanity checks f
+00013090: 6169 6c2e 2222 220a 2020 2020 2020 2020  ail.""".        
+000130a0: 2320 5061 7463 6820 6365 7263 6973 2e61  # Patch cercis.a
+000130b0: 7373 6572 745f 6571 7569 7661 6c65 6e74  ssert_equivalent
+000130c0: 2074 6f20 656e 7375 7265 2074 6865 2073   to ensure the s
+000130d0: 616e 6974 7920 6368 6563 6b73 2066 6169  anity checks fai
+000130e0: 6c0a 2020 2020 2020 2020 7769 7468 2070  l.        with p
+000130f0: 6174 6368 2e6f 626a 6563 7428 6365 7263  atch.object(cerc
+00013100: 6973 2c20 2261 7373 6572 745f 6571 7569  is, "assert_equi
+00013110: 7661 6c65 6e74 222c 2073 6964 655f 6566  valent", side_ef
+00013120: 6665 6374 3d41 7373 6572 7469 6f6e 4572  fect=AssertionEr
+00013130: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+00013140: 2020 636f 6465 203d 2022 7072 696e 7428    code = "print(
+00013150: 2748 656c 6c6f 2077 6f72 6c64 2729 220a  'Hello world')".
+00013160: 2020 2020 2020 2020 2020 2020 666f 726d              form
+00013170: 6174 7465 6420 3d20 6365 7263 6973 2e66  atted = cercis.f
+00013180: 6f72 6d61 745f 7374 7228 636f 6465 2c20  ormat_str(code, 
+00013190: 6d6f 6465 3d44 4546 4155 4c54 5f4d 4f44  mode=DEFAULT_MOD
+000131a0: 4529 0a0a 2020 2020 2020 2020 2020 2020  E)..            
+000131b0: 6172 6773 203d 205b 222d 2d66 6173 7422  args = ["--fast"
+000131c0: 2c20 222d 2d63 6f64 6522 2c20 636f 6465  , "--code", code
+000131d0: 2c20 222d 2d73 696e 676c 652d 7175 6f74  , "--single-quot
+000131e0: 653d 5472 7565 225d 0a20 2020 2020 2020  e=True"].       
+000131f0: 2020 2020 2072 6573 756c 7420 3d20 436c       result = Cl
+00013200: 6952 756e 6e65 7228 292e 696e 766f 6b65  iRunner().invoke
+00013210: 2863 6572 6369 732e 6d61 696e 2c20 6172  (cercis.main, ar
+00013220: 6773 290a 0a20 2020 2020 2020 2020 2020  gs)..           
+00013230: 2073 656c 662e 636f 6d70 6172 655f 7265   self.compare_re
+00013240: 7375 6c74 7328 7265 7375 6c74 2c20 666f  sults(result, fo
+00013250: 726d 6174 7465 642c 2030 290a 0a20 2020  rmatted, 0)..   
+00013260: 2040 7079 7465 7374 2e6d 6172 6b2e 696e   @pytest.mark.in
+00013270: 636f 6d70 6174 6962 6c65 5f77 6974 685f  compatible_with_
+00013280: 6d79 7079 630a 2020 2020 6465 6620 7465  mypyc.    def te
+00013290: 7374 5f63 6f64 655f 6f70 7469 6f6e 5f63  st_code_option_c
+000132a0: 6f6e 6669 6728 7365 6c66 2920 2d3e 204e  onfig(self) -> N
+000132b0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000132c0: 0a20 2020 2020 2020 2054 6573 7420 7468  .        Test th
+000132d0: 6174 2074 6865 2063 6f64 6520 6f70 7469  at the code opti
+000132e0: 6f6e 2066 696e 6473 2074 6865 2070 7970  on finds the pyp
+000132f0: 726f 6a65 6374 2e74 6f6d 6c20 696e 2074  roject.toml in t
+00013300: 6865 2063 7572 7265 6e74 2064 6972 6563  he current direc
+00013310: 746f 7279 2e0a 2020 2020 2020 2020 2222  tory..        ""
+00013320: 220a 2020 2020 2020 2020 7769 7468 2070  ".        with p
+00013330: 6174 6368 2e6f 626a 6563 7428 6365 7263  atch.object(cerc
+00013340: 6973 2c20 2270 6172 7365 5f70 7970 726f  is, "parse_pypro
+00013350: 6a65 6374 5f74 6f6d 6c22 2c20 7265 7475  ject_toml", retu
+00013360: 726e 5f76 616c 7565 3d7b 7d29 2061 7320  rn_value={}) as 
+00013370: 7061 7273 653a 0a20 2020 2020 2020 2020  parse:.         
+00013380: 2020 2061 7267 7320 3d20 5b22 2d2d 636f     args = ["--co
+00013390: 6465 222c 2022 7072 696e 7422 5d0a 2020  de", "print"].  
+000133a0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
+000133b0: 2069 7320 7468 6520 6f6e 6c79 2064 6972   is the only dir
+000133c0: 6563 746f 7279 206b 6e6f 776e 2074 6f20  ectory known to 
+000133d0: 636f 6e74 6169 6e20 6120 7079 7072 6f6a  contain a pyproj
+000133e0: 6563 742e 746f 6d6c 0a20 2020 2020 2020  ect.toml.       
+000133f0: 2020 2020 2077 6974 6820 6368 616e 6765       with change
+00013400: 5f64 6972 6563 746f 7279 2850 524f 4a45  _directory(PROJE
+00013410: 4354 5f52 4f4f 5429 3a0a 2020 2020 2020  CT_ROOT):.      
+00013420: 2020 2020 2020 2020 2020 436c 6952 756e            CliRun
+00013430: 6e65 7228 292e 696e 766f 6b65 2863 6572  ner().invoke(cer
+00013440: 6369 732e 6d61 696e 2c20 6172 6773 290a  cis.main, args).
+00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013460: 7079 7072 6f6a 6563 745f 7061 7468 203d  pyproject_path =
+00013470: 2050 6174 6828 5061 7468 2e63 7764 2829   Path(Path.cwd()
+00013480: 2c20 2270 7970 726f 6a65 6374 2e74 6f6d  , "pyproject.tom
+00013490: 6c22 292e 7265 736f 6c76 6528 290a 0a20  l").resolve().. 
+000134a0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000134b0: 7420 280a 2020 2020 2020 2020 2020 2020  t (.            
+000134c0: 2020 2020 6c65 6e28 7061 7273 652e 6d6f      len(parse.mo
+000134d0: 636b 5f63 616c 6c73 2920 3e3d 2031 0a20  ck_calls) >= 1. 
+000134e0: 2020 2020 2020 2020 2020 2029 2c20 2245             ), "E
+000134f0: 7870 6563 7465 6420 636f 6e66 6967 2070  xpected config p
+00013500: 6172 7365 2074 6f20 6265 2063 616c 6c65  arse to be calle
+00013510: 6420 7769 7468 2074 6865 2063 7572 7265  d with the curre
+00013520: 6e74 2064 6972 6563 746f 7279 2e22 0a0a  nt directory."..
+00013530: 2020 2020 2020 2020 2020 2020 5f2c 2063              _, c
+00013540: 616c 6c5f 6172 6773 2c20 5f20 3d20 7061  all_args, _ = pa
+00013550: 7273 652e 6d6f 636b 5f63 616c 6c73 5b30  rse.mock_calls[0
+00013560: 5d0a 2020 2020 2020 2020 2020 2020 6173  ].            as
+00013570: 7365 7274 2028 0a20 2020 2020 2020 2020  sert (.         
+00013580: 2020 2020 2020 2063 616c 6c5f 6172 6773         call_args
+00013590: 5b30 5d2e 6c6f 7765 7228 2920 3d3d 2073  [0].lower() == s
+000135a0: 7472 2870 7970 726f 6a65 6374 5f70 6174  tr(pyproject_pat
+000135b0: 6829 2e6c 6f77 6572 2829 0a20 2020 2020  h).lower().     
+000135c0: 2020 2020 2020 2029 2c20 2249 6e63 6f72         ), "Incor
+000135d0: 7265 6374 2063 6f6e 6669 6720 6c6f 6164  rect config load
+000135e0: 6564 2e22 0a0a 2020 2020 4070 7974 6573  ed."..    @pytes
+000135f0: 742e 6d61 726b 2e69 6e63 6f6d 7061 7469  t.mark.incompati
+00013600: 626c 655f 7769 7468 5f6d 7970 7963 0a20  ble_with_mypyc. 
+00013610: 2020 2064 6566 2074 6573 745f 636f 6465     def test_code
+00013620: 5f6f 7074 696f 6e5f 7061 7265 6e74 5f63  _option_parent_c
+00013630: 6f6e 6669 6728 7365 6c66 2920 2d3e 204e  onfig(self) -> N
+00013640: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00013650: 0a20 2020 2020 2020 2054 6573 7420 7468  .        Test th
+00013660: 6174 2074 6865 2063 6f64 6520 6f70 7469  at the code opti
+00013670: 6f6e 2066 696e 6473 2074 6865 2070 7970  on finds the pyp
+00013680: 726f 6a65 6374 2e74 6f6d 6c20 696e 2074  roject.toml in t
+00013690: 6865 2070 6172 656e 7420 6469 7265 6374  he parent direct
+000136a0: 6f72 792e 0a20 2020 2020 2020 2022 2222  ory..        """
+000136b0: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
+000136c0: 7463 682e 6f62 6a65 6374 2863 6572 6369  tch.object(cerci
+000136d0: 732c 2022 7061 7273 655f 7079 7072 6f6a  s, "parse_pyproj
+000136e0: 6563 745f 746f 6d6c 222c 2072 6574 7572  ect_toml", retur
+000136f0: 6e5f 7661 6c75 653d 7b7d 2920 6173 2070  n_value={}) as p
+00013700: 6172 7365 3a0a 2020 2020 2020 2020 2020  arse:.          
+00013710: 2020 7769 7468 2063 6861 6e67 655f 6469    with change_di
+00013720: 7265 6374 6f72 7928 5448 4953 5f44 4952  rectory(THIS_DIR
+00013730: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00013740: 2020 2061 7267 7320 3d20 5b22 2d2d 636f     args = ["--co
+00013750: 6465 222c 2022 7072 696e 7422 5d0a 2020  de", "print"].  
+00013760: 2020 2020 2020 2020 2020 2020 2020 436c                Cl
+00013770: 6952 756e 6e65 7228 292e 696e 766f 6b65  iRunner().invoke
+00013780: 2863 6572 6369 732e 6d61 696e 2c20 6172  (cercis.main, ar
+00013790: 6773 290a 0a20 2020 2020 2020 2020 2020  gs)..           
+000137a0: 2020 2020 2070 7970 726f 6a65 6374 5f70       pyproject_p
+000137b0: 6174 6820 3d20 5061 7468 2850 6174 6828  ath = Path(Path(
+000137c0: 292e 6377 6428 292e 7061 7265 6e74 2c20  ).cwd().parent, 
+000137d0: 2270 7970 726f 6a65 6374 2e74 6f6d 6c22  "pyproject.toml"
+000137e0: 292e 7265 736f 6c76 6528 290a 2020 2020  ).resolve().    
+000137f0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00013800: 7274 2028 0a20 2020 2020 2020 2020 2020  rt (.           
+00013810: 2020 2020 2020 2020 206c 656e 2870 6172           len(par
+00013820: 7365 2e6d 6f63 6b5f 6361 6c6c 7329 203e  se.mock_calls) >
+00013830: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00013840: 2020 2020 292c 2022 4578 7065 6374 6564      ), "Expected
+00013850: 2063 6f6e 6669 6720 7061 7273 6520 746f   config parse to
+00013860: 2062 6520 6361 6c6c 6564 2077 6974 6820   be called with 
+00013870: 7468 6520 6375 7272 656e 7420 6469 7265  the current dire
+00013880: 6374 6f72 792e 220a 0a20 2020 2020 2020  ctory."..       
+00013890: 2020 2020 2020 2020 205f 2c20 6361 6c6c           _, call
+000138a0: 5f61 7267 732c 205f 203d 2070 6172 7365  _args, _ = parse
+000138b0: 2e6d 6f63 6b5f 6361 6c6c 735b 305d 0a20  .mock_calls[0]. 
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000138d0: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
+000138e0: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+000138f0: 5f61 7267 735b 305d 2e6c 6f77 6572 2829  _args[0].lower()
+00013900: 203d 3d20 7374 7228 7079 7072 6f6a 6563   == str(pyprojec
+00013910: 745f 7061 7468 292e 6c6f 7765 7228 290a  t_path).lower().
+00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013930: 292c 2022 496e 636f 7272 6563 7420 636f  ), "Incorrect co
+00013940: 6e66 6967 206c 6f61 6465 642e 220a 0a20  nfig loaded.".. 
+00013950: 2020 2064 6566 2074 6573 745f 666f 725f     def test_for_
+00013960: 6861 6e64 6c65 645f 756e 6578 7065 6374  handled_unexpect
+00013970: 6564 5f65 6f66 5f65 7272 6f72 2873 656c  ed_eof_error(sel
+00013980: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00013990: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000139a0: 5465 7374 2074 6861 7420 616e 2075 6e65  Test that an une
+000139b0: 7870 6563 7465 6420 454f 4620 5379 6e74  xpected EOF Synt
+000139c0: 6178 4572 726f 7220 6973 206e 6963 656c  axError is nicel
+000139d0: 7920 7072 6573 656e 7465 642e 0a20 2020  y presented..   
+000139e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000139f0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
+00013a00: 7365 7328 6365 7263 6973 2e70 6172 7369  ses(cercis.parsi
+00013a10: 6e67 2e49 6e76 616c 6964 496e 7075 7429  ng.InvalidInput)
+00013a20: 2061 7320 6578 635f 696e 666f 3a0a 2020   as exc_info:.  
+00013a30: 2020 2020 2020 2020 2020 6365 7263 6973            cercis
+00013a40: 2e6c 6962 3274 6f33 5f70 6172 7365 2822  .lib2to3_parse("
+00013a50: 7072 696e 7428 222c 207b 7d29 0a0a 2020  print(", {})..  
+00013a60: 2020 2020 2020 6578 635f 696e 666f 2e6d        exc_info.m
+00013a70: 6174 6368 2822 4361 6e6e 6f74 2070 6172  atch("Cannot par
+00013a80: 7365 3a20 323a 303a 2045 4f46 2069 6e20  se: 2:0: EOF in 
+00013a90: 6d75 6c74 692d 6c69 6e65 2073 7461 7465  multi-line state
+00013aa0: 6d65 6e74 2229 0a0a 2020 2020 6465 6620  ment")..    def 
+00013ab0: 7465 7374 5f65 7175 6976 616c 656e 6379  test_equivalency
+00013ac0: 5f61 7374 5f70 6172 7365 5f66 6169 6c75  _ast_parse_failu
+00013ad0: 7265 5f69 6e63 6c75 6465 735f 6572 726f  re_includes_erro
+00013ae0: 7228 7365 6c66 2920 2d3e 204e 6f6e 653a  r(self) -> None:
+00013af0: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+00013b00: 7465 7374 2e72 6169 7365 7328 4173 7365  test.raises(Asse
+00013b10: 7274 696f 6e45 7272 6f72 2920 6173 2065  rtionError) as e
+00013b20: 7272 3a0a 2020 2020 2020 2020 2020 2020  rr:.            
+00013b30: 6365 7263 6973 2e61 7373 6572 745f 6571  cercis.assert_eq
+00013b40: 7569 7661 6c65 6e74 2822 61c2 abc2 bb61  uivalent("a....a
+00013b50: 2020 3d20 3122 2c20 2261 c2ab c2bb 6120    = 1", "a....a 
+00013b60: 203d 2031 2229 0a0a 2020 2020 2020 2020   = 1")..        
+00013b70: 6572 722e 6d61 7463 6828 222d 2d73 6166  err.match("--saf
+00013b80: 6522 290a 2020 2020 2020 2020 2320 556e  e").        # Un
+00013b90: 666f 7274 756e 6174 656c 7920 7468 6520  fortunately the 
+00013ba0: 5379 6e74 6178 4572 726f 7220 6d65 7373  SyntaxError mess
+00013bb0: 6167 6520 6861 7320 6368 616e 6765 6420  age has changed 
+00013bc0: 696e 206e 6577 6572 2076 6572 7369 6f6e  in newer version
+00013bd0: 7320 736f 2077 650a 2020 2020 2020 2020  s so we.        
+00013be0: 2320 6361 6e27 7420 6d61 7463 6820 6974  # can't match it
+00013bf0: 2064 6972 6563 746c 792e 0a20 2020 2020   directly..     
+00013c00: 2020 2065 7272 2e6d 6174 6368 2822 696e     err.match("in
+00013c10: 7661 6c69 6420 6368 6172 6163 7465 7222  valid character"
+00013c20: 290a 2020 2020 2020 2020 6572 722e 6d61  ).        err.ma
+00013c30: 7463 6828 7222 5c28 3c75 6e6b 6e6f 776e  tch(r"\(<unknown
+00013c40: 3e2c 206c 696e 6520 315c 2922 290a 0a0a  >, line 1\)")...
+00013c50: 636c 6173 7320 5465 7374 4361 6368 696e  class TestCachin
+00013c60: 673a 0a20 2020 2064 6566 2074 6573 745f  g:.    def test_
+00013c70: 6765 745f 6361 6368 655f 6469 7228 0a20  get_cache_dir(. 
+00013c80: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00013c90: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
+00013ca0: 5f70 6174 683a 2050 6174 682c 0a20 2020  _path: Path,.   
+00013cb0: 2020 2020 2020 2020 206d 6f6e 6b65 7970           monkeyp
+00013cc0: 6174 6368 3a20 7079 7465 7374 2e4d 6f6e  atch: pytest.Mon
+00013cd0: 6b65 7950 6174 6368 2c0a 2020 2020 2920  keyPatch,.    ) 
+00013ce0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00013cf0: 2023 2043 7265 6174 6520 6d75 6c74 6970   # Create multip
+00013d00: 6c65 2063 6163 6865 2064 6972 6563 746f  le cache directo
+00013d10: 7269 6573 0a20 2020 2020 2020 2077 6f72  ries.        wor
+00013d20: 6b73 7061 6365 3120 3d20 746d 705f 7061  kspace1 = tmp_pa
+00013d30: 7468 202f 2022 7773 3122 0a20 2020 2020  th / "ws1".     
+00013d40: 2020 2077 6f72 6b73 7061 6365 312e 6d6b     workspace1.mk
+00013d50: 6469 7228 290a 2020 2020 2020 2020 776f  dir().        wo
+00013d60: 726b 7370 6163 6532 203d 2074 6d70 5f70  rkspace2 = tmp_p
+00013d70: 6174 6820 2f20 2277 7332 220a 2020 2020  ath / "ws2".    
+00013d80: 2020 2020 776f 726b 7370 6163 6532 2e6d      workspace2.m
+00013d90: 6b64 6972 2829 0a0a 2020 2020 2020 2020  kdir()..        
+00013da0: 2320 466f 7263 6520 7573 6572 5f63 6163  # Force user_cac
+00013db0: 6865 5f64 6972 2074 6f20 7573 6520 7468  he_dir to use th
+00013dc0: 6520 7465 6d70 6f72 6172 7920 6469 7265  e temporary dire
+00013dd0: 6374 6f72 7920 666f 7220 6561 7369 6572  ctory for easier
+00013de0: 2061 7373 6572 7469 6f6e 730a 2020 2020   assertions.    
+00013df0: 2020 2020 7061 7463 685f 7573 6572 5f63      patch_user_c
+00013e00: 6163 6865 5f64 6972 203d 2070 6174 6368  ache_dir = patch
+00013e10: 280a 2020 2020 2020 2020 2020 2020 7461  (.            ta
+00013e20: 7267 6574 3d22 6365 7263 6973 2e63 6163  rget="cercis.cac
+00013e30: 6865 2e75 7365 725f 6361 6368 655f 6469  he.user_cache_di
+00013e40: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00013e50: 6175 746f 7370 6563 3d54 7275 652c 0a20  autospec=True,. 
+00013e60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00013e70: 6e5f 7661 6c75 653d 7374 7228 776f 726b  n_value=str(work
+00013e80: 7370 6163 6531 292c 0a20 2020 2020 2020  space1),.       
+00013e90: 2029 0a0a 2020 2020 2020 2020 2320 4966   )..        # If
+00013ea0: 2042 4c41 434b 5f43 4143 4845 5f44 4952   BLACK_CACHE_DIR
+00013eb0: 2069 7320 6e6f 7420 7365 742c 2075 7365   is not set, use
+00013ec0: 2075 7365 725f 6361 6368 655f 6469 720a   user_cache_dir.
+00013ed0: 2020 2020 2020 2020 6d6f 6e6b 6579 7061          monkeypa
+00013ee0: 7463 682e 6465 6c65 6e76 2822 424c 4143  tch.delenv("BLAC
+00013ef0: 4b5f 4341 4348 455f 4449 5222 2c20 7261  K_CACHE_DIR", ra
+00013f00: 6973 696e 673d 4661 6c73 6529 0a20 2020  ising=False).   
+00013f10: 2020 2020 2077 6974 6820 7061 7463 685f       with patch_
+00013f20: 7573 6572 5f63 6163 6865 5f64 6972 3a0a  user_cache_dir:.
+00013f30: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00013f40: 7274 2067 6574 5f63 6163 6865 5f64 6972  rt get_cache_dir
+00013f50: 2829 203d 3d20 776f 726b 7370 6163 6531  () == workspace1
+00013f60: 0a0a 2020 2020 2020 2020 2320 4966 2069  ..        # If i
+00013f70: 7420 6973 2073 6574 2c20 7573 6520 7468  t is set, use th
+00013f80: 6520 7061 7468 2070 726f 7669 6465 6420  e path provided 
+00013f90: 696e 2074 6865 2065 6e76 2076 6172 2e0a  in the env var..
+00013fa0: 2020 2020 2020 2020 6d6f 6e6b 6579 7061          monkeypa
+00013fb0: 7463 682e 7365 7465 6e76 2822 424c 4143  tch.setenv("BLAC
+00013fc0: 4b5f 4341 4348 455f 4449 5222 2c20 7374  K_CACHE_DIR", st
+00013fd0: 7228 776f 726b 7370 6163 6532 2929 0a20  r(workspace2)). 
+00013fe0: 2020 2020 2020 2061 7373 6572 7420 6765         assert ge
+00013ff0: 745f 6361 6368 655f 6469 7228 2920 3d3d  t_cache_dir() ==
+00014000: 2077 6f72 6b73 7061 6365 320a 0a20 2020   workspace2..   
+00014010: 2064 6566 2074 6573 745f 6361 6368 655f   def test_cache_
+00014020: 6272 6f6b 656e 5f66 696c 6528 7365 6c66  broken_file(self
+00014030: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00014040: 2020 206d 6f64 6520 3d20 4445 4641 554c     mode = DEFAUL
+00014050: 545f 4d4f 4445 0a20 2020 2020 2020 2077  T_MODE.        w
+00014060: 6974 6820 6361 6368 655f 6469 7228 2920  ith cache_dir() 
+00014070: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
+00014080: 2020 2020 2020 2020 2020 6361 6368 655f            cache_
+00014090: 6669 6c65 203d 2067 6574 5f63 6163 6865  file = get_cache
+000140a0: 5f66 696c 6528 6d6f 6465 290a 2020 2020  _file(mode).    
+000140b0: 2020 2020 2020 2020 6361 6368 655f 6669          cache_fi
+000140c0: 6c65 2e77 7269 7465 5f74 6578 7428 2274  le.write_text("t
+000140d0: 6869 7320 6973 206e 6f74 2061 2070 6963  his is not a pic
+000140e0: 6b6c 6522 290a 2020 2020 2020 2020 2020  kle").          
+000140f0: 2020 6173 7365 7274 2063 6572 6369 732e    assert cercis.
+00014100: 7265 6164 5f63 6163 6865 286d 6f64 6529  read_cache(mode)
+00014110: 203d 3d20 7b7d 0a20 2020 2020 2020 2020   == {}.         
+00014120: 2020 2073 7263 203d 2028 776f 726b 7370     src = (worksp
+00014130: 6163 6520 2f20 2274 6573 742e 7079 2229  ace / "test.py")
+00014140: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
+00014150: 2020 2020 2020 2073 7263 2e77 7269 7465         src.write
+00014160: 5f74 6578 7428 2270 7269 6e74 2827 6865  _text("print('he
+00014170: 6c6c 6f27 2922 290a 2020 2020 2020 2020  llo')").        
+00014180: 2020 2020 696e 766f 6b65 426c 6163 6b28      invokeBlack(
+00014190: 5b73 7472 2873 7263 295d 290a 2020 2020  [str(src)]).    
+000141a0: 2020 2020 2020 2020 6361 6368 6520 3d20          cache = 
+000141b0: 6365 7263 6973 2e72 6561 645f 6361 6368  cercis.read_cach
+000141c0: 6528 6d6f 6465 290a 2020 2020 2020 2020  e(mode).        
+000141d0: 2020 2020 6173 7365 7274 2073 7472 2873      assert str(s
+000141e0: 7263 2920 696e 2063 6163 6865 0a0a 2020  rc) in cache..  
+000141f0: 2020 6465 6620 7465 7374 5f63 6163 6865    def test_cache
+00014200: 5f73 696e 676c 655f 6669 6c65 5f61 6c72  _single_file_alr
+00014210: 6561 6479 5f63 6163 6865 6428 7365 6c66  eady_cached(self
+00014220: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00014230: 2020 206d 6f64 6520 3d20 4445 4641 554c     mode = DEFAUL
+00014240: 545f 4d4f 4445 0a20 2020 2020 2020 2077  T_MODE.        w
+00014250: 6974 6820 6361 6368 655f 6469 7228 2920  ith cache_dir() 
+00014260: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
+00014270: 2020 2020 2020 2020 2020 7372 6320 3d20            src = 
+00014280: 2877 6f72 6b73 7061 6365 202f 2022 7465  (workspace / "te
+00014290: 7374 2e70 7922 292e 7265 736f 6c76 6528  st.py").resolve(
+000142a0: 290a 2020 2020 2020 2020 2020 2020 7372  ).            sr
+000142b0: 632e 7772 6974 655f 7465 7874 2822 7072  c.write_text("pr
+000142c0: 696e 7428 2768 656c 6c6f 2729 2229 0a20  int('hello')"). 
+000142d0: 2020 2020 2020 2020 2020 2063 6572 6369             cerci
+000142e0: 732e 7772 6974 655f 6361 6368 6528 7b7d  s.write_cache({}
+000142f0: 2c20 5b73 7263 5d2c 206d 6f64 6529 0a20  , [src], mode). 
+00014300: 2020 2020 2020 2020 2020 2069 6e76 6f6b             invok
+00014310: 6542 6c61 636b 285b 7374 7228 7372 6329  eBlack([str(src)
+00014320: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+00014330: 7373 6572 7420 7372 632e 7265 6164 5f74  ssert src.read_t
+00014340: 6578 7428 2920 3d3d 2022 7072 696e 7428  ext() == "print(
+00014350: 2768 656c 6c6f 2729 220a 0a20 2020 2040  'hello')"..    @
+00014360: 6576 656e 745f 6c6f 6f70 2829 0a20 2020  event_loop().   
+00014370: 2064 6566 2074 6573 745f 6361 6368 655f   def test_cache_
+00014380: 6d75 6c74 6970 6c65 5f66 696c 6573 2873  multiple_files(s
+00014390: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+000143a0: 2020 2020 2020 6d6f 6465 203d 2044 4546        mode = DEF
+000143b0: 4155 4c54 5f4d 4f44 450a 2020 2020 2020  AULT_MODE.      
+000143c0: 2020 7769 7468 2063 6163 6865 5f64 6972    with cache_dir
+000143d0: 2829 2061 7320 776f 726b 7370 6163 652c  () as workspace,
+000143e0: 2070 6174 6368 280a 2020 2020 2020 2020   patch(.        
+000143f0: 2020 2020 2263 6f6e 6375 7272 656e 742e      "concurrent.
+00014400: 6675 7475 7265 732e 5072 6f63 6573 7350  futures.ProcessP
+00014410: 6f6f 6c45 7865 6375 746f 7222 2c20 6e65  oolExecutor", ne
+00014420: 773d 5468 7265 6164 506f 6f6c 4578 6563  w=ThreadPoolExec
+00014430: 7574 6f72 0a20 2020 2020 2020 2029 3a0a  utor.        ):.
+00014440: 2020 2020 2020 2020 2020 2020 6f6e 6520              one 
+00014450: 3d20 2877 6f72 6b73 7061 6365 202f 2022  = (workspace / "
+00014460: 6f6e 652e 7079 2229 2e72 6573 6f6c 7665  one.py").resolve
+00014470: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
+00014480: 6974 6820 6f6e 652e 6f70 656e 2822 7722  ith one.open("w"
+00014490: 2920 6173 2066 6f62 6a3a 0a20 2020 2020  ) as fobj:.     
+000144a0: 2020 2020 2020 2020 2020 2066 6f62 6a2e             fobj.
+000144b0: 7772 6974 6528 2270 7269 6e74 2827 6865  write("print('he
+000144c0: 6c6c 6f27 2922 290a 2020 2020 2020 2020  llo')").        
+000144d0: 2020 2020 7477 6f20 3d20 2877 6f72 6b73      two = (works
+000144e0: 7061 6365 202f 2022 7477 6f2e 7079 2229  pace / "two.py")
+000144f0: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
+00014500: 2020 2020 2020 2077 6974 6820 7477 6f2e         with two.
+00014510: 6f70 656e 2822 7722 2920 6173 2066 6f62  open("w") as fob
+00014520: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
+00014530: 2020 2066 6f62 6a2e 7772 6974 6528 2270     fobj.write("p
+00014540: 7269 6e74 2827 6865 6c6c 6f27 2922 290a  rint('hello')").
+00014550: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+00014560: 6973 2e77 7269 7465 5f63 6163 6865 287b  is.write_cache({
+00014570: 7d2c 205b 6f6e 655d 2c20 6d6f 6465 290a  }, [one], mode).
+00014580: 2020 2020 2020 2020 2020 2020 696e 766f              invo
+00014590: 6b65 426c 6163 6b28 5b73 7472 2877 6f72  keBlack([str(wor
+000145a0: 6b73 7061 6365 292c 2022 2d2d 7369 6e67  kspace), "--sing
+000145b0: 6c65 2d71 756f 7465 3d46 616c 7365 225d  le-quote=False"]
+000145c0: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+000145d0: 7468 206f 6e65 2e6f 7065 6e28 2272 2229  th one.open("r")
+000145e0: 2061 7320 666f 626a 3a0a 2020 2020 2020   as fobj:.      
+000145f0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00014600: 2066 6f62 6a2e 7265 6164 2829 203d 3d20   fobj.read() == 
+00014610: 2270 7269 6e74 2827 6865 6c6c 6f27 2922  "print('hello')"
+00014620: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00014630: 6820 7477 6f2e 6f70 656e 2822 7222 2920  h two.open("r") 
+00014640: 6173 2066 6f62 6a3a 0a20 2020 2020 2020  as fobj:.       
+00014650: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00014660: 666f 626a 2e72 6561 6428 2920 3d3d 2027  fobj.read() == '
+00014670: 7072 696e 7428 2268 656c 6c6f 2229 5c6e  print("hello")\n
+00014680: 270a 2020 2020 2020 2020 2020 2020 6361  '.            ca
+00014690: 6368 6520 3d20 6365 7263 6973 2e72 6561  che = cercis.rea
+000146a0: 645f 6361 6368 6528 6d6f 6465 290a 2020  d_cache(mode).  
+000146b0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+000146c0: 2073 7472 286f 6e65 2920 696e 2063 6163   str(one) in cac
+000146d0: 6865 0a20 2020 2020 2020 2020 2020 2061  he.            a
+000146e0: 7373 6572 7420 7374 7228 7477 6f29 2069  ssert str(two) i
+000146f0: 6e20 6361 6368 650a 0a20 2020 2040 7079  n cache..    @py
+00014700: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+00014710: 7472 697a 6528 2263 6f6c 6f72 222c 205b  trize("color", [
+00014720: 4661 6c73 652c 2054 7275 655d 2c20 6964  False, True], id
+00014730: 733d 5b22 6e6f 2d63 6f6c 6f72 222c 2022  s=["no-color", "
+00014740: 7769 7468 2d63 6f6c 6f72 225d 290a 2020  with-color"]).  
+00014750: 2020 6465 6620 7465 7374 5f6e 6f5f 6361    def test_no_ca
+00014760: 6368 655f 7768 656e 5f77 7269 7465 6261  che_when_writeba
+00014770: 636b 5f64 6966 6628 7365 6c66 2c20 636f  ck_diff(self, co
+00014780: 6c6f 723a 2062 6f6f 6c29 202d 3e20 4e6f  lor: bool) -> No
+00014790: 6e65 3a0a 2020 2020 2020 2020 6d6f 6465  ne:.        mode
+000147a0: 203d 2044 4546 4155 4c54 5f4d 4f44 450a   = DEFAULT_MODE.
+000147b0: 2020 2020 2020 2020 7769 7468 2063 6163          with cac
+000147c0: 6865 5f64 6972 2829 2061 7320 776f 726b  he_dir() as work
+000147d0: 7370 6163 653a 0a20 2020 2020 2020 2020  space:.         
+000147e0: 2020 2073 7263 203d 2028 776f 726b 7370     src = (worksp
+000147f0: 6163 6520 2f20 2274 6573 742e 7079 2229  ace / "test.py")
+00014800: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
+00014810: 2020 2020 2020 2077 6974 6820 7372 632e         with src.
+00014820: 6f70 656e 2822 7722 2920 6173 2066 6f62  open("w") as fob
+00014830: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
+00014840: 2020 2066 6f62 6a2e 7772 6974 6528 2270     fobj.write("p
+00014850: 7269 6e74 2827 6865 6c6c 6f27 2922 290a  rint('hello')").
+00014860: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00014870: 2070 6174 6368 2822 6365 7263 6973 2e72   patch("cercis.r
+00014880: 6561 645f 6361 6368 6522 2920 6173 2072  ead_cache") as r
+00014890: 6561 645f 6361 6368 652c 2070 6174 6368  ead_cache, patch
+000148a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000148b0: 2020 2263 6572 6369 732e 7772 6974 655f    "cercis.write_
+000148c0: 6361 6368 6522 0a20 2020 2020 2020 2020  cache".         
+000148d0: 2020 2029 2061 7320 7772 6974 655f 6361     ) as write_ca
+000148e0: 6368 653a 0a20 2020 2020 2020 2020 2020  che:.           
+000148f0: 2020 2020 2063 6d64 203d 205b 7374 7228       cmd = [str(
+00014900: 7372 6329 2c20 222d 2d64 6966 6622 5d0a  src), "--diff"].
+00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014920: 6966 2063 6f6c 6f72 3a0a 2020 2020 2020  if color:.      
+00014930: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00014940: 642e 6170 7065 6e64 2822 2d2d 636f 6c6f  d.append("--colo
+00014950: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
+00014960: 2020 2020 696e 766f 6b65 426c 6163 6b28      invokeBlack(
+00014970: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
+00014980: 2020 2020 2063 6163 6865 5f66 696c 6520       cache_file 
+00014990: 3d20 6765 745f 6361 6368 655f 6669 6c65  = get_cache_file
+000149a0: 286d 6f64 6529 0a20 2020 2020 2020 2020  (mode).         
+000149b0: 2020 2020 2020 2061 7373 6572 7420 6361         assert ca
+000149c0: 6368 655f 6669 6c65 2e65 7869 7374 7328  che_file.exists(
+000149d0: 2920 6973 2046 616c 7365 0a20 2020 2020  ) is False.     
+000149e0: 2020 2020 2020 2020 2020 2077 7269 7465             write
+000149f0: 5f63 6163 6865 2e61 7373 6572 745f 6e6f  _cache.assert_no
+00014a00: 745f 6361 6c6c 6564 2829 0a20 2020 2020  t_called().     
+00014a10: 2020 2020 2020 2020 2020 2072 6561 645f             read_
+00014a20: 6361 6368 652e 6173 7365 7274 5f6e 6f74  cache.assert_not
+00014a30: 5f63 616c 6c65 6428 290a 0a20 2020 2040  _called()..    @
+00014a40: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+00014a50: 6d65 7472 697a 6528 2263 6f6c 6f72 222c  metrize("color",
+00014a60: 205b 4661 6c73 652c 2054 7275 655d 2c20   [False, True], 
+00014a70: 6964 733d 5b22 6e6f 2d63 6f6c 6f72 222c  ids=["no-color",
+00014a80: 2022 7769 7468 2d63 6f6c 6f72 225d 290a   "with-color"]).
+00014a90: 2020 2020 4065 7665 6e74 5f6c 6f6f 7028      @event_loop(
+00014aa0: 290a 2020 2020 6465 6620 7465 7374 5f6f  ).    def test_o
+00014ab0: 7574 7075 745f 6c6f 636b 696e 675f 7768  utput_locking_wh
+00014ac0: 656e 5f77 7269 7465 6261 636b 5f64 6966  en_writeback_dif
+00014ad0: 6628 7365 6c66 2c20 636f 6c6f 723a 2062  f(self, color: b
+00014ae0: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
+00014af0: 2020 2020 2020 7769 7468 2063 6163 6865        with cache
+00014b00: 5f64 6972 2829 2061 7320 776f 726b 7370  _dir() as worksp
+00014b10: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
+00014b20: 2066 6f72 2074 6167 2069 6e20 7261 6e67   for tag in rang
+00014b30: 6528 302c 2034 293a 0a20 2020 2020 2020  e(0, 4):.       
+00014b40: 2020 2020 2020 2020 2073 7263 203d 2028           src = (
+00014b50: 776f 726b 7370 6163 6520 2f20 6622 7465  workspace / f"te
+00014b60: 7374 7b74 6167 7d2e 7079 2229 2e72 6573  st{tag}.py").res
+00014b70: 6f6c 7665 2829 0a20 2020 2020 2020 2020  olve().         
+00014b80: 2020 2020 2020 2077 6974 6820 7372 632e         with src.
+00014b90: 6f70 656e 2822 7722 2920 6173 2066 6f62  open("w") as fob
+00014ba0: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
+00014bb0: 2020 2020 2020 2066 6f62 6a2e 7772 6974         fobj.writ
+00014bc0: 6528 2270 7269 6e74 2827 6865 6c6c 6f27  e("print('hello'
+00014bd0: 2922 290a 2020 2020 2020 2020 2020 2020  )").            
+00014be0: 7769 7468 2070 6174 6368 280a 2020 2020  with patch(.    
+00014bf0: 2020 2020 2020 2020 2020 2020 2263 6572              "cer
+00014c00: 6369 732e 636f 6e63 7572 7265 6e63 792e  cis.concurrency.
+00014c10: 4d61 6e61 6765 7222 2c20 7772 6170 733d  Manager", wraps=
+00014c20: 6d75 6c74 6970 726f 6365 7373 696e 672e  multiprocessing.
+00014c30: 4d61 6e61 6765 720a 2020 2020 2020 2020  Manager.        
+00014c40: 2020 2020 2920 6173 206d 6772 3a0a 2020      ) as mgr:.  
+00014c50: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00014c60: 6420 3d20 5b22 2d2d 6469 6666 222c 2073  d = ["--diff", s
+00014c70: 7472 2877 6f72 6b73 7061 6365 295d 0a20  tr(workspace)]. 
+00014c80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014c90: 6620 636f 6c6f 723a 0a20 2020 2020 2020  f color:.       
+00014ca0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00014cb0: 2e61 7070 656e 6428 222d 2d63 6f6c 6f72  .append("--color
+00014cc0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00014cd0: 2020 2069 6e76 6f6b 6542 6c61 636b 2863     invokeBlack(c
+00014ce0: 6d64 2c20 6578 6974 5f63 6f64 653d 3029  md, exit_code=0)
+00014cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014d00: 2023 2074 6869 7320 6973 6e27 7420 7175   # this isn't qu
+00014d10: 6974 6520 646f 696e 6720 7768 6174 2077  ite doing what w
+00014d20: 6520 7761 6e74 2c20 6275 7420 6966 2069  e want, but if i
+00014d30: 7420 5f69 736e 2774 5f0a 2020 2020 2020  t _isn't_.      
+00014d40: 2020 2020 2020 2020 2020 2320 6361 6c6c            # call
+00014d50: 6564 2074 6865 6e20 7765 2063 616e 6e6f  ed then we canno
+00014d60: 7420 6265 2075 7369 6e67 2074 6865 206c  t be using the l
+00014d70: 6f63 6b20 6974 2070 726f 7669 6465 730a  ock it provides.
+00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d90: 6d67 722e 6173 7365 7274 5f63 616c 6c65  mgr.assert_calle
+00014da0: 6428 290a 0a20 2020 2064 6566 2074 6573  d()..    def tes
+00014db0: 745f 6e6f 5f63 6163 6865 5f77 6865 6e5f  t_no_cache_when_
+00014dc0: 7374 6469 6e28 7365 6c66 2920 2d3e 204e  stdin(self) -> N
+00014dd0: 6f6e 653a 0a20 2020 2020 2020 206d 6f64  one:.        mod
+00014de0: 6520 3d20 4445 4641 554c 545f 4d4f 4445  e = DEFAULT_MODE
+00014df0: 0a20 2020 2020 2020 2077 6974 6820 6361  .        with ca
+00014e00: 6368 655f 6469 7228 293a 0a20 2020 2020  che_dir():.     
+00014e10: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00014e20: 436c 6952 756e 6e65 7228 292e 696e 766f  CliRunner().invo
+00014e30: 6b65 280a 2020 2020 2020 2020 2020 2020  ke(.            
+00014e40: 2020 2020 6365 7263 6973 2e6d 6169 6e2c      cercis.main,
+00014e50: 205b 222d 225d 2c20 696e 7075 743d 4279   ["-"], input=By
+00014e60: 7465 7349 4f28 6222 7072 696e 7428 2768  tesIO(b"print('h
+00014e70: 656c 6c6f 2729 2229 0a20 2020 2020 2020  ello')").       
+00014e80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014e90: 2020 2061 7373 6572 7420 6e6f 7420 7265     assert not re
+00014ea0: 7375 6c74 2e65 7869 745f 636f 6465 0a20  sult.exit_code. 
+00014eb0: 2020 2020 2020 2020 2020 2063 6163 6865             cache
+00014ec0: 5f66 696c 6520 3d20 6765 745f 6361 6368  _file = get_cach
+00014ed0: 655f 6669 6c65 286d 6f64 6529 0a20 2020  e_file(mode).   
+00014ee0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00014ef0: 6e6f 7420 6361 6368 655f 6669 6c65 2e65  not cache_file.e
+00014f00: 7869 7374 7328 290a 0a20 2020 2064 6566  xists()..    def
+00014f10: 2074 6573 745f 7265 6164 5f63 6163 6865   test_read_cache
+00014f20: 5f6e 6f5f 6361 6368 6566 696c 6528 7365  _no_cachefile(se
+00014f30: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00014f40: 2020 2020 206d 6f64 6520 3d20 4445 4641       mode = DEFA
+00014f50: 554c 545f 4d4f 4445 0a20 2020 2020 2020  ULT_MODE.       
+00014f60: 2077 6974 6820 6361 6368 655f 6469 7228   with cache_dir(
+00014f70: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+00014f80: 7373 6572 7420 6365 7263 6973 2e72 6561  ssert cercis.rea
+00014f90: 645f 6361 6368 6528 6d6f 6465 2920 3d3d  d_cache(mode) ==
+00014fa0: 207b 7d0a 0a20 2020 2064 6566 2074 6573   {}..    def tes
+00014fb0: 745f 7772 6974 655f 6361 6368 655f 7265  t_write_cache_re
+00014fc0: 6164 5f63 6163 6865 2873 656c 6629 202d  ad_cache(self) -
+00014fd0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00014fe0: 6d6f 6465 203d 2044 4546 4155 4c54 5f4d  mode = DEFAULT_M
+00014ff0: 4f44 450a 2020 2020 2020 2020 7769 7468  ODE.        with
+00015000: 2063 6163 6865 5f64 6972 2829 2061 7320   cache_dir() as 
+00015010: 776f 726b 7370 6163 653a 0a20 2020 2020  workspace:.     
+00015020: 2020 2020 2020 2073 7263 203d 2028 776f         src = (wo
+00015030: 726b 7370 6163 6520 2f20 2274 6573 742e  rkspace / "test.
+00015040: 7079 2229 2e72 6573 6f6c 7665 2829 0a20  py").resolve(). 
+00015050: 2020 2020 2020 2020 2020 2073 7263 2e74             src.t
+00015060: 6f75 6368 2829 0a20 2020 2020 2020 2020  ouch().         
+00015070: 2020 2063 6572 6369 732e 7772 6974 655f     cercis.write_
+00015080: 6361 6368 6528 7b7d 2c20 5b73 7263 5d2c  cache({}, [src],
+00015090: 206d 6f64 6529 0a20 2020 2020 2020 2020   mode).         
+000150a0: 2020 2063 6163 6865 203d 2063 6572 6369     cache = cerci
+000150b0: 732e 7265 6164 5f63 6163 6865 286d 6f64  s.read_cache(mod
+000150c0: 6529 0a20 2020 2020 2020 2020 2020 2061  e).            a
+000150d0: 7373 6572 7420 7374 7228 7372 6329 2069  ssert str(src) i
+000150e0: 6e20 6361 6368 650a 2020 2020 2020 2020  n cache.        
+000150f0: 2020 2020 6173 7365 7274 2063 6163 6865      assert cache
+00015100: 5b73 7472 2873 7263 295d 203d 3d20 6365  [str(src)] == ce
+00015110: 7263 6973 2e67 6574 5f63 6163 6865 5f69  rcis.get_cache_i
+00015120: 6e66 6f28 7372 6329 0a0a 2020 2020 6465  nfo(src)..    de
+00015130: 6620 7465 7374 5f66 696c 7465 725f 6361  f test_filter_ca
+00015140: 6368 6564 2873 656c 6629 202d 3e20 4e6f  ched(self) -> No
+00015150: 6e65 3a0a 2020 2020 2020 2020 7769 7468  ne:.        with
+00015160: 2054 656d 706f 7261 7279 4469 7265 6374   TemporaryDirect
+00015170: 6f72 7928 2920 6173 2077 6f72 6b73 7061  ory() as workspa
+00015180: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+00015190: 7061 7468 203d 2050 6174 6828 776f 726b  path = Path(work
+000151a0: 7370 6163 6529 0a20 2020 2020 2020 2020  space).         
+000151b0: 2020 2075 6e63 6163 6865 6420 3d20 2870     uncached = (p
+000151c0: 6174 6820 2f20 2275 6e63 6163 6865 6422  ath / "uncached"
+000151d0: 292e 7265 736f 6c76 6528 290a 2020 2020  ).resolve().    
+000151e0: 2020 2020 2020 2020 6361 6368 6564 203d          cached =
+000151f0: 2028 7061 7468 202f 2022 6361 6368 6564   (path / "cached
+00015200: 2229 2e72 6573 6f6c 7665 2829 0a20 2020  ").resolve().   
+00015210: 2020 2020 2020 2020 2063 6163 6865 645f           cached_
+00015220: 6275 745f 6368 616e 6765 6420 3d20 2870  but_changed = (p
+00015230: 6174 6820 2f20 2263 6861 6e67 6564 2229  ath / "changed")
+00015240: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
+00015250: 2020 2020 2020 2075 6e63 6163 6865 642e         uncached.
+00015260: 746f 7563 6828 290a 2020 2020 2020 2020  touch().        
+00015270: 2020 2020 6361 6368 6564 2e74 6f75 6368      cached.touch
+00015280: 2829 0a20 2020 2020 2020 2020 2020 2063  ().            c
+00015290: 6163 6865 645f 6275 745f 6368 616e 6765  ached_but_change
+000152a0: 642e 746f 7563 6828 290a 2020 2020 2020  d.touch().      
+000152b0: 2020 2020 2020 6361 6368 6520 3d20 7b0a        cache = {.
+000152c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152d0: 7374 7228 6361 6368 6564 293a 2063 6572  str(cached): cer
+000152e0: 6369 732e 6765 745f 6361 6368 655f 696e  cis.get_cache_in
+000152f0: 666f 2863 6163 6865 6429 2c0a 2020 2020  fo(cached),.    
+00015300: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00015310: 6361 6368 6564 5f62 7574 5f63 6861 6e67  cached_but_chang
+00015320: 6564 293a 2028 302e 302c 2030 292c 0a20  ed): (0.0, 0),. 
+00015330: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00015340: 2020 2020 2020 2020 2074 6f64 6f2c 2064           todo, d
+00015350: 6f6e 6520 3d20 6365 7263 6973 2e63 6163  one = cercis.cac
+00015360: 6865 2e66 696c 7465 725f 6361 6368 6564  he.filter_cached
+00015370: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00015380: 2020 6361 6368 652c 207b 756e 6361 6368    cache, {uncach
+00015390: 6564 2c20 6361 6368 6564 2c20 6361 6368  ed, cached, cach
+000153a0: 6564 5f62 7574 5f63 6861 6e67 6564 7d0a  ed_but_changed}.
+000153b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000153c0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+000153d0: 2074 6f64 6f20 3d3d 207b 756e 6361 6368   todo == {uncach
+000153e0: 6564 2c20 6361 6368 6564 5f62 7574 5f63  ed, cached_but_c
+000153f0: 6861 6e67 6564 7d0a 2020 2020 2020 2020  hanged}.        
+00015400: 2020 2020 6173 7365 7274 2064 6f6e 6520      assert done 
+00015410: 3d3d 207b 6361 6368 6564 7d0a 0a20 2020  == {cached}..   
+00015420: 2064 6566 2074 6573 745f 7772 6974 655f   def test_write_
+00015430: 6361 6368 655f 6372 6561 7465 735f 6469  cache_creates_di
+00015440: 7265 6374 6f72 795f 6966 5f6e 6565 6465  rectory_if_neede
+00015450: 6428 7365 6c66 2920 2d3e 204e 6f6e 653a  d(self) -> None:
+00015460: 0a20 2020 2020 2020 206d 6f64 6520 3d20  .        mode = 
+00015470: 4445 4641 554c 545f 4d4f 4445 0a20 2020  DEFAULT_MODE.   
+00015480: 2020 2020 2077 6974 6820 6361 6368 655f       with cache_
+00015490: 6469 7228 6578 6973 7473 3d46 616c 7365  dir(exists=False
+000154a0: 2920 6173 2077 6f72 6b73 7061 6365 3a0a  ) as workspace:.
+000154b0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+000154c0: 7274 206e 6f74 2077 6f72 6b73 7061 6365  rt not workspace
+000154d0: 2e65 7869 7374 7328 290a 2020 2020 2020  .exists().      
+000154e0: 2020 2020 2020 6365 7263 6973 2e77 7269        cercis.wri
+000154f0: 7465 5f63 6163 6865 287b 7d2c 205b 5d2c  te_cache({}, [],
+00015500: 206d 6f64 6529 0a20 2020 2020 2020 2020   mode).         
+00015510: 2020 2061 7373 6572 7420 776f 726b 7370     assert worksp
+00015520: 6163 652e 6578 6973 7473 2829 0a0a 2020  ace.exists()..  
+00015530: 2020 4065 7665 6e74 5f6c 6f6f 7028 290a    @event_loop().
+00015540: 2020 2020 6465 6620 7465 7374 5f66 6169      def test_fai
+00015550: 6c65 645f 666f 726d 6174 7469 6e67 5f64  led_formatting_d
+00015560: 6f65 735f 6e6f 745f 6765 745f 6361 6368  oes_not_get_cach
+00015570: 6564 2873 656c 6629 202d 3e20 4e6f 6e65  ed(self) -> None
+00015580: 3a0a 2020 2020 2020 2020 6d6f 6465 203d  :.        mode =
+00015590: 2044 4546 4155 4c54 5f4d 4f44 450a 2020   DEFAULT_MODE.  
+000155a0: 2020 2020 2020 7769 7468 2063 6163 6865        with cache
+000155b0: 5f64 6972 2829 2061 7320 776f 726b 7370  _dir() as worksp
+000155c0: 6163 652c 2070 6174 6368 280a 2020 2020  ace, patch(.    
+000155d0: 2020 2020 2020 2020 2263 6f6e 6375 7272          "concurr
+000155e0: 656e 742e 6675 7475 7265 732e 5072 6f63  ent.futures.Proc
+000155f0: 6573 7350 6f6f 6c45 7865 6375 746f 7222  essPoolExecutor"
+00015600: 2c20 6e65 773d 5468 7265 6164 506f 6f6c  , new=ThreadPool
+00015610: 4578 6563 7574 6f72 0a20 2020 2020 2020  Executor.       
+00015620: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00015630: 6661 696c 696e 6720 3d20 2877 6f72 6b73  failing = (works
+00015640: 7061 6365 202f 2022 6661 696c 696e 672e  pace / "failing.
+00015650: 7079 2229 2e72 6573 6f6c 7665 2829 0a20  py").resolve(). 
+00015660: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00015670: 6661 696c 696e 672e 6f70 656e 2822 7722  failing.open("w"
+00015680: 2920 6173 2066 6f62 6a3a 0a20 2020 2020  ) as fobj:.     
+00015690: 2020 2020 2020 2020 2020 2066 6f62 6a2e             fobj.
+000156a0: 7772 6974 6528 226e 6f74 2061 6374 7561  write("not actua
+000156b0: 6c6c 7920 7079 7468 6f6e 2229 0a20 2020  lly python").   
+000156c0: 2020 2020 2020 2020 2063 6c65 616e 203d           clean =
+000156d0: 2028 776f 726b 7370 6163 6520 2f20 2263   (workspace / "c
+000156e0: 6c65 616e 2e70 7922 292e 7265 736f 6c76  lean.py").resolv
+000156f0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00015700: 7769 7468 2063 6c65 616e 2e6f 7065 6e28  with clean.open(
+00015710: 2277 2229 2061 7320 666f 626a 3a0a 2020  "w") as fobj:.  
+00015720: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00015730: 626a 2e77 7269 7465 2827 7072 696e 7428  bj.write('print(
+00015740: 2268 656c 6c6f 2229 5c6e 2729 0a20 2020  "hello")\n').   
+00015750: 2020 2020 2020 2020 2069 6e76 6f6b 6542           invokeB
+00015760: 6c61 636b 285b 7374 7228 776f 726b 7370  lack([str(worksp
+00015770: 6163 6529 5d2c 2065 7869 745f 636f 6465  ace)], exit_code
+00015780: 3d31 3233 290a 2020 2020 2020 2020 2020  =123).          
+00015790: 2020 6361 6368 6520 3d20 6365 7263 6973    cache = cercis
+000157a0: 2e72 6561 645f 6361 6368 6528 6d6f 6465  .read_cache(mode
+000157b0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
+000157c0: 7365 7274 2073 7472 2866 6169 6c69 6e67  sert str(failing
+000157d0: 2920 6e6f 7420 696e 2063 6163 6865 0a20  ) not in cache. 
+000157e0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000157f0: 7420 7374 7228 636c 6561 6e29 2069 6e20  t str(clean) in 
+00015800: 6361 6368 650a 0a20 2020 2064 6566 2074  cache..    def t
+00015810: 6573 745f 7772 6974 655f 6361 6368 655f  est_write_cache_
+00015820: 7772 6974 655f 6661 696c 2873 656c 6629  write_fail(self)
+00015830: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00015840: 2020 6d6f 6465 203d 2044 4546 4155 4c54    mode = DEFAULT
+00015850: 5f4d 4f44 450a 2020 2020 2020 2020 7769  _MODE.        wi
+00015860: 7468 2063 6163 6865 5f64 6972 2829 2c20  th cache_dir(), 
+00015870: 7061 7463 682e 6f62 6a65 6374 2850 6174  patch.object(Pat
+00015880: 682c 2022 6f70 656e 2229 2061 7320 6d6f  h, "open") as mo
+00015890: 636b 3a0a 2020 2020 2020 2020 2020 2020  ck:.            
+000158a0: 6d6f 636b 2e73 6964 655f 6566 6665 6374  mock.side_effect
+000158b0: 203d 204f 5345 7272 6f72 0a20 2020 2020   = OSError.     
+000158c0: 2020 2020 2020 2063 6572 6369 732e 7772         cercis.wr
+000158d0: 6974 655f 6361 6368 6528 7b7d 2c20 5b5d  ite_cache({}, []
+000158e0: 2c20 6d6f 6465 290a 0a20 2020 2064 6566  , mode)..    def
+000158f0: 2074 6573 745f 7265 6164 5f63 6163 6865   test_read_cache
+00015900: 5f6c 696e 655f 6c65 6e67 7468 7328 7365  _line_lengths(se
+00015910: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00015920: 2020 2020 206d 6f64 6520 3d20 4445 4641       mode = DEFA
+00015930: 554c 545f 4d4f 4445 0a20 2020 2020 2020  ULT_MODE.       
+00015940: 2073 686f 7274 5f6d 6f64 6520 3d20 7265   short_mode = re
+00015950: 706c 6163 6528 4445 4641 554c 545f 4d4f  place(DEFAULT_MO
+00015960: 4445 2c20 6c69 6e65 5f6c 656e 6774 683d  DE, line_length=
+00015970: 3129 0a20 2020 2020 2020 2077 6974 6820  1).        with 
+00015980: 6361 6368 655f 6469 7228 2920 6173 2077  cache_dir() as w
+00015990: 6f72 6b73 7061 6365 3a0a 2020 2020 2020  orkspace:.      
+000159a0: 2020 2020 2020 7061 7468 203d 2028 776f        path = (wo
+000159b0: 726b 7370 6163 6520 2f20 2266 696c 652e  rkspace / "file.
+000159c0: 7079 2229 2e72 6573 6f6c 7665 2829 0a20  py").resolve(). 
+000159d0: 2020 2020 2020 2020 2020 2070 6174 682e             path.
+000159e0: 746f 7563 6828 290a 2020 2020 2020 2020  touch().        
+000159f0: 2020 2020 6365 7263 6973 2e77 7269 7465      cercis.write
+00015a00: 5f63 6163 6865 287b 7d2c 205b 7061 7468  _cache({}, [path
+00015a10: 5d2c 206d 6f64 6529 0a20 2020 2020 2020  ], mode).       
+00015a20: 2020 2020 206f 6e65 203d 2063 6572 6369       one = cerci
+00015a30: 732e 7265 6164 5f63 6163 6865 286d 6f64  s.read_cache(mod
+00015a40: 6529 0a20 2020 2020 2020 2020 2020 2061  e).            a
+00015a50: 7373 6572 7420 7374 7228 7061 7468 2920  ssert str(path) 
+00015a60: 696e 206f 6e65 0a20 2020 2020 2020 2020  in one.         
+00015a70: 2020 2074 776f 203d 2063 6572 6369 732e     two = cercis.
+00015a80: 7265 6164 5f63 6163 6865 2873 686f 7274  read_cache(short
+00015a90: 5f6d 6f64 6529 0a20 2020 2020 2020 2020  _mode).         
+00015aa0: 2020 2061 7373 6572 7420 7374 7228 7061     assert str(pa
+00015ab0: 7468 2920 6e6f 7420 696e 2074 776f 0a0a  th) not in two..
+00015ac0: 0a64 6566 2061 7373 6572 745f 636f 6c6c  .def assert_coll
+00015ad0: 6563 7465 645f 736f 7572 6365 7328 0a20  ected_sources(. 
+00015ae0: 2020 2020 2020 2073 7263 3a20 5365 7175         src: Sequ
+00015af0: 656e 6365 5b55 6e69 6f6e 5b73 7472 2c20  ence[Union[str, 
+00015b00: 5061 7468 5d5d 2c0a 2020 2020 2020 2020  Path]],.        
+00015b10: 6578 7065 6374 6564 3a20 5365 7175 656e  expected: Sequen
+00015b20: 6365 5b55 6e69 6f6e 5b73 7472 2c20 5061  ce[Union[str, Pa
+00015b30: 7468 5d5d 2c0a 2020 2020 2020 2020 2a2c  th]],.        *,
+00015b40: 0a20 2020 2020 2020 2063 7478 3a20 4f70  .        ctx: Op
+00015b50: 7469 6f6e 616c 5b46 616b 6543 6f6e 7465  tional[FakeConte
+00015b60: 7874 5d20 3d20 4e6f 6e65 2c0a 2020 2020  xt] = None,.    
+00015b70: 2020 2020 6578 636c 7564 653a 204f 7074      exclude: Opt
+00015b80: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00015b90: 652c 0a20 2020 2020 2020 2069 6e63 6c75  e,.        inclu
+00015ba0: 6465 3a20 4f70 7469 6f6e 616c 5b73 7472  de: Optional[str
+00015bb0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00015bc0: 2020 6578 7465 6e64 5f65 7863 6c75 6465    extend_exclude
+00015bd0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00015be0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00015bf0: 666f 7263 655f 6578 636c 7564 653a 204f  force_exclude: O
+00015c00: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00015c10: 6f6e 652c 0a20 2020 2020 2020 2073 7464  one,.        std
+00015c20: 696e 5f66 696c 656e 616d 653a 204f 7074  in_filename: Opt
+00015c30: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00015c40: 652c 0a29 202d 3e20 4e6f 6e65 3a0a 2020  e,.) -> None:.  
+00015c50: 2020 6773 5f73 7263 203d 2074 7570 6c65    gs_src = tuple
+00015c60: 2873 7472 2850 6174 6828 7329 2920 666f  (str(Path(s)) fo
+00015c70: 7220 7320 696e 2073 7263 290a 2020 2020  r s in src).    
+00015c80: 6773 5f65 7870 6563 7465 6420 3d20 5b50  gs_expected = [P
+00015c90: 6174 6828 7329 2066 6f72 2073 2069 6e20  ath(s) for s in 
+00015ca0: 6578 7065 6374 6564 5d0a 2020 2020 6773  expected].    gs
+00015cb0: 5f65 7863 6c75 6465 203d 204e 6f6e 6520  _exclude = None 
+00015cc0: 6966 2065 7863 6c75 6465 2069 7320 4e6f  if exclude is No
+00015cd0: 6e65 2065 6c73 6520 636f 6d70 696c 655f  ne else compile_
+00015ce0: 7061 7474 6572 6e28 6578 636c 7564 6529  pattern(exclude)
+00015cf0: 0a20 2020 2067 735f 696e 636c 7564 6520  .    gs_include 
+00015d00: 3d20 4445 4641 554c 545f 494e 434c 5544  = DEFAULT_INCLUD
+00015d10: 4520 6966 2069 6e63 6c75 6465 2069 7320  E if include is 
+00015d20: 4e6f 6e65 2065 6c73 6520 636f 6d70 696c  None else compil
+00015d30: 655f 7061 7474 6572 6e28 696e 636c 7564  e_pattern(includ
+00015d40: 6529 0a20 2020 2067 735f 6578 7465 6e64  e).    gs_extend
+00015d50: 5f65 7863 6c75 6465 203d 2028 0a20 2020  _exclude = (.   
+00015d60: 2020 2020 204e 6f6e 6520 6966 2065 7874       None if ext
+00015d70: 656e 645f 6578 636c 7564 6520 6973 204e  end_exclude is N
+00015d80: 6f6e 6520 656c 7365 2063 6f6d 7069 6c65  one else compile
+00015d90: 5f70 6174 7465 726e 2865 7874 656e 645f  _pattern(extend_
+00015da0: 6578 636c 7564 6529 0a20 2020 2029 0a20  exclude).    ). 
+00015db0: 2020 2067 735f 666f 7263 655f 6578 636c     gs_force_excl
+00015dc0: 7564 6520 3d20 4e6f 6e65 2069 6620 666f  ude = None if fo
+00015dd0: 7263 655f 6578 636c 7564 6520 6973 204e  rce_exclude is N
+00015de0: 6f6e 6520 656c 7365 2063 6f6d 7069 6c65  one else compile
+00015df0: 5f70 6174 7465 726e 2866 6f72 6365 5f65  _pattern(force_e
+00015e00: 7863 6c75 6465 290a 2020 2020 636f 6c6c  xclude).    coll
+00015e10: 6563 7465 6420 3d20 6365 7263 6973 2e67  ected = cercis.g
+00015e20: 6574 5f73 6f75 7263 6573 280a 2020 2020  et_sources(.    
+00015e30: 2020 2020 6374 783d 6374 7820 6f72 2046      ctx=ctx or F
+00015e40: 616b 6543 6f6e 7465 7874 2829 2c0a 2020  akeContext(),.  
+00015e50: 2020 2020 2020 7372 633d 6773 5f73 7263        src=gs_src
+00015e60: 2c0a 2020 2020 2020 2020 7175 6965 743d  ,.        quiet=
+00015e70: 4661 6c73 652c 0a20 2020 2020 2020 2076  False,.        v
+00015e80: 6572 626f 7365 3d46 616c 7365 2c0a 2020  erbose=False,.  
+00015e90: 2020 2020 2020 696e 636c 7564 653d 6773        include=gs
+00015ea0: 5f69 6e63 6c75 6465 2c0a 2020 2020 2020  _include,.      
+00015eb0: 2020 6578 636c 7564 653d 6773 5f65 7863    exclude=gs_exc
+00015ec0: 6c75 6465 2c0a 2020 2020 2020 2020 6578  lude,.        ex
+00015ed0: 7465 6e64 5f65 7863 6c75 6465 3d67 735f  tend_exclude=gs_
+00015ee0: 6578 7465 6e64 5f65 7863 6c75 6465 2c0a  extend_exclude,.
+00015ef0: 2020 2020 2020 2020 666f 7263 655f 6578          force_ex
+00015f00: 636c 7564 653d 6773 5f66 6f72 6365 5f65  clude=gs_force_e
+00015f10: 7863 6c75 6465 2c0a 2020 2020 2020 2020  xclude,.        
+00015f20: 7265 706f 7274 3d63 6572 6369 732e 5265  report=cercis.Re
+00015f30: 706f 7274 2829 2c0a 2020 2020 2020 2020  port(),.        
+00015f40: 7374 6469 6e5f 6669 6c65 6e61 6d65 3d73  stdin_filename=s
+00015f50: 7464 696e 5f66 696c 656e 616d 652c 0a20  tdin_filename,. 
+00015f60: 2020 2029 0a20 2020 2061 7373 6572 7420     ).    assert 
+00015f70: 736f 7274 6564 2863 6f6c 6c65 6374 6564  sorted(collected
+00015f80: 2920 3d3d 2073 6f72 7465 6428 6773 5f65  ) == sorted(gs_e
+00015f90: 7870 6563 7465 6429 0a0a 0a63 6c61 7373  xpected)...class
+00015fa0: 2054 6573 7446 696c 6543 6f6c 6c65 6374   TestFileCollect
+00015fb0: 696f 6e3a 0a20 2020 2064 6566 2074 6573  ion:.    def tes
+00015fc0: 745f 696e 636c 7564 655f 6578 636c 7564  t_include_exclud
+00015fd0: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+00015fe0: 0a20 2020 2020 2020 2070 6174 6820 3d20  .        path = 
+00015ff0: 5448 4953 5f44 4952 202f 2022 6461 7461  THIS_DIR / "data
+00016000: 2220 2f20 2269 6e63 6c75 6465 5f65 7863  " / "include_exc
+00016010: 6c75 6465 5f74 6573 7473 220a 2020 2020  lude_tests".    
+00016020: 2020 2020 7372 6320 3d20 5b70 6174 685d      src = [path]
+00016030: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+00016040: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
+00016050: 2020 5061 7468 2870 6174 6820 2f20 2262    Path(path / "b
+00016060: 2f64 6f6e 745f 6578 636c 7564 652f 612e  /dont_exclude/a.
+00016070: 7079 2229 2c0a 2020 2020 2020 2020 2020  py"),.          
+00016080: 2020 5061 7468 2870 6174 6820 2f20 2262    Path(path / "b
+00016090: 2f64 6f6e 745f 6578 636c 7564 652f 612e  /dont_exclude/a.
+000160a0: 7079 6922 292c 0a20 2020 2020 2020 205d  pyi"),.        ]
+000160b0: 0a20 2020 2020 2020 2061 7373 6572 745f  .        assert_
+000160c0: 636f 6c6c 6563 7465 645f 736f 7572 6365  collected_source
+000160d0: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
+000160e0: 7263 2c0a 2020 2020 2020 2020 2020 2020  rc,.            
+000160f0: 6578 7065 6374 6564 2c0a 2020 2020 2020  expected,.      
+00016100: 2020 2020 2020 696e 636c 7564 653d 7222        include=r"
+00016110: 5c2e 7079 693f 2422 2c0a 2020 2020 2020  \.pyi?$",.      
+00016120: 2020 2020 2020 6578 636c 7564 653d 7222        exclude=r"
+00016130: 2f65 7863 6c75 6465 2f7c 2f5c 2e64 6566  /exclude/|/\.def
+00016140: 696e 6974 656c 795f 6578 636c 7564 652f  initely_exclude/
+00016150: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
+00016160: 2020 6465 6620 7465 7374 5f67 6974 6967    def test_gitig
+00016170: 6e6f 7265 5f75 7365 645f 6173 5f64 6566  nore_used_as_def
+00016180: 6175 6c74 2873 656c 6629 202d 3e20 4e6f  ault(self) -> No
+00016190: 6e65 3a0a 2020 2020 2020 2020 6261 7365  ne:.        base
+000161a0: 203d 2050 6174 6828 4441 5441 5f44 4952   = Path(DATA_DIR
+000161b0: 202f 2022 696e 636c 7564 655f 6578 636c   / "include_excl
+000161c0: 7564 655f 7465 7374 7322 290a 2020 2020  ude_tests").    
+000161d0: 2020 2020 6578 7065 6374 6564 203d 205b      expected = [
+000161e0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+000161f0: 6520 2f20 2262 2f2e 6465 6669 6e69 7465  e / "b/.definite
+00016200: 6c79 5f65 7863 6c75 6465 2f61 2e70 7922  ly_exclude/a.py"
+00016210: 2c0a 2020 2020 2020 2020 2020 2020 6261  ,.            ba
+00016220: 7365 202f 2022 622f 2e64 6566 696e 6974  se / "b/.definit
+00016230: 656c 795f 6578 636c 7564 652f 612e 7079  ely_exclude/a.py
+00016240: 6922 2c0a 2020 2020 2020 2020 5d0a 2020  i",.        ].  
+00016250: 2020 2020 2020 7372 6320 3d20 5b62 6173        src = [bas
+00016260: 6520 2f20 2262 2f22 5d0a 2020 2020 2020  e / "b/"].      
+00016270: 2020 6374 7820 3d20 4661 6b65 436f 6e74    ctx = FakeCont
+00016280: 6578 7428 290a 2020 2020 2020 2020 6374  ext().        ct
+00016290: 782e 6f62 6a5b 2272 6f6f 7422 5d20 3d20  x.obj["root"] = 
+000162a0: 6261 7365 0a20 2020 2020 2020 2061 7373  base.        ass
+000162b0: 6572 745f 636f 6c6c 6563 7465 645f 736f  ert_collected_so
+000162c0: 7572 6365 7328 7372 632c 2065 7870 6563  urces(src, expec
+000162d0: 7465 642c 2063 7478 3d63 7478 2c20 6578  ted, ctx=ctx, ex
+000162e0: 7465 6e64 5f65 7863 6c75 6465 3d72 222f  tend_exclude=r"/
+000162f0: 6578 636c 7564 652f 2229 0a0a 2020 2020  exclude/")..    
+00016300: 6465 6620 7465 7374 5f67 6974 6967 6e6f  def test_gitigno
+00016310: 7265 5f75 7365 645f 6f6e 5f6d 756c 7469  re_used_on_multi
+00016320: 706c 655f 736f 7572 6365 7328 7365 6c66  ple_sources(self
+00016330: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00016340: 2020 2072 6f6f 7420 3d20 5061 7468 2844     root = Path(D
+00016350: 4154 415f 4449 5220 2f20 2267 6974 6967  ATA_DIR / "gitig
+00016360: 6e6f 7265 5f75 7365 645f 6f6e 5f6d 756c  nore_used_on_mul
+00016370: 7469 706c 655f 736f 7572 6365 7322 290a  tiple_sources").
+00016380: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+00016390: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+000163a0: 2072 6f6f 7420 2f20 2264 6972 3122 202f   root / "dir1" /
+000163b0: 2022 622e 7079 222c 0a20 2020 2020 2020   "b.py",.       
+000163c0: 2020 2020 2072 6f6f 7420 2f20 2264 6972       root / "dir
+000163d0: 3222 202f 2022 622e 7079 222c 0a20 2020  2" / "b.py",.   
+000163e0: 2020 2020 205d 0a20 2020 2020 2020 2063       ].        c
+000163f0: 7478 203d 2046 616b 6543 6f6e 7465 7874  tx = FakeContext
+00016400: 2829 0a20 2020 2020 2020 2063 7478 2e6f  ().        ctx.o
+00016410: 626a 5b22 726f 6f74 225d 203d 2072 6f6f  bj["root"] = roo
+00016420: 740a 2020 2020 2020 2020 7372 6320 3d20  t.        src = 
+00016430: 5b72 6f6f 7420 2f20 2264 6972 3122 2c20  [root / "dir1", 
+00016440: 726f 6f74 202f 2022 6469 7232 225d 0a20  root / "dir2"]. 
+00016450: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
+00016460: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
+00016470: 7372 632c 2065 7870 6563 7465 642c 2063  src, expected, c
+00016480: 7478 3d63 7478 290a 0a20 2020 2040 7061  tx=ctx)..    @pa
+00016490: 7463 6828 2263 6572 6369 732e 6669 6e64  tch("cercis.find
+000164a0: 5f70 726f 6a65 6374 5f72 6f6f 7422 2c20  _project_root", 
+000164b0: 6c61 6d62 6461 202a 6172 6773 3a20 2854  lambda *args: (T
+000164c0: 4849 535f 4449 522e 7265 736f 6c76 6528  HIS_DIR.resolve(
+000164d0: 292c 204e 6f6e 6529 290a 2020 2020 6465  ), None)).    de
+000164e0: 6620 7465 7374 5f65 7863 6c75 6465 5f66  f test_exclude_f
+000164f0: 6f72 5f69 7373 7565 5f31 3537 3228 7365  or_issue_1572(se
+00016500: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00016510: 2020 2020 2023 2045 7863 6c75 6465 2073       # Exclude s
+00016520: 686f 756c 646e 2774 2074 6f75 6368 2066  houldn't touch f
+00016530: 696c 6573 2074 6861 7420 7765 7265 2065  iles that were e
+00016540: 7870 6c69 6369 746c 7920 6769 7665 6e20  xplicitly given 
+00016550: 746f 2042 6c61 636b 2074 6872 6f75 6768  to Black through
+00016560: 2074 6865 0a20 2020 2020 2020 2023 2043   the.        # C
+00016570: 4c49 2e20 4578 636c 7564 6520 6973 2073  LI. Exclude is s
+00016580: 7570 706f 7365 6420 746f 206f 6e6c 7920  upposed to only 
+00016590: 6170 706c 7920 746f 2074 6865 2072 6563  apply to the rec
+000165a0: 7572 7369 7665 2064 6973 636f 7665 7279  ursive discovery
+000165b0: 206f 6620 6669 6c65 732e 0a20 2020 2020   of files..     
+000165c0: 2020 2023 2068 7474 7073 3a2f 2f67 6974     # https://git
+000165d0: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
+000165e0: 6b2f 6973 7375 6573 2f31 3537 320a 2020  k/issues/1572.  
+000165f0: 2020 2020 2020 7061 7468 203d 2044 4154        path = DAT
+00016600: 415f 4449 5220 2f20 2269 6e63 6c75 6465  A_DIR / "include
+00016610: 5f65 7863 6c75 6465 5f74 6573 7473 220a  _exclude_tests".
+00016620: 2020 2020 2020 2020 7372 6320 3d20 5b70          src = [p
+00016630: 6174 6820 2f20 2262 2f65 7863 6c75 6465  ath / "b/exclude
+00016640: 2f61 2e70 7922 5d0a 2020 2020 2020 2020  /a.py"].        
+00016650: 6578 7065 6374 6564 203d 205b 7061 7468  expected = [path
+00016660: 202f 2022 622f 6578 636c 7564 652f 612e   / "b/exclude/a.
+00016670: 7079 225d 0a20 2020 2020 2020 2061 7373  py"].        ass
+00016680: 6572 745f 636f 6c6c 6563 7465 645f 736f  ert_collected_so
+00016690: 7572 6365 7328 7372 632c 2065 7870 6563  urces(src, expec
+000166a0: 7465 642c 2069 6e63 6c75 6465 3d22 222c  ted, include="",
+000166b0: 2065 7863 6c75 6465 3d72 222f 6578 636c   exclude=r"/excl
+000166c0: 7564 652f 7c61 5c2e 7079 2229 0a0a 2020  ude/|a\.py")..  
+000166d0: 2020 6465 6620 7465 7374 5f67 6974 6967    def test_gitig
+000166e0: 6e6f 7265 5f65 7863 6c75 6465 2873 656c  nore_exclude(sel
+000166f0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00016700: 2020 2020 7061 7468 203d 2054 4849 535f      path = THIS_
+00016710: 4449 5220 2f20 2264 6174 6122 202f 2022  DIR / "data" / "
+00016720: 696e 636c 7564 655f 6578 636c 7564 655f  include_exclude_
+00016730: 7465 7374 7322 0a20 2020 2020 2020 2069  tests".        i
+00016740: 6e63 6c75 6465 203d 2072 652e 636f 6d70  nclude = re.comp
+00016750: 696c 6528 7222 5c2e 7079 693f 2422 290a  ile(r"\.pyi?$").
+00016760: 2020 2020 2020 2020 6578 636c 7564 6520          exclude 
+00016770: 3d20 7265 2e63 6f6d 7069 6c65 2872 2222  = re.compile(r""
+00016780: 290a 2020 2020 2020 2020 7265 706f 7274  ).        report
+00016790: 203d 2063 6572 6369 732e 5265 706f 7274   = cercis.Report
+000167a0: 2829 0a20 2020 2020 2020 2067 6974 6967  ().        gitig
+000167b0: 6e6f 7265 203d 2050 6174 6853 7065 632e  nore = PathSpec.
+000167c0: 6672 6f6d 5f6c 696e 6573 280a 2020 2020  from_lines(.    
+000167d0: 2020 2020 2020 2020 2267 6974 7769 6c64          "gitwild
+000167e0: 6d61 7463 6822 2c20 5b22 6578 636c 7564  match", ["exclud
+000167f0: 652f 222c 2022 2e64 6566 696e 6974 656c  e/", ".definitel
+00016800: 795f 6578 636c 7564 6522 5d0a 2020 2020  y_exclude"].    
+00016810: 2020 2020 290a 2020 2020 2020 2020 736f      ).        so
+00016820: 7572 6365 733a 204c 6973 745b 5061 7468  urces: List[Path
+00016830: 5d20 3d20 5b5d 0a20 2020 2020 2020 2065  ] = [].        e
+00016840: 7870 6563 7465 6420 3d20 5b0a 2020 2020  xpected = [.    
+00016850: 2020 2020 2020 2020 5061 7468 2870 6174          Path(pat
+00016860: 6820 2f20 2262 2f64 6f6e 745f 6578 636c  h / "b/dont_excl
+00016870: 7564 652f 612e 7079 2229 2c0a 2020 2020  ude/a.py"),.    
+00016880: 2020 2020 2020 2020 5061 7468 2870 6174          Path(pat
+00016890: 6820 2f20 2262 2f64 6f6e 745f 6578 636c  h / "b/dont_excl
+000168a0: 7564 652f 612e 7079 6922 292c 0a20 2020  ude/a.pyi"),.   
+000168b0: 2020 2020 205d 0a20 2020 2020 2020 2074       ].        t
+000168c0: 6869 735f 6162 7320 3d20 5448 4953 5f44  his_abs = THIS_D
+000168d0: 4952 2e72 6573 6f6c 7665 2829 0a20 2020  IR.resolve().   
+000168e0: 2020 2020 2073 6f75 7263 6573 2e65 7874       sources.ext
+000168f0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+00016900: 2063 6572 6369 732e 6765 6e5f 7079 7468   cercis.gen_pyth
+00016910: 6f6e 5f66 696c 6573 280a 2020 2020 2020  on_files(.      
+00016920: 2020 2020 2020 2020 2020 7061 7468 2e69            path.i
+00016930: 7465 7264 6972 2829 2c0a 2020 2020 2020  terdir(),.      
+00016940: 2020 2020 2020 2020 2020 7468 6973 5f61            this_a
+00016950: 6273 2c0a 2020 2020 2020 2020 2020 2020  bs,.            
+00016960: 2020 2020 696e 636c 7564 652c 0a20 2020      include,.   
+00016970: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00016980: 6c75 6465 2c0a 2020 2020 2020 2020 2020  lude,.          
+00016990: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
+000169a0: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
+000169b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000169c0: 2020 7265 706f 7274 2c0a 2020 2020 2020    report,.      
+000169d0: 2020 2020 2020 2020 2020 7b70 6174 683a            {path:
+000169e0: 2067 6974 6967 6e6f 7265 7d2c 0a20 2020   gitignore},.   
+000169f0: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+00016a00: 626f 7365 3d46 616c 7365 2c0a 2020 2020  bose=False,.    
+00016a10: 2020 2020 2020 2020 2020 2020 7175 6965              quie
+00016a20: 743d 4661 6c73 652c 0a20 2020 2020 2020  t=False,.       
+00016a30: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+00016a40: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00016a50: 736f 7274 6564 2865 7870 6563 7465 6429  sorted(expected)
+00016a60: 203d 3d20 736f 7274 6564 2873 6f75 7263   == sorted(sourc
+00016a70: 6573 290a 0a20 2020 2064 6566 2074 6573  es)..    def tes
+00016a80: 745f 6e65 7374 6564 5f67 6974 6967 6e6f  t_nested_gitigno
+00016a90: 7265 2873 656c 6629 202d 3e20 4e6f 6e65  re(self) -> None
+00016aa0: 3a0a 2020 2020 2020 2020 7061 7468 203d  :.        path =
+00016ab0: 2050 6174 6828 5448 4953 5f44 4952 202f   Path(THIS_DIR /
+00016ac0: 2022 6461 7461 2220 2f20 226e 6573 7465   "data" / "neste
+00016ad0: 645f 6769 7469 676e 6f72 655f 7465 7374  d_gitignore_test
+00016ae0: 7322 290a 2020 2020 2020 2020 696e 636c  s").        incl
+00016af0: 7564 6520 3d20 7265 2e63 6f6d 7069 6c65  ude = re.compile
+00016b00: 2872 225c 2e70 7969 3f24 2229 0a20 2020  (r"\.pyi?$").   
+00016b10: 2020 2020 2065 7863 6c75 6465 203d 2072       exclude = r
+00016b20: 652e 636f 6d70 696c 6528 7222 2229 0a20  e.compile(r""). 
+00016b30: 2020 2020 2020 2072 6f6f 745f 6769 7469         root_giti
+00016b40: 676e 6f72 6520 3d20 6365 7263 6973 2e66  gnore = cercis.f
+00016b50: 696c 6573 2e67 6574 5f67 6974 6967 6e6f  iles.get_gitigno
+00016b60: 7265 2870 6174 6829 0a20 2020 2020 2020  re(path).       
+00016b70: 2072 6570 6f72 7420 3d20 6365 7263 6973   report = cercis
+00016b80: 2e52 6570 6f72 7428 290a 2020 2020 2020  .Report().      
+00016b90: 2020 6578 7065 6374 6564 3a20 4c69 7374    expected: List
+00016ba0: 5b50 6174 685d 203d 205b 0a20 2020 2020  [Path] = [.     
+00016bb0: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
+00016bc0: 202f 2022 782e 7079 2229 2c0a 2020 2020   / "x.py"),.    
+00016bd0: 2020 2020 2020 2020 5061 7468 2870 6174          Path(pat
+00016be0: 6820 2f20 2272 6f6f 742f 622e 7079 2229  h / "root/b.py")
+00016bf0: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
+00016c00: 7468 2870 6174 6820 2f20 2272 6f6f 742f  th(path / "root/
+00016c10: 632e 7079 2229 2c0a 2020 2020 2020 2020  c.py"),.        
+00016c20: 2020 2020 5061 7468 2870 6174 6820 2f20      Path(path / 
+00016c30: 2272 6f6f 742f 6368 696c 642f 632e 7079  "root/child/c.py
+00016c40: 2229 2c0a 2020 2020 2020 2020 5d0a 2020  "),.        ].  
+00016c50: 2020 2020 2020 7468 6973 5f61 6273 203d        this_abs =
+00016c60: 2054 4849 535f 4449 522e 7265 736f 6c76   THIS_DIR.resolv
+00016c70: 6528 290a 2020 2020 2020 2020 736f 7572  e().        sour
+00016c80: 6365 7320 3d20 6c69 7374 280a 2020 2020  ces = list(.    
+00016c90: 2020 2020 2020 2020 6365 7263 6973 2e67          cercis.g
+00016ca0: 656e 5f70 7974 686f 6e5f 6669 6c65 7328  en_python_files(
+00016cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016cc0: 2070 6174 682e 6974 6572 6469 7228 292c   path.iterdir(),
+00016cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ce0: 2074 6869 735f 6162 732c 0a20 2020 2020   this_abs,.     
+00016cf0: 2020 2020 2020 2020 2020 2069 6e63 6c75             inclu
+00016d00: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00016d10: 2020 2020 6578 636c 7564 652c 0a20 2020      exclude,.   
+00016d20: 2020 2020 2020 2020 2020 2020 204e 6f6e               Non
+00016d30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00016d40: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
+00016d50: 2020 2020 2020 2020 2072 6570 6f72 742c           report,
+00016d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d70: 207b 7061 7468 3a20 726f 6f74 5f67 6974   {path: root_git
+00016d80: 6967 6e6f 7265 7d2c 0a20 2020 2020 2020  ignore},.       
+00016d90: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
+00016da0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00016db0: 2020 2020 2020 2020 7175 6965 743d 4661          quiet=Fa
+00016dc0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00016dd0: 2029 0a20 2020 2020 2020 2029 0a20 2020   ).        ).   
+00016de0: 2020 2020 2061 7373 6572 7420 736f 7274       assert sort
+00016df0: 6564 2865 7870 6563 7465 6429 203d 3d20  ed(expected) == 
+00016e00: 736f 7274 6564 2873 6f75 7263 6573 290a  sorted(sources).
+00016e10: 0a20 2020 2064 6566 2074 6573 745f 6e65  .    def test_ne
+00016e20: 7374 6564 5f67 6974 6967 6e6f 7265 5f64  sted_gitignore_d
+00016e30: 6972 6563 746c 795f 696e 5f73 6f75 7263  irectly_in_sourc
+00016e40: 655f 6469 7265 6374 6f72 7928 7365 6c66  e_directory(self
+00016e50: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00016e60: 2020 2023 2068 7474 7073 3a2f 2f67 6974     # https://git
+00016e70: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
+00016e80: 6b2f 6973 7375 6573 2f32 3539 380a 2020  k/issues/2598.  
+00016e90: 2020 2020 2020 7061 7468 203d 2050 6174        path = Pat
+00016ea0: 6828 4441 5441 5f44 4952 202f 2022 6e65  h(DATA_DIR / "ne
+00016eb0: 7374 6564 5f67 6974 6967 6e6f 7265 5f74  sted_gitignore_t
+00016ec0: 6573 7473 2229 0a20 2020 2020 2020 2073  ests").        s
+00016ed0: 7263 203d 2050 6174 6828 7061 7468 202f  rc = Path(path /
+00016ee0: 2022 726f 6f74 2220 2f20 2263 6869 6c64   "root" / "child
+00016ef0: 2229 0a20 2020 2020 2020 2065 7870 6563  ").        expec
+00016f00: 7465 6420 3d20 5b73 7263 202f 2022 612e  ted = [src / "a.
+00016f10: 7079 222c 2073 7263 202f 2022 632e 7079  py", src / "c.py
+00016f20: 225d 0a20 2020 2020 2020 2061 7373 6572  "].        asser
+00016f30: 745f 636f 6c6c 6563 7465 645f 736f 7572  t_collected_sour
+00016f40: 6365 7328 5b73 7263 5d2c 2065 7870 6563  ces([src], expec
+00016f50: 7465 6429 0a0a 2020 2020 6465 6620 7465  ted)..    def te
+00016f60: 7374 5f69 6e76 616c 6964 5f67 6974 6967  st_invalid_gitig
+00016f70: 6e6f 7265 2873 656c 6629 202d 3e20 4e6f  nore(self) -> No
+00016f80: 6e65 3a0a 2020 2020 2020 2020 7061 7468  ne:.        path
+00016f90: 203d 2054 4849 535f 4449 5220 2f20 2264   = THIS_DIR / "d
+00016fa0: 6174 6122 202f 2022 696e 7661 6c69 645f  ata" / "invalid_
+00016fb0: 6769 7469 676e 6f72 655f 7465 7374 7322  gitignore_tests"
+00016fc0: 0a20 2020 2020 2020 2065 6d70 7479 5f63  .        empty_c
+00016fd0: 6f6e 6669 6720 3d20 7061 7468 202f 2022  onfig = path / "
+00016fe0: 7079 7072 6f6a 6563 742e 746f 6d6c 220a  pyproject.toml".
+00016ff0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00017000: 2042 6c61 636b 5275 6e6e 6572 2829 2e69   BlackRunner().i
+00017010: 6e76 6f6b 6528 0a20 2020 2020 2020 2020  nvoke(.         
+00017020: 2020 2063 6572 6369 732e 6d61 696e 2c20     cercis.main, 
+00017030: 5b22 2d2d 7665 7262 6f73 6522 2c20 222d  ["--verbose", "-
+00017040: 2d63 6f6e 6669 6722 2c20 7374 7228 656d  -config", str(em
+00017050: 7074 795f 636f 6e66 6967 292c 2073 7472  pty_config), str
+00017060: 2870 6174 6829 5d0a 2020 2020 2020 2020  (path)].        
+00017070: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00017080: 2072 6573 756c 742e 6578 6974 5f63 6f64   result.exit_cod
+00017090: 6520 3d3d 2031 0a20 2020 2020 2020 2061  e == 1.        a
+000170a0: 7373 6572 7420 7265 7375 6c74 2e73 7464  ssert result.std
+000170b0: 6572 725f 6279 7465 7320 6973 206e 6f74  err_bytes is not
+000170c0: 204e 6f6e 650a 0a20 2020 2020 2020 2067   None..        g
+000170d0: 6974 6967 6e6f 7265 203d 2070 6174 6820  itignore = path 
+000170e0: 2f20 222e 6769 7469 676e 6f72 6522 0a20  / ".gitignore". 
+000170f0: 2020 2020 2020 2061 7373 6572 7420 6622         assert f"
+00017100: 436f 756c 6420 6e6f 7420 7061 7273 6520  Could not parse 
+00017110: 7b67 6974 6967 6e6f 7265 7d22 2069 6e20  {gitignore}" in 
+00017120: 7265 7375 6c74 2e73 7464 6572 725f 6279  result.stderr_by
+00017130: 7465 732e 6465 636f 6465 2829 0a0a 2020  tes.decode()..  
+00017140: 2020 6465 6620 7465 7374 5f69 6e76 616c    def test_inval
+00017150: 6964 5f6e 6573 7465 645f 6769 7469 676e  id_nested_gitign
+00017160: 6f72 6528 7365 6c66 2920 2d3e 204e 6f6e  ore(self) -> Non
+00017170: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
+00017180: 3d20 5448 4953 5f44 4952 202f 2022 6461  = THIS_DIR / "da
+00017190: 7461 2220 2f20 2269 6e76 616c 6964 5f6e  ta" / "invalid_n
+000171a0: 6573 7465 645f 6769 7469 676e 6f72 655f  ested_gitignore_
+000171b0: 7465 7374 7322 0a20 2020 2020 2020 2065  tests".        e
+000171c0: 6d70 7479 5f63 6f6e 6669 6720 3d20 7061  mpty_config = pa
+000171d0: 7468 202f 2022 7079 7072 6f6a 6563 742e  th / "pyproject.
+000171e0: 746f 6d6c 220a 2020 2020 2020 2020 7265  toml".        re
+000171f0: 7375 6c74 203d 2042 6c61 636b 5275 6e6e  sult = BlackRunn
+00017200: 6572 2829 2e69 6e76 6f6b 6528 0a20 2020  er().invoke(.   
+00017210: 2020 2020 2020 2020 2063 6572 6369 732e           cercis.
+00017220: 6d61 696e 2c20 5b22 2d2d 7665 7262 6f73  main, ["--verbos
+00017230: 6522 2c20 222d 2d63 6f6e 6669 6722 2c20  e", "--config", 
+00017240: 7374 7228 656d 7074 795f 636f 6e66 6967  str(empty_config
+00017250: 292c 2073 7472 2870 6174 6829 5d0a 2020  ), str(path)].  
+00017260: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00017270: 6173 7365 7274 2072 6573 756c 742e 6578  assert result.ex
+00017280: 6974 5f63 6f64 6520 3d3d 2031 0a20 2020  it_code == 1.   
+00017290: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
+000172a0: 6c74 2e73 7464 6572 725f 6279 7465 7320  lt.stderr_bytes 
+000172b0: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
+000172c0: 2020 2020 2067 6974 6967 6e6f 7265 203d       gitignore =
+000172d0: 2070 6174 6820 2f20 2261 2220 2f20 222e   path / "a" / ".
+000172e0: 6769 7469 676e 6f72 6522 0a20 2020 2020  gitignore".     
+000172f0: 2020 2061 7373 6572 7420 6622 436f 756c     assert f"Coul
+00017300: 6420 6e6f 7420 7061 7273 6520 7b67 6974  d not parse {git
+00017310: 6967 6e6f 7265 7d22 2069 6e20 7265 7375  ignore}" in resu
+00017320: 6c74 2e73 7464 6572 725f 6279 7465 732e  lt.stderr_bytes.
+00017330: 6465 636f 6465 2829 0a0a 2020 2020 6465  decode()..    de
+00017340: 6620 7465 7374 5f67 6974 6967 6e6f 7265  f test_gitignore
+00017350: 5f74 6861 745f 6967 6e6f 7265 735f 7375  _that_ignores_su
+00017360: 6266 6f6c 6465 7273 2873 656c 6629 202d  bfolders(self) -
+00017370: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00017380: 2320 4966 2067 6974 6967 6e6f 7265 2077  # If gitignore w
+00017390: 6974 6820 2a2f 2a20 6973 2069 6e20 726f  ith */* is in ro
+000173a0: 6f74 0a20 2020 2020 2020 2072 6f6f 7420  ot.        root 
+000173b0: 3d20 5061 7468 2844 4154 415f 4449 5220  = Path(DATA_DIR 
+000173c0: 2f20 2269 676e 6f72 655f 7375 6266 6f6c  / "ignore_subfol
+000173d0: 6465 7273 5f67 6974 6967 6e6f 7265 5f74  ders_gitignore_t
+000173e0: 6573 7473 2220 2f20 2273 7562 6469 7222  ests" / "subdir"
+000173f0: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
+00017400: 6564 203d 205b 726f 6f74 202f 2022 622e  ed = [root / "b.
+00017410: 7079 225d 0a20 2020 2020 2020 2063 7478  py"].        ctx
+00017420: 203d 2046 616b 6543 6f6e 7465 7874 2829   = FakeContext()
+00017430: 0a20 2020 2020 2020 2063 7478 2e6f 626a  .        ctx.obj
+00017440: 5b22 726f 6f74 225d 203d 2072 6f6f 740a  ["root"] = root.
+00017450: 2020 2020 2020 2020 6173 7365 7274 5f63          assert_c
+00017460: 6f6c 6c65 6374 6564 5f73 6f75 7263 6573  ollected_sources
+00017470: 285b 726f 6f74 5d2c 2065 7870 6563 7465  ([root], expecte
+00017480: 642c 2063 7478 3d63 7478 290a 0a20 2020  d, ctx=ctx)..   
+00017490: 2020 2020 2023 2049 6620 2e67 6974 6967       # If .gitig
+000174a0: 6e6f 7265 2077 6974 6820 2a2f 2a20 6973  nore with */* is
+000174b0: 206e 6573 7465 640a 2020 2020 2020 2020   nested.        
+000174c0: 726f 6f74 203d 2050 6174 6828 4441 5441  root = Path(DATA
+000174d0: 5f44 4952 202f 2022 6967 6e6f 7265 5f73  _DIR / "ignore_s
+000174e0: 7562 666f 6c64 6572 735f 6769 7469 676e  ubfolders_gitign
+000174f0: 6f72 655f 7465 7374 7322 290a 2020 2020  ore_tests").    
+00017500: 2020 2020 6578 7065 6374 6564 203d 205b      expected = [
+00017510: 0a20 2020 2020 2020 2020 2020 2072 6f6f  .            roo
+00017520: 7420 2f20 2261 2e70 7922 2c0a 2020 2020  t / "a.py",.    
+00017530: 2020 2020 2020 2020 726f 6f74 202f 2022          root / "
+00017540: 7375 6264 6972 2220 2f20 2262 2e70 7922  subdir" / "b.py"
+00017550: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00017560: 2020 2020 6374 7820 3d20 4661 6b65 436f      ctx = FakeCo
+00017570: 6e74 6578 7428 290a 2020 2020 2020 2020  ntext().        
+00017580: 6374 782e 6f62 6a5b 2272 6f6f 7422 5d20  ctx.obj["root"] 
+00017590: 3d20 726f 6f74 0a20 2020 2020 2020 2061  = root.        a
+000175a0: 7373 6572 745f 636f 6c6c 6563 7465 645f  ssert_collected_
+000175b0: 736f 7572 6365 7328 5b72 6f6f 745d 2c20  sources([root], 
+000175c0: 6578 7065 6374 6564 2c20 6374 783d 6374  expected, ctx=ct
+000175d0: 7829 0a0a 2020 2020 2020 2020 2320 4966  x)..        # If
+000175e0: 2063 6f6d 6d61 6e64 2069 7320 6578 6563   command is exec
+000175f0: 7574 6564 2066 726f 6d20 6f75 7465 7220  uted from outer 
+00017600: 6469 720a 2020 2020 2020 2020 726f 6f74  dir.        root
+00017610: 203d 2050 6174 6828 4441 5441 5f44 4952   = Path(DATA_DIR
+00017620: 202f 2022 6967 6e6f 7265 5f73 7562 666f   / "ignore_subfo
+00017630: 6c64 6572 735f 6769 7469 676e 6f72 655f  lders_gitignore_
+00017640: 7465 7374 7322 290a 2020 2020 2020 2020  tests").        
+00017650: 7461 7267 6574 203d 2072 6f6f 7420 2f20  target = root / 
+00017660: 2273 7562 6469 7222 0a20 2020 2020 2020  "subdir".       
+00017670: 2065 7870 6563 7465 6420 3d20 5b74 6172   expected = [tar
+00017680: 6765 7420 2f20 2262 2e70 7922 5d0a 2020  get / "b.py"].  
+00017690: 2020 2020 2020 6374 7820 3d20 4661 6b65        ctx = Fake
+000176a0: 436f 6e74 6578 7428 290a 2020 2020 2020  Context().      
+000176b0: 2020 6374 782e 6f62 6a5b 2272 6f6f 7422    ctx.obj["root"
+000176c0: 5d20 3d20 726f 6f74 0a20 2020 2020 2020  ] = root.       
+000176d0: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
+000176e0: 645f 736f 7572 6365 7328 5b74 6172 6765  d_sources([targe
+000176f0: 745d 2c20 6578 7065 6374 6564 2c20 6374  t], expected, ct
+00017700: 783d 6374 7829 0a0a 2020 2020 6465 6620  x=ctx)..    def 
+00017710: 7465 7374 5f65 6d70 7479 5f69 6e63 6c75  test_empty_inclu
+00017720: 6465 2873 656c 6629 202d 3e20 4e6f 6e65  de(self) -> None
+00017730: 3a0a 2020 2020 2020 2020 7061 7468 203d  :.        path =
+00017740: 2044 4154 415f 4449 5220 2f20 2269 6e63   DATA_DIR / "inc
+00017750: 6c75 6465 5f65 7863 6c75 6465 5f74 6573  lude_exclude_tes
+00017760: 7473 220a 2020 2020 2020 2020 7372 6320  ts".        src 
+00017770: 3d20 5b70 6174 685d 0a20 2020 2020 2020  = [path].       
+00017780: 2065 7870 6563 7465 6420 3d20 5b0a 2020   expected = [.  
+00017790: 2020 2020 2020 2020 2020 5061 7468 2870            Path(p
+000177a0: 6174 6820 2f20 2262 2f65 7863 6c75 6465  ath / "b/exclude
+000177b0: 2f61 2e70 6965 2229 2c0a 2020 2020 2020  /a.pie"),.      
+000177c0: 2020 2020 2020 5061 7468 2870 6174 6820        Path(path 
+000177d0: 2f20 2262 2f65 7863 6c75 6465 2f61 2e70  / "b/exclude/a.p
+000177e0: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
+000177f0: 2050 6174 6828 7061 7468 202f 2022 622f   Path(path / "b/
+00017800: 6578 636c 7564 652f 612e 7079 6922 292c  exclude/a.pyi"),
+00017810: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
+00017820: 6828 7061 7468 202f 2022 622f 646f 6e74  h(path / "b/dont
+00017830: 5f65 7863 6c75 6465 2f61 2e70 6965 2229  _exclude/a.pie")
+00017840: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
+00017850: 7468 2870 6174 6820 2f20 2262 2f64 6f6e  th(path / "b/don
+00017860: 745f 6578 636c 7564 652f 612e 7079 2229  t_exclude/a.py")
+00017870: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
+00017880: 7468 2870 6174 6820 2f20 2262 2f64 6f6e  th(path / "b/don
+00017890: 745f 6578 636c 7564 652f 612e 7079 6922  t_exclude/a.pyi"
+000178a0: 292c 0a20 2020 2020 2020 2020 2020 2050  ),.            P
+000178b0: 6174 6828 7061 7468 202f 2022 622f 2e64  ath(path / "b/.d
+000178c0: 6566 696e 6974 656c 795f 6578 636c 7564  efinitely_exclud
+000178d0: 652f 612e 7069 6522 292c 0a20 2020 2020  e/a.pie"),.     
+000178e0: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
+000178f0: 202f 2022 622f 2e64 6566 696e 6974 656c   / "b/.definitel
+00017900: 795f 6578 636c 7564 652f 612e 7079 2229  y_exclude/a.py")
+00017910: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
+00017920: 7468 2870 6174 6820 2f20 2262 2f2e 6465  th(path / "b/.de
+00017930: 6669 6e69 7465 6c79 5f65 7863 6c75 6465  finitely_exclude
+00017940: 2f61 2e70 7969 2229 2c0a 2020 2020 2020  /a.pyi"),.      
+00017950: 2020 2020 2020 5061 7468 2870 6174 6820        Path(path 
+00017960: 2f20 222e 6769 7469 676e 6f72 6522 292c  / ".gitignore"),
+00017970: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
+00017980: 6828 7061 7468 202f 2022 7079 7072 6f6a  h(path / "pyproj
+00017990: 6563 742e 746f 6d6c 2229 2c0a 2020 2020  ect.toml"),.    
+000179a0: 2020 2020 5d0a 2020 2020 2020 2020 2320      ].        # 
+000179b0: 5365 7474 696e 6720 6578 636c 7564 6520  Setting exclude 
+000179c0: 6578 706c 6963 6974 6c79 2074 6f20 616e  explicitly to an
+000179d0: 2065 6d70 7479 2073 7472 696e 6720 746f   empty string to
+000179e0: 2062 6c6f 636b 202e 6769 7469 676e 6f72   block .gitignor
+000179f0: 6520 7573 6167 652e 0a20 2020 2020 2020  e usage..       
+00017a00: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
+00017a10: 645f 736f 7572 6365 7328 7372 632c 2065  d_sources(src, e
+00017a20: 7870 6563 7465 642c 2069 6e63 6c75 6465  xpected, include
+00017a30: 3d22 222c 2065 7863 6c75 6465 3d22 2229  ="", exclude="")
+00017a40: 0a0a 2020 2020 6465 6620 7465 7374 5f65  ..    def test_e
+00017a50: 7874 656e 645f 6578 636c 7564 6528 7365  xtend_exclude(se
+00017a60: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00017a70: 2020 2020 2070 6174 6820 3d20 4441 5441       path = DATA
+00017a80: 5f44 4952 202f 2022 696e 636c 7564 655f  _DIR / "include_
+00017a90: 6578 636c 7564 655f 7465 7374 7322 0a20  exclude_tests". 
+00017aa0: 2020 2020 2020 2073 7263 203d 205b 7061         src = [pa
+00017ab0: 7468 5d0a 2020 2020 2020 2020 6578 7065  th].        expe
+00017ac0: 6374 6564 203d 205b 0a20 2020 2020 2020  cted = [.       
+00017ad0: 2020 2020 2050 6174 6828 7061 7468 202f       Path(path /
+00017ae0: 2022 622f 6578 636c 7564 652f 612e 7079   "b/exclude/a.py
+00017af0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00017b00: 5061 7468 2870 6174 6820 2f20 2262 2f64  Path(path / "b/d
+00017b10: 6f6e 745f 6578 636c 7564 652f 612e 7079  ont_exclude/a.py
+00017b20: 2229 2c0a 2020 2020 2020 2020 5d0a 2020  "),.        ].  
+00017b30: 2020 2020 2020 6173 7365 7274 5f63 6f6c        assert_col
+00017b40: 6c65 6374 6564 5f73 6f75 7263 6573 280a  lected_sources(.
+00017b50: 2020 2020 2020 2020 2020 2020 7372 632c              src,
+00017b60: 2065 7870 6563 7465 642c 2065 7863 6c75   expected, exclu
+00017b70: 6465 3d72 225c 2e70 7969 2422 2c20 6578  de=r"\.pyi$", ex
+00017b80: 7465 6e64 5f65 7863 6c75 6465 3d72 225c  tend_exclude=r"\
+00017b90: 2e64 6566 696e 6974 656c 795f 6578 636c  .definitely_excl
+00017ba0: 7564 6522 0a20 2020 2020 2020 2029 0a0a  ude".        )..
+00017bb0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00017bc0: 2e69 6e63 6f6d 7061 7469 626c 655f 7769  .incompatible_wi
+00017bd0: 7468 5f6d 7970 7963 0a20 2020 2064 6566  th_mypyc.    def
+00017be0: 2074 6573 745f 7379 6d6c 696e 6b5f 6f75   test_symlink_ou
+00017bf0: 745f 6f66 5f72 6f6f 745f 6469 7265 6374  t_of_root_direct
+00017c00: 6f72 7928 7365 6c66 2920 2d3e 204e 6f6e  ory(self) -> Non
+00017c10: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
+00017c20: 3d20 4d61 6769 634d 6f63 6b28 290a 2020  = MagicMock().  
+00017c30: 2020 2020 2020 726f 6f74 203d 2054 4849        root = THI
+00017c40: 535f 4449 522e 7265 736f 6c76 6528 290a  S_DIR.resolve().
+00017c50: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
+00017c60: 4d61 6769 634d 6f63 6b28 290a 2020 2020  MagicMock().    
+00017c70: 2020 2020 696e 636c 7564 6520 3d20 7265      include = re
+00017c80: 2e63 6f6d 7069 6c65 2863 6572 6369 732e  .compile(cercis.
+00017c90: 4445 4641 554c 545f 494e 434c 5544 4553  DEFAULT_INCLUDES
+00017ca0: 290a 2020 2020 2020 2020 6578 636c 7564  ).        exclud
+00017cb0: 6520 3d20 7265 2e63 6f6d 7069 6c65 2863  e = re.compile(c
+00017cc0: 6572 6369 732e 4445 4641 554c 545f 4558  ercis.DEFAULT_EX
+00017cd0: 434c 5544 4553 290a 2020 2020 2020 2020  CLUDES).        
+00017ce0: 7265 706f 7274 203d 2063 6572 6369 732e  report = cercis.
+00017cf0: 5265 706f 7274 2829 0a20 2020 2020 2020  Report().       
+00017d00: 2067 6974 6967 6e6f 7265 203d 2050 6174   gitignore = Pat
+00017d10: 6853 7065 632e 6672 6f6d 5f6c 696e 6573  hSpec.from_lines
+00017d20: 2822 6769 7477 696c 646d 6174 6368 222c  ("gitwildmatch",
+00017d30: 205b 5d29 0a20 2020 2020 2020 2023 2060   []).        # `
+00017d40: 6368 696c 6460 2073 686f 756c 6420 6265  child` should be
+00017d50: 6861 7665 206c 696b 6520 6120 7379 6d6c  have like a syml
+00017d60: 696e 6b20 7768 6963 6820 7265 736f 6c76  ink which resolv
+00017d70: 6564 2070 6174 6820 6973 2063 6c65 6172  ed path is clear
+00017d80: 6c79 0a20 2020 2020 2020 2023 206f 7574  ly.        # out
+00017d90: 7369 6465 206f 6620 7468 6520 6072 6f6f  side of the `roo
+00017da0: 7460 2064 6972 6563 746f 7279 2e0a 2020  t` directory..  
+00017db0: 2020 2020 2020 7061 7468 2e69 7465 7264        path.iterd
+00017dc0: 6972 2e72 6574 7572 6e5f 7661 6c75 6520  ir.return_value 
+00017dd0: 3d20 5b63 6869 6c64 5d0a 2020 2020 2020  = [child].      
+00017de0: 2020 6368 696c 642e 7265 736f 6c76 652e    child.resolve.
+00017df0: 7265 7475 726e 5f76 616c 7565 203d 2050  return_value = P
+00017e00: 6174 6828 222f 612f 622f 6322 290a 2020  ath("/a/b/c").  
+00017e10: 2020 2020 2020 6368 696c 642e 6173 5f70        child.as_p
+00017e20: 6f73 6978 2e72 6574 7572 6e5f 7661 6c75  osix.return_valu
+00017e30: 6520 3d20 222f 612f 622f 6322 0a20 2020  e = "/a/b/c".   
+00017e40: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00017e50: 2020 2020 2020 6c69 7374 280a 2020 2020        list(.    
+00017e60: 2020 2020 2020 2020 2020 2020 6365 7263              cerc
+00017e70: 6973 2e67 656e 5f70 7974 686f 6e5f 6669  is.gen_python_fi
+00017e80: 6c65 7328 0a20 2020 2020 2020 2020 2020  les(.           
+00017e90: 2020 2020 2020 2020 2070 6174 682e 6974           path.it
+00017ea0: 6572 6469 7228 292c 0a20 2020 2020 2020  erdir(),.       
+00017eb0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00017ec0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00017ed0: 2020 2020 2020 2069 6e63 6c75 6465 2c0a         include,.
+00017ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ef0: 2020 2020 6578 636c 7564 652c 0a20 2020      exclude,.   
+00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f10: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00017f20: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
+00017f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017f40: 2020 2020 2072 6570 6f72 742c 0a20 2020       report,.   
+00017f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f60: 207b 7061 7468 3a20 6769 7469 676e 6f72   {path: gitignor
+00017f70: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
+00017f80: 2020 2020 2020 2020 7665 7262 6f73 653d          verbose=
+00017f90: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00017fa0: 2020 2020 2020 2020 2020 2071 7569 6574             quiet
+00017fb0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00017fc0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00017fd0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00017fe0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+00017ff0: 7220 6173 2076 653a 0a20 2020 2020 2020  r as ve:.       
+00018000: 2020 2020 2070 7974 6573 742e 6661 696c       pytest.fail
+00018010: 2866 2260 6765 745f 7079 7468 6f6e 5f66  (f"`get_python_f
+00018020: 696c 6573 5f69 6e5f 6469 7228 2960 2066  iles_in_dir()` f
+00018030: 6169 6c65 643a 207b 7665 7d22 290a 2020  ailed: {ve}").  
+00018040: 2020 2020 2020 7061 7468 2e69 7465 7264        path.iterd
+00018050: 6972 2e61 7373 6572 745f 6361 6c6c 6564  ir.assert_called
+00018060: 5f6f 6e63 6528 290a 2020 2020 2020 2020  _once().        
+00018070: 6368 696c 642e 7265 736f 6c76 652e 6173  child.resolve.as
+00018080: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+00018090: 2829 0a0a 2020 2020 4070 6174 6368 2822  ()..    @patch("
+000180a0: 6365 7263 6973 2e66 696e 645f 7072 6f6a  cercis.find_proj
+000180b0: 6563 745f 726f 6f74 222c 206c 616d 6264  ect_root", lambd
+000180c0: 6120 2a61 7267 733a 2028 5448 4953 5f44  a *args: (THIS_D
+000180d0: 4952 2e72 6573 6f6c 7665 2829 2c20 4e6f  IR.resolve(), No
+000180e0: 6e65 2929 0a20 2020 2064 6566 2074 6573  ne)).    def tes
+000180f0: 745f 6765 745f 736f 7572 6365 735f 7769  t_get_sources_wi
+00018100: 7468 5f73 7464 696e 2873 656c 6629 202d  th_stdin(self) -
+00018110: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00018120: 7372 6320 3d20 5b22 2d22 5d0a 2020 2020  src = ["-"].    
+00018130: 2020 2020 6578 7065 6374 6564 203d 205b      expected = [
+00018140: 222d 225d 0a20 2020 2020 2020 2061 7373  "-"].        ass
+00018150: 6572 745f 636f 6c6c 6563 7465 645f 736f  ert_collected_so
+00018160: 7572 6365 7328 7372 632c 2065 7870 6563  urces(src, expec
+00018170: 7465 642c 2069 6e63 6c75 6465 3d22 222c  ted, include="",
+00018180: 2065 7863 6c75 6465 3d72 222f 6578 636c   exclude=r"/excl
+00018190: 7564 652f 7c61 5c2e 7079 2229 0a0a 2020  ude/|a\.py")..  
+000181a0: 2020 4070 6174 6368 2822 6365 7263 6973    @patch("cercis
+000181b0: 2e66 696e 645f 7072 6f6a 6563 745f 726f  .find_project_ro
+000181c0: 6f74 222c 206c 616d 6264 6120 2a61 7267  ot", lambda *arg
+000181d0: 733a 2028 5448 4953 5f44 4952 2e72 6573  s: (THIS_DIR.res
+000181e0: 6f6c 7665 2829 2c20 4e6f 6e65 2929 0a20  olve(), None)). 
+000181f0: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
+00018200: 736f 7572 6365 735f 7769 7468 5f73 7464  sources_with_std
+00018210: 696e 5f66 696c 656e 616d 6528 7365 6c66  in_filename(self
+00018220: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00018230: 2020 2073 7263 203d 205b 222d 225d 0a20     src = ["-"]. 
+00018240: 2020 2020 2020 2073 7464 696e 5f66 696c         stdin_fil
+00018250: 656e 616d 6520 3d20 7374 7228 5448 4953  ename = str(THIS
+00018260: 5f44 4952 202f 2022 6461 7461 2f63 6f6c  _DIR / "data/col
+00018270: 6c65 6374 696f 6e73 2e70 7922 290a 2020  lections.py").  
+00018280: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
+00018290: 205b 6622 5f5f 424c 4143 4b5f 5354 4449   [f"__BLACK_STDI
+000182a0: 4e5f 4649 4c45 4e41 4d45 5f5f 7b73 7464  N_FILENAME__{std
+000182b0: 696e 5f66 696c 656e 616d 657d 225d 0a20  in_filename}"]. 
+000182c0: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
+000182d0: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
+000182e0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
+000182f0: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
+00018300: 7065 6374 6564 2c0a 2020 2020 2020 2020  pected,.        
+00018310: 2020 2020 6578 636c 7564 653d 7222 2f65      exclude=r"/e
+00018320: 7863 6c75 6465 2f61 5c2e 7079 222c 0a20  xclude/a\.py",. 
+00018330: 2020 2020 2020 2020 2020 2073 7464 696e             stdin
+00018340: 5f66 696c 656e 616d 653d 7374 6469 6e5f  _filename=stdin_
+00018350: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
+00018360: 2020 290a 0a20 2020 2040 7061 7463 6828    )..    @patch(
+00018370: 2263 6572 6369 732e 6669 6e64 5f70 726f  "cercis.find_pro
+00018380: 6a65 6374 5f72 6f6f 7422 2c20 6c61 6d62  ject_root", lamb
+00018390: 6461 202a 6172 6773 3a20 2854 4849 535f  da *args: (THIS_
+000183a0: 4449 522e 7265 736f 6c76 6528 292c 204e  DIR.resolve(), N
+000183b0: 6f6e 6529 290a 2020 2020 6465 6620 7465  one)).    def te
+000183c0: 7374 5f67 6574 5f73 6f75 7263 6573 5f77  st_get_sources_w
+000183d0: 6974 685f 7374 6469 6e5f 6669 6c65 6e61  ith_stdin_filena
+000183e0: 6d65 5f61 6e64 5f65 7863 6c75 6465 2873  me_and_exclude(s
+000183f0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00018400: 2020 2020 2020 2320 4578 636c 7564 6520        # Exclude 
+00018410: 7368 6f75 6c64 6e27 7420 6578 636c 7564  shouldn't exclud
+00018420: 6520 7374 6469 6e5f 6669 6c65 6e61 6d65  e stdin_filename
+00018430: 2073 696e 6365 2069 7420 6973 206d 696d   since it is mim
+00018440: 6963 6b69 6e67 2074 6865 0a20 2020 2020  icking the.     
+00018450: 2020 2023 2066 696c 6520 6265 696e 6720     # file being 
+00018460: 7061 7373 6564 2064 6972 6563 746c 792e  passed directly.
+00018470: 2054 6869 7320 6973 2074 6865 2073 616d   This is the sam
+00018480: 6520 6173 0a20 2020 2020 2020 2023 2074  e as.        # t
+00018490: 6573 745f 6578 636c 7564 655f 666f 725f  est_exclude_for_
+000184a0: 6973 7375 655f 3135 3732 0a20 2020 2020  issue_1572.     
+000184b0: 2020 2070 6174 6820 3d20 4441 5441 5f44     path = DATA_D
+000184c0: 4952 202f 2022 696e 636c 7564 655f 6578  IR / "include_ex
+000184d0: 636c 7564 655f 7465 7374 7322 0a20 2020  clude_tests".   
+000184e0: 2020 2020 2073 7263 203d 205b 222d 225d       src = ["-"]
+000184f0: 0a20 2020 2020 2020 2073 7464 696e 5f66  .        stdin_f
+00018500: 696c 656e 616d 6520 3d20 7374 7228 7061  ilename = str(pa
+00018510: 7468 202f 2022 622f 6578 636c 7564 652f  th / "b/exclude/
+00018520: 612e 7079 2229 0a20 2020 2020 2020 2065  a.py").        e
+00018530: 7870 6563 7465 6420 3d20 5b66 225f 5f42  xpected = [f"__B
+00018540: 4c41 434b 5f53 5444 494e 5f46 494c 454e  LACK_STDIN_FILEN
+00018550: 414d 455f 5f7b 7374 6469 6e5f 6669 6c65  AME__{stdin_file
+00018560: 6e61 6d65 7d22 5d0a 2020 2020 2020 2020  name}"].        
+00018570: 6173 7365 7274 5f63 6f6c 6c65 6374 6564  assert_collected
+00018580: 5f73 6f75 7263 6573 280a 2020 2020 2020  _sources(.      
+00018590: 2020 2020 2020 7372 632c 0a20 2020 2020        src,.     
+000185a0: 2020 2020 2020 2065 7870 6563 7465 642c         expected,
+000185b0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+000185c0: 6c75 6465 3d72 222f 6578 636c 7564 652f  lude=r"/exclude/
+000185d0: 7c61 5c2e 7079 222c 0a20 2020 2020 2020  |a\.py",.       
+000185e0: 2020 2020 2073 7464 696e 5f66 696c 656e       stdin_filen
+000185f0: 616d 653d 7374 6469 6e5f 6669 6c65 6e61  ame=stdin_filena
+00018600: 6d65 2c0a 2020 2020 2020 2020 290a 0a20  me,.        ).. 
+00018610: 2020 2040 7061 7463 6828 2263 6572 6369     @patch("cerci
+00018620: 732e 6669 6e64 5f70 726f 6a65 6374 5f72  s.find_project_r
+00018630: 6f6f 7422 2c20 6c61 6d62 6461 202a 6172  oot", lambda *ar
+00018640: 6773 3a20 2854 4849 535f 4449 522e 7265  gs: (THIS_DIR.re
+00018650: 736f 6c76 6528 292c 204e 6f6e 6529 290a  solve(), None)).
+00018660: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
+00018670: 5f73 6f75 7263 6573 5f77 6974 685f 7374  _sources_with_st
+00018680: 6469 6e5f 6669 6c65 6e61 6d65 5f61 6e64  din_filename_and
+00018690: 5f65 7874 656e 645f 6578 636c 7564 6528  _extend_exclude(
+000186a0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000186b0: 2020 2020 2020 2023 2045 7874 656e 6420         # Extend 
+000186c0: 6578 636c 7564 6520 7368 6f75 6c64 6e27  exclude shouldn'
+000186d0: 7420 6578 636c 7564 6520 7374 6469 6e5f  t exclude stdin_
+000186e0: 6669 6c65 6e61 6d65 2073 696e 6365 2069  filename since i
+000186f0: 7420 6973 206d 696d 6963 6b69 6e67 2074  t is mimicking t
+00018700: 6865 0a20 2020 2020 2020 2023 2066 696c  he.        # fil
+00018710: 6520 6265 696e 6720 7061 7373 6564 2064  e being passed d
+00018720: 6972 6563 746c 792e 2054 6869 7320 6973  irectly. This is
+00018730: 2074 6865 2073 616d 6520 6173 0a20 2020   the same as.   
+00018740: 2020 2020 2023 2074 6573 745f 6578 636c       # test_excl
+00018750: 7564 655f 666f 725f 6973 7375 655f 3135  ude_for_issue_15
+00018760: 3732 0a20 2020 2020 2020 2073 7263 203d  72.        src =
+00018770: 205b 222d 225d 0a20 2020 2020 2020 2070   ["-"].        p
+00018780: 6174 6820 3d20 5448 4953 5f44 4952 202f  ath = THIS_DIR /
+00018790: 2022 6461 7461 2220 2f20 2269 6e63 6c75   "data" / "inclu
+000187a0: 6465 5f65 7863 6c75 6465 5f74 6573 7473  de_exclude_tests
+000187b0: 220a 2020 2020 2020 2020 7374 6469 6e5f  ".        stdin_
+000187c0: 6669 6c65 6e61 6d65 203d 2073 7472 2870  filename = str(p
+000187d0: 6174 6820 2f20 2262 2f65 7863 6c75 6465  ath / "b/exclude
+000187e0: 2f61 2e70 7922 290a 2020 2020 2020 2020  /a.py").        
+000187f0: 6578 7065 6374 6564 203d 205b 6622 5f5f  expected = [f"__
+00018800: 424c 4143 4b5f 5354 4449 4e5f 4649 4c45  BLACK_STDIN_FILE
+00018810: 4e41 4d45 5f5f 7b73 7464 696e 5f66 696c  NAME__{stdin_fil
+00018820: 656e 616d 657d 225d 0a20 2020 2020 2020  ename}"].       
+00018830: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
+00018840: 645f 736f 7572 6365 7328 0a20 2020 2020  d_sources(.     
+00018850: 2020 2020 2020 2073 7263 2c0a 2020 2020         src,.    
+00018860: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+00018870: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
+00018880: 7465 6e64 5f65 7863 6c75 6465 3d72 222f  tend_exclude=r"/
+00018890: 6578 636c 7564 652f 7c61 5c2e 7079 222c  exclude/|a\.py",
+000188a0: 0a20 2020 2020 2020 2020 2020 2073 7464  .            std
+000188b0: 696e 5f66 696c 656e 616d 653d 7374 6469  in_filename=stdi
+000188c0: 6e5f 6669 6c65 6e61 6d65 2c0a 2020 2020  n_filename,.    
+000188d0: 2020 2020 290a 0a20 2020 2040 7061 7463      )..    @patc
+000188e0: 6828 2263 6572 6369 732e 6669 6e64 5f70  h("cercis.find_p
+000188f0: 726f 6a65 6374 5f72 6f6f 7422 2c20 6c61  roject_root", la
+00018900: 6d62 6461 202a 6172 6773 3a20 2854 4849  mbda *args: (THI
+00018910: 535f 4449 522e 7265 736f 6c76 6528 292c  S_DIR.resolve(),
+00018920: 204e 6f6e 6529 290a 2020 2020 6465 6620   None)).    def 
+00018930: 7465 7374 5f67 6574 5f73 6f75 7263 6573  test_get_sources
+00018940: 5f77 6974 685f 7374 6469 6e5f 6669 6c65  _with_stdin_file
+00018950: 6e61 6d65 5f61 6e64 5f66 6f72 6365 5f65  name_and_force_e
+00018960: 7863 6c75 6465 2873 656c 6629 202d 3e20  xclude(self) -> 
+00018970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2320  None:.        # 
+00018980: 466f 7263 6520 6578 636c 7564 6520 7368  Force exclude sh
+00018990: 6f75 6c64 2065 7863 6c75 6465 2074 6865  ould exclude the
+000189a0: 2066 696c 6520 7768 656e 2070 6173 7369   file when passi
+000189b0: 6e67 2069 7420 7468 726f 7567 680a 2020  ng it through.  
+000189c0: 2020 2020 2020 2320 7374 6469 6e5f 6669        # stdin_fi
+000189d0: 6c65 6e61 6d65 0a20 2020 2020 2020 2070  lename.        p
+000189e0: 6174 6820 3d20 5448 4953 5f44 4952 202f  ath = THIS_DIR /
+000189f0: 2022 6461 7461 2220 2f20 2269 6e63 6c75   "data" / "inclu
+00018a00: 6465 5f65 7863 6c75 6465 5f74 6573 7473  de_exclude_tests
+00018a10: 220a 2020 2020 2020 2020 7374 6469 6e5f  ".        stdin_
+00018a20: 6669 6c65 6e61 6d65 203d 2073 7472 2870  filename = str(p
+00018a30: 6174 6820 2f20 2262 2f65 7863 6c75 6465  ath / "b/exclude
+00018a40: 2f61 2e70 7922 290a 2020 2020 2020 2020  /a.py").        
+00018a50: 6173 7365 7274 5f63 6f6c 6c65 6374 6564  assert_collected
+00018a60: 5f73 6f75 7263 6573 280a 2020 2020 2020  _sources(.      
+00018a70: 2020 2020 2020 7372 633d 5b22 2d22 5d2c        src=["-"],
+00018a80: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+00018a90: 6563 7465 643d 5b5d 2c0a 2020 2020 2020  ected=[],.      
+00018aa0: 2020 2020 2020 666f 7263 655f 6578 636c        force_excl
+00018ab0: 7564 653d 7222 2f65 7863 6c75 6465 2f7c  ude=r"/exclude/|
+00018ac0: 615c 2e70 7922 2c0a 2020 2020 2020 2020  a\.py",.        
+00018ad0: 2020 2020 7374 6469 6e5f 6669 6c65 6e61      stdin_filena
+00018ae0: 6d65 3d73 7464 696e 5f66 696c 656e 616d  me=stdin_filenam
+00018af0: 652c 0a20 2020 2020 2020 2029 0a0a 0a74  e,.        )...t
+00018b00: 7279 3a0a 2020 2020 7769 7468 206f 7065  ry:.    with ope
+00018b10: 6e28 6365 7263 6973 2e5f 5f66 696c 655f  n(cercis.__file_
+00018b20: 5f2c 2022 7222 2c20 656e 636f 6469 6e67  _, "r", encoding
+00018b30: 3d22 7574 662d 3822 2920 6173 205f 6266  ="utf-8") as _bf
+00018b40: 3a0a 2020 2020 2020 2020 626c 6163 6b5f  :.        black_
+00018b50: 736f 7572 6365 5f6c 696e 6573 203d 205f  source_lines = _
+00018b60: 6266 2e72 6561 646c 696e 6573 2829 0a65  bf.readlines().e
+00018b70: 7863 6570 7420 556e 6963 6f64 6544 6563  xcept UnicodeDec
+00018b80: 6f64 6545 7272 6f72 3a0a 2020 2020 6966  odeError:.    if
+00018b90: 206e 6f74 2063 6572 6369 732e 434f 4d50   not cercis.COMP
+00018ba0: 494c 4544 3a0a 2020 2020 2020 2020 7261  ILED:.        ra
+00018bb0: 6973 650a 0a0a 6465 6620 7472 6163 6566  ise...def tracef
+00018bc0: 756e 6328 0a20 2020 2020 2020 2066 7261  unc(.        fra
+00018bd0: 6d65 3a20 7479 7065 732e 4672 616d 6554  me: types.FrameT
+00018be0: 7970 652c 2065 7665 6e74 3a20 7374 722c  ype, event: str,
+00018bf0: 2061 7267 3a20 416e 790a 2920 2d3e 2043   arg: Any.) -> C
+00018c00: 616c 6c61 626c 655b 5b74 7970 6573 2e46  allable[[types.F
+00018c10: 7261 6d65 5479 7065 2c20 7374 722c 2041  rameType, str, A
+00018c20: 6e79 5d2c 2041 6e79 5d3a 0a20 2020 2022  ny], Any]:.    "
+00018c30: 2222 5368 6f77 2066 756e 6374 696f 6e20  ""Show function 
+00018c40: 6361 6c6c 7320 6066 726f 6d20 6365 7263  calls `from cerc
+00018c50: 6973 2f5f 5f69 6e69 745f 5f2e 7079 6020  is/__init__.py` 
+00018c60: 6173 2074 6865 7920 6861 7070 656e 2e0a  as they happen..
+00018c70: 0a20 2020 2052 6567 6973 7465 7220 7468  .    Register th
+00018c80: 6973 2077 6974 6820 6073 7973 2e73 6574  is with `sys.set
+00018c90: 7472 6163 6528 2960 2069 6e20 6120 7465  trace()` in a te
+00018ca0: 7374 2079 6f75 2772 6520 6465 6275 6767  st you're debugg
+00018cb0: 696e 672e 0a20 2020 2022 2222 0a20 2020  ing..    """.   
+00018cc0: 2069 6620 6576 656e 7420 213d 2022 6361   if event != "ca
+00018cd0: 6c6c 223a 0a20 2020 2020 2020 2072 6574  ll":.        ret
+00018ce0: 7572 6e20 7472 6163 6566 756e 630a 0a20  urn tracefunc.. 
+00018cf0: 2020 2073 7461 636b 203d 206c 656e 2869     stack = len(i
+00018d00: 6e73 7065 6374 2e73 7461 636b 2829 2920  nspect.stack()) 
+00018d10: 2d20 3139 0a20 2020 2073 7461 636b 202a  - 19.    stack *
+00018d20: 3d20 320a 2020 2020 6669 6c65 6e61 6d65  = 2.    filename
+00018d30: 203d 2066 7261 6d65 2e66 5f63 6f64 652e   = frame.f_code.
+00018d40: 636f 5f66 696c 656e 616d 650a 2020 2020  co_filename.    
+00018d50: 6c69 6e65 6e6f 203d 2066 7261 6d65 2e66  lineno = frame.f
+00018d60: 5f6c 696e 656e 6f0a 2020 2020 6675 6e63  _lineno.    func
+00018d70: 5f73 6967 5f6c 696e 656e 6f20 3d20 6c69  _sig_lineno = li
+00018d80: 6e65 6e6f 202d 2031 0a20 2020 2066 756e  neno - 1.    fun
+00018d90: 636e 616d 6520 3d20 626c 6163 6b5f 736f  cname = black_so
+00018da0: 7572 6365 5f6c 696e 6573 5b66 756e 635f  urce_lines[func_
+00018db0: 7369 675f 6c69 6e65 6e6f 5d2e 7374 7269  sig_lineno].stri
+00018dc0: 7028 290a 2020 2020 7768 696c 6520 6675  p().    while fu
+00018dd0: 6e63 6e61 6d65 2e73 7461 7274 7377 6974  ncname.startswit
+00018de0: 6828 2240 2229 3a0a 2020 2020 2020 2020  h("@"):.        
+00018df0: 6675 6e63 5f73 6967 5f6c 696e 656e 6f20  func_sig_lineno 
+00018e00: 2b3d 2031 0a20 2020 2020 2020 2066 756e  += 1.        fun
+00018e10: 636e 616d 6520 3d20 626c 6163 6b5f 736f  cname = black_so
+00018e20: 7572 6365 5f6c 696e 6573 5b66 756e 635f  urce_lines[func_
+00018e30: 7369 675f 6c69 6e65 6e6f 5d2e 7374 7269  sig_lineno].stri
+00018e40: 7028 290a 2020 2020 6966 2022 6365 7263  p().    if "cerc
+00018e50: 6973 2f5f 5f69 6e69 745f 5f2e 7079 2220  is/__init__.py" 
+00018e60: 696e 2066 696c 656e 616d 653a 0a20 2020  in filename:.   
+00018e70: 2020 2020 2070 7269 6e74 2866 227b 2720       print(f"{' 
+00018e80: 2720 2a20 7374 6163 6b7d 7b6c 696e 656e  ' * stack}{linen
+00018e90: 6f7d 3a7b 6675 6e63 6e61 6d65 7d22 290a  o}:{funcname}").
+00018ea0: 2020 2020 7265 7475 726e 2074 7261 6365      return trace
+00018eb0: 6675 6e63 0a                             func.
```

### Comparing `cercis-0.1.6/tests/test_blackd.py` & `cercis-0.1.7/tests/test_blackd.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         )
         self.assertEqual(response.status, 200)
         self.assertEqual(await response.text(), expected)
 
     @unittest_run_loop
     async def test_blackd_diff(self) -> None:
         diff_header = re.compile(
-            r"(In|Out)\t\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d\.\d\d\d\d\d\d \+\d\d\d\d"
+            r"(In|Out)\t\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d\.\d\d\d\d\d\d\+\d\d:\d\d"
         )
 
         source, _ = read_data("miscellaneous", "blackd_diff")
         expected, _ = read_data("miscellaneous", "blackd_diff.diff")
 
         response = await self.client.post(
             "/", data=source, headers={blackd.DIFF_HEADER: "true"}
```

### Comparing `cercis-0.1.6/tests/test_format.py` & `cercis-0.1.7/tests/test_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,23 @@
 def test_python_311(filename: str) -> None:
     source, expected = read_data("py_311", filename)
     mode = cercis.Mode(target_versions={cercis.TargetVersion.PY311})
     _override_single_quote_for_cleaner_future_rebase(mode)
     assert_format(source, expected, mode, minimum_version=(3, 11))
 
 
+@pytest.mark.parametrize("filename", all_data_cases("py_312"))
+def test_python_312(filename: str) -> None:
+    source, expected = read_data("py_312", filename)
+    mode = cercis.Mode(target_versions={cercis.TargetVersion.PY312})
+    _override_single_quote_for_cleaner_future_rebase(mode)
+    mode.function_definition_extra_indent = False
+    assert_format(source, expected, mode, minimum_version=(3, 12))
+
+
 @pytest.mark.parametrize("filename", all_data_cases("fast"))
 def test_fast_cases(filename: str) -> None:
     source, expected = read_data("fast", filename)
     assert_format(source, expected, fast=True)
 
 
 def test_python_2_hint() -> None:
```

### Comparing `cercis-0.1.6/tests/test_ipynb.py` & `cercis-0.1.7/tests/test_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/test_no_ipynb.py` & `cercis-0.1.7/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/test_trans.py` & `cercis-0.1.7/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/test_utils_line_wrapping.py` & `cercis-0.1.7/tests/test_utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/util.py` & `cercis-0.1.7/tests/util.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/conditional_expression.py` & `cercis-0.1.7/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py` & `cercis-0.1.7/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py` & `cercis-0.1.7/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py` & `cercis-0.1.7/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py` & `cercis-0.1.7/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py` & `cercis-0.1.7/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py` & `cercis-0.1.7/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py` & `cercis-0.1.7/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/edge_cases.py` & `cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/edge_cases.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py` & `cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py` & `cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py` & `cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py` & `cercis-0.1.7/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py` & `cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py` & `cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py` & `cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py` & `cercis-0.1.7/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Black_default.py` & `cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Black_default_2.py` & `cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Black_default_2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Cercis_default.py` & `cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py` & `cercis-0.1.7/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring.py` & `cercis-0.1.7/tests/data/configurable_cases/single_quote/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring_preview.py` & `cercis-0.1.7/tests/data/configurable_cases/single_quote/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/single_quote/more_quotes.py` & `cercis-0.1.7/tests/data/configurable_cases/single_quote/more_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/single_quote/string_prefixes.py` & `cercis-0.1.7/tests/data/configurable_cases/single_quote/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/configurable_cases/single_quote/torture.py` & `cercis-0.1.7/tests/data/configurable_cases/single_quote/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `cercis-0.1.7/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/jupyter/notebook_trailing_newline.ipynb` & `cercis-0.1.7/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/jupyter/notebook_without_changes.ipynb` & `cercis-0.1.7/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/debug_visitor.out` & `cercis-0.1.7/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/debug_visitor.py` & `cercis-0.1.7/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/decorators.py` & `cercis-0.1.7/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/docstring_no_string_normalization.py` & `cercis-0.1.7/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `cercis-0.1.7/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/force_py36.py` & `cercis-0.1.7/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/force_pyi.py` & `cercis-0.1.7/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/long_strings_flag_disabled.py` & `cercis-0.1.7/tests/data/miscellaneous/long_strings_flag_disabled.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/python2_detection.py` & `cercis-0.1.7/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/string_quotes.py` & `cercis-0.1.7/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/miscellaneous/stub.pyi` & `cercis-0.1.7/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/cantfit.py` & `cercis-0.1.7/tests/data/preview/cantfit.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/comments7.py` & `cercis-0.1.7/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/format_unicode_escape_seq.py` & `cercis-0.1.7/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/long_dict_values.py` & `cercis-0.1.7/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/long_strings.py` & `cercis-0.1.7/tests/data/preview/long_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/long_strings__east_asian_width.py` & `cercis-0.1.7/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/long_strings__edge_case.py` & `cercis-0.1.7/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/long_strings__regression.py` & `cercis-0.1.7/tests/data/preview/long_strings__regression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/long_strings__type_annotations.py` & `cercis-0.1.7/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/multiline_strings.py` & `cercis-0.1.7/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/no_blank_line_before_docstring.py` & `cercis-0.1.7/tests/data/preview/no_blank_line_before_docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/prefer_rhs_split.py` & `cercis-0.1.7/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview/trailing_comma.py` & `cercis-0.1.7/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview_context_managers/targeting_py38.py` & `cercis-0.1.7/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview_context_managers/targeting_py39.py` & `cercis-0.1.7/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `cercis-0.1.7/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_310/parenthesized_context_managers.py` & `cercis-0.1.7/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_310/pattern_matching_complex.py` & `cercis-0.1.7/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_310/pattern_matching_extras.py` & `cercis-0.1.7/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_310/pattern_matching_generic.py` & `cercis-0.1.7/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_310/pattern_matching_simple.py` & `cercis-0.1.7/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_310/pattern_matching_style.py` & `cercis-0.1.7/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_311/pep_646.py` & `cercis-0.1.7/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_311/pep_654.py` & `cercis-0.1.7/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_311/pep_654_style.py` & `cercis-0.1.7/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_36/numeric_literals.py` & `cercis-0.1.7/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_37/python37.py` & `cercis-0.1.7/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_38/pep_570.py` & `cercis-0.1.7/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_38/pep_572.py` & `cercis-0.1.7/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_38/pep_572_remove_parens.py` & `cercis-0.1.7/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_38/python38.py` & `cercis-0.1.7/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_39/python39.py` & `cercis-0.1.7/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/py_39/remove_with_brackets.py` & `cercis-0.1.7/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/attribute_access_on_number_literals.py` & `cercis-0.1.7/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/class_blank_parentheses.py` & `cercis-0.1.7/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/class_methods_new_line.py` & `cercis-0.1.7/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/collections.py` & `cercis-0.1.7/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments.py` & `cercis-0.1.7/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments2.py` & `cercis-0.1.7/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments3.py` & `cercis-0.1.7/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments4.py` & `cercis-0.1.7/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments5.py` & `cercis-0.1.7/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments6.py` & `cercis-0.1.7/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments9.py` & `cercis-0.1.7/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/comments_non_breaking_space.py` & `cercis-0.1.7/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/composition.py` & `cercis-0.1.7/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/composition_no_trailing_comma.py` & `cercis-0.1.7/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/docstring.py` & `cercis-0.1.7/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/docstring_preview.py` & `cercis-0.1.7/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/empty_lines.py` & `cercis-0.1.7/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/expression.diff` & `cercis-0.1.7/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/expression.py` & `cercis-0.1.7/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/fmtonoff.py` & `cercis-0.1.7/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/fmtonoff2.py` & `cercis-0.1.7/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/fmtonoff5.py` & `cercis-0.1.7/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/fmtskip2.py` & `cercis-0.1.7/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/fmtskip8.py` & `cercis-0.1.7/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/fstring.py` & `cercis-0.1.7/tests/data/simple_cases/fstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/function.py` & `cercis-0.1.7/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/function2.py` & `cercis-0.1.7/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/function_trailing_comma.py` & `cercis-0.1.7/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/import_spacing.py` & `cercis-0.1.7/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/one_element_subscript.py` & `cercis-0.1.7/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/power_op_spacing.py` & `cercis-0.1.7/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `cercis-0.1.7/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/remove_await_parens.py` & `cercis-0.1.7/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/remove_except_parens.py` & `cercis-0.1.7/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/remove_for_brackets.py` & `cercis-0.1.7/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `cercis-0.1.7/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/remove_parens.py` & `cercis-0.1.7/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/return_annotation_brackets.py` & `cercis-0.1.7/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/skip_magic_trailing_comma.py` & `cercis-0.1.7/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/slices.py` & `cercis-0.1.7/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/string_prefixes.py` & `cercis-0.1.7/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/torture.py` & `cercis-0.1.7/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `cercis-0.1.7/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `cercis-0.1.7/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `cercis-0.1.7/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/LICENSE` & `cercis-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/LICENSE_ORIGINAL` & `cercis-0.1.7/LICENSE_ORIGINAL`

 * *Files identical despite different names*

### Comparing `cercis-0.1.6/pyproject.toml` & `cercis-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cercis"
-version = "0.1.6"
+version = "0.1.7"
 description = "A more configurable Python code formatter"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 authors = [
   { name = "Łukasz Langa", email = "lukasz@langa.pl" },
   { name = "jsh9", email = "" },
 ]
@@ -216,8 +216,10 @@
     '''ignore:Middleware decorator is deprecated since 4\.0 and its behaviour is default, you can simply remove this decorator:DeprecationWarning''',
     # this is mitigated by https://github.com/python/cpython/issues/79071 in python 3.8+
     # this ignore can be removed when support for 3.7 is dropped.
     '''ignore:Bare functions are deprecated, use async ones:DeprecationWarning''',
     # aiohttp is using deprecated cgi modules - Safe to remove when fixed:
     # https://github.com/aio-libs/aiohttp/issues/6905
     '''ignore:'cgi' is deprecated and slated for removal in Python 3.13:DeprecationWarning''',
+    # Work around https://github.com/pytest-dev/pytest/issues/10977 for Python 3.12
+    '''ignore:(Attribute s|Attribute n|ast.Str|ast.Bytes|ast.NameConstant|ast.Num) is deprecated and will be removed in Python 3.14:DeprecationWarning'''
 ]
```

### Comparing `cercis-0.1.6/PKG-INFO` & `cercis-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cercis
-Version: 0.1.6
+Version: 0.1.7
 Summary: A more configurable Python code formatter
 Project-URL: Changelog, https://github.com/jsh9/cercis/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/jsh9/cercis
 Author: jsh9
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 License-File: LICENSE
@@ -755,14 +755,20 @@
 wrap-line-with-long-string = true
 collapse-nested-brackets = false
 wrap-comments = true
 wrap-pragma-comments = true
 ```
 # Change Log
 
+## [0.1.7] - 2023-06-19
+
+- Changed
+  - Pulled in the latest changes from psf/black (code diff:
+    https://github.com/jsh9/cercis/pull/27)
+
 ## [0.1.6] - 2023-05-23
 
 - Added
   - A new option `--wrap-comments` to not wrap any comments (not just pragma comments)
   - A new option `--keep-blank-lines-in-brackets`
 - Changed
   - Improved the CLI output text colors because the current colors are confusing or not
```


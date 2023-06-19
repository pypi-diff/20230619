# Comparing `tmp/jupyter_releaser-1.1.5.tar.gz` & `tmp/jupyter_releaser-1.1.6.tar.gz`

## Comparing `jupyter_releaser-1.1.5.tar` & `jupyter_releaser-1.1.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0   123302 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/RELEASE.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/codecov.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/readthedocs.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/dependabot.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/actions/check-release/action.yml
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/actions/finalize-release/action.yml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/actions/install-releaser/action.yml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/actions/populate-release/action.yml
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/actions/prep-release/action.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/scripts/bump_tag.sh
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/workflows/generate-changelog.yml
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/make.bat
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/conf.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/index.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/_static/custom.css
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/_static/images/logo/favicon.svg
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/_static/images/logo/logo.svg
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/background/index.rst
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/background/theory.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/get_started/generate_changelog.md
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/get_started/index.rst
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/get_started/making_release_from_releaser.md
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/get_started/making_release_from_repo.md
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/how_to_guides/convert_repo_from_releaser.md
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/how_to_guides/convert_repo_from_repo.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/how_to_guides/index.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/how_to_guides/maintain_fork.md
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/how_to_guides/write_config.md
--rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/draft_github_release.png
--rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/final_github_release.png
--rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/fork_fetch.png
--rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/generate_changelog.png
--rw-r--r--   0        0        0    99291 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/prep_release.png
--rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/prep_release_next_step.png
--rw-r--r--   0        0        0   237681 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/prep_release_repo.png
--rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/publish_release.png
--rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/publish_release_next_step.png
--rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/images/publish_release_repo.png
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/reference/api_docs.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/reference/configuration.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/reference/faq.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/reference/index.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/docs/source/reference/releaser_cli.rst
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/example-workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/example-workflows/publish-release.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/__main__.py
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/changelog.py
--rw-r--r--   0        0        0    19360 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/cli.py
--rw-r--r--   0        0        0    18823 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/lib.py
--rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/mock_github.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/npm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/py.typed
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/python.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/schema.json
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/tee.py
--rw-r--r--   0        0        0    24289 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/actions/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/actions/common.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/actions/finalize_release.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/actions/generate_changelog.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/actions/populate_release.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/actions/prep_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/tests/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/tests/conftest.py
--rw-r--r--   0        0        0    26425 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/tests/test_cli.py
--rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/tests/test_functions.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/tests/test_mock_github.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/jupyter_releaser/tests/util.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/.gitignore
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/LICENSE
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/README.md
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.readthedocs.yml
+-rw-r--r--   0        0        0   125164 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/RELEASE.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/check-release/action.yml
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/finalize-release/action.yml
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/install-releaser/action.yml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/populate-release/action.yml
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/prep-release/action.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/scripts/bump_tag.sh
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/generate-changelog.yml
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/make.bat
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/conf.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/index.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/_static/custom.css
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/_static/images/logo/favicon.svg
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/_static/images/logo/logo.svg
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/background/index.rst
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/background/theory.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/generate_changelog.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/index.rst
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_releaser.md
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_repo.md
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_releaser.md
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_repo.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/index.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/maintain_fork.md
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/write_config.md
+-rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/draft_github_release.png
+-rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/final_github_release.png
+-rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/fork_fetch.png
+-rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/generate_changelog.png
+-rw-r--r--   0        0        0    99291 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/prep_release.png
+-rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/prep_release_next_step.png
+-rw-r--r--   0        0        0   237681 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/prep_release_repo.png
+-rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/publish_release.png
+-rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/publish_release_next_step.png
+-rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/publish_release_repo.png
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/api_docs.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/configuration.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/faq.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/index.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/releaser_cli.rst
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/example-workflows/full-release.yml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/example-workflows/prep-release.yml
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/example-workflows/publish-release.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/__main__.py
+-rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/changelog.py
+-rw-r--r--   0        0        0    19367 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/cli.py
+-rw-r--r--   0        0        0    18954 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/lib.py
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/mock_github.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/npm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/py.typed
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/python.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/schema.json
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tee.py
+-rw-r--r--   0        0        0    24466 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/common.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/finalize_release.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/generate_changelog.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/populate_release.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/prep_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/conftest.py
+-rw-r--r--   0        0        0    26407 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/test_cli.py
+-rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/test_functions.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/test_mock_github.py
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/util.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.gitignore
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/LICENSE
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/README.md
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/PKG-INFO
```

### Comparing `jupyter_releaser-1.1.5/.pre-commit-config.yaml` & `jupyter_releaser-1.1.6/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,28 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.19.2
+    rev: 0.23.1
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
         additional_dependencies:
           [mdformat-gfm, mdformat-frontmatter, mdformat-footnote]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.206
+    rev: v0.0.270
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyter_releaser-1.1.5/CHANGELOG.md` & `jupyter_releaser-1.1.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.1.6
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...0b4c9cc2b257e799794c6d02735b659da09e2336))
+
+### Maintenance and upkeep improvements
+
+- Pin ghapi [#512](https://github.com/jupyter-server/jupyter_releaser/pull/512) ([@blink1073](https://github.com/blink1073))
+- Use local coverage [#503](https://github.com/jupyter-server/jupyter_releaser/pull/503) ([@blink1073](https://github.com/blink1073))
+- Remove `target` from the example releaser workflows [#500](https://github.com/jupyter-server/jupyter_releaser/pull/500) ([@jtpio](https://github.com/jtpio))
+- Update ruff and address typing error [#498](https://github.com/jupyter-server/jupyter_releaser/pull/498) ([@blink1073](https://github.com/blink1073))
+- Add more linting [#492](https://github.com/jupyter-server/jupyter_releaser/pull/492) ([@blink1073](https://github.com/blink1073))
+
+### Documentation improvements
+
+- Add a Full Release workflow to the example workflows [#501](https://github.com/jupyter-server/jupyter_releaser/pull/501) ([@jtpio](https://github.com/jtpio))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2023-01-26&to=2023-06-19&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ablink1073+updated%3A2023-01-26..2023-06-19&type=Issues) | [@codecov](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Acodecov+updated%3A2023-01-26..2023-06-19&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ajtpio+updated%3A2023-01-26..2023-06-19&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Apre-commit-ci+updated%3A2023-01-26..2023-06-19&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.1.5
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...2acb616f67cf9edc926bf5d877a434f59dbb0ee6))
 
 ### Enhancements made
 
 - Add whitelist for http request in yarn [#491](https://github.com/jupyter-server/jupyter_releaser/pull/491) ([@brichet](https://github.com/brichet))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2023-01-09&to=2023-01-26&type=c))
 
 [@brichet](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Abrichet+updated%3A2023-01-09..2023-01-26&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.1.4
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...e9d498b2398a2880e06d45f4119a1d537fe48402))
 
 ### Bugs fixed
 
 - Pass the authentication to `format_pr_entry` [#489](https://github.com/jupyter-server/jupyter_releaser/pull/489) ([@fcollonval](https://github.com/fcollonval))
```

### Comparing `jupyter_releaser-1.1.5/CONTRIBUTING.md` & `jupyter_releaser-1.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/actions/check-release/action.yml` & `jupyter_releaser-1.1.6/.github/actions/check-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/actions/finalize-release/action.yml` & `jupyter_releaser-1.1.6/.github/actions/finalize-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/actions/populate-release/action.yml` & `jupyter_releaser-1.1.6/.github/actions/populate-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/actions/prep-release/action.yml` & `jupyter_releaser-1.1.6/.github/actions/prep-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/workflows/check-release.yml` & `jupyter_releaser-1.1.6/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/workflows/generate-changelog.yml` & `jupyter_releaser-1.1.6/.github/workflows/generate-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/workflows/prep-release.yml` & `jupyter_releaser-1.1.6/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/workflows/publish-release.yml` & `jupyter_releaser-1.1.6/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/.github/workflows/test.yml` & `jupyter_releaser-1.1.6/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,23 @@
         run: |
           hatch run cov:test -n auto --cov-fail-under 80 || hatch run test:test --lf
 
       - name: Run the tests on Windows and MacOS
         if: ${{ matrix.os != 'ubuntu-latest' }}
         run: hatch run cov:test -s -n auto || hatch run cov:test -s --lf
 
-      - name: Codecov
-        run: |
-          pip install codecov coverage[toml]
-          codecov
+      - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
+
+  coverage:
+    runs-on: ubuntu-latest
+    needs:
+      - test
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
 
   generate_changelog:
     runs-on: ubuntu-20.04
     timeout-minutes: 10
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
@@ -147,15 +152,15 @@
           release_url: ${{ steps.populate-release.outputs.release_url }}
           dry_run: true
 
   check: # This job does nothing and is only used for the branch protection
     if: always()
     needs:
       - check_links
-      - test
+      - coverage
       - docs
       - lint
       - check_local_actions
       - test_minimum_versions
       - test_prereleases
       - generate_changelog
     runs-on: ubuntu-latest
```

### Comparing `jupyter_releaser-1.1.5/docs/Makefile` & `jupyter_releaser-1.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/make.bat` & `jupyter_releaser-1.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/conf.py` & `jupyter_releaser-1.1.6/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import shutil
 
 HERE = osp.abspath(osp.dirname(__file__))
 
 # -- Project information -----------------------------------------------------
 
 project = "Jupyter Releaser"
-copyright = "2021, Project Jupyter"
+copyright = "2021, Project Jupyter"  # noqa
 author = "Project Jupyter"
 
 # The full version, including alpha/beta/rc tags.
 release = importlib.metadata.version("jupyter_releaser")
 # The short X.Y version.
 version = ".".join(release.split(".")[:2])
```

### Comparing `jupyter_releaser-1.1.5/docs/source/_static/images/logo/favicon.svg` & `jupyter_releaser-1.1.6/docs/source/_static/images/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/_static/images/logo/logo.svg` & `jupyter_releaser-1.1.6/docs/source/_static/images/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/background/theory.md` & `jupyter_releaser-1.1.6/docs/source/background/theory.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/get_started/generate_changelog.md` & `jupyter_releaser-1.1.6/docs/source/get_started/generate_changelog.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/get_started/making_release_from_releaser.md` & `jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/get_started/making_release_from_repo.md` & `jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_repo.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/how_to_guides/convert_repo_from_releaser.md` & `jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/how_to_guides/convert_repo_from_repo.md` & `jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_repo.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/how_to_guides/write_config.md` & `jupyter_releaser-1.1.6/docs/source/how_to_guides/write_config.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/draft_github_release.png` & `jupyter_releaser-1.1.6/docs/source/images/draft_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/final_github_release.png` & `jupyter_releaser-1.1.6/docs/source/images/final_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/fork_fetch.png` & `jupyter_releaser-1.1.6/docs/source/images/fork_fetch.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/generate_changelog.png` & `jupyter_releaser-1.1.6/docs/source/images/generate_changelog.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/prep_release.png` & `jupyter_releaser-1.1.6/docs/source/images/prep_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/prep_release_next_step.png` & `jupyter_releaser-1.1.6/docs/source/images/prep_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/prep_release_repo.png` & `jupyter_releaser-1.1.6/docs/source/images/prep_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/publish_release.png` & `jupyter_releaser-1.1.6/docs/source/images/publish_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/publish_release_next_step.png` & `jupyter_releaser-1.1.6/docs/source/images/publish_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/images/publish_release_repo.png` & `jupyter_releaser-1.1.6/docs/source/images/publish_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/reference/api_docs.rst` & `jupyter_releaser-1.1.6/docs/source/reference/api_docs.rst`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/docs/source/reference/faq.md` & `jupyter_releaser-1.1.6/docs/source/reference/faq.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/example-workflows/prep-release.yml` & `jupyter_releaser-1.1.6/example-workflows/prep-release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
       - name: Prep Release
         id: prep-release
         uses: jupyter-server/jupyter_releaser/.github/actions/prep-release@v2
         with:
           token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
           version_spec: ${{ github.event.inputs.version_spec }}
           post_version_spec: ${{ github.event.inputs.post_version_spec }}
-          target: ${{ github.event.inputs.target }}
           branch: ${{ github.event.inputs.branch }}
           since: ${{ github.event.inputs.since }}
           since_last_stable: ${{ github.event.inputs.since_last_stable }}
 
       - name: "** Next Step **"
         run: |
           echo "Optional): Review Draft Release: ${{ steps.prep-release.outputs.release_url }}"
```

### Comparing `jupyter_releaser-1.1.5/example-workflows/publish-release.yml` & `jupyter_releaser-1.1.6/example-workflows/publish-release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,28 @@
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
       - name: Populate Release
         id: populate-release
         uses: jupyter-server/jupyter_releaser/.github/actions/populate-release@v2
         with:
           token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
-          target: ${{ github.event.inputs.target }}
           branch: ${{ github.event.inputs.branch }}
           release_url: ${{ github.event.inputs.release_url }}
           steps_to_skip: ${{ github.event.inputs.steps_to_skip }}
 
       - name: Finalize Release
         id: finalize-release
         env:
           PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
           PYPI_TOKEN_MAP: ${{ secrets.PYPI_TOKEN_MAP }}
           TWINE_USERNAME: __token__
           NPM_TOKEN: ${{ secrets.NPM_TOKEN }}
         uses: jupyter-server/jupyter-releaser/.github/actions/finalize-release@v2
         with:
           token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
-          target: ${{ github.event.inputs.target }}
           release_url: ${{ steps.populate-release.outputs.release_url }}
 
       - name: "** Next Step **"
         if: ${{ success() }}
         run: |
           echo "Verify the final release"
           echo ${{ steps.finalize-release.outputs.release_url }}
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/changelog.py` & `jupyter_releaser-1.1.6/jupyter_releaser/changelog.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,23 +85,20 @@
     -------
     str
         A formatted changelog entry with markers
     """
     branch = branch or util.get_branch()
     since = since or util.get_latest_tag(ref or branch, since_last_stable)
 
-    if since == "":
+    if since == "":  # noqa
         since = util.get_first_commit(ref or branch)
 
     util.log(f"Getting changes to {repo} since {since} on branch {branch}...")
 
-    if until:
-        until = until.replace("%", "")
-    else:
-        until = None
+    until = until.replace("%", "") if until else None
 
     md = generate_activity_md(
         repo,
         since=since,
         until=until,
         kind="pr",
         heading_level=2,
@@ -111,22 +108,19 @@
 
     if not md:
         util.log("No PRs found")
         return f"## {version}\n\nNo merged PRs"
 
     entry = md.replace("[full changelog]", "[Full Changelog]")
 
-    if until:
-        entry = entry.replace("...None", f"...{until}")
-    else:
-        entry = entry.replace("...None", "")
+    entry = entry.replace("...None", f"...{until}") if until else entry.replace("...None", "")
 
     entry = entry.splitlines()[2:]
 
-    for (ind, line) in enumerate(entry):
+    for ind, line in enumerate(entry):
         # Look for a backport, either manual or automatic.
         match = re.search(r"Backport PR #(\d+) on branch", line)
         if match:
             entry[ind] = format_pr_entry(repo, match.groups()[0], auth=auth, dry_run=dry_run)
 
     # Remove github actions PRs
     gh_actions = "[@github-actions](https://github.com/github-actions)"
@@ -182,18 +176,20 @@
     # Get the new version
     version = util.get_version()
 
     # Get the existing changelog and run some validation
     changelog = Path(changelog_path).read_text(encoding="utf-8")
 
     if START_MARKER not in changelog or END_MARKER not in changelog:
-        raise ValueError("Missing insert marker for changelog")
+        msg = "Missing insert marker for changelog"
+        raise ValueError(msg)
 
     if changelog.find(START_MARKER) != changelog.rfind(START_MARKER):
-        raise ValueError("Insert marker appears more than once in changelog")
+        msg = "Insert marker appears more than once in changelog"
+        raise ValueError(msg)
 
     changelog = insert_entry(changelog, entry, version=version)
     Path(changelog_path).write_text(changelog, encoding="utf-8")
 
 
 def insert_entry(changelog, entry, version=None):
     """Insert the entry into the existing changelog."""
@@ -218,21 +214,21 @@
     else:
         changelog = changelog.replace(END_MARKER, "")
         changelog = changelog.replace(START_MARKER, new_entry)
 
     return format(changelog)
 
 
-def format(changelog):
+def format(changelog):  # noqa
     """Clean up changelog formatting"""
     changelog = re.sub(r"\n\n+", r"\n\n", changelog)
     return re.sub(r"\n\n+$", r"\n", changelog)
 
 
-def check_entry(
+def check_entry(  # noqa
     ref,
     branch,
     repo,
     auth,
     changelog_path,
     since,
     since_last_stable,
@@ -248,18 +244,20 @@
     # Finalize changelog
     changelog = Path(changelog_path).read_text(encoding="utf-8")
 
     start = changelog.find(START_MARKER)
     end = changelog.find(END_MARKER)
 
     if start == -1 or end == -1:  # pragma: no cover
-        raise ValueError("Missing new changelog entry delimiter(s)")
+        msg = "Missing new changelog entry delimiter(s)"
+        raise ValueError(msg)
 
     if start != changelog.rfind(START_MARKER):  # pragma: no cover
-        raise ValueError("Insert marker appears more than once in changelog")
+        msg = "Insert marker appears more than once in changelog"
+        raise ValueError(msg)
 
     final_entry = changelog[start + len(START_MARKER) : end]
 
     repo = repo or util.get_repo()
 
     raw_entry = get_version_entry(
         ref,
@@ -270,33 +268,36 @@
         since_last_stable=since_last_stable,
         auth=auth,
         resolve_backports=resolve_backports,
     )
 
     if f"# {version}" not in final_entry:  # pragma: no cover
         util.log(final_entry)
-        raise ValueError(f"Did not find entry for {version}")
+        msg = f"Did not find entry for {version}"
+        raise ValueError(msg)
 
     final_prs = re.findall(r"\[#(\d+)\]", final_entry)
     raw_prs = re.findall(r"\[#(\d+)\]", raw_entry)
 
     for pr in raw_prs:
         # Allow for changelog PR to not be in changelog itself
         skip = False
         for line in raw_entry.splitlines():
             if f"[#{pr}]" in line and "changelog" in line.lower():
                 skip = True
                 break
         if skip:
             continue
         if f"[#{pr}]" not in final_entry:  # pragma: no cover
-            raise ValueError(f"Missing PR #{pr} in changelog")
+            msg = f"Missing PR #{pr} in changelog"
+            raise ValueError(msg)
     for pr in final_prs:
         if f"[#{pr}]" not in raw_entry:  # pragma: no cover
-            raise ValueError(f"PR #{pr} does not belong in changelog for {version}")
+            msg = f"PR #{pr} does not belong in changelog for {version}"
+            raise ValueError(msg)
 
     if output:
         Path(output).write_text(final_entry, encoding="utf-8")
 
 
 def splice_github_entry(orig_entry, github_entry):
     """Splice an entry created on GitHub into one created by build_entry"""
@@ -306,15 +307,15 @@
     cl_regex = re.compile(r"^- (.*?) \[#(\d+)\]")
 
     lut = {}
     for title, pr in re.findall(gh_regex, github_entry):
         lut[pr] = title
 
     lines = orig_entry.splitlines()
-    for (ind, line) in enumerate(lines):
+    for ind, line in enumerate(lines):
         match = re.match(cl_regex, line)
         if not match:
             continue
         title, pr = re.findall(cl_regex, line)[0]
         if pr in lut:
             lines[ind] = line.replace(title, lut[pr])
 
@@ -323,15 +324,15 @@
     if preamble_index > 0:
         preamble = github_entry[:preamble_index]
         if preamble.startswith("# "):
             preamble = preamble.replace("# ", "## ")
         if preamble.startswith("## "):
             preamble = preamble.replace("## ", "### ")
 
-        lines = preamble.splitlines() + [""] + lines
+        lines = [*preamble.splitlines(), "", *lines]
 
     return "\n".join(lines)
 
 
 def extract_current(changelog_path):
     """Extract the current changelog entry"""
     body = ""
@@ -346,9 +347,10 @@
 
 
 def extract_current_version(changelog_path):
     """Extract the current released version from the changelog"""
     body = extract_current(changelog_path)
     match = re.match(r"#+ (\d\S+)", body.strip())
     if not match:
-        raise ValueError("Could not find previous version")
+        msg = "Could not find previous version"
+        raise ValueError(msg)
     return match.groups()[0]
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/cli.py` & `jupyter_releaser-1.1.6/jupyter_releaser/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,39 @@
 
 
 class ReleaseHelperGroup(click.Group):
     """Click group tailored to jupyter-releaser"""
 
     _needs_checkout_dir: t.Dict[str, bool] = {}
 
-    def invoke(self, ctx):
+    def invoke(self, ctx):  # noqa
         """Handle jupyter-releaser config while invoking a command"""
         # Get the command name and make sure it is valid
         cmd_name = ctx.protected_args[0]
         if cmd_name not in self.commands:
             super().invoke(ctx)
 
         if cmd_name == "list-envvars":
             envvars: t.Dict[str, str] = {}
             for cmd_name in self.commands:
                 for param in self.commands[cmd_name].params:
-                    if isinstance(param, click.Option):
-                        if param.envvar:
-                            envvars[str(param.name)] = str(param.envvar)
+                    if isinstance(param, click.Option) and param.envvar:
+                        envvars[str(param.name)] = str(param.envvar)
 
             for key in sorted(envvars):
                 util.log(f"{key.replace('_', '-')}: {envvars[key]}")
 
             return
 
         orig_dir = os.getcwd()
 
         if cmd_name.replace("-", "_") in self._needs_checkout_dir:
             if not osp.exists(util.CHECKOUT_NAME):
-                raise ValueError("Please run prep-git first")
+                msg = "Please run prep-git first"
+                raise ValueError(msg)
             os.chdir(util.CHECKOUT_NAME)
 
         # Read in the config
         config = util.read_config()
         hooks = config.get("hooks", {})
         options = config.get("options", {})
         skip = config.get("skip", [])
@@ -310,14 +310,15 @@
         help="Resource paths that should be available when installed",
     ),
 ]
 
 
 def add_options(options):
     """Add extracted common options to a click command"""
+
     # https://stackoverflow.com/a/40195800
     def _add_options(func):
         for option in reversed(options):
             func = option(func)
         return func
 
     return _add_options
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/lib.py` & `jupyter_releaser-1.1.6/jupyter_releaser/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import os
 import os.path as osp
 import re
 import shutil
 import tempfile
 import uuid
-from datetime import datetime
+from datetime import datetime, timezone
 from glob import glob
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Type, Union
 
 import mdformat
 from packaging.version import parse as parse_version
@@ -27,15 +27,16 @@
 
     version = util.get_version()
 
     # A properly parsed version will have a "major" attribute
     parsed = parse_version(version)
 
     if util.SETUP_PY.exists() and not hasattr(parsed, "major"):
-        raise ValueError(f"Invalid version {version}")
+        msg = f"Invalid version {version}"
+        raise ValueError(msg)
 
     # Bail if tag already exists
     tag_name = f"v{version}"
     if tag_name in util.run("git --no-pager tag", quiet=True).splitlines():
         msg = f"Tag {tag_name} already exists!"
         msg += " To delete run: `git push --delete origin {tag_name}`"
         raise ValueError(msg)
@@ -68,15 +69,16 @@
     npm_versions = None
     if util.PACKAGE_JSON.exists():
         npm_versions = npm.get_package_versions(version)
         util.log(npm_versions)
 
     tags = util.run("git --no-pager tag", quiet=True)
     if f"v{version}" in tags.splitlines():
-        raise ValueError(f"Tag v{version} already exists")
+        msg = f"Tag v{version} already exists"
+        raise ValueError(msg)
 
     current = changelog.extract_current(changelog_path)
     util.log(f"\n\nCurrent Changelog Entry:\n{current}")
 
     # Check out all changed files.
     try:
         util.run("git checkout .", echo=True)
@@ -112,16 +114,18 @@
 
     # Remove draft releases over a day old
     if bool(os.environ.get("GITHUB_ACTIONS")):
         for rel in gh.repos.list_releases():
             if str(rel.draft).lower() == "false":
                 continue
             created = rel.created_at
-            d_created = datetime.strptime(created, r"%Y-%m-%dT%H:%M:%SZ")
-            delta = datetime.utcnow() - d_created
+            d_created = datetime.strptime(created, r"%Y-%m-%dT%H:%M:%SZ").astimezone(
+                tz=timezone.utc
+            )
+            delta = datetime.now(tz=timezone.utc) - d_created
             if delta.days > 0:
                 gh.repos.delete_release(rel.id)
 
     # Set the GitHub action output for the release url.
     util.actions_output("release_url", release.html_url)
 
 
@@ -130,15 +134,15 @@
     repo = repo or util.get_repo()
     branch = branch or util.get_branch()
 
     # Make a new branch with a uuid suffix
     pr_branch = f"changelog-{uuid.uuid1().hex}"
 
     if not dry_run:
-        dirty = util.run("git --no-pager diff --stat") != ""
+        dirty = util.run("git --no-pager diff --stat") != ""  # noqa
         if dirty:
             util.run("git stash")
         util.run(f"{util.GIT_FETCH_CMD} {branch}")
         util.run(f"git checkout -b {pr_branch} origin/{branch}")
         if dirty:
             util.run("git stash apply")
 
@@ -250,15 +254,16 @@
 
 def delete_release(auth, release_url, dry_run=False):
     """Delete a draft GitHub release by url to the release page"""
     pattern = util.RELEASE_HTML_PATTERN % util.get_mock_github_url()
     match = re.match(pattern, release_url)
     match = match or re.match(util.RELEASE_API_PATTERN, release_url)
     if not match:
-        raise ValueError(f"Release url is not valid: {release_url}")
+        msg = f"Release url is not valid: {release_url}"
+        raise ValueError(msg)
 
     gh = util.get_gh_object(dry_run=dry_run, owner=match["owner"], repo=match["repo"], token=auth)
     release = util.release_for_url(gh, release_url)
     for asset in release.assets:
         gh.repos.delete_release_asset(asset.id)
 
     gh.repos.delete_release(release.id)
@@ -296,22 +301,24 @@
         asset_shas = json.load(fid)
     asset_shas_file.unlink()
 
     for asset in assets:
         if asset.name.endswith(".json"):
             continue
         if asset.name not in asset_shas:
-            raise ValueError(f"{asset.name} was not found in asset_shas file")
+            msg = f"{asset.name} was not found in asset_shas file"
+            raise ValueError(msg)
         if util.compute_sha256(dist / asset.name) != asset_shas[asset.name]:
-            raise ValueError(f"sha for {asset.name} does not match asset_shas file")
+            msg = f"sha for {asset.name} does not match asset_shas file"
+            raise ValueError(msg)
 
     os.chdir(orig_dir)
 
 
-def publish_assets(
+def publish_assets(  # noqa
     dist_dir,
     npm_token,
     npm_cmd,
     twine_cmd,
     npm_registry,
     twine_repository_url,
     dry_run,
@@ -326,18 +333,15 @@
     if len(glob(f"{dist_dir}/*.tgz")):
         npm.handle_npm_config(npm_token)
         if npm_token:
             util.run("npm whoami")
 
     res = python_package.split(":")
     python_package_path = res[0]
-    if len(res) == 2:
-        python_package_name = res[1].replace("-", "_")
-    else:
-        python_package_name = ""
+    python_package_name = res[1].replace("-", "_") if len(res) == 2 else ""  # noqa
 
     if release_url and len(glob(f"{dist_dir}/*.whl")):
         twine_token = python.get_pypi_token(release_url, python_package_path)
 
     if dry_run:
         # Start local pypi server with no auth, allowing overwrites,
         # in a temporary directory
@@ -353,18 +357,15 @@
     found = False
     for path in sorted(glob(f"{dist_dir}/*.*")):
         name = Path(path).name
         util.log(f"Handling dist file {path}")
         suffix = Path(path).suffix
         if suffix in [".gz", ".whl"]:
             dist: Union[Type[SDist], Type[Wheel]]
-            if suffix == ".gz":
-                dist = SDist
-            else:
-                dist = Wheel
+            dist = SDist if suffix == ".gz" else Wheel
             pkg = dist(path)
             if not python_package_name or python_package_name == pkg.name:
                 env = os.environ.copy()
                 env["TWINE_PASSWORD"] = twine_token
                 # NOTE: Do not print the env since a twine token extracted from
                 # a PYPI_TOKEN_MAP will not be sanitized in output
                 util.retry(f"{twine_cmd} {name}", cwd=dist_dir, env=env, echo=True)
@@ -405,15 +406,15 @@
         release.prerelease,
     )
 
     # Set the GitHub action output
     util.actions_output("release_url", release.html_url)
 
 
-def prep_git(ref, branch, repo, auth, username, url):
+def prep_git(ref, branch, repo, auth, username, url):  # noqa
     """Set up git"""
     repo = repo or util.get_repo()
 
     # Set up the repository
     checkout_dir = os.environ.get("RH_CHECKOUT_DIR", util.CHECKOUT_NAME)
     checkout_exists = False
     if osp.exists(osp.join(checkout_dir, ".git")):
@@ -534,15 +535,16 @@
     prev_header = ""
     for line in full_log[start:].splitlines():
         if line.strip().startswith("#"):
             prev_header = line
             break
 
     if not prev_header:
-        raise ValueError("No anchor for previous entry")
+        msg = "No anchor for previous entry"
+        raise ValueError(msg)
 
     # Check out the branch again
     util.run(f"git checkout -B {branch} origin/{branch}")
 
     default_entry = changelog.extract_current(changelog_path)
 
     # Look for the previous header
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/mock_github.py` & `jupyter_releaser-1.1.6/jupyter_releaser/mock_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A mock GitHub API implementation."""
 import atexit
-import datetime
 import json
 import os
 import tempfile
 import uuid
+from datetime import datetime, timezone
 from typing import Dict, List
 
 from fastapi import FastAPI, Request
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 
 from jupyter_releaser.util import get_mock_github_url
@@ -53,15 +53,15 @@
     with open(source_file, "w") as fid:
         json.dump(result, fid)
 
 
 class Asset(BaseModel):
     """An asset model."""
 
-    id: int
+    id: int  # noqa
     name: str
     content_type: str
     size: int
     state: str = "uploaded"
     url: str
     node_id: str = ""
     download_count: int = 0
@@ -79,15 +79,15 @@
     upload_url: str
     tarball_url: str = ""
     zipball_url: str = ""
     created_at: str
     published_at: str = ""
     draft: bool
     body: str = ""
-    id: int
+    id: int  # noqa
     node_id: str = ""
     author: str = ""
     html_url: str
     name: str = ""
     prerelease: bool
     tag_name: str
     target_commitish: str
@@ -117,15 +117,15 @@
     sha: str
 
 
 class Tag(BaseModel):
     """A tag model."""
 
     ref: str
-    object: TagObject
+    object: TagObject  # noqa
 
 
 releases: Dict[str, "Release"] = load_from_file("releases", Release)
 pulls: Dict[str, "PullRequest"] = load_from_file("pulls", PullRequest)
 release_ids_for_asset: Dict[str, str] = load_from_file("release_ids_for_asset", int)
 tag_refs: Dict[str, "Tag"] = load_from_file("tag_refs", Tag)
 
@@ -148,15 +148,15 @@
     release_id = uuid.uuid4().int
     data = await request.json()
     base_url = get_mock_github_url()
     url = f"{base_url}/repos/{owner}/{repo}/releases/{release_id}"
     html_url = f"{base_url}/{owner}/{repo}/releases/tag/{data['tag_name']}"
     upload_url = f"{base_url}/repos/{owner}/{repo}/releases/{release_id}/assets"
     fmt_str = r"%Y-%m-%dT%H:%M:%SZ"
-    created_at = datetime.datetime.utcnow().strftime(fmt_str)
+    created_at = datetime.now(tz=timezone.utc).strftime(fmt_str)
     model = Release(
         id=release_id,
         url=url,
         html_url=html_url,
         assets=[],
         upload_url=upload_url,
         created_at=created_at,
@@ -189,15 +189,15 @@
         async for chunk in request.stream():
             fid.write(chunk)
     headers = request.headers
     url = f"{base_url}/static/{asset_id}"
     asset = Asset(
         id=asset_id,
         name=name,
-        size=headers["content-length"],
+        size=int(headers["content-length"]),
         url=url,
         content_type=headers["content-type"],
     )
     release_ids_for_asset[str(asset_id)] = str(release_id)
     model.assets.append(asset)
     write_to_file("releases", releases)
     write_to_file("release_ids_for_asset", release_ids_for_asset)
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/npm.py` & `jupyter_releaser-1.1.6/jupyter_releaser/npm.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,25 +77,25 @@
         tar = tarfile.open(path)
         tar.extractall(target)
         tar.close()
 
         if "main" in data:
             main = osp.join(target, "package", data["main"])
             if not osp.exists(main):
-                raise ValueError(f"{name} is missing 'main' file {data['main']}")
+                msg = f"{name} is missing 'main' file {data['main']}"
+                raise ValueError(msg)
 
         shutil.move(str(target / "package"), str(pkg_dir))
 
     return names
 
 
 def check_dist(dist_dir, install_options):
     """Check npm dist file(s) in a dist dir"""
     with TemporaryDirectory() as td:
-
         util.run("npm init -y", cwd=td, quiet=True)
         names = []
         staging = Path(td) / "staging"
 
         names = extract_dist(dist_dir, staging)
 
         install_str = " ".join(f"./staging/{name}" for name in names)
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/python.py` & `jupyter_releaser-1.1.6/jupyter_releaser/python.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     resource_paths=None,
 ):
     """Check a Python package locally (not as a cli)"""
     resource_paths = resource_paths or []
     dist_file = util.normalize_path(dist_file)
     dist_dir = os.path.dirname(dist_file)  # used for check cmds.
 
-    for cmd in [check_cmd] + list(extra_check_cmds or []):
+    for cmd in [check_cmd, *list(extra_check_cmds or [])]:
         util.run(cmd.format(**locals()))
 
     test_commands = []
 
     if test_cmd:
         test_commands.append(test_cmd)
     elif python_imports is not None:
@@ -59,29 +59,29 @@
         name = name.replace("-", "_")
         test_commands.append(f'python -c "import {name}"')
 
     # Create venvs to install dist file
     # run the test command in the venv
     with TemporaryDirectory() as td:
         env_path = util.normalize_path(osp.abspath(td))
-        if os.name == "nt":  # pragma: no cover
+        if os.name == "nt":  # noqa  # pragma: no cover
             bin_path = f"{env_path}/Scripts/"
         else:
             bin_path = f"{env_path}/bin"
 
         # Create the virtual env, upgrade pip,
         # install, and run test command
         util.run(f"python -m venv {env_path}")
         util.run(f"{bin_path}/python -m pip install -q -U pip")
         util.run(f"{bin_path}/pip install -q {dist_file}")
         try:
             for cmd in test_commands:
                 util.run(f"{bin_path}/{cmd}")
         except CalledProcessError as e:
-            if test_cmd == "":
+            if test_cmd == "":  # noqa
                 util.log(
                     'You may need to set "check_imports" to appropriate Python package names in the config file.'
                 )
             raise e
         for resource_path in resource_paths:
             name, _, _ = resource_path.partition("/")
             test_file = Path(td) / "test_path.py"
@@ -125,15 +125,15 @@
     return twine_pwd
 
 
 def start_local_pypi():
     """Start a local PyPI server"""
     temp_dir = TemporaryDirectory()
     cmd = f"pypi-server run -p 8081  -P . -a . -o  -v {temp_dir.name}"
-    proc = Popen(shlex.split(cmd), stdout=PIPE)
+    proc = Popen(shlex.split(cmd), stdout=PIPE)  # noqa
     # Wait for the server to start
     while True:
         assert proc.stdout is not None
         line = proc.stdout.readline().decode("utf-8").strip()
         util.log(line)
         if "Listening on" in line:
             break
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/schema.json` & `jupyter_releaser-1.1.6/jupyter_releaser/schema.json`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/tee.py` & `jupyter_releaser-1.1.6/jupyter_releaser/tee.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,27 +48,27 @@
         line = await stream.readline()
         if line:
             callback(line)
         else:
             break
 
 
-async def _stream_subprocess(args: str, **kwargs: Any) -> CompletedProcess:
+async def _stream_subprocess(args: str, **kwargs: Any) -> CompletedProcess:  # noqa
     platform_settings: Dict[str, Any] = {}
     if platform.system() == "Windows":
         platform_settings["env"] = os.environ
 
     # this part keeps behavior backwards compatible with subprocess.run
     tee = kwargs.get("tee", True)
     stdout = kwargs.get("stdout", sys.stdout)
     if stdout == subprocess.DEVNULL or not tee:
-        stdout = open(os.devnull, "w")
+        stdout = open(os.devnull, "w")  # noqa
     stderr = kwargs.get("stderr", sys.stderr)
     if stderr == subprocess.DEVNULL or not tee:
-        stderr = open(os.devnull, "w")
+        stderr = open(os.devnull, "w")  # noqa
 
     # We need to tell subprocess which shell to use when running shell-like
     # commands.
     # * SHELL is not always defined
     # * /bin/bash does not exit on alpine, /bin/sh seems bit more portable
     if "executable" not in kwargs and isinstance(args, str) and " " in args:
         platform_settings["executable"] = os.environ.get("SHELL", "/bin/sh")
@@ -133,15 +133,15 @@
 def run(args: Union[str, List[str]], **kwargs: Any) -> CompletedProcess:
     """Drop-in replacement for subprocess.run that behaves like tee.
     Extra arguments added by our version:
     echo: False - Prints command before executing it.
     quiet: False - Avoid printing output
     show_cwd: False - Prints the current working directory.
     """
-    if isinstance(args, str):
+    if isinstance(args, str):  # noqa
         cmd = args
     else:
         # run was called with a list instead of a single item but asyncio
         # create_subprocess_shell requires command as a single string, so
         # we need to convert it to string
         cmd = join(args)
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/util.py` & `jupyter_releaser-1.1.6/jupyter_releaser/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         if not executable:
             raise CalledProcessError(1, f'Could not find executable "{parts[0]}"')
         parts[0] = normalize_path(executable)
 
     check = kwargs.pop("check", True)
 
     try:
-        output = check_output(parts, **kwargs).decode("utf-8").strip()
+        output = check_output(parts, **kwargs).decode("utf-8").strip()  # noqa
         log(output)
         return output
     except CalledProcessError as e:
         e.output = e.output.decode("utf-8")
         if quiet:
             e.stderr = e.stderr.decode("utf-8")
             log("stderr:\n", e.stderr.strip(), "\n\n")
@@ -167,15 +167,15 @@
         # If this is a hatchling project, use hatch to get
         # the dynamic version.
         if data.get("build-system", {}).get("build-backend") == "hatchling.build":
             cmd = _get_hatch_version_cmd()
             return run(cmd).split("\n")[-1]
 
     if SETUP_PY.exists():
-        warnings.warn("Using deprecated setup.py invocation")
+        warnings.warn("Using deprecated setup.py invocation", stacklevel=2)
         try:
             return run("python setup.py --version").split("\n")[-1]
         except CalledProcessError as e:
             log(e)
 
     # Build the wheel and extract the version.
     if PYPROJECT.exists():
@@ -185,15 +185,17 @@
             wheel = Wheel(wheel_path)
             version = wheel.version
             return version
 
     if PACKAGE_JSON.exists():
         return json.loads(PACKAGE_JSON.read_text(encoding="utf-8")).get("version", "")
 
-    raise ValueError("No version identifier could be found!")
+    msg = "No version identifier could be found!"
+
+    raise ValueError(msg)
 
 
 def normalize_path(path):
     """Normalize a path to use backslashes"""
     return str(path).replace(os.sep, "/")
 
 
@@ -220,15 +222,15 @@
     shas = {}
 
     files = glob(f"{dist_dir}/*")
     if files:  # pragma: no cover
         cmd += ' -m "SHA256 hashes:"'
 
     for path in sorted(files):
-        path = normalize_path(path)
+        path = normalize_path(path)  # noqa
         sha256 = compute_sha256(path)
         shas[path] = sha256
         name = osp.basename(path)
         cmd += f' -m "{name}: {sha256}"'
 
     run(cmd)
 
@@ -237,15 +239,15 @@
 
 def _get_hatch_version_cmd():
     if shutil.which("hatch"):
         return "hatch version"
     return "pipx run hatch version"
 
 
-def bump_version(version_spec, *, changelog_path="", version_cmd=""):
+def bump_version(version_spec, *, changelog_path="", version_cmd=""):  # noqa
     """Bump the version"""
     # Look for config files to determine version command if not given
     if not version_cmd:
         for name in "bumpversion", ".bumpversion", "bump2version", ".bump2version":
             if osp.exists(name + ".cfg"):
                 version_cmd = "bump2version"
 
@@ -255,34 +257,30 @@
         if PYPROJECT.exists():
             pyproject_text = PYPROJECT.read_text(encoding="utf-8")
             if "tool.tbump" in pyproject_text:
                 version_cmd = version_cmd or TBUMP_CMD
             elif "hatchling.build" in pyproject_text:
                 version_cmd = version_cmd or _get_hatch_version_cmd()
 
-        if SETUP_CFG.exists():
-            if "bumpversion" in SETUP_CFG.read_text(encoding="utf-8"):
-                version_cmd = version_cmd or "bump2version"
+        if SETUP_CFG.exists() and "bumpversion" in SETUP_CFG.read_text(encoding="utf-8"):
+            version_cmd = version_cmd or "bump2version"
 
     if not version_cmd and PACKAGE_JSON.exists():
         version_cmd = "npm version --git-tag-version false"
 
     if not version_cmd:  # pragma: no cover
-        raise ValueError("Please specify a version bump command to run")
+        msg = "Please specify a version bump command to run"
+        raise ValueError(msg)
 
     # Assign default values if no version spec was given
     if not version_spec:
-        if "tbump" in version_cmd or "hatch" in version_cmd:
-            version_spec = "next"
-        else:
-            version_spec = "patch"
+        version_spec = "next" if "tbump" in version_cmd or "hatch" in version_cmd else "patch"
 
     # Add some convenience options on top of "tbump" and "hatch"
     if "tbump" in version_cmd or "hatch" in version_cmd:
-
         v = parse_version(get_version())
         log(f"Current version was: {v}")
         assert isinstance(v, Version)
 
         if v.is_devrelease:
             # bump from the version in the changelog unless the spec is dev.
             # Import here to avoid circular import.
@@ -317,15 +315,15 @@
             # Bump to the next dev version.
             elif version_spec == "dev":
                 assert v.dev is not None
                 version_spec = f"{v.major}.{v.minor}.{v.micro}.dev{v.dev + 1}"
 
         else:
             # Handle dev version spec.
-            if version_spec == "dev":
+            if version_spec == "dev":  # noqa
                 if v.pre:
                     version_spec = f"{v.major}.{v.minor}.{v.micro}.dev0"
                 # Bump to next minor dev.
                 else:
                     version_spec = f"{v.major}.{v.minor + 1}.0.dev0"
 
             # For next, go to next prerelease or patch if it is a final version.
@@ -361,15 +359,16 @@
 def release_for_url(gh, url):
     """Get release response data given a release url"""
     release = None
     for rel in gh.repos.list_releases():
         if rel.html_url == url or rel.url == url:
             release = rel
     if not release:
-        raise ValueError(f"No release found for url {url}")
+        msg = f"No release found for url {url}"
+        raise ValueError(msg)
     return release
 
 
 def latest_draft_release(gh, branch=None):
     """Get the latest draft release for a given repo"""
     newest_time = None
     newest_release = None
@@ -379,15 +378,15 @@
         log("Getting latest draft release")
     for release in gh.repos.list_releases():
         if str(release.draft).lower() == "false":
             continue
         if branch and release.target_commitish != branch:
             continue
         created = release.created_at
-        d_created = datetime.strptime(created, r"%Y-%m-%dT%H:%M:%SZ")
+        d_created = datetime.strptime(created, r"%Y-%m-%dT%H:%M:%SZ")  # noqa
         if newest_time is None or d_created > newest_time:
             newest_time = d_created
             newest_release = release
     if not newest_release:
         log("No draft release found!")
     else:
         log(f"Found draft release at {newest_release.html_url}")
@@ -434,15 +433,15 @@
     while True:
         time.sleep(attempt)
         try:
             run(cmd, **kwargs)
             return
         except Exception as e:
             attempt += 1
-            if attempt == 3:
+            if attempt == 3:  # noqa
                 raise e
 
 
 def read_config():
     """Read the jupyter-releaser config data"""
     config = None
 
@@ -477,40 +476,41 @@
 
 def parse_release_url(release_url):
     """Parse a release url into a regex match"""
     pattern = RELEASE_HTML_PATTERN % get_mock_github_url()
     match = re.match(pattern, release_url)
     match = match or re.match(RELEASE_API_PATTERN, release_url)
     if not match:
-        raise ValueError(f"Release url is not valid: {release_url}")
+        msg = f"Release url is not valid: {release_url}"
+        raise ValueError(msg)
     return match
 
 
 def fetch_release_asset(target_dir, asset, auth):
     """Fetch a release asset into a target directory."""
     log(f"Fetching {asset.name}...")
     url = asset.url
     headers = {"Authorization": f"token {auth}", "Accept": "application/octet-stream"}
     path = Path(target_dir) / asset.name
-    with requests.get(url, headers=headers, stream=True) as r:
+    with requests.get(url, headers=headers, stream=True, timeout=60) as r:
         r.raise_for_status()
         with open(path, "wb") as f:
             for chunk in r.iter_content(chunk_size=8192):
                 f.write(chunk)
     return path
 
 
 def fetch_release_asset_data(asset, auth):
     """Fetch the data for a release asset."""
     log(f"Fetching data for {asset.name}...")
     url = asset.url
     headers = {"Authorization": f"token {auth}", "Accept": "application/octet-stream"}
 
     sink = BytesIO()
-    with requests.get(url, headers=headers, stream=True) as r:
+    with requests.get(url, headers=headers, stream=True, timeout=60) as r:
         r.raise_for_status()
         for chunk in r.iter_content(chunk_size=8192):
             sink.write(chunk)
     sink.seek(0)
     return json.loads(sink.read().decode("utf-8"))
 
 
@@ -541,28 +541,27 @@
     for asset in release.assets:
         if asset.name != METADATA_JSON.name:
             continue
 
         data = fetch_release_asset_data(asset, auth)
 
     if data is None:
-        raise ValueError(
-            f'Could not find "{METADATA_JSON.name}" file in draft release {release_url}'
-        )
+        msg = f'Could not find "{METADATA_JSON.name}" file in draft release {release_url}'
+        raise ValueError(msg)
 
     # Update environment variables.
     for key, value in data.items():
         if value is not None:
             env_name = f"RH_{key.upper()}"
             os.environ[env_name] = str(value)
 
     return data
 
 
-def prepare_environment(fetch_draft_release=True):
+def prepare_environment(fetch_draft_release=True):  # noqa
     """Prepare the environment variables, for use when running one of the
     action scripts."""
     # Set up env variables
     if not os.environ.get("RH_REPOSITORY"):
         if os.environ.get("RH_RELEASE_URL"):
             match = parse_release_url(os.environ["RH_RELEASE_URL"])
             owner, repo = match["owner"], match["repo"]
@@ -603,22 +602,22 @@
 
     # Ensure the user is an admin.
     if not dry_run:
         user = os.environ["GITHUB_ACTOR"]
         log(f"Getting permission level for {user}")
         try:
             collab_level = gh.repos.get_collaborator_permission_level(user)
-            if not collab_level["permission"] == "admin":
-                raise RuntimeError(f"User {user} does not have admin permission")
+            if collab_level["permission"] != "admin":
+                msg = f"User {user} does not have admin permission"
+                raise RuntimeError(msg)
             log("User was admin!")
         except Exception as e:
             log(str(e))
-            raise RuntimeError(
-                "Could not get user permission level, assuming user was not admin!"
-            ) from None
+            msg = "Could not get user permission level, assuming user was not admin!"
+            raise RuntimeError(msg) from None
 
     # Get the latest draft release if none is given.
     release_url = os.environ.get("RH_RELEASE_URL")
     log(f"Environment release url was {release_url}")
     if not release_url and fetch_draft_release:
         release = latest_draft_release(gh, branch)
         if release:
@@ -677,22 +676,22 @@
 
 
 _local_remote = None
 
 
 def get_remote_name(dry_run):
     """Get the appropriate remote git name."""
-    global _local_remote
+    global _local_remote  # noqa
     if not dry_run:
         return "origin"
 
     if _local_remote:
         try:
             run(f"git remote add test {_local_remote}")
-        except Exception:
+        except Exception:  # noqa
             pass
         return "test"
 
     tfile = tempfile.NamedTemporaryFile(suffix=".git")
     tfile.close()
     _local_remote = tfile.name.replace(os.sep, "/")
     run(f"git init --bare {_local_remote}")
@@ -710,40 +709,41 @@
     """Check for or start a mock github server."""
     core.GH_HOST = host = get_mock_github_url()
     port = urlparse(host).port
 
     log("Ensuring mock GitHub")
     # First see if it is already running.
     try:
-        requests.get(host)
+        requests.get(host, timeout=60)
         return
     except requests.ConnectionError:
         pass
 
     # Next make sure we have the required libraries.
     python = sys.executable.replace(os.sep, "/")
     try:
         import fastapi  # noqa
         import univcorn  # type: ignore  # noqa
     except ImportError:
         run(f"'{python}' -m pip install fastapi uvicorn")
 
     proc = subprocess.Popen(
-        [python, "-m", "uvicorn", "jupyter_releaser.mock_github:app", "--port", str(port)]
+        [python, "-m", "uvicorn", "jupyter_releaser.mock_github:app", "--port", str(port)]  # noqa
     )
 
     try:
         ret = proc.wait(1)
         if ret > 0:
-            raise ValueError(f"mock_github failed with {proc.returncode}")
+            msg = f"mock_github failed with {proc.returncode}"
+            raise ValueError(msg)
     except subprocess.TimeoutExpired:
         pass
     log("Mock GitHub started")
     atexit.register(proc.kill)
 
     while 1:
         try:
-            requests.get(host)
+            requests.get(host, timeout=60)
             break
         except requests.ConnectionError:
             pass
     return proc
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/actions/common.py` & `jupyter_releaser-1.1.6/jupyter_releaser/actions/common.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/actions/generate_changelog.py` & `jupyter_releaser-1.1.6/jupyter_releaser/actions/generate_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/actions/populate_release.py` & `jupyter_releaser-1.1.6/jupyter_releaser/actions/populate_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         log("Skipping populate assets")
         actions_output("release_url", release_url)
         sys.exit(0)
 
 dry_run = os.environ.get("RH_DRY_RUN", "").lower() == "true"
 
 if not os.environ.get("RH_RELEASE_URL"):
-    raise RuntimeError("Cannot complete Draft Release, no draft GitHub release url found!")
+    msg = "Cannot complete Draft Release, no draft GitHub release url found!"
+    raise RuntimeError(msg)
 
 run_action("jupyter-releaser prep-git")
 run_action("jupyter-releaser ensure-sha")
 run_action("jupyter-releaser bump-version")
 run_action("jupyter-releaser extract-changelog")
 
 # Make sure npm comes before python in case it produces
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/actions/prep_release.py` & `jupyter_releaser-1.1.6/jupyter_releaser/actions/prep_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/tests/conftest.py` & `jupyter_releaser-1.1.6/jupyter_releaser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/tests/test_cli.py` & `jupyter_releaser-1.1.6/jupyter_releaser/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,17 +572,16 @@
     orig_run = util.run
     called = 0
 
     os.environ["PYPI_TOKEN_MAP"] = "foo/bar,foo-token\nfizz/buzz,bar"
 
     def wrapped(cmd, **kwargs):
         nonlocal called
-        if "twine upload" in cmd:
-            if kwargs["env"]["TWINE_PASSWORD"] == "foo-token":
-                called += 1
+        if "twine upload" in cmd and kwargs["env"]["TWINE_PASSWORD"] == "foo-token":
+            called += 1
         return orig_run(cmd, **kwargs)
 
     mock_run = mocker.patch("jupyter_releaser.util.run", wraps=wrapped)
 
     dist_dir = py_package / util.CHECKOUT_NAME / "dist"
     release = create_draft_release(files=glob(f"{dist_dir}/*.*"))
     os.environ["RH_RELEASE_URL"] = release.html_url
@@ -677,15 +676,14 @@
 
     log = get_log()
     assert "before-publish-release" in log
     assert "after-publish-release" in log
 
 
 def test_config_file(py_package, runner, mocker, git_prep):
-
     config = Path(util.CHECKOUT_NAME) / util.JUPYTER_RELEASER_CONFIG
     config_data = util.toml.loads(config.read_text(encoding="utf-8"))
     config_data["options"] = {"dist-dir": "foo"}
     config.write_text(util.toml.dumps(config_data), encoding="utf-8")
 
     orig_run = util.run
     called = False
@@ -704,15 +702,14 @@
 
     log = get_log()
     assert "before-build-python" in log
     assert "after-build-python" in log
 
 
 def test_config_file_env_override(py_package, runner, mocker, git_prep):
-
     orig_run = util.run
     called = False
 
     def wrapped(cmd, **kwargs):
         nonlocal called
         if cmd.startswith("pipx run build --outdir bar"):
             called = True
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/tests/test_functions.py` & `jupyter_releaser-1.1.6/jupyter_releaser/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/tests/test_mock_github.py` & `jupyter_releaser-1.1.6/jupyter_releaser/tests/test_mock_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         release["prerelease"],
     )
     assert release.draft is False
 
     for asset in release.assets:
         headers = dict(Authorization=f"token {auth}", Accept="application/octet-stream")
         print(asset.name)
-        with requests.get(asset.url, headers=headers, stream=True) as r:
+        with requests.get(asset.url, headers=headers, stream=True, timeout=60) as r:
             r.raise_for_status()
             for _ in r.iter_content(chunk_size=8192):
                 pass
 
     gh.git.create_ref("v1.1.0", "aaaa")
     tags = gh.list_tags("v1.1.0")
     assert tags[0]["object"]["sha"] == "aaaa"
```

### Comparing `jupyter_releaser-1.1.5/jupyter_releaser/tests/util.py` & `jupyter_releaser-1.1.6/jupyter_releaser/tests/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,28 +179,27 @@
 def get_log():
     log = Path(util.CHECKOUT_NAME) / "log.txt"
     return log.read_text(encoding="utf-8").splitlines()
 
 
 def create_python_package(git_repo, multi=False, not_matching_name=False):
     def write_files(git_repo, sub_packages=None, package_name="foo", module_name=None):
-
         sub_packages = sub_packages or []
 
         module_name = module_name or package_name
 
         pyproject = git_repo / "pyproject.toml"
         pyproject.write_text(
             pyproject_template(package_name, module_name, sub_packages), encoding="utf-8"
         )
 
         foopy = git_repo / f"{module_name}.py"
         foopy.write_text(PY_MODULE_TEMPLATE, encoding="utf-8")
 
-        license = git_repo / "LICENSE"
+        license = git_repo / "LICENSE"  # noqa
         license.write_text(LICENSE_TEMPLATE, encoding="utf-8")
 
         here = Path(__file__).parent
         text = here.parent.parent.joinpath(".pre-commit-config.yaml").read_text(encoding="utf-8")
 
         readme = git_repo / "README.md"
         readme.write_text(README_TEMPLATE, encoding="utf-8")
```

### Comparing `jupyter_releaser-1.1.5/.gitignore` & `jupyter_releaser-1.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/LICENSE` & `jupyter_releaser-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.5/README.md` & `jupyter_releaser-1.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Jupyter Releaser
 
 [![Build Status](https://github.com/jupyter-server/jupyter-releaser/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter-server/jupyter_releaser/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)
-[![codecov](https://codecov.io/gh/jupyter-server/jupyter_releaser/branch/main/graph/badge.svg?token=6OPBSEMMUG)](https://codecov.io/gh/jupyter-server/jupyter_releaser)
 [![Documentation Status](https://readthedocs.org/projects/jupyter-releaser/badge/?version=latest)](http://jupyter-releaser.readthedocs.io/en/latest/?badge=latest)
 
 **Jupyter Releaser** contains a set of helper scripts and GitHub Actions to aid in automated releases of Python and npm packages.
 
 ## Installation
 
 To install the latest release locally, make sure you have
```

### Comparing `jupyter_releaser-1.1.5/pyproject.toml` & `jupyter_releaser-1.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 urls = {Homepage = "https://jupyter.org"}
 requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = [
     "click",
-    "ghapi",
+    "ghapi<=1.0.4",
     "github-activity~=0.2",
     "importlib_resources",
     "jsonschema>=3.0.1",
     "mdformat",
     "packaging",
     "pkginfo",
     "pypiserver",
@@ -50,19 +50,17 @@
   "myst-parser",
   "pydata_sphinx_theme",
   "sphinxcontrib_spelling",
   "numpydoc",
   "sphinx-click",
 ]
 test = [
-  "coverage",
   "fastapi",
   "pre-commit",
   "pytest>=7.0",
-  "pytest-cov",
   "pytest-mock",
   "pytest-xdist[psutil]",
   "uvicorn"
 ]
 
 [project.scripts]
 jupyter-releaser = "jupyter_releaser.cli:main"
@@ -80,31 +78,31 @@
 features = ["test"]
 [tool.hatch.envs.test.scripts]
 test = "python -m pytest -vv {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.cov]
 features = ["test"]
-dependencies = ["coverage", "pytest-cov"]
+dependencies = ["coverage[toml]", "pytest-cov"]
 [tool.hatch.envs.cov.scripts]
 test = "python -m pytest -vv --cov jupyter_releaser --cov-branch --cov-report term-missing:skip-covered {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.typing]
 features = ["test"]
 dependencies = ["mypy>=0.990"]
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:jupyter_releaser}"
 
 [tool.hatch.envs.lint]
 dependencies = [
-  "black==22.12.0",
+  "black==23.3.0",
   "mdformat>0.7",
   "mdformat-gfm>=0.3.5",
-  "ruff==0.0.206"
+  "ruff==0.0.270"
 ]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
@@ -143,14 +141,18 @@
   "raise NotImplementedError",
   "if 0:",
   "if __name__ == .__main__.:",
   "class .*\bProtocol\\):",
 "@(abc\\.)?abstractmethod",
 ]
 
+[tool.coverage.run]
+relative_files = true
+source = ["jupyter_releaser"]
+
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = false
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 no_implicit_reexport = false
@@ -180,46 +182,35 @@
 skip-string-normalization = true
 target-version = ["py37"]
 
 [tool.ruff]
 target-version = "py37"
 line-length = 100
 select = [
-  "A", "B", "C", "E", "F", "FBT", "I", "N", "Q", "RUF", "S", "T",
-  "UP", "W", "YTT",
+  "A", "B", "C", "DTZ", "E", "EM", "F", "FBT", "I", "ICN", "ISC", "N",
+  "PLC", "PLE", "PLR", "PLW", "Q", "RUF", "S", "SIM", "T", "TID", "UP",
+  "W", "YTT",
 ]
 ignore = [
-  # Allow non-abstract empty methods in abstract base classes
-  "B027",
-  # Ignore McCabe complexity
-  "C901",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Use of `assert` detected
-  "S101",
-  # Line too long
-  "E501",
-  # Relative imports are banned
-  "TID252",
-  # Boolean ... in function definition
-  "FBT001", "FBT002",
-  # Module level import not at top of file
-  "E402",
-  # A001/A002/A003 .. is shadowing a python builtin
-  "A001", "A002", "A003",
-  # Possible hardcoded password
-  "S105", "S106",
   # Q000 Single quotes found but double quotes preferred
   "Q000",
-  # N806 Variable `B` in function should be lowercase
-  "N806",
+  # FBT001 Boolean positional arg in function definition
+  "FBT001", "FBT002", "FBT003",
+  # E501 Line too long (158 > 100 characters)
+  "E501",
+  # SIM105 Use `contextlib.suppress(...)`
+  "SIM105",
   # T201 `print` found
   "T201",
   # N802 Function name `CreateWellKnownSid` should be lowercase
-  "N802", "N803"
+  "N802", "N803",
+  # S101 Use of `assert` detected
+  "S101",
+  # PLR0913 Too many arguments to function call
+  "PLR0913",
 ]
 unfixable = [
   # Don't touch print statements
   "T201",
   # Don't touch noqa lines
   "RUF100",
 ]
@@ -228,15 +219,17 @@
 # B011 Do not call assert False since python -O removes these calls
 # F841 local variable 'foo' is assigned to but never used
 # C408 Unnecessary `dict` call
 # E402 Module level import not at top of file
 # T201 `print` found
 # B007 Loop control variable `i` not used within the loop body.
 # N802 Function name `assertIn` should be lowercase
-"jupyter_releaser/tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802"]
+# PLR2004 Magic value used in comparison
+# S105 Possible hardcoded password
+"jupyter_releaser/tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "PLR2004", "S105", "S106"]
 
 [tool.interrogate]
 ignore-init-module=true
 ignore-private=true
 ignore-semiprivate=true
 ignore-property-decorators=true
 ignore-nested-functions=true
```

### Comparing `jupyter_releaser-1.1.5/PKG-INFO` & `jupyter_releaser-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_releaser
-Version: 1.1.5
+Version: 1.1.6
 Summary: Jupyter Releaser for Python and/or npm packages.
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: Copyright (c) 2021 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -47,15 +47,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: click
-Requires-Dist: ghapi
+Requires-Dist: ghapi<=1.0.4
 Requires-Dist: github-activity~=0.2
 Requires-Dist: importlib-resources
 Requires-Dist: jsonschema>=3.0.1
 Requires-Dist: mdformat
 Requires-Dist: packaging
 Requires-Dist: pipx
 Requires-Dist: pkginfo
@@ -69,28 +69,25 @@
 Requires-Dist: pip; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-click; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: coverage; extra == 'test'
 Requires-Dist: fastapi; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-mock; extra == 'test'
 Requires-Dist: pytest-xdist[psutil]; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: uvicorn; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Jupyter Releaser
 
 [![Build Status](https://github.com/jupyter-server/jupyter-releaser/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter-server/jupyter_releaser/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)
-[![codecov](https://codecov.io/gh/jupyter-server/jupyter_releaser/branch/main/graph/badge.svg?token=6OPBSEMMUG)](https://codecov.io/gh/jupyter-server/jupyter_releaser)
 [![Documentation Status](https://readthedocs.org/projects/jupyter-releaser/badge/?version=latest)](http://jupyter-releaser.readthedocs.io/en/latest/?badge=latest)
 
 **Jupyter Releaser** contains a set of helper scripts and GitHub Actions to aid in automated releases of Python and npm packages.
 
 ## Installation
 
 To install the latest release locally, make sure you have
```


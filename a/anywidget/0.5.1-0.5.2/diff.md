# Comparing `tmp/anywidget-0.5.1.tar.gz` & `tmp/anywidget-0.5.2.tar.gz`

## Comparing `anywidget-0.5.1.tar` & `anywidget-0.5.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.5.1/CITATION.cff
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.5.1/package.json
--rw-r--r--   0        0        0   259753 2020-02-02 00:00:00.000000 anywidget-0.5.1/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.5.1/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.5.1/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/__init__.py
--rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/138.8acbfebf26b04f3c9d53.js
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/326.f2f979ab7119ae78c2be.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/remoteEntry.73f706fd5f93400afdaf.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/astro.config.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/scripts/render.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.5.1/examples/Counter.ipynb
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.5.1/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_descriptor.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_utils.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.5.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.5.1/LICENSE
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 anywidget-0.5.1/README.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 anywidget-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.5.2/CITATION.cff
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.5.2/package.json
+-rw-r--r--   0        0        0   259753 2020-02-02 00:00:00.000000 anywidget-0.5.2/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.5.2/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.5.2/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/__init__.py
+-rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/labextension/static/138.0c72d6d2736b3c54bde2.js
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/labextension/static/326.cc621ff41abd2006f96d.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/labextension/static/remoteEntry.7a8d20f76e614816a656.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 anywidget-0.5.2/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.5.2/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.5.2/examples/Counter.ipynb
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.5.2/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 anywidget-0.5.2/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.5.2/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.5.2/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.5.2/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.5.2/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 anywidget-0.5.2/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.5.2/tests/test_descriptor.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.5.2/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.5.2/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.5.2/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.5.2/tests/test_utils.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.5.2/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 anywidget-0.5.2/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 anywidget-0.5.2/PKG-INFO
```

### Comparing `anywidget-0.5.1/.pre-commit-config.yaml` & `anywidget-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/CITATION.cff` & `anywidget-0.5.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/package.json` & `anywidget-0.5.2/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/pnpm-lock.yaml` & `anywidget-0.5.2/pnpm-lock.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,18 @@
       vite:
         specifier: ^4.1.4
         version: 4.1.4(@types/node@18.14.6)
 
   packages/anywidget:
     dependencies:
       '@anywidget/types':
-        specifier: workspace:*
+        specifier: workspace:~
         version: link:../types
       '@anywidget/vite':
-        specifier: workspace:*
+        specifier: workspace:~
         version: link:../vite
       '@jupyter-widgets/base':
         specifier: ^2 || ^3 || ^4 || ^5 || ^6
         version: 6.0.2(crypto@1.0.1)
     devDependencies:
       '@jupyterlab/builder':
         specifier: ^3.6.2
```

### Comparing `anywidget-0.5.1/anywidget/_descriptor.py` & `anywidget-0.5.2/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/anywidget/_file_contents.py` & `anywidget-0.5.2/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/anywidget/_protocols.py` & `anywidget-0.5.2/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/anywidget/_util.py` & `anywidget-0.5.2/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/anywidget/experimental.py` & `anywidget-0.5.2/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/anywidget/widget.py` & `anywidget-0.5.2/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/anywidget/labextension/package.json` & `anywidget-0.5.2/anywidget/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9431423611111112%*

 * *Differences: {"'dependencies'": "{'@anywidget/vite': 'workspace:~', '@anywidget/types': 'workspace:~'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7a8d20f76e614816a656.js'}}",*

 * * "'version'": "'0.5.2'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "author": "Trevor Manz",
     "dependencies": {
-        "@anywidget/types": "workspace:*",
-        "@anywidget/vite": "workspace:*",
+        "@anywidget/types": "workspace:~",
+        "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
         "@jupyterlab/builder": "^3.6.2"
     },
     "exports": {
         ".": "./dist/index.js",
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.73f706fd5f93400afdaf.js"
+            "load": "static/remoteEntry.7a8d20f76e614816a656.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.5.1"
+    "version": "0.5.2"
 }
```

### Comparing `anywidget-0.5.1/anywidget/labextension/static/138.8acbfebf26b04f3c9d53.js` & `anywidget-0.5.2/anywidget/labextension/static/138.0c72d6d2736b3c54bde2.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -53,14 +53,15 @@
 
             function o(e) {
                 return {
                     model: {
                         get: e.model.get.bind(e.model),
                         set: e.model.set.bind(e.model),
                         save_changes: e.model.save_changes.bind(e.model),
+                        send: e.model.send.bind(e.model),
                         on(t, n) {
                             e.model.on(t, n, e)
                         },
                         off(t, n) {
                             e.model.off(t, n, e)
                         }
                     },
@@ -116,11 +117,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.5.1/anywidget/labextension/static/326.f2f979ab7119ae78c2be.js` & `anywidget-0.5.2/anywidget/labextension/static/326.cc621ff41abd2006f96d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
                     })
                 },
                 autoStart: !0
             }
         },
         203: (e, t, n) => {
             n.d(t, {
-                Z: () => c
+                Z: () => l
             });
             var i = n(147);
 
             function a(e) {
                 return e.startsWith("http://") || e.startsWith("https://")
             }
             async function d(e, t) {
@@ -71,26 +71,27 @@
 
             function o(e) {
                 return {
                     model: {
                         get: e.model.get.bind(e.model),
                         set: e.model.set.bind(e.model),
                         save_changes: e.model.save_changes.bind(e.model),
+                        send: e.model.send.bind(e.model),
                         on(t, n) {
                             e.model.on(t, n, e)
                         },
                         off(t, n) {
                             e.model.off(t, n, e)
                         }
                     },
                     el: e.el
                 }
             }
 
-            function c({
+            function l({
                 DOMWidgetModel: e,
                 DOMWidgetView: t
             }) {
                 class n extends e {
                     static model_name = "AnyModel";
                     static model_module = i.u2;
                     static model_module_version = i.i8;
@@ -134,11 +135,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.5.1/anywidget/labextension/static/remoteEntry.73f706fd5f93400afdaf.js` & `anywidget-0.5.2/anywidget/labextension/static/remoteEntry.7a8d20f76e614816a656.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,274 +1,274 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
+    var e, r, t, n, o, i, a, u, l, s, f, d, c, p, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    i = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => a
+                    init: () => i
                 })
             }
         },
         g = {};
 
-    function m(e) {
+    function b(e) {
         var r = g[e];
         if (void 0 !== r) return r.exports;
         var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, m), t.exports
+        return v[e](t, t.exports, b), t.exports
     }
-    m.m = v, m.c = g, m.n = e => {
+    b.m = v, b.c = g, b.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return m.d(r, {
+        return b.d(r, {
             a: r
         }), r
-    }, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    }, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "8acbfebf26b04f3c9d53",
-        326: "f2f979ab7119ae78c2be"
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
+        138: "0c72d6d2736b3c54bde2",
+        326: "cc621ff41abd2006f96d"
     } [e] + ".js?v=" + {
-        138: "8acbfebf26b04f3c9d53",
-        326: "f2f979ab7119ae78c2be"
-    } [e], m.g = function() {
+        138: "0c72d6d2736b3c54bde2",
+        326: "cc621ff41abd2006f96d"
+    } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", b.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var i, u;
+            var a, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        a = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    a.onerror = a.onload = null, clearTimeout(c);
                     var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
-                    target: i
+                    target: a
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), u && document.head.appendChild(a)
         }
-    }, m.r = e => {
+    }, b.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        m.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var a = m.S[t],
-                    i = "anywidget",
+                b.o(b.S, t) || (b.S[t] = {});
+                var i = b.S[t],
+                    a = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var o = a[e] = a[e] || {},
+                    var o = i[e] = i[e] || {},
                         u = o[r];
-                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => m.e(138).then((() => () => m(138))),
-                        from: i,
+                    (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
+                        get: () => b.e(138).then((() => () => b(138))),
+                        from: a,
                         eager: !1
                     })
-                })("anywidget", "0.5.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.5.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
-            var i = r[n],
-                u = (typeof i)[0];
-            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+                i = (typeof o)[0];
+            if (n >= r.length) return "u" == i;
+            var a = r[n],
+                u = (typeof a)[0];
+            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
+            if ("o" != i && "u" != i && o != a) return o < a;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
-        var i = [];
-        for (a = 1; a < e.length; a++) {
-            var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+        var a = [];
+        for (i = 1; i < e.length; i++) {
+            var u = e[i];
+            a.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
         }
         return l();
 
         function l() {
-            return i.pop().replace(/^\((.+)\)$/, "$1")
+            return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == s) {
+            for (var a = 0, u = 1, l = !0;; u++, a++) {
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (a >= r.length || "o" == (f = (typeof(s = r[a]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
                     if (!l || "u" != d) return !1
                 } else if (l)
-                    if (d == s)
+                    if (d == f)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < d != o) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
-        for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+        var c = [],
+            p = c.pop.bind(c);
+        for (a = 1; a < e.length; a++) {
+            var h = e[a];
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
-        return !!c()
-    }, i = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        return !!p()
+    }, a = (e, r) => {
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
-    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var a = m.I(r);
-        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
+        return i(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
+    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+        var i = b.I(r);
+        return i && i.then ? i.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), c = {}, p = {
         395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
-    }, m.f.consumes = (e, r) => {
-        m.o(h, e) && h[e].forEach((e => {
-            if (m.o(p, e)) return r.push(p[e]);
+    }, b.f.consumes = (e, r) => {
+        b.o(h, e) && h[e].forEach((e => {
+            if (b.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    p[e] = 0, m.m[e] = t => {
-                        delete m.c[e], t.exports = r()
+                    c[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], m.m[e] = t => {
-                        throw delete m.c[e], r
+                    delete c[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
-                var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                var o = p[e]();
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = m.p + m.u(r),
-                        i = new Error;
-                    m.l(a, (t => {
-                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    var i = b.p + b.u(r),
+                        a = new Error;
+                    b.l(i, (t => {
+                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
-                                a = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                                i = t && t.target && t.target.src;
+                            a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [a, i, u] = t,
+                var n, o, [i, a, u] = t,
                     l = 0;
-                if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
-                    u && u(m)
+                if (i.some((r => 0 !== e[r]))) {
+                    for (n in a) b.o(a, n) && (b.m[n] = a[n]);
+                    u && u(b)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < i.length; l++) o = i[l], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var y = m(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
+    var m = b(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = m
 })();
```

### Comparing `anywidget-0.5.1/anywidget/nbextension/index.js` & `anywidget-0.5.2/anywidget/nbextension/index.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.5.1";
+var version = "0.5.2";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
@@ -72,29 +72,21 @@
     }
     URL.revokeObjectURL(url);
     return widget;
 }
 
 function extract_context(view) {
     let model = {
-        /** @param {string} name */
         get: view.model.get.bind(view.model),
         set: view.model.set.bind(view.model),
         save_changes: view.model.save_changes.bind(view.model),
-        /**
-         * @param {string} name
-         * @param {any} callback
-         */
+        send: view.model.send.bind(view.model),
         on(name2, callback) {
             view.model.on(name2, callback, view);
         },
-        /**
-         * @param {string} name
-         * @param {any} callback
-         */
         off(name2, callback) {
             view.model.off(name2, callback, view);
         }
     };
     return {
         model,
         el: view.el
```

### Comparing `anywidget-0.5.1/docs/README.md` & `anywidget-0.5.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/astro.config.js` & `anywidget-0.5.2/docs/astro.config.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/package.json` & `anywidget-0.5.2/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/anywidget-overview.png` & `anywidget-0.5.2/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/banner-dark.png` & `anywidget-0.5.2/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/banner-light.png` & `anywidget-0.5.2/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/banner-minimal.png` & `anywidget-0.5.2/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/client-js-diagram.png` & `anywidget-0.5.2/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/default-og-image.png` & `anywidget-0.5.2/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/favicon.svg` & `anywidget-0.5.2/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/public/widget-overview.png` & `anywidget-0.5.2/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/scripts/ipynb.mjs` & `anywidget-0.5.2/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/scripts/utils.mjs` & `anywidget-0.5.2/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/consts.ts` & `anywidget-0.5.2/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/CodeHero.astro` & `anywidget-0.5.2/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/CounterButton.astro` & `anywidget-0.5.2/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/HeadCommon.astro` & `anywidget-0.5.2/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/HeadSEO.astro` & `anywidget-0.5.2/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Hero.astro` & `anywidget-0.5.2/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.5.2/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.5.2/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.5.2/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/Header.astro` & `anywidget-0.5.2/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/HeaderButton.css` & `anywidget-0.5.2/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.5.2/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.5.2/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/Search.css` & `anywidget-0.5.2/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/Search.tsx` & `anywidget-0.5.2/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.5.2/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.5.2/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.5.2/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.5.2/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.5.2/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.5.2/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.5.2/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.5.2/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/components/examples/Counter.astro` & `anywidget-0.5.2/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/layouts/MainLayout.astro` & `anywidget-0.5.2/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/layouts/SplashLayout.astro` & `anywidget-0.5.2/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.5.2/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.5.2/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/pages/en/bundling.md` & `anywidget-0.5.2/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/pages/en/experimental.md` & `anywidget-0.5.2/docs/src/pages/en/experimental.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/pages/en/getting-started.mdx` & `anywidget-0.5.2/docs/src/pages/en/getting-started.mdx`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 an abstraction for creating custom Jupyter widgets using modern web standards.
 **anywidget** solves the multi-platform packaging problem for the fragmented Jupyter
 ecosystem, allowing your widget to run automatically in **Jupyter Notebooks**,
 **Jupyter Lab**, **Google Colab**, **VSCode**, and more.
 
 ## Key features
 
-- Create widgets **without complicated cookiecutter templates**
-- **Build and publish to PyPI** like a pure Python package
-- Prototype **within** `.ipynb` or `.py` files
-- Run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
-- Develop (optionally) with [Vite](https://vitejs.dev/) for **instant HMR**
+- 🛠️ Create widgets **without complicated cookiecutter templates**
+- 📚 **Publish to PyPI** like any other Python package
+- 🤖 Prototype **within** `.ipynb` or `.py` files
+- 🚀 Run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
+- ⚡ Develop with **instant HMR**, like modern web frameworks
 
 ## Example
 
 ```
 pip install "anywidget[dev]"
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `anywidget-0.5.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.5.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.5.2/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/styles/index.css` & `anywidget-0.5.2/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/docs/src/styles/theme.css` & `anywidget-0.5.2/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/examples/Counter.ipynb` & `anywidget-0.5.2/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/examples/minimal_example.ipynb` & `anywidget-0.5.2/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/packages/anywidget/CHANGELOG.md` & `anywidget-0.5.2/packages/anywidget/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # anywidget
 
+## 0.5.2
+
+### Patch Changes
+
+- fix: re-expose model.send for custom messages ([#146](https://github.com/manzt/anywidget/pull/146))
+
+- Updated dependencies [[`5a5787b`](https://github.com/manzt/anywidget/commit/5a5787b517075dd8f2c6607dcbc0deac481a9df3), [`774f139`](https://github.com/manzt/anywidget/commit/774f139f45b747caafaa0fac0fd7588d97078db2)]:
+  - @anywidget/vite@0.1.1
+  - @anywidget/types@0.1.1
+
 ## 0.5.1
 
 ### Patch Changes
 
 - Updated dependencies [[`79098be`](https://github.com/manzt/anywidget/commit/79098be4bc5a1ce1023318b179b8e73ab3e59be3)]:
   - @anywidget/vite@0.1.0
```

### Comparing `anywidget-0.5.1/packages/anywidget/build.mjs` & `anywidget-0.5.2/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/packages/anywidget/package.json` & `anywidget-0.5.2/packages/anywidget/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444445%*

 * *Differences: {"'dependencies'": "{'@anywidget/vite': 'workspace:~', '@anywidget/types': 'workspace:~'}",*

 * * "'version'": "'0.5.2'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "author": "Trevor Manz",
     "dependencies": {
-        "@anywidget/types": "workspace:*",
-        "@anywidget/vite": "workspace:*",
+        "@anywidget/types": "workspace:~",
+        "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
         "@jupyterlab/builder": "^3.6.2"
     },
     "exports": {
         ".": "./dist/index.js",
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.5.1"
+    "version": "0.5.2"
 }
```

### Comparing `anywidget-0.5.1/packages/anywidget/src/widget.js` & `anywidget-0.5.2/packages/anywidget/src/widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -109,30 +109,23 @@
  *
  * Prunes the view down to the minimum context necessary for rendering.
  * Calls to `model.get` and `model.set` automatically add the view as
  * context to the model, so we can gracefully unsubscribe from events
  * added by the user-defined render.
  */
 function extract_context(view) {
+    /** @type {import("@anywidget/types").AnyModel} */
     let model = {
-        /** @param {string} name */
         get: view.model.get.bind(view.model),
         set: view.model.set.bind(view.model),
         save_changes: view.model.save_changes.bind(view.model),
-        /**
-         * @param {string} name
-         * @param {any} callback
-         */
+        send: view.model.send.bind(view.model),
         on(name, callback) {
             view.model.on(name, callback, view);
         },
-        /**
-         * @param {string} name
-         * @param {any} callback
-         */
         off(name, callback) {
             view.model.off(name, callback, view);
         },
     };
     return {
         model,
         el: view.el
```

### Comparing `anywidget-0.5.1/tests/test_descriptor.py` & `anywidget-0.5.2/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/tests/test_experimental.py` & `anywidget-0.5.2/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/tests/test_file_contents.py` & `anywidget-0.5.2/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/tests/test_utils.py` & `anywidget-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/tests/test_widget.py` & `anywidget-0.5.2/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/LICENSE` & `anywidget-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/README.md` & `anywidget-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/pyproject.toml` & `anywidget-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.1/PKG-INFO` & `anywidget-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.5.1
+Version: 0.5.2
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
```


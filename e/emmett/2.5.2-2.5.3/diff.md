# Comparing `tmp/emmett-2.5.2.tar.gz` & `tmp/emmett-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett-2.5.2.tar", max compression
+gzip compressed data, was "emmett-2.5.3.tar", max compression
```

## Comparing `emmett-2.5.2.tar` & `emmett-2.5.3.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0    14193 2023-05-19 11:27:14.001857 emmett-2.5.2/CHANGES.md
--rw-r--r--   0        0        0     2074 2023-05-19 11:27:14.001857 emmett-2.5.2/LICENSE
--rw-r--r--   0        0        0     2922 2023-05-19 11:27:14.001857 emmett-2.5.2/README.md
--rw-r--r--   0        0        0     9917 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/app_and_modules.md
--rw-r--r--   0        0        0    15873 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/auth.md
--rw-r--r--   0        0        0    12150 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/caching.md
--rw-r--r--   0        0        0     2613 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/cli.md
--rw-r--r--   0        0        0     4481 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/debug_and_logging.md
--rw-r--r--   0        0        0     3056 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/deployment.md
--rw-r--r--   0        0        0     5295 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/extensions.md
--rw-r--r--   0        0        0     5174 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/foreword.md
--rw-r--r--   0        0        0     6493 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/forms.md
--rw-r--r--   0        0        0     2105 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/installation.md
--rw-r--r--   0        0        0     3596 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/languages.md
--rw-r--r--   0        0        0     3087 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/mailer.md
--rw-r--r--   0        0        0     9672 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/advanced.md
--rw-r--r--   0        0        0    12917 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/callbacks.md
--rw-r--r--   0        0        0     7060 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/connecting.md
--rw-r--r--   0        0        0    20808 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/migrations.md
--rw-r--r--   0        0        0    14034 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/models.md
--rw-r--r--   0        0        0    29245 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/operations.md
--rw-r--r--   0        0        0    27472 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/relations.md
--rw-r--r--   0        0        0     5523 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/scopes.md
--rw-r--r--   0        0        0     6732 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/virtuals.md
--rw-r--r--   0        0        0     3172 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm.md
--rw-r--r--   0        0        0     4100 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/patterns.md
--rw-r--r--   0        0        0    14161 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/pipeline.md
--rw-r--r--   0        0        0    15916 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/quickstart.md
--rw-r--r--   0        0        0     6082 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/request.md
--rw-r--r--   0        0        0     3378 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/response.md
--rw-r--r--   0        0        0    11727 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/routing.md
--rw-r--r--   0        0        0     2424 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/services.md
--rw-r--r--   0        0        0     4535 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/sessions.md
--rw-r--r--   0        0        0     6405 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/templates.md
--rw-r--r--   0        0        0     6776 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/testing.md
--rw-r--r--   0        0        0      440 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/tree.yml
--rw-r--r--   0        0        0    14840 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/tutorial.md
--rw-r--r--   0        0        0    16597 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/upgrading.md
--rw-r--r--   0        0        0    15878 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/validations.md
--rw-r--r--   0        0        0     2307 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/websocket.md
--rw-r--r--   0        0        0      386 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/__init__.py
--rw-r--r--   0        0        0      248 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/__main__.py
--rw-r--r--   0        0        0       22 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/__version__.py
--rw-r--r--   0        0        0    11242 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/_internal.py
--rw-r--r--   0        0        0     5633 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/_reloader.py
--rw-r--r--   0        0        0      771 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/_shortcuts.py
--rw-r--r--   0        0        0    27001 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/app.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/__init__.py
--rw-r--r--   0        0        0    15264 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/handlers.py
--rw-r--r--   0        0        0      220 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/helpers.py
--rw-r--r--   0        0        0      533 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/typing.py
--rw-r--r--   0        0        0     3064 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/workers.py
--rw-r--r--   0        0        0     8029 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/wrappers.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/__init__.py
--rw-r--r--   0        0        0     2437 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shBrushPython.js
--rw-r--r--   0        0        0     6204 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shCore.css
--rw-r--r--   0        0        0    16175 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shCore.js
--rw-r--r--   0        0        0     2499 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shTheme.css
--rw-r--r--   0        0        0      647 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/view.css
--rw-r--r--   0        0        0     4626 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/view.html
--rw-r--r--   0        0        0     1630 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/helpers.js
--rw-r--r--   0        0        0    89476 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/jquery.min.js
--rw-r--r--   0        0        0   137986 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/jquery.min.map
--rw-r--r--   0        0        0    18871 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/cache.py
--rw-r--r--   0        0        0    15186 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/cli.py
--rw-r--r--   0        0        0     2547 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/ctx.py
--rw-r--r--   0        0        0     8165 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/datastructures.py
--rw-r--r--   0        0        0     5076 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/debug.py
--rw-r--r--   0        0        0     3201 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/extensions.py
--rw-r--r--   0        0        0    25617 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/forms.py
--rw-r--r--   0        0        0     3095 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/helpers.py
--rw-r--r--   0        0        0     6435 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/html.py
--rw-r--r--   0        0        0     8750 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/http.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/language/__init__.py
--rw-r--r--   0        0        0     1096 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/language/helpers.py
--rw-r--r--   0        0        0      933 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/language/translator.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/libs/__init__.py
--rw-r--r--   0        0        0    25207 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/libs/contenttype.py
--rw-r--r--   0        0        0     3915 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/libs/portalocker.py
--rw-r--r--   0        0        0      925 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/locals.py
--rw-r--r--   0        0        0     3084 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/logger.py
--rw-r--r--   0        0        0      478 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/__init__.py
--rw-r--r--   0        0        0     2373 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/_patches.py
--rw-r--r--   0        0        0    13015 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/adapters.py
--rw-r--r--   0        0        0     3224 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/apis.py
--rw-r--r--   0        0        0     8857 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/base.py
--rw-r--r--   0        0        0    12058 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/connection.py
--rw-r--r--   0        0        0       80 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/engines/__init__.py
--rw-r--r--   0        0        0     5577 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/engines/postgres.py
--rw-r--r--   0        0        0     1191 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/engines/sqlite.py
--rw-r--r--   0        0        0      605 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/errors.py
--rw-r--r--   0        0        0     1677 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/geo.py
--rw-r--r--   0        0        0    18102 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/helpers.py
--rw-r--r--   0        0        0       62 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/__init__.py
--rw-r--r--   0        0        0     2892 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/base.py
--rw-r--r--   0        0        0    15289 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/commands.py
--rw-r--r--   0        0        0    14381 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/engine.py
--rw-r--r--   0        0        0     1058 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/exceptions.py
--rw-r--r--   0        0        0    21829 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/generation.py
--rw-r--r--   0        0        0     3636 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/helpers.py
--rw-r--r--   0        0        0      491 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/migration.tmpl
--rw-r--r--   0        0        0    23246 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/operations.py
--rw-r--r--   0        0        0    14902 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/revisions.py
--rw-r--r--   0        0        0    12034 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/scripts.py
--rw-r--r--   0        0        0     1150 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/utils.py
--rw-r--r--   0        0        0    46716 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/models.py
--rw-r--r--   0        0        0    57286 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/objects.py
--rw-r--r--   0        0        0     4208 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/transactions.py
--rw-r--r--   0        0        0      978 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/wrappers.py
--rw-r--r--   0        0        0      917 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/parsers.py
--rw-r--r--   0        0        0    12040 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/pipeline.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/__init__.py
--rw-r--r--   0        0        0     5303 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/dispatchers.py
--rw-r--r--   0        0        0     4112 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/response.py
--rw-r--r--   0        0        0    11518 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/router.py
--rw-r--r--   0        0        0     8479 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/routes.py
--rw-r--r--   0        0        0     7026 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/rules.py
--rw-r--r--   0        0        0     9704 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/urls.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/__init__.py
--rw-r--r--   0        0        0     9938 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/handlers.py
--rw-r--r--   0        0        0      878 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/helpers.py
--rw-r--r--   0        0        0     4338 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/wrappers.py
--rw-r--r--   0        0        0     5490 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/security.py
--rw-r--r--   0        0        0     2207 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/serializers.py
--rw-r--r--   0        0        0     1003 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/server.py
--rw-r--r--   0        0        0    11649 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/sessions.py
--rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/templating/__init__.py
--rw-r--r--   0        0        0     1843 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/templating/lexers.py
--rw-r--r--   0        0        0     1957 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/templating/templater.py
--rw-r--r--   0        0        0       37 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/__init__.py
--rw-r--r--   0        0        0    11877 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/client.py
--rw-r--r--   0        0        0    10674 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/env.py
--rw-r--r--   0        0        0    12272 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/helpers.py
--rw-r--r--   0        0        0    15936 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/urls.py
--rw-r--r--   0        0        0      125 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/tools/__init__.py
--rw-r--r--   0        0        0       52 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/tools/auth/__init__.py
--rw-r--r--   0        0        0     9035 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/tools/auth/apis.py
--rw-r--r--   0        0        0    19190 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/exposer.py
--rw-r--r--   0        0        0    13469 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/ext.py
--rw-r--r--   0        0        0     5270 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/forms.py
--rw-r--r--   0        0        0     7485 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/models.py
--rw-r--r--   0        0        0     1417 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/decorators.py
--rw-r--r--   0        0        0    10953 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/mailer.py
--rw-r--r--   0        0        0     1565 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/service.py
--rw-r--r--   0        0        0      355 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/typing.py
--rw-r--r--   0        0        0     5357 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/utils.py
--rw-r--r--   0        0        0    11554 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/__init__.py
--rw-r--r--   0        0        0     7636 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/basic.py
--rw-r--r--   0        0        0    31120 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/consist.py
--rw-r--r--   0        0        0    19038 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/helpers.py
--rw-r--r--   0        0        0     7367 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/inside.py
--rw-r--r--   0        0        0     4614 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/process.py
--rw-r--r--   0        0        0     2190 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/__init__.py
--rw-r--r--   0        0        0     2886 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/helpers.py
--rw-r--r--   0        0        0     3984 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/request.py
--rw-r--r--   0        0        0     1525 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/response.py
--rw-r--r--   0        0        0     1062 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/websocket.py
--rw-r--r--   0        0        0     2091 2023-05-19 11:27:14.013857 emmett-2.5.2/pyproject.toml
--rw-r--r--   0        0        0     1524 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/helpers.py
--rw-r--r--   0        0        0       46 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/languages/de.json
--rw-r--r--   0        0        0       49 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/languages/it.json
--rw-r--r--   0        0        0       69 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/languages/ru.json
--rw-r--r--   0        0        0      134 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/templates/auth/auth.html
--rw-r--r--   0        0        0      479 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/templates/layout.html
--rw-r--r--   0        0        0      153 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/templates/test.html
--rw-r--r--   0        0        0     8027 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_auth.py
--rw-r--r--   0        0        0     4658 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_cache.py
--rw-r--r--   0        0        0     1415 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_http.py
--rw-r--r--   0        0        0      861 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_logger.py
--rw-r--r--   0        0        0    11854 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_mailer.py
--rw-r--r--   0        0        0     8618 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_migrations.py
--rw-r--r--   0        0        0    33038 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm.py
--rw-r--r--   0        0        0      853 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_connections.py
--rw-r--r--   0        0        0    10074 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_gis.py
--rw-r--r--   0        0        0    22722 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_pks.py
--rw-r--r--   0        0        0     9863 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_row.py
--rw-r--r--   0        0        0     2958 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_transactions.py
--rw-r--r--   0        0        0    22478 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_pipeline.py
--rw-r--r--   0        0        0     8659 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_routing.py
--rw-r--r--   0        0        0     1475 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_session.py
--rw-r--r--   0        0        0     2705 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_templates.py
--rw-r--r--   0        0        0      622 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_translator.py
--rw-r--r--   0        0        0     2045 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_utils.py
--rw-r--r--   0        0        0    18633 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_validators.py
--rw-r--r--   0        0        0      822 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_wrappers.py
--rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 emmett-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0    14193 2023-06-22 12:43:38.962889 emmett-2.5.3/CHANGES.md
+-rw-r--r--   0        0        0     2074 2023-06-22 12:43:38.962889 emmett-2.5.3/LICENSE
+-rw-r--r--   0        0        0     2926 2023-06-22 12:43:38.962889 emmett-2.5.3/README.md
+-rw-r--r--   0        0        0     9917 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/app_and_modules.md
+-rw-r--r--   0        0        0    15873 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/auth.md
+-rw-r--r--   0        0        0    12150 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/caching.md
+-rw-r--r--   0        0        0     2613 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/cli.md
+-rw-r--r--   0        0        0     4481 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/debug_and_logging.md
+-rw-r--r--   0        0        0     3056 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/deployment.md
+-rw-r--r--   0        0        0     5295 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/extensions.md
+-rw-r--r--   0        0        0     5174 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/foreword.md
+-rw-r--r--   0        0        0     6493 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/forms.md
+-rw-r--r--   0        0        0     2105 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/installation.md
+-rw-r--r--   0        0        0     3596 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/languages.md
+-rw-r--r--   0        0        0     3087 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/mailer.md
+-rw-r--r--   0        0        0     9672 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/advanced.md
+-rw-r--r--   0        0        0    12917 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/callbacks.md
+-rw-r--r--   0        0        0     7060 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/connecting.md
+-rw-r--r--   0        0        0    20808 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/migrations.md
+-rw-r--r--   0        0        0    14034 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/models.md
+-rw-r--r--   0        0        0    29245 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/operations.md
+-rw-r--r--   0        0        0    27472 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/relations.md
+-rw-r--r--   0        0        0     5523 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/scopes.md
+-rw-r--r--   0        0        0     6732 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm/virtuals.md
+-rw-r--r--   0        0        0     3172 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/orm.md
+-rw-r--r--   0        0        0     4100 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/patterns.md
+-rw-r--r--   0        0        0    14161 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/pipeline.md
+-rw-r--r--   0        0        0    15916 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/quickstart.md
+-rw-r--r--   0        0        0     6082 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/request.md
+-rw-r--r--   0        0        0     3378 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/response.md
+-rw-r--r--   0        0        0    11727 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/routing.md
+-rw-r--r--   0        0        0     2424 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/services.md
+-rw-r--r--   0        0        0     4535 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/sessions.md
+-rw-r--r--   0        0        0     6405 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/templates.md
+-rw-r--r--   0        0        0     6776 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/testing.md
+-rw-r--r--   0        0        0      440 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/tree.yml
+-rw-r--r--   0        0        0    14840 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/tutorial.md
+-rw-r--r--   0        0        0    16597 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/upgrading.md
+-rw-r--r--   0        0        0    15878 2023-06-22 12:43:38.962889 emmett-2.5.3/docs/validations.md
+-rw-r--r--   0        0        0     2307 2023-06-22 12:43:38.966889 emmett-2.5.3/docs/websocket.md
+-rw-r--r--   0        0        0      386 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/__version__.py
+-rw-r--r--   0        0        0    11242 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/_internal.py
+-rw-r--r--   0        0        0     5633 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/_reloader.py
+-rw-r--r--   0        0        0      771 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/_shortcuts.py
+-rw-r--r--   0        0        0    27001 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/app.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/asgi/__init__.py
+-rw-r--r--   0        0        0    15264 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/asgi/handlers.py
+-rw-r--r--   0        0        0      220 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/asgi/helpers.py
+-rw-r--r--   0        0        0      533 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/asgi/typing.py
+-rw-r--r--   0        0        0     3064 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/asgi/workers.py
+-rw-r--r--   0        0        0     8029 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/asgi/wrappers.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/debug/__init__.py
+-rw-r--r--   0        0        0     2437 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/debug/shBrushPython.js
+-rw-r--r--   0        0        0     6204 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/debug/shCore.css
+-rw-r--r--   0        0        0    16175 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/debug/shCore.js
+-rw-r--r--   0        0        0     2499 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/debug/shTheme.css
+-rw-r--r--   0        0        0      647 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/debug/view.css
+-rw-r--r--   0        0        0     4626 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/debug/view.html
+-rw-r--r--   0        0        0     1630 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/helpers.js
+-rw-r--r--   0        0        0    89476 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/jquery.min.js
+-rw-r--r--   0        0        0   137986 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/assets/jquery.min.map
+-rw-r--r--   0        0        0    18871 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/cache.py
+-rw-r--r--   0        0        0    15318 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/cli.py
+-rw-r--r--   0        0        0     2547 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/ctx.py
+-rw-r--r--   0        0        0     8165 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/datastructures.py
+-rw-r--r--   0        0        0     5076 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/debug.py
+-rw-r--r--   0        0        0     3201 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/extensions.py
+-rw-r--r--   0        0        0    25679 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/forms.py
+-rw-r--r--   0        0        0     3095 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/helpers.py
+-rw-r--r--   0        0        0     6435 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/html.py
+-rw-r--r--   0        0        0    10598 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/http.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/language/__init__.py
+-rw-r--r--   0        0        0     1096 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/language/helpers.py
+-rw-r--r--   0        0        0      933 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/language/translator.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/libs/__init__.py
+-rw-r--r--   0        0        0    25207 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/libs/contenttype.py
+-rw-r--r--   0        0        0     3915 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/libs/portalocker.py
+-rw-r--r--   0        0        0      925 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/locals.py
+-rw-r--r--   0        0        0     3084 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/logger.py
+-rw-r--r--   0        0        0      478 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/orm/__init__.py
+-rw-r--r--   0        0        0     2373 2023-06-22 12:43:38.966889 emmett-2.5.3/emmett/orm/_patches.py
+-rw-r--r--   0        0        0    12979 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/adapters.py
+-rw-r--r--   0        0        0     3224 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/apis.py
+-rw-r--r--   0        0        0     8857 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/base.py
+-rw-r--r--   0        0        0    12058 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/connection.py
+-rw-r--r--   0        0        0       80 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/engines/__init__.py
+-rw-r--r--   0        0        0     5577 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/engines/postgres.py
+-rw-r--r--   0        0        0     1191 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/engines/sqlite.py
+-rw-r--r--   0        0        0      605 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/errors.py
+-rw-r--r--   0        0        0     1677 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/geo.py
+-rw-r--r--   0        0        0    18102 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/helpers.py
+-rw-r--r--   0        0        0       62 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/__init__.py
+-rw-r--r--   0        0        0     2892 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/base.py
+-rw-r--r--   0        0        0    15289 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/commands.py
+-rw-r--r--   0        0        0    14381 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/engine.py
+-rw-r--r--   0        0        0     1058 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/exceptions.py
+-rw-r--r--   0        0        0    21829 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/generation.py
+-rw-r--r--   0        0        0     3636 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/helpers.py
+-rw-r--r--   0        0        0      491 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/migration.tmpl
+-rw-r--r--   0        0        0    23246 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/operations.py
+-rw-r--r--   0        0        0    14902 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/revisions.py
+-rw-r--r--   0        0        0    12034 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/scripts.py
+-rw-r--r--   0        0        0     1150 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/migrations/utils.py
+-rw-r--r--   0        0        0    46716 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/models.py
+-rw-r--r--   0        0        0    57286 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/objects.py
+-rw-r--r--   0        0        0     4208 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/transactions.py
+-rw-r--r--   0        0        0      978 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/orm/wrappers.py
+-rw-r--r--   0        0        0      917 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/parsers.py
+-rw-r--r--   0        0        0    12040 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/pipeline.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/routing/__init__.py
+-rw-r--r--   0        0        0     5303 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/routing/dispatchers.py
+-rw-r--r--   0        0        0     4112 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/routing/response.py
+-rw-r--r--   0        0        0    11518 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/routing/router.py
+-rw-r--r--   0        0        0     8479 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/routing/routes.py
+-rw-r--r--   0        0        0     7026 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/routing/rules.py
+-rw-r--r--   0        0        0     9704 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/routing/urls.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/rsgi/__init__.py
+-rw-r--r--   0        0        0     9973 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/rsgi/handlers.py
+-rw-r--r--   0        0        0      878 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/rsgi/helpers.py
+-rw-r--r--   0        0        0     4338 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/rsgi/wrappers.py
+-rw-r--r--   0        0        0     5490 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/security.py
+-rw-r--r--   0        0        0     2207 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/serializers.py
+-rw-r--r--   0        0        0     1050 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/server.py
+-rw-r--r--   0        0        0    11649 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/sessions.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/templating/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/templating/lexers.py
+-rw-r--r--   0        0        0     1957 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/templating/templater.py
+-rw-r--r--   0        0        0       37 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/testing/__init__.py
+-rw-r--r--   0        0        0    11877 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/testing/client.py
+-rw-r--r--   0        0        0    10674 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/testing/env.py
+-rw-r--r--   0        0        0    12272 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/testing/helpers.py
+-rw-r--r--   0        0        0    15936 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/testing/urls.py
+-rw-r--r--   0        0        0      125 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/auth/__init__.py
+-rw-r--r--   0        0        0     9035 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/auth/apis.py
+-rw-r--r--   0        0        0    19190 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/auth/exposer.py
+-rw-r--r--   0        0        0    13469 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/auth/ext.py
+-rw-r--r--   0        0        0     5270 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/auth/forms.py
+-rw-r--r--   0        0        0     7485 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/auth/models.py
+-rw-r--r--   0        0        0     1417 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/decorators.py
+-rw-r--r--   0        0        0    10953 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/mailer.py
+-rw-r--r--   0        0        0     1565 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/tools/service.py
+-rw-r--r--   0        0        0      355 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/typing.py
+-rw-r--r--   0        0        0     5357 2023-06-22 12:43:38.970889 emmett-2.5.3/emmett/utils.py
+-rw-r--r--   0        0        0    11554 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/validators/__init__.py
+-rw-r--r--   0        0        0     7636 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/validators/basic.py
+-rw-r--r--   0        0        0    31120 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/validators/consist.py
+-rw-r--r--   0        0        0    19038 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/validators/helpers.py
+-rw-r--r--   0        0        0     7367 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/validators/inside.py
+-rw-r--r--   0        0        0     4614 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/validators/process.py
+-rw-r--r--   0        0        0     2190 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/wrappers/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/wrappers/helpers.py
+-rw-r--r--   0        0        0     4269 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/wrappers/request.py
+-rw-r--r--   0        0        0     1525 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/wrappers/response.py
+-rw-r--r--   0        0        0     1062 2023-06-22 12:43:38.974889 emmett-2.5.3/emmett/wrappers/websocket.py
+-rw-r--r--   0        0        0     2091 2023-06-22 12:43:38.974889 emmett-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1524 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/helpers.py
+-rw-r--r--   0        0        0       46 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/languages/de.json
+-rw-r--r--   0        0        0       49 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/languages/it.json
+-rw-r--r--   0        0        0       69 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/languages/ru.json
+-rw-r--r--   0        0        0      134 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/templates/auth/auth.html
+-rw-r--r--   0        0        0      479 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/templates/layout.html
+-rw-r--r--   0        0        0      153 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/templates/test.html
+-rw-r--r--   0        0        0     8027 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_auth.py
+-rw-r--r--   0        0        0     4658 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_cache.py
+-rw-r--r--   0        0        0     1415 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_http.py
+-rw-r--r--   0        0        0      861 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_logger.py
+-rw-r--r--   0        0        0    11854 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_mailer.py
+-rw-r--r--   0        0        0     8618 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_migrations.py
+-rw-r--r--   0        0        0    33038 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_orm.py
+-rw-r--r--   0        0        0      853 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_orm_connections.py
+-rw-r--r--   0        0        0    10074 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_orm_gis.py
+-rw-r--r--   0        0        0    22722 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_orm_pks.py
+-rw-r--r--   0        0        0     9863 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_orm_row.py
+-rw-r--r--   0        0        0     2958 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_orm_transactions.py
+-rw-r--r--   0        0        0    22478 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_pipeline.py
+-rw-r--r--   0        0        0     8659 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_routing.py
+-rw-r--r--   0        0        0     1475 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_session.py
+-rw-r--r--   0        0        0     2705 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_templates.py
+-rw-r--r--   0        0        0      622 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_translator.py
+-rw-r--r--   0        0        0     2045 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_utils.py
+-rw-r--r--   0        0        0    18633 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_validators.py
+-rw-r--r--   0        0        0      822 2023-06-22 12:43:38.974889 emmett-2.5.3/tests/test_wrappers.py
+-rw-r--r--   0        0        0     4780 1970-01-01 00:00:00.000000 emmett-2.5.3/PKG-INFO
```

### Comparing `emmett-2.5.2/CHANGES.md` & `emmett-2.5.3/CHANGES.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/LICENSE` & `emmett-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/README.md` & `emmett-2.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 app = App(__name__)
 app.config.db.uri = "postgres://user:password@localhost/foo"
 db = Database(app)
 db.define_models(Task)
 app.pipeline = [db.pipe]
 
 def is_authenticated():
-    return request.headers["Api-Key"] == "foobar"
+    return request.headers.get("api-key") == "foobar"
     
 def not_authorized():
     response.status = 401
     return {'error': 'not authorized'}
 
 @app.route(methods='get')
-@service.json
 @requires(is_authenticated, otherwise=not_authorized)
+@service.json
 async def todo():
     page = request.query_params.page or 1
     tasks = Task.where(
         lambda t: t.is_completed == False
     ).select(paginate=(page, 20))
     return {'tasks': tasks}
 ```
```

### Comparing `emmett-2.5.2/docs/app_and_modules.md` & `emmett-2.5.3/docs/app_and_modules.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/auth.md` & `emmett-2.5.3/docs/auth.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/caching.md` & `emmett-2.5.3/docs/caching.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/cli.md` & `emmett-2.5.3/docs/cli.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/debug_and_logging.md` & `emmett-2.5.3/docs/debug_and_logging.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/deployment.md` & `emmett-2.5.3/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/extensions.md` & `emmett-2.5.3/docs/extensions.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/foreword.md` & `emmett-2.5.3/docs/foreword.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/forms.md` & `emmett-2.5.3/docs/forms.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/installation.md` & `emmett-2.5.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/languages.md` & `emmett-2.5.3/docs/languages.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/mailer.md` & `emmett-2.5.3/docs/mailer.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/advanced.md` & `emmett-2.5.3/docs/orm/advanced.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/callbacks.md` & `emmett-2.5.3/docs/orm/callbacks.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/connecting.md` & `emmett-2.5.3/docs/orm/connecting.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/migrations.md` & `emmett-2.5.3/docs/orm/migrations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/models.md` & `emmett-2.5.3/docs/orm/models.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/operations.md` & `emmett-2.5.3/docs/orm/operations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/relations.md` & `emmett-2.5.3/docs/orm/relations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/scopes.md` & `emmett-2.5.3/docs/orm/scopes.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm/virtuals.md` & `emmett-2.5.3/docs/orm/virtuals.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/orm.md` & `emmett-2.5.3/docs/orm.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/patterns.md` & `emmett-2.5.3/docs/patterns.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/pipeline.md` & `emmett-2.5.3/docs/pipeline.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/quickstart.md` & `emmett-2.5.3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/request.md` & `emmett-2.5.3/docs/request.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/response.md` & `emmett-2.5.3/docs/response.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/routing.md` & `emmett-2.5.3/docs/routing.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/services.md` & `emmett-2.5.3/docs/services.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/sessions.md` & `emmett-2.5.3/docs/sessions.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/templates.md` & `emmett-2.5.3/docs/templates.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/testing.md` & `emmett-2.5.3/docs/testing.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/tutorial.md` & `emmett-2.5.3/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/upgrading.md` & `emmett-2.5.3/docs/upgrading.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/validations.md` & `emmett-2.5.3/docs/validations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/docs/websocket.md` & `emmett-2.5.3/docs/websocket.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/_internal.py` & `emmett-2.5.3/emmett/_internal.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/_reloader.py` & `emmett-2.5.3/emmett/_reloader.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/_shortcuts.py` & `emmett-2.5.3/emmett/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/app.py` & `emmett-2.5.3/emmett/app.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/asgi/handlers.py` & `emmett-2.5.3/emmett/asgi/handlers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/asgi/typing.py` & `emmett-2.5.3/emmett/asgi/typing.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/asgi/workers.py` & `emmett-2.5.3/emmett/asgi/workers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/asgi/wrappers.py` & `emmett-2.5.3/emmett/asgi/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/debug/shBrushPython.js` & `emmett-2.5.3/emmett/assets/debug/shBrushPython.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/debug/shCore.css` & `emmett-2.5.3/emmett/assets/debug/shCore.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/debug/shCore.js` & `emmett-2.5.3/emmett/assets/debug/shCore.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/debug/shTheme.css` & `emmett-2.5.3/emmett/assets/debug/shTheme.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/debug/view.css` & `emmett-2.5.3/emmett/assets/debug/view.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/debug/view.html` & `emmett-2.5.3/emmett/assets/debug/view.html`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/helpers.js` & `emmett-2.5.3/emmett/assets/helpers.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/jquery.min.js` & `emmett-2.5.3/emmett/assets/jquery.min.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/assets/jquery.min.map` & `emmett-2.5.3/emmett/assets/jquery.min.map`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/cache.py` & `emmett-2.5.3/emmett/cache.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/cli.py` & `emmett-2.5.3/emmett/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,35 +317,39 @@
 @click.option(
     '--ws/--no-ws', is_flag=True, default=True,
     help='Enable websockets support.')
 @click.option(
     '--loop', type=click.Choice(['auto', 'asyncio', 'uvloop']), default='auto',
     help='Event loop implementation.')
 @click.option(
+    '--opt/--no-opt', is_flag=True, default=False,
+    help='Enable loop optimizations.')
+@click.option(
     '--log-level', type=click.Choice(LOG_LEVELS.keys()), default='info',
     help='Logging level.')
 @click.option(
     '--backlog', type=int, default=2048,
     help='Maximum number of connections to hold in backlog')
 @click.option(
     '--ssl-certfile', type=str, default=None, help='SSL certificate file')
 @click.option(
     '--ssl-keyfile', type=str, default=None, help='SSL key file')
 @pass_script_info
 def serve_command(
-    info, host, port, workers, threads, threading_mode, interface, ws, loop, log_level,
-    backlog, ssl_certfile, ssl_keyfile
+    info, host, port, workers, threads, threading_mode, interface, ws, loop, opt,
+    log_level, backlog, ssl_certfile, ssl_keyfile
 ):
     app_target = info._get_import_name()
     sgi_run(
         interface,
         app_target,
         host=host,
         port=port,
         loop=loop,
+        loop_opt=opt,
         log_level=log_level,
         workers=workers,
         threads=threads,
         threading_mode=threading_mode,
         backlog=backlog,
         enable_websockets=ws,
         ssl_certfile=ssl_certfile,
```

### Comparing `emmett-2.5.2/emmett/ctx.py` & `emmett-2.5.3/emmett/ctx.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/datastructures.py` & `emmett-2.5.3/emmett/datastructures.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/debug.py` & `emmett-2.5.3/emmett/debug.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/extensions.py` & `emmett-2.5.3/emmett/extensions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/forms.py` & `emmett-2.5.3/emmett/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,18 +543,18 @@
             ],
             _name=field.name,
             _class=_class,
             _multiple="multiple",
             _id=_id or field.name
         )
 
-    #: TO-DO
-    #@staticmethod
-    #def widget_list(attr, field, value, _class="", _id=None):
-    #    return ""
+    @staticmethod
+    def widget_list(field, value):
+        options, _ = FormStyle._field_options(field)
+        return FormStyle.widget_multiple(None, field, value, options)
 
     @staticmethod
     def widget_upload(attr, field, value, _class="upload", _id=None):
         def is_image(value):
             return value.split(".")[-1].lower() in ["gif", "png", "jpg", "jpeg", "bmp"]
 
         def _coerce_value(value):
```

### Comparing `emmett-2.5.2/emmett/helpers.py` & `emmett-2.5.3/emmett/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/html.py` & `emmett-2.5.3/emmett/html.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/http.py` & `emmett-2.5.3/emmett/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import errno
 import os
 import stat
 
 from email.utils import formatdate
 from hashlib import md5
-from typing import Any, BinaryIO, Dict, Generator, Tuple
+from typing import Any, AsyncIterable, BinaryIO, Dict, Generator, Iterable, Tuple
 
 from granian.rsgi import HTTPProtocol
 
 from ._internal import loop_open_file
 from .ctx import current
 from .libs.contenttype import contenttype
 
@@ -280,20 +280,83 @@
         self._headers.update(self._get_io_headers())
         await self._send_headers(send)
         await self._send_body(send)
 
     async def _send_body(self, send):
         more_body = True
         while more_body:
-            chunk = await self.io_stream.read(self.chunk_size)
+            chunk = self.io_stream.read(self.chunk_size)
             more_body = len(chunk) == self.chunk_size
             await send({
                 'type': 'http.response.body',
                 'body': chunk,
                 'more_body': more_body,
             })
 
+    def rsgi(self, protocol: HTTPProtocol):
+        protocol.response_bytes(
+            self.status_code,
+            list(self.rsgi_headers),
+            self.io_stream.read()
+        )
+
+
+class HTTPIter(HTTPResponse):
+    def __init__(
+        self,
+        iter: Iterable[bytes],
+        headers: Dict[str, str] = {},
+        cookies: Dict[str, Any] = {}
+    ):
+        super().__init__(200, headers=headers, cookies=cookies)
+        self.iter = iter
+
+    async def _send_body(self, send):
+        for chunk in self.iter:
+            await send({
+                'type': 'http.response.body',
+                'body': chunk,
+                'more_body': True
+            })
+        await send({'type': 'http.response.body', 'body': b'', 'more_body': False})
+
+    async def rsgi(self, protocol: HTTPProtocol):
+        trx = protocol.response_stream(
+            self.status_code,
+            list(self.rsgi_headers)
+        )
+        for chunk in self.iter:
+            await trx.send_bytes(chunk)
+
+
+class HTTPAiter(HTTPResponse):
+    def __init__(
+        self,
+        iter: AsyncIterable[bytes],
+        headers: Dict[str, str] = {},
+        cookies: Dict[str, Any] = {}
+    ):
+        super().__init__(200, headers=headers, cookies=cookies)
+        self.iter = iter
+
+    async def _send_body(self, send):
+        async for chunk in self.iter:
+            await send({
+                'type': 'http.response.body',
+                'body': chunk,
+                'more_body': True
+            })
+        await send({'type': 'http.response.body', 'body': b'', 'more_body': False})
+
+    async def rsgi(self, protocol: HTTPProtocol):
+        trx = protocol.response_stream(
+            self.status_code,
+            list(self.rsgi_headers)
+        )
+        async for chunk in self.iter:
+            await trx.send_bytes(chunk)
+
 
 def redirect(location: str, status_code: int = 303):
     response = current.response
     response.status = status_code
     raise HTTPRedirect(status_code, location, response.cookies)
```

### Comparing `emmett-2.5.2/emmett/language/helpers.py` & `emmett-2.5.3/emmett/language/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/language/translator.py` & `emmett-2.5.3/emmett/language/translator.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/libs/contenttype.py` & `emmett-2.5.3/emmett/libs/contenttype.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/libs/portalocker.py` & `emmett-2.5.3/emmett/libs/portalocker.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/locals.py` & `emmett-2.5.3/emmett/locals.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/logger.py` & `emmett-2.5.3/emmett/logger.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/_patches.py` & `emmett-2.5.3/emmett/orm/_patches.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/adapters.py` & `emmett-2.5.3/emmett/orm/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     :license: BSD-3-Clause
 """
 
 import sys
 
 from functools import wraps
 
-from pydal.adapters import adapters
 from pydal.adapters.base import SQLAdapter
 from pydal.adapters.mssql import (
     MSSQL1,
     MSSQL3,
     MSSQL4,
     MSSQL1N,
     MSSQL3N,
```

### Comparing `emmett-2.5.2/emmett/orm/apis.py` & `emmett-2.5.3/emmett/orm/apis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/base.py` & `emmett-2.5.3/emmett/orm/base.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/connection.py` & `emmett-2.5.3/emmett/orm/connection.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/engines/postgres.py` & `emmett-2.5.3/emmett/orm/engines/postgres.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/engines/sqlite.py` & `emmett-2.5.3/emmett/orm/engines/sqlite.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/errors.py` & `emmett-2.5.3/emmett/orm/errors.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/geo.py` & `emmett-2.5.3/emmett/orm/geo.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/helpers.py` & `emmett-2.5.3/emmett/orm/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/base.py` & `emmett-2.5.3/emmett/orm/migrations/base.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/commands.py` & `emmett-2.5.3/emmett/orm/migrations/commands.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/engine.py` & `emmett-2.5.3/emmett/orm/migrations/engine.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/exceptions.py` & `emmett-2.5.3/emmett/orm/migrations/exceptions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/generation.py` & `emmett-2.5.3/emmett/orm/migrations/generation.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/helpers.py` & `emmett-2.5.3/emmett/orm/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/operations.py` & `emmett-2.5.3/emmett/orm/migrations/operations.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/revisions.py` & `emmett-2.5.3/emmett/orm/migrations/revisions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/scripts.py` & `emmett-2.5.3/emmett/orm/migrations/scripts.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/migrations/utils.py` & `emmett-2.5.3/emmett/orm/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/models.py` & `emmett-2.5.3/emmett/orm/models.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/objects.py` & `emmett-2.5.3/emmett/orm/objects.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/transactions.py` & `emmett-2.5.3/emmett/orm/transactions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/orm/wrappers.py` & `emmett-2.5.3/emmett/orm/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/parsers.py` & `emmett-2.5.3/emmett/parsers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/pipeline.py` & `emmett-2.5.3/emmett/pipeline.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/routing/dispatchers.py` & `emmett-2.5.3/emmett/routing/dispatchers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/routing/response.py` & `emmett-2.5.3/emmett/routing/response.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/routing/router.py` & `emmett-2.5.3/emmett/routing/router.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/routing/routes.py` & `emmett-2.5.3/emmett/routing/routes.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/routing/rules.py` & `emmett-2.5.3/emmett/routing/rules.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/routing/urls.py` & `emmett-2.5.3/emmett/routing/urls.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/rsgi/handlers.py` & `emmett-2.5.3/emmett/rsgi/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,16 @@
     ):
         try:
             http = await self.pre_handler(scope, protocol, scope.path)
         except asyncio.TimeoutError:
             self.app.log.warn(
                 f"Timeout sending response: ({scope.path})"
             )
-        http.rsgi(protocol)
+        if coro := http.rsgi(protocol):
+            await coro
 
     @cachedprop
     def error_handler(self) -> Callable[[], Awaitable[str]]:
         return (
             self._debug_handler if self.app.debug else self.exception_handler
         )
```

### Comparing `emmett-2.5.2/emmett/rsgi/helpers.py` & `emmett-2.5.3/emmett/rsgi/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/rsgi/wrappers.py` & `emmett-2.5.3/emmett/rsgi/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/security.py` & `emmett-2.5.3/emmett/security.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/serializers.py` & `emmett-2.5.3/emmett/serializers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/server.py` & `emmett-2.5.3/emmett/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 def run(
     interface,
     app,
     host='127.0.0.1',
     port=8000,
     loop='auto',
+    loop_opt=False,
     log_level=None,
     workers=1,
     threads=1,
     threading_mode='workers',
     backlog=1024,
     enable_websockets=True,
     ssl_certfile: Optional[str] = None,
@@ -36,14 +37,15 @@
         port=port,
         interface=interface,
         workers=workers,
         threads=threads,
         pthreads=threads,
         threading_mode=threading_mode,
         loop=loop,
+        loop_opt=loop_opt,
         websockets=enable_websockets,
         backlog=backlog,
         log_level=log_level,
         ssl_cert=ssl_certfile,
         ssl_key=ssl_keyfile
     )
     runner.serve()
```

### Comparing `emmett-2.5.2/emmett/sessions.py` & `emmett-2.5.3/emmett/sessions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/templating/lexers.py` & `emmett-2.5.3/emmett/templating/lexers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/templating/templater.py` & `emmett-2.5.3/emmett/templating/templater.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/testing/client.py` & `emmett-2.5.3/emmett/testing/client.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/testing/env.py` & `emmett-2.5.3/emmett/testing/env.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/testing/helpers.py` & `emmett-2.5.3/emmett/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/testing/urls.py` & `emmett-2.5.3/emmett/testing/urls.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/auth/apis.py` & `emmett-2.5.3/emmett/tools/auth/apis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/auth/exposer.py` & `emmett-2.5.3/emmett/tools/auth/exposer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/auth/ext.py` & `emmett-2.5.3/emmett/tools/auth/ext.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/auth/forms.py` & `emmett-2.5.3/emmett/tools/auth/forms.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/auth/models.py` & `emmett-2.5.3/emmett/tools/auth/models.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/decorators.py` & `emmett-2.5.3/emmett/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/mailer.py` & `emmett-2.5.3/emmett/tools/mailer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/tools/service.py` & `emmett-2.5.3/emmett/tools/service.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/utils.py` & `emmett-2.5.3/emmett/utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/validators/__init__.py` & `emmett-2.5.3/emmett/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/validators/basic.py` & `emmett-2.5.3/emmett/validators/basic.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/validators/consist.py` & `emmett-2.5.3/emmett/validators/consist.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/validators/helpers.py` & `emmett-2.5.3/emmett/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/validators/inside.py` & `emmett-2.5.3/emmett/validators/inside.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/validators/process.py` & `emmett-2.5.3/emmett/validators/process.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/wrappers/__init__.py` & `emmett-2.5.3/emmett/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/wrappers/helpers.py` & `emmett-2.5.3/emmett/wrappers/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/wrappers/request.py` & `emmett-2.5.3/emmett/wrappers/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,43 +88,51 @@
             rv[key] = values
         return rv, sdict()
 
     @property
     def _multipart_headers(self):
         return self.headers
 
+    @staticmethod
+    def _file_param_from_field(field):
+        return FileStorage(
+            BytesIO(field.file.read()),
+            field.filename,
+            field.name,
+            field.type,
+            field.headers
+        )
+
     def _load_params_form_multipart(self, data):
         params, files = sdict(), sdict()
         field_storage = FieldStorage(
             BytesIO(data),
             headers=self._multipart_headers,
             environ={'REQUEST_METHOD': self.method},
             keep_blank_values=True
         )
         for key in field_storage:
             field = field_storage[key]
             if isinstance(field, list):
                 if len(field) > 1:
-                    params[key] = []
-                    for element in field:
-                        params[key].append(element.value)
+                    pvalues, fvalues = [], []
+                    for item in field:
+                        if item.filename is not None:
+                            fvalues.append(self._file_param_from_field(item))
+                        else:
+                            pvalues.append(item.value)
+                    if pvalues:
+                        params[key] = pvalues
+                    if fvalues:
+                        files[key] = fvalues
+                    continue
                 else:
-                    params[key] = field[0].value
-            elif (
-                isinstance(field, FieldStorage) and
-                field.filename is not None
-            ):
-                files[key] = FileStorage(
-                    BytesIO(field.file.read()),
-                    field.filename,
-                    field.name,
-                    field.type,
-                    field.headers
-                )
-                continue
+                   field = field[0]
+            if field.filename is not None:
+                files[key] = self._file_param_from_field(field)
             else:
                 params[key] = field.value
         return params, files
 
     _params_loaders = {
         'application/json': _load_params_json,
         'application/x-www-form-urlencoded': _load_params_form_urlencoded,
```

### Comparing `emmett-2.5.2/emmett/wrappers/response.py` & `emmett-2.5.3/emmett/wrappers/response.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/emmett/wrappers/websocket.py` & `emmett-2.5.3/emmett/wrappers/websocket.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/pyproject.toml` & `emmett-2.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett"
-version = "2.5.2"
+version = "2.5.3"
 description = "The web framework for inventors"
 authors = ["Giovanni Barillari <gi0baro@d4net.org>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://emmett.sh"
 repository = "https://github.com/emmett-framework/emmett"
@@ -39,15 +39,15 @@
 
 [tool.poetry.scripts]
 emmett = "emmett.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = ">=6.0"
-granian = "~0.4.2"
+granian = "~0.5.0"
 emmett-crypto = "~0.3"
 pendulum = "~2.1.2"
 pyDAL = "17.3"
 python-rapidjson = "^1.0"
 pyyaml = "^6.0"
 renoir = "^1.6"
 severus = "^1.1"
```

### Comparing `emmett-2.5.2/tests/helpers.py` & `emmett-2.5.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_auth.py` & `emmett-2.5.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_cache.py` & `emmett-2.5.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_http.py` & `emmett-2.5.3/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_logger.py` & `emmett-2.5.3/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_mailer.py` & `emmett-2.5.3/tests/test_mailer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_migrations.py` & `emmett-2.5.3/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_orm.py` & `emmett-2.5.3/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_orm_connections.py` & `emmett-2.5.3/tests/test_orm_connections.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_orm_gis.py` & `emmett-2.5.3/tests/test_orm_gis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_orm_pks.py` & `emmett-2.5.3/tests/test_orm_pks.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_orm_row.py` & `emmett-2.5.3/tests/test_orm_row.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_orm_transactions.py` & `emmett-2.5.3/tests/test_orm_transactions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_pipeline.py` & `emmett-2.5.3/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_routing.py` & `emmett-2.5.3/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_session.py` & `emmett-2.5.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_templates.py` & `emmett-2.5.3/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_translator.py` & `emmett-2.5.3/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_utils.py` & `emmett-2.5.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_validators.py` & `emmett-2.5.3/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/tests/test_wrappers.py` & `emmett-2.5.3/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.2/PKG-INFO` & `emmett-2.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett
-Version: 2.5.2
+Version: 2.5.3
 Summary: The web framework for inventors
 Home-page: https://emmett.sh
 License: BSD-3-Clause
 Keywords: web,asyncio
 Author: Giovanni Barillari
 Author-email: gi0baro@d4net.org
 Requires-Python: >=3.8,<4.0
@@ -15,26 +15,21 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: orjson
 Provides-Extra: uvicorn
 Requires-Dist: click (>=6.0)
 Requires-Dist: emmett-crypto (>=0.3,<0.4)
-Requires-Dist: granian (>=0.4.2,<0.5.0)
+Requires-Dist: granian (>=0.5.0,<0.6.0)
 Requires-Dist: h11 (>=0.12.0) ; extra == "uvicorn"
 Requires-Dist: httptools (>=0.5.0,<0.6.0) ; (sys_platform != "win32") and (extra == "uvicorn")
 Requires-Dist: orjson (>=3.8,<3.9) ; extra == "orjson"
 Requires-Dist: pendulum (>=2.1.2,<2.2.0)
 Requires-Dist: pyDAL (==17.3)
 Requires-Dist: python-rapidjson (>=1.0,<2.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
@@ -66,23 +61,23 @@
 app = App(__name__)
 app.config.db.uri = "postgres://user:password@localhost/foo"
 db = Database(app)
 db.define_models(Task)
 app.pipeline = [db.pipe]
 
 def is_authenticated():
-    return request.headers["Api-Key"] == "foobar"
+    return request.headers.get("api-key") == "foobar"
     
 def not_authorized():
     response.status = 401
     return {'error': 'not authorized'}
 
 @app.route(methods='get')
-@service.json
 @requires(is_authenticated, otherwise=not_authorized)
+@service.json
 async def todo():
     page = request.query_params.page or 1
     tasks = Task.where(
         lambda t: t.is_completed == False
     ).select(paginate=(page, 20))
     return {'tasks': tasks}
 ```
```


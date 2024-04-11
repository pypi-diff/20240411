# Comparing `tmp/openbb_nightly-4.1.6.dev202404090009.tar.gz` & `tmp/openbb_nightly-4.1.6.dev202404100009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.6.dev202404090009.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.6.dev202404100009.tar", max compression
```

## Comparing `openbb_nightly-4.1.6.dev202404090009.tar` & `openbb_nightly-4.1.6.dev202404100009.tar`

### file list

```diff
@@ -1,769 +1,769 @@
--rw-r--r--   0        0        0     6818 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/README.md
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1945 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7196 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    17435 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2525 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5312 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2474 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2691 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8333 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2137 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      859 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2047 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      239 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       52 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      428 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      177 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      321 2024-04-09 00:09:39.299227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0      906 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      346 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3864 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      808 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/custom_parameter.py
--rw-r--r--   0        0        0      435 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2233 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1912 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/fast_api_settings.py
--rw-r--r--   0        0        0     1940 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/hub/features_keys.py
--rw-r--r--   0        0        0      561 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      472 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     4694 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9866 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1418 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      450 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0       92 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     3898 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    17912 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    24767 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2632 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10218 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3443 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3025 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7759 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2024 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1542 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1685 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    62645 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3067 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     1639 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5959 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2316 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2581 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     9401 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0      630 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1288 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     1591 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-04-09 00:09:39.303227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      423 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1750 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      888 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      768 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     2390 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6153 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-04-09 00:09:39.307227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3083 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3474 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     4909 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9293 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.311227 openbb_nightly-4.1.6.dev202404090009/core/openbb_core/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3844 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.315227 openbb_nightly-4.1.6.dev202404090009/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4036 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0     9735 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1742 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-04-09 00:09:39.319227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2326 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1109 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5811 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3487 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     3832 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3769 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6060 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4082 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.323227 openbb_nightly-4.1.6.dev202404090009/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8610 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14280 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1313 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10975 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1885 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4204 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16751 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    57458 2024-04-09 00:09:39.327227 openbb_nightly-4.1.6.dev202404090009/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0     7652 2024-04-09 00:09:39.331227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-04-09 00:09:39.331227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    16542 2024-04-09 00:09:39.331227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.331227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-04-09 00:09:39.331227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-04-09 00:09:39.347227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17390 2024-04-09 00:09:39.347227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-04-09 00:09:39.347227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.347227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     7156 2024-04-09 00:09:39.347227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2422 2024-04-09 00:09:39.347227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58414 2024-04-09 00:09:39.347227 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228603 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7101 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12351 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8398 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    18829 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3240 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5661 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6817 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3510 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    22181 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1379 2024-04-09 00:09:39.371228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   857302 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2252 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0     3666 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0     3204 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0    23603 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0      600 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0     1440 2024-04-09 00:09:39.375228 openbb_nightly-4.1.6.dev202404090009/openbb/__init__.py
--rw-r--r--   0        0        0  1185810 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/assets/reference.json
--rw-r--r--   0        0        0     2794 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/__extensions__.py
--rw-r--r--   0        0        0       50 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/crypto.py
--rw-r--r--   0        0        0     6589 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    11777 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/currency.py
--rw-r--r--   0        0        0     6481 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12160 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    53423 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/economy.py
--rw-r--r--   0        0        0    12674 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27673 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity.py
--rw-r--r--   0        0        0    18754 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2869 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    26106 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    39105 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   169108 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30667 2024-04-09 00:09:39.379228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26819 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3567 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    74985 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/etf.py
--rw-r--r--   0        0        0     4649 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    20027 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7155 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26900 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    11204 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11919 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/index.py
--rw-r--r--   0        0        0    15535 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/regulators.py
--rw-r--r--   0        0        0    16562 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/package/regulators_sec.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/openbb/py.typed
--rw-r--r--   0        0        0     1106 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12446 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2516 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      877 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    14906 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9745 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.383228 openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      779 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3829 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     1779 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2154 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6469 2024-04-09 00:09:39.387228 openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      895 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-04-09 00:09:39.395228 openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      716 2024-04-09 00:09:39.443229 openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-04-09 00:09:39.443229 openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-04-09 00:09:39.443229 openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-04-09 00:09:39.443229 openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      538 2024-04-09 00:09:39.451229 openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-09 00:09:39.451229 openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-04-09 00:09:39.451229 openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-04-09 00:09:39.451229 openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5360 2024-04-09 00:09:39.451229 openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1005 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9574 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.507230 openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     8255 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6022 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5202 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6763 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2774 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5050 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2064 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3903 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     5922 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3131 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3270 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-04-09 00:09:39.511230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.515230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.515230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-09 00:09:39.515230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4243 2024-04-09 00:09:39.515230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.515230 openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     3126 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6656 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-04-09 00:09:39.535230 openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      988 2024-04-09 00:09:39.539230 openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-04-09 00:09:39.539230 openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-09 00:09:39.539230 openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5221 2024-04-09 00:09:39.539230 openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.539230 openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-04-09 00:09:39.539230 openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     5393 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3273 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2377 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7025 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8414 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9691 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     4829 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3328 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8829 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6510 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2550 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-04-09 00:09:39.543231 openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     1840 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3954 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6262 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     5969 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2173 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5090 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-04-09 00:09:39.555231 openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      981 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8668 2024-04-09 00:09:39.559231 openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2100 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6130 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6054 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7020 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     5973 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3618 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3690 2024-04-09 00:09:39.563231 openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1562 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8277 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2617 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13834 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7410 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.579231 openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      512 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      677 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1120 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-09 00:09:39.671233 openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3319 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5170 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4373 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8830 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5446 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12441 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4439 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3055 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10268 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6055 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5986 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-04-09 00:09:39.683233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38297 2024-04-09 00:09:39.687233 openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1241 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6568 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9162 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10222 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-09 00:09:39.783234 openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      440 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4529 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4567 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3636 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1044 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4232 2024-04-09 00:09:39.787234 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     1935 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5722 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10040 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4230 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6639 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-04-09 00:09:39.791235 openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     6884 2024-04-09 00:09:55.127482 openbb_nightly-4.1.6.dev202404090009/pyproject.toml
--rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404090009/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/README.md
+-rw-r--r--   0        0        0       19 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7196 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    17483 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1035 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3875 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      856 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/custom_parameter.py
+-rw-r--r--   0        0        0      502 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2233 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1912 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/fast_api_settings.py
+-rw-r--r--   0        0        0     2032 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/features_keys.py
+-rw-r--r--   0        0        0      694 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      542 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     4806 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9866 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1418 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0       37 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     3898 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    17912 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    24789 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10256 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3484 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7759 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2058 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1685 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    62954 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2224 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1368 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2581 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     9401 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0      630 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1288 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     1591 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      423 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1750 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      888 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      768 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     2390 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3083 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3474 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9293 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/py.typed
+-rw-r--r--   0        0        0       34 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0       31 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3848 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0       32 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0     9797 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6060 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0       29 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0       35 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16765 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    57458 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0     9791 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    16542 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17442 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     7188 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58384 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228603 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12351 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0     8398 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    18829 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3299 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5696 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6876 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3546 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    22283 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0     3666 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0     3204 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0    23603 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0     1440 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/openbb/__init__.py
+-rw-r--r--   0        0        0  1186310 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2794 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0       50 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6589 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    11777 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/currency.py
+-rw-r--r--   0        0        0     6481 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12160 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    53423 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/economy.py
+-rw-r--r--   0        0        0    12674 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27673 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity.py
+-rw-r--r--   0        0        0    18754 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2869 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    26106 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    39105 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   169108 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30667 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26819 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3567 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    75052 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/etf.py
+-rw-r--r--   0        0        0     4649 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    20027 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7155 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26900 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    11204 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11919 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/index.py
+-rw-r--r--   0        0        0    15535 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/regulators.py
+-rw-r--r--   0        0        0    16562 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/regulators_sec.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/py.typed
+-rw-r--r--   0        0        0     1106 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12452 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      877 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    14934 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9745 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     1779 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4725 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     5698 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-04-10 00:09:21.490668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      895 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      716 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3510 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      538 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1005 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9573 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     8255 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6022 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5202 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6763 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2774 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5050 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2064 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3903 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     5922 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3131 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3270 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     3126 2024-04-10 00:09:21.630666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-04-10 00:09:21.630666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-04-10 00:09:21.630666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6338 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6656 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      988 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5269 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     5393 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22983 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     3273 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     8675 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2376 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7321 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8417 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9694 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5090 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3357 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8829 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6513 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     2550 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     1840 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6262 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5090 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      981 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2100 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     6961 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6130 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6054 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6125 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     7020 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     5973 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3618 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1562 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0     8328 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     2615 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2720 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    32406 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2754 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2079 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2790 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3009 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1714 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    13896 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7434 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      512 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1120 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3651 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5295 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4662 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5323 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3319 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5162 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4647 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8843 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5455 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12451 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10325 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5986 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5133 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1241 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6568 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9162 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10264 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      440 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     4606 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1044 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4232 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     1978 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5722 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10040 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4230 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6639 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     6884 2024-04-10 00:09:31.614510 openbb_nightly-4.1.6.dev202404100009/pyproject.toml
+-rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404100009/PKG-INFO
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/README.md` & `openbb_nightly-4.1.6.dev202404100009/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/app_loader.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/app_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/auth/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""User authentication."""
+
 import secrets
 from typing import Optional
 
 from fastapi import Depends, HTTPException, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from openbb_core.app.model.user_settings import UserSettings
 from openbb_core.app.service.user_service import UserService
@@ -11,15 +13,14 @@
 security = HTTPBasic() if Env().API_AUTH else lambda: None
 
 
 async def authenticate_user(
     credentials: Annotated[Optional[HTTPBasicCredentials], Depends(security)]
 ):
     """Authenticate the user."""
-
     if credentials:
         username = Env().API_USERNAME
         password = Env().API_PASSWORD
 
         is_correct_username = False
         is_correct_password = False
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/command_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     def __init__(
         self,
         command_map: CommandMap,
         route: str,
         system_settings: SystemSettings,
         user_settings: UserSettings,
     ) -> None:
+        """Initialize the execution context."""
         self.command_map = command_map
         self.route = route
         self.system_settings = system_settings
         self.user_settings = user_settings
 
 
 class ParametersBuilder:
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/deprecation.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     def __init__(
         self,
         message: str,
         *args: object,
         since: Optional[Tuple[int, int]] = None,
         expected_removal: Optional[Tuple[int, int]] = None,
     ) -> None:
+        """Initialize the warning."""
         super().__init__(message, *args)
         self.message = message.rstrip(".")
         self.since = since or get_major_minor(VERSION)
         self.expected_removal = expected_removal or (self.since[0] + 1, 0)
         self.long_message = (
             f"{self.message}. Deprecated in OpenBB Platform V{self.since[0]}.{self.since[1]}"
             f" to be removed in V{self.expected_removal[0]}.{self.expected_removal[1]}."
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,167 +1,179 @@
-# IMPORTATION STANDARD
+"""Logging Formatter that includes formatting of Exceptions."""
+
 import logging
 import re
 from copy import deepcopy
 from pathlib import Path
 
-# IMPORTATION THIRDPARTY
-# IMPORTATION INTERNAL
 from openbb_core.app.logs.models.logging_settings import LoggingSettings
 
 
 class FormatterWithExceptions(logging.Formatter):
-    """Logging Formatter that includes formatting of Exceptions"""
+    """Logging Formatter that includes formatting of Exceptions."""
 
     DATEFORMAT = "%Y-%m-%dT%H:%M:%S%z"
     LOGFORMAT = "%(asctime)s|%(name)s|%(funcName)s|%(lineno)s|%(message)s"
     LOGPREFIXFORMAT = (
         "%(levelname)s|%(appName)s|%(commitHash)s|%(appId)s|%(sessionId)s|%(userId)s|"
     )
 
     @staticmethod
     def calculate_level_name(record: logging.LogRecord) -> str:
+        """Calculate the level name of the log record."""
         if record.exc_text:
             level_name = "X"
         elif record.levelname:
             level_name = record.levelname[0]
         else:
             level_name = "U"
 
         return level_name
 
     @staticmethod
     def extract_log_extra(record: logging.LogRecord):
+        """Extract extra log information from the record."""
         log_extra = dict()
 
         if hasattr(record, "func_name_override"):
             record.funcName = record.func_name_override  # type: ignore
             record.lineno = 0
 
         if hasattr(record, "session_id"):
             log_extra["sessionId"] = record.session_id  # type: ignore
 
         return log_extra
 
     @staticmethod
     def mock_ipv4(text: str) -> str:
+        """Mock IPv4 addresses in the text."""
         pattern = r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}"
         replacement = " FILTERED_IP "
         text_mocked = re.sub(pattern, replacement, text)
 
         return text_mocked
 
     @staticmethod
     def mock_email(text: str) -> str:
+        """Mock email addresses in the text."""
         pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b"
         replacement = " FILTERED_EMAIL "
         text_mocked = re.sub(pattern, replacement, text)
 
         return text_mocked
 
     @staticmethod
     def mock_password(text: str) -> str:
+        """Mock passwords in the text."""
         pattern = r'("password": ")[^"]+'
         replacement = r"\1 FILTERED_PASSWORD "
         text_mocked = re.sub(pattern, replacement, text)
         return text_mocked
 
     @staticmethod
     def mock_flair(text: str) -> str:
+        """Mock flair in the text."""
         pattern = r'("FLAIR": "\[)(.*?)\]'
         replacement = r"\1 FILTERED_FLAIR ]"
         text_mocked = re.sub(pattern, replacement, text)
 
         return text_mocked
 
     @staticmethod
     def mock_home_directory(text: str) -> str:
+        """Mock home directory in the text."""
         user_home_directory = str(Path.home().as_posix())
         text_mocked = text.replace("\\", "/").replace(
             user_home_directory, "MOCKING_USER_PATH"
         )
 
         return text_mocked
 
     @staticmethod
     def filter_special_tags(text: str) -> str:
+        """Filter special tags in the text."""
         text_filtered = text.replace("\n", " MOCKING_BREAKLINE ")
         text_filtered = text_filtered.replace("'Traceback", "Traceback")
 
         return text_filtered
 
     @classmethod
     def filter_piis(cls, text: str) -> str:
+        """Filter Personally Identifiable Information in the text."""
         text_filtered = cls.mock_ipv4(text=text)
         text_filtered = cls.mock_email(text=text_filtered)
         text_filtered = cls.mock_password(text=text_filtered)
         text_filtered = cls.mock_home_directory(text=text_filtered)
         text_filtered = cls.mock_flair(text=text_filtered)
 
         return text_filtered
 
     @classmethod
     def filter_log_line(cls, text: str):
+        """Filter log line."""
         text_filtered = cls.filter_special_tags(text=text)
         text_filtered = cls.filter_piis(text=text_filtered)
 
         return text_filtered
 
     # OVERRIDE
     def __init__(
         self,
         settings: LoggingSettings,
         style="%",
         validate=True,
     ) -> None:
+        """Initialize the FormatterWithExceptions."""
         super().__init__(
             fmt=self.LOGFORMAT,
             datefmt=self.DATEFORMAT,
             style=style,
             validate=validate,
         )
         self.settings = settings
 
     @property
     def settings(self) -> LoggingSettings:
+        """Get the settings."""
         return deepcopy(self.__settings)
 
     @settings.setter
     def settings(self, settings: LoggingSettings) -> None:
+        """Set the settings."""
         self.__settings = settings
 
     # OVERRIDE
     def formatException(self, ei) -> str:
-        """Exception formatting handler
+        """Define the Exception formatting handler.
+
         Parameters
         ----------
         ei : logging._SysExcInfoType
             Exception to be logged
         Returns
         ----------
         str
             Formatted exception
         """
-
         result = super().formatException(ei)
         return repr(result)
 
     # OVERRIDE
     def format(self, record: logging.LogRecord) -> str:
-        """Log formatter
+        """Define the Log formatter.
+
         Parameters
         ----------
         record : logging.LogRecord
             Logging record
         Returns
         ----------
         str
             Formatted_log message
         """
-
         level_name = self.calculate_level_name(record=record)
         log_prefix_content = {
             "appName": self.settings.app_name,
             "levelname": level_name,
             "appId": self.settings.app_id,
             "sessionId": self.settings.session_id,
             "commitHash": "unknown-commit",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# IMPORT STANDARD
+"""Handlers Manager."""
+
 import logging
 import sys
 
-# IMPORT THIRD-PARTY
-# IMPORT INTERNAL
 from openbb_core.app.logs.formatters.formatter_with_exceptions import (
     FormatterWithExceptions,
 )
 from openbb_core.app.logs.handlers.path_tracking_file_handler import (
     PathTrackingFileHandler,
 )
 from openbb_core.app.logs.handlers.posthog_handler import PosthogHandler
 from openbb_core.app.logs.models.logging_settings import LoggingSettings
 
 
 class HandlersManager:
+    """Handlers Manager."""
+
     def __init__(self, settings: LoggingSettings):
+        """Initialize the HandlersManager."""
         self._handlers = settings.handler_list
         self._settings = settings
 
         for handler_type in self._handlers:
             if handler_type == "stdout":
                 self._add_stdout_handler()
             elif handler_type == "stderr":
@@ -30,42 +32,48 @@
                 self._add_file_handler()
             elif handler_type == "posthog":
                 self._add_posthog_handler()
             else:
                 logging.getLogger().debug("Unknown log handler.")
 
     def _add_posthog_handler(self):
+        """Add a Posthog handler."""
         handler = PosthogHandler(settings=self._settings)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_stdout_handler(self):
+        """Add a stdout handler."""
         handler = logging.StreamHandler(sys.stdout)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_stderr_handler(self):
+        """Add a stderr handler."""
         handler = logging.StreamHandler(sys.stderr)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_noop_handler(self):
+        """Add a null handler."""
         handler = logging.NullHandler()
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_file_handler(self):
+        """Add a file handler."""
         handler = PathTrackingFileHandler(settings=self._settings)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def update_handlers(self, settings: LoggingSettings):
+        """Update the handlers with new settings."""
         logger = logging.getLogger()
         for hdlr in logger.handlers:
             if isinstance(hdlr, (PathTrackingFileHandler, PosthogHandler)):
                 hdlr.settings = settings
                 hdlr.formatter.settings = settings  # type: ignore
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/logging_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from openbb_core.app.model.abstract.singleton import SingletonMeta
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
 from pydantic_core import to_jsonable_python
 
 
 class LoggingService(metaclass=SingletonMeta):
-    """
-    Logging Manager class responsible for managing logging settings and handling logs.
+    """Logging Manager class responsible for managing logging settings and handling logs.
 
     Attributes
     ----------
     _user_settings : Optional[UserSettings]
         User Settings object.
     _system_settings : Optional[SystemSettings]
         System Settings object.
@@ -55,16 +54,15 @@
     """
 
     def __init__(
         self,
         system_settings: SystemSettings,
         user_settings: UserSettings,
     ) -> None:
-        """
-        Logging Service Constructor.
+        """Define the Logging Service Constructor.
 
         Sets up the logging settings and handlers and then logs the startup information.
 
         Parameters
         ----------
         system_settings : SystemSettings
             System Settings, by default None
@@ -78,43 +76,40 @@
             system_settings=self._system_settings,
         )
         self._handlers_manager = self._setup_handlers()
         self._log_startup()
 
     @property
     def logging_settings(self) -> LoggingSettings:
-        """
-        Current logging settings.
+        """Define the Current logging settings.
 
         Returns
         -------
         LoggingSettings
             LoggingSettings object containing the current logging settings.
         """
         return self._logging_settings
 
     @logging_settings.setter
     def logging_settings(self, value: Tuple[SystemSettings, UserSettings]):
-        """
-        Setter for updating the logging settings.
+        """Define the Setter for updating the logging settings.
 
         Parameters
         ----------
         value : Tuple[SystemSettings, UserSettings]
             Tuple containing updated SystemSettings and UserSettings.
         """
         system_settings, user_settings = value
         self._logging_settings = LoggingSettings(
             user_settings=user_settings,
             system_settings=system_settings,
         )
 
     def _setup_handlers(self) -> HandlersManager:
-        """
-        Setup Logging Handlers.
+        """Set up Logging Handlers.
 
         Returns
         -------
         HandlersManager
             Handlers Manager object.
         """
         logger = logging.getLogger(__name__)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+"""Logging settings."""
+
 from pathlib import Path
 from typing import List, Optional
 
 from openbb_core.app.logs.utils.utils import get_app_id, get_log_dir, get_session_id
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
 
 
 # pylint: disable=too-many-instance-attributes
 class LoggingSettings:
+    """Logging settings."""
+
     def __init__(
         self,
         user_settings: Optional[UserSettings] = None,
         system_settings: Optional[SystemSettings] = None,
     ):
+        """Initialize the logging settings."""
         user_settings = user_settings or UserSettings()
         system_settings = system_settings or SystemSettings()
 
         user_data_directory = (
             str(Path.home() / "OpenBBUserData")
             if not user_settings.preferences
             else user_settings.preferences.data_directory
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# IMPORT STANDARD
+"""Utility functions for logging."""
+
 import time
 import uuid
 import warnings
 from pathlib import Path, PosixPath
 
-# IMPORT THIRD-PARTY
-# IMPORT INTERNAL
-
 
 def get_session_id() -> str:
     """UUID of the current session."""
     session_id = str(uuid.uuid4()) + "-" + str(int(time.time()))
     return session_id
 
 
@@ -37,36 +35,40 @@
     logging_uuid = create_log_uuid_if_not_exists(log_dir)
     uuid_log_dir = create_uuid_dir_if_not_exists(log_dir, logging_uuid)
 
     return uuid_log_dir
 
 
 def create_log_dir_if_not_exists(contextual_user_data_directory: str) -> Path:
+    """Create a log directory for the current installation."""
     log_dir = Path(contextual_user_data_directory).joinpath("logs").absolute()
     if not log_dir.is_dir():
         log_dir.mkdir(parents=True, exist_ok=True)
 
     return log_dir
 
 
 def create_log_uuid_if_not_exists(log_dir: Path) -> str:
+    """Create a log id file for the current logging session."""
     log_id = get_log_id(log_dir)
     if not log_id.is_file():
         logging_id = f"{uuid.uuid4()}"
         log_id.write_text(logging_id, encoding="utf-8")
     else:
         logging_id = log_id.read_text(encoding="utf-8").rstrip()
 
     return logging_id
 
 
 def get_log_id(log_dir):
+    """Get the log id file."""
     return (log_dir / ".logid").absolute()
 
 
 def create_uuid_dir_if_not_exists(log_dir, logging_id) -> PosixPath:
+    """Create a directory for the current logging session."""
     uuid_log_dir = (log_dir / logging_id).absolute()
 
     if not uuid_log_dir.is_dir():
         uuid_log_dir.mkdir(parents=True, exist_ok=True)
 
     return uuid_log_dir
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+"""OpenBB Core Chart model."""
+
 from enum import Enum
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, ConfigDict, Field
 
 
 class ChartFormat(str, Enum):
+    """Chart format."""
+
     plotly = "plotly"
 
 
 class Chart(BaseModel):
+    """Model for Chart."""
+
     content: Optional[Dict[str, Any]] = Field(
         default=None,
         description="Raw textual representation of the chart.",
     )
     format: Optional[ChartFormat] = Field(
         default=ChartFormat.plotly,
         description="Complementary attribute to the `content` attribute. It specifies the format of the chart.",
@@ -21,10 +27,11 @@
         default=None,
         description="The figure object.",
         json_schema_extra={"exclude_from_api": True},
     )
     model_config = ConfigDict(validate_assignment=True)
 
     def __repr__(self) -> str:
+        """Return string representation."""
         return f"{self.__class__.__name__}\n\n" + "\n".join(
             f"{k}: {v}" for k, v in self.model_dump().items()
         )
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 _Credentials = CredentialsLoader().load()
 
 
 class Credentials(_Credentials):  # type: ignore
     """Credentials model used to store provider credentials."""
 
     def __repr__(self) -> str:
-        """String representation of the credentials."""
+        """Define the string representation of the credentials."""
         return (
             self.__class__.__name__
             + "\n\n"
             + "\n".join([f"{k}: {v}" for k, v in sorted(self.__dict__.items())])
         )
 
     def show(self):
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/custom_parameter.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/custom_parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Custom parameter and choices for OpenBB."""
+
 import sys
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from typing_extensions import LiteralString
 
 # `slots` is available on Python >= 3.10
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/fast_api_settings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/fast_api_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/hub/features_keys.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/features_keys.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+"""Model for API keys for various providers."""
+
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 
 class FeaturesKeys(BaseModel):
+    """API keys for various providers."""
+
     API_BITQUERY_KEY: Optional[str] = Field(default=None)
     API_BIZTOC_TOKEN: Optional[str] = Field(default=None)
     API_CMC_KEY: Optional[str] = Field(default=None)
     API_COINGLASS_KEY: Optional[str] = Field(default=None)
     API_CRYPTO_PANIC_KEY: Optional[str] = Field(default=None)
     API_DAPPRADAR_KEY: Optional[str] = Field(default=None)
     API_DATABENTO_KEY: Optional[str] = Field(default=None)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+"""Metadata model."""
+
 from datetime import datetime
 from inspect import isclass
 from typing import Any, Dict, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel, Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 
 
 class Metadata(BaseModel):
+    """Metadata of a command execution."""
+
     arguments: Dict[str, Any] = Field(
         default_factory=dict,
         description="Arguments of the command.",
     )
     duration: int = Field(
         description="Execution duration in nano second of the command."
     )
     route: str = Field(description="Route of the command.")
     timestamp: datetime = Field(description="Execution starting timestamp.")
 
     def __repr__(self) -> str:
+        """Return string representation."""
         return f"{self.__class__.__name__}\n\n" + "\n".join(
             f"{k}: {v}" for k, v in self.model_dump().items()
         )
 
     @field_validator("arguments")
     @classmethod
     def scale_arguments(cls, v):
         """Scale arguments.
+
         This function is meant to limit the size of the input arguments of a command.
         If the type is one of the following: `Data`, `List[Data]`, `DataFrame`, `List[DataFrame]`,
         `Series`, `List[Series]` or `ndarray`, the value of the argument is swapped by a dictionary
         containing the type and the columns. If the type is not one of the previous, the
         value is kept or trimmed to 80 characters.
         """
         for arg, arg_val in v.items():
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/obbject.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/preferences.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/provider_interface.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/query.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/router.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,27 +205,27 @@
 
     @property
     def prefix(self) -> str:
         """Prefix."""
         return self._api_router.prefix
 
     @property
-    def description(self) -> str:
+    def description(self) -> Optional[str]:
         """Description."""
         return self._description
 
     @property
     def routers(self) -> Dict[str, "Router"]:
         """Routers nested within the Router, i.e. sub-routers."""
         return self._routers
 
     def __init__(
         self,
         prefix: str = "",
-        description: str = "",
+        description: Optional[str] = None,
     ) -> None:
         """Initialize Router."""
         self._api_router = APIRouter(
             prefix=prefix,
             responses={404: {"description": "Not found"}},
         )
         self._description = description
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/auth_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,38 +25,38 @@
     """Authentication service error."""
 
 
 class AuthService(metaclass=SingletonMeta):
     """Auth service."""
 
     def __init__(self, ext_name: Optional[str] = EXT_NAME) -> None:
-        """Initializes AuthService."""
+        """Initialize AuthService."""
         if not self._load_extension(ext_name):
             self._router = default_router
             self._auth_hook = default_auth_hook
             self._user_settings_hook = default_user_settings_hook
 
     @property
     def router(self) -> APIRouter:
-        """Gets router."""
+        """Get router."""
         return self._router
 
     @property
     def auth_hook(self) -> Callable[..., Awaitable[None]]:
-        """Gets general authentication hook."""
+        """Get general authentication hook."""
         return self._auth_hook
 
     @property
     def user_settings_hook(self) -> Callable[..., Awaitable[UserSettings]]:
-        """Gets user settings hook."""
+        """Get user settings hook."""
         return self._user_settings_hook
 
     @staticmethod
     def _is_installed(ext_name: str) -> bool:
-        """Checks if auth_extension is installed."""
+        """Check if auth_extension is installed."""
         extension = ExtensionLoader().get_core_entry_point(ext_name) or False
         return extension and ext_name == extension.name  # type: ignore
 
     @staticmethod
     def _get_entry_mod(ext_name: str) -> ModuleType:
         """Get the module of the given auth_extension."""
         extension = ExtensionLoader().get_core_entry_point(ext_name)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/hub_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     TIMEOUT = 10
 
     def __init__(
         self,
         session: Optional[HubSession] = None,
         base_url: Optional[str] = None,
     ):
+        """Initialize Hub service."""
         self._base_url = base_url or Env().HUB_BACKEND
         self._session = session
 
     @property
     def base_url(self) -> str:
         """Get base url."""
         return self._base_url
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/system_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     PRO_VALIDATION_HASH = "300ac59fdcc8f899e0bc5c18cda8652220735da1a00e2af365efe9d8e5fe8306"  # pragma: allowlist secret
 
     def __init__(
         self,
         **kwargs,
     ):
+        """Initialize system service."""
         self._system_settings = self._read_default_system_settings(
             path=self.SYSTEM_SETTINGS_PATH, **kwargs
         )
 
     @classmethod
     def _compare_hash(cls, input_value, existing_hash: Optional[str] = None):
         existing_hash = existing_hash or cls.PRO_VALIDATION_HASH
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/user_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     USER_SETTINGS_PATH = USER_SETTINGS_PATH
     USER_SETTINGS_ALLOWED_FIELD_SET = {"credentials", "preferences", "defaults"}
 
     def __init__(
         self,
         default_user_settings: Optional[UserSettings] = None,
     ):
+        """Initialize user service."""
         self._default_user_settings = (
             default_user_settings or self.read_default_user_settings()
         )
 
     @classmethod
     def read_default_user_settings(cls, path: Optional[Path] = None) -> UserSettings:
         """Read default user settings."""
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/app_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 """
 
 
 class BaseApp:
     """Base app."""
 
     def __init__(self, command_runner: CommandRunner):
+        """Initialize the app."""
         command_runner.init_logging_service()
         self._command_runner = command_runner
         self._account = Account(self)
         self._coverage = Coverage(self)
         self._reference = ReferenceLoader().reference
 
     @property
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from openbb_core.app.model.obbject import OBBject
 
 
 class Container:
     """Container class for the command runner session."""
 
     def __init__(self, command_runner: CommandRunner) -> None:
+        """Initialize the container."""
         self._command_runner = command_runner
         OBBject._user_settings = command_runner.user_settings
         OBBject._system_settings = command_runner.system_settings
 
     def _run(self, *args, **kwargs) -> Any:
         """Run a command in the container."""
         obbject = self._command_runner.sync_run(*args, **kwargs)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/package_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1680,12 +1680,20 @@
         -------
         Dict[str, Dict[str, Any]]
             Dictionary containing the description for each router.
         """
         main_router = RouterLoader.from_extensions()
         routers = {}
         for path in route_map:
-            # Strip the command name from the path
-            _path = "/".join(path.split("/")[:-1])
-            if description := main_router.get_attr(_path, "description"):
-                routers[_path] = {"description": description}
+            path_parts = path.split("/")
+            # We start at 2: ["/", "some_router"] "/some_router"
+            i = 2
+            p = "/".join(path_parts[:i])
+            while p != path:
+                if p not in routers:
+                    description = main_router.get_attr(p, "description")
+                    if description is not None:
+                        routers[p] = {"description": description}
+                # We go down the path to include sub-routers
+                i += 1
+                p = "/".join(path_parts[:i])
         return routers
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def validate(
     func: Optional[Callable[P, R]] = None,
     **dec_kwargs,
 ) -> Any:
     """Validate function calls."""
 
     def decorated(f: Callable[P, R]):
-        """Decorated function."""
+        """Use for decorating functions."""
 
         @wraps(f)
         def wrapper(*f_args, **f_kwargs):
             return validate_call(f, **dec_kwargs)(*f_args, **f_kwargs)
 
         return wrapper
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,9 +38,20 @@
                             check_single_item(
                                 new,
                                 f"{field} -> multiple items not allowed for '{provider}'",
                             )
 
                         kwargs[p][field] = new
                         break
+    else:
+        provider = kwargs.get("provider_choices", {}).get("provider")
+        for param_category in ("standard_params", "extra_params"):
+            if param_category in kwargs:
+                for field, value in kwargs[param_category].items():
+                    if isinstance(value, list):
+                        kwargs[param_category][field] = ",".join(map(str, value))
+                    check_single_item(
+                        kwargs[param_category][field],
+                        f"{field} -> multiple items not allowed for '{provider}'",
+                    )
 
     return kwargs
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,10 +162,10 @@
     return cache_dir
 
 
 def check_single_item(
     value: Optional[str], message: Optional[str] = None
 ) -> Optional[str]:
     """Check that string contains a single item."""
-    if value and ("," in value or ";" in value):
+    if value and isinstance(value, str) and ("," in value or ";" in value):
         raise OpenBBError(message if message else "multiple items not allowed")
     return value
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/app/version.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/env.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Environment variables."""
+
 import os
 from pathlib import Path
 from typing import Dict, Optional
 
 import dotenv
 
 from openbb_core.app.constants import OPENBB_DIRECTORY
@@ -10,55 +12,56 @@
 
 class Env(metaclass=SingletonMeta):
     """Environment variables."""
 
     _environ: Dict[str, str]
 
     def __init__(self) -> None:
+        """Initialize the environment."""
         dotenv.load_dotenv(Path(OPENBB_DIRECTORY, ".env"))
         self._environ = os.environ.copy()
 
     @property
     def API_AUTH(self) -> bool:
-        """API authentication: enables API endpoint authentication"""
+        """API authentication: enables API endpoint authentication."""
         return self.str2bool(self._environ.get("OPENBB_API_AUTH", False))
 
     @property
     def API_USERNAME(self) -> Optional[str]:
-        """API username: sets API username"""
+        """API username: sets API username."""
         return self._environ.get("OPENBB_API_USERNAME", None)
 
     @property
     def API_PASSWORD(self) -> Optional[str]:
-        """API password: sets API password"""
+        """API password: sets API password."""
         return self._environ.get("OPENBB_API_PASSWORD", None)
 
     @property
     def API_AUTH_EXTENSION(self) -> Optional[str]:
-        """Auth extension: specifies which authentication extension to use"""
+        """Auth extension: specifies which authentication extension to use."""
         return self._environ.get("OPENBB_API_AUTH_EXTENSION", None)
 
     @property
     def AUTO_BUILD(self) -> bool:
-        """Automatic build: enables automatic package build on import"""
+        """Automatic build: enables automatic package build on import."""
         return self.str2bool(self._environ.get("OPENBB_AUTO_BUILD", True))
 
     @property
     def DEBUG_MODE(self) -> bool:
-        """Debug mode: enables debug mode"""
+        """Debug mode: enables debug mode."""
         return self.str2bool(self._environ.get("OPENBB_DEBUG_MODE", False))
 
     @property
     def DEV_MODE(self) -> bool:
-        """Dev mode: enables development mode"""
+        """Dev mode: enables development mode."""
         return self.str2bool(self._environ.get("OPENBB_DEV_MODE", False))
 
     @property
     def HUB_BACKEND(self) -> str:
-        """Hub backend: sets the backend for the OpenBB Hub"""
+        """Hub backend: sets the backend for the OpenBB Hub."""
         return self._environ.get("OPENBB_HUB_BACKEND", "https://payments.openbb.co")
 
     @staticmethod
     def str2bool(value) -> bool:
         """Match a value to its boolean correspondent."""
         if isinstance(value, bool):
             return value
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_chains.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     """Options Chains Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @classmethod
     @field_validator("symbol", mode="before", check_fields=False)
     def to_upper(cls, v: str) -> str:
+        """Return the symbol in uppercase."""
         return v.upper()
 
 
 class OptionsChainsData(Data):
     """Options Chains Data."""
 
     symbol: Optional[str] = Field(
@@ -147,13 +148,13 @@
     theta: Optional[float] = Field(default=None, description="Theta of the option.")
     vega: Optional[float] = Field(default=None, description="Vega of the option.")
     rho: Optional[float] = Field(default=None, description="Rho of the option.")
 
     @field_validator("expiration", mode="before", check_fields=False)
     @classmethod
     def date_validate(cls, v):  # pylint: disable=E0213
-        """Return the datetime object from the date string"""
+        """Return the datetime object from the date string."""
         if isinstance(v, datetime):
             return datetime.strftime(v, "%Y-%m-%d")
         if isinstance(v, str):
             return datetime.strptime(v, "%Y-%m-%d")
         return v
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/standard_models/world_news.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     return random.choice(user_agent_strings)  # nosec # noqa: S311
 
 
 class ClientResponse(aiohttp.ClientResponse):
     """Client response class."""
 
     def __init__(self, *args, **kwargs):
+        """Initialize the response."""
         kwargs["request_info"] = self.obfuscate_request_info(kwargs["request_info"])
         super().__init__(*args, **kwargs)
 
     @classmethod
     def obfuscate_request_info(
         cls, request_info: aiohttp.RequestInfo
     ) -> aiohttp.RequestInfo:
@@ -57,18 +58,21 @@
 
     async def json(self, **kwargs) -> Union[dict, list]:
         """Return the json response."""
         return await super().json(**kwargs)
 
 
 class ClientSession(aiohttp.ClientSession):
+    """Client session."""
+
     _response_class: Type[ClientResponse]
     _session: "ClientSession"
 
     def __init__(self, *args, **kwargs):
+        """Initialize the session."""
         kwargs["connector"] = kwargs.get(
             "connector", aiohttp.TCPConnector(ttl_dns_cache=300)
         )
         kwargs["response_class"] = kwargs.get("response_class", ClientResponse)
         kwargs["auto_decompress"] = kwargs.get("auto_decompress", False)
 
         super().__init__(*args, **kwargs)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/currency_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 )
 async def reference_rates(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Current, official, currency reference rates.
+    """Get current, official, currency reference rates.
 
     Foreign exchange reference rates are the exchange rates set by a major financial institution or regulatory body,
     serving as a benchmark for the value of currencies around the world.
     These rates are used as a standard to facilitate international trade and financial transactions,
     ensuring consistency and reliability in currency conversion.
     They are typically updated on a daily basis and reflect the market conditions at a specific time.
     Central banks and financial institutions often use these rates to guide their own exchange rates,
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Utility functions for the econometrics extension of the OpenBB platform."""
+
 import warnings
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
 from statsmodels.tsa.stattools import adfuller
 
 
 def get_engle_granger_two_step_cointegration_test(
     dependent_series: pd.Series, independent_series: pd.Series
 ) -> Tuple[float, float, float, pd.Series, float, float]:
-    """Estimates long-run and short-run cointegration relationship for series y and x and apply
-    the two-step Engle & Granger test for cointegration.
+    """Estimate long-run and short-run cointegration relationship for series y and x.
+
+    Then apply the two-step Engle & Granger test for cointegration.
 
     Uses a 2-step process to first estimate coefficients for the long-run relationship
         y_t = c + gamma * x_t + z_t
 
     and then the short-term relationship,
         y_t - y_(t-1) = alpha * z_(t-1) + epsilon_t,
 
@@ -83,15 +86,15 @@
 
     adfstat, pvalue, _, _, _ = adfuller(z, maxlag=1, autolag=None)
 
     return c, gamma, alpha, z, adfstat, pvalue
 
 
 def mock_multi_index_data():
-    """Creates a mock multi-index dataframe for testing purposes."""
+    """Create a mock multi-index dataframe for testing purposes."""
     arrays = [
         ["individual_" + str(i) for i in range(1, 11) for _ in range(5)],
         list(range(1, 6)) * 10,
     ]
     index = pd.MultiIndex.from_arrays(arrays, names=("individual", "time"))
 
     df = pd.DataFrame(
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/economy_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,32 @@
 )
 async def cpi(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Consumer Price Index (CPI).  Returns either the rescaled index value, or a rate of change (inflation)."""
+    """Get Consumer Price Index (CPI).
+
+    Returns either the rescaled index value, or a rate of change (inflation).
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="RiskPremium",
     examples=[APIEx(parameters={"provider": "fmp"})],
 )
 async def risk_premium(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Market Risk Premium by country."""
+    """Get Market Risk Premium by country."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="BalanceOfPayments",
     examples=[
         APIEx(parameters={"provider": "ecb"}),
@@ -111,16 +114,16 @@
 @router.command(model="FredSearch", examples=[APIEx(parameters={"provider": "fred"})])
 async def fred_search(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Search for FRED series or economic releases by ID or string.
+    """Search for FRED series or economic releases by ID or string.
+
     This does not return the observation values, only the metadata.
     Use this function to find series IDs for `fred_series()`.
     """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
@@ -156,15 +159,18 @@
 )
 async def money_measures(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Money Measures (M1/M2 and components). The Federal Reserve publishes as part of the H.6 Release."""
+    """Get Money Measures (M1/M2 and components).
+
+    The Federal Reserve publishes as part of the H.6 Release.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="Unemployment",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -184,15 +190,15 @@
 )
 async def unemployment(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Global unemployment data."""
+    """Get global unemployment data."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="CLI",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -201,16 +207,19 @@
 )
 async def composite_leading_indicator(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """The composite leading indicator (CLI) is designed to provide early signals of turning points
+    """Use the composite leading indicator (CLI).
+
+    It is designed to provide early signals of turning points
     in business cycles showing fluctuation of the economic activity around its long term potential level.
+
     CLIs show short-term economic movements in qualitative rather than quantitative terms.
     """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="STIR",
@@ -223,17 +232,19 @@
 )
 async def short_term_interest_rate(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Short-term interest rates are the rates at which short-term borrowings are effected between
+    """Get Short-term interest rates.
+
+    They are the rates at which short-term borrowings are effected between
     financial institutions or the rate at which short-term government paper is issued or traded in the market.
+
     Short-term interest rates are generally averages of daily rates, measured as a percentage.
     Short-term interest rates are based on three-month money market rates where available.
     Typical standardised names are "money market rate" and "treasury bill rate".
     """
     return await OBBject.from_query(Query(**locals()))
 
 
@@ -248,24 +259,25 @@
 )
 async def long_term_interest_rate(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Long-term interest rates refer to government bonds maturing in ten years.
+    """Get Long-term interest rates that refer to government bonds maturing in ten years.
+
     Rates are mainly determined by the price charged by the lender, the risk from the borrower and the
     fall in the capital value. Long-term interest rates are generally averages of daily rates,
     measured as a percentage. These interest rates are implied by the prices at which the government bonds are
     traded on financial markets, not the interest rates at which the loans were issued.
     In all cases, they refer to bonds whose capital repayment is guaranteed by governments.
     Long-term interest rates are one of the determinants of business investment.
     Low long-term interest rates encourage investment in new equipment and high interest rates discourage it.
-    Investment is, in turn, a major source of economic growth."""
+    Investment is, in turn, a major source of economic growth.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="FredRegional",
     examples=[
         APIEx(
@@ -285,12 +297,12 @@
 )
 async def fred_regional(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Query the Geo Fred API for regional economic data by series group.
+    """Query the Geo Fred API for regional economic data by series group.
+
     The series group ID is found by using `fred_search` and the `series_id` parameter.
     """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 )
 async def forecast(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Forecasted GDP Data."""
+    """Get Forecasted GDP Data."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="GdpNominal",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -42,15 +42,15 @@
 )
 async def nominal(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Nominal GDP Data."""
+    """Get Nominal GDP Data."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="GdpReal",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -59,9 +59,9 @@
 )
 async def real(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Real GDP Data."""
+    """Get Real GDP Data."""
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
     """Get the closest peers for a given company.
 
     Peers consist of companies trading on the same exchange, operating within the same sector
-    and with comparable market capitalizations."""
+    and with comparable market capitalizations.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="CompareGroups",
     examples=[
         APIEx(parameters={"provider": "finviz"}),
@@ -63,9 +64,10 @@
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
     """Get company data grouped by sector, industry or country and display either performance or valuation metrics.
 
     Valuation metrics include price to earnings, price to book, price to sales ratios and price to cash flow.
-    Performance metrics include the stock price change for different time periods."""
+    Performance metrics include the stock price change for different time periods.
+    """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,9 +31,10 @@
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
     """Get the weekly aggregate trade data for Over The Counter deals.
 
     ATS and non-ATS trading data for each ATS/firm
-    with trade reporting obligations under FINRA rules."""
+    with trade reporting obligations under FINRA rules.
+    """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,18 +140,19 @@
 )
 async def top_retail(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Tracks over $30B USD/day of individual investors trades.
+    """Track over $30B USD/day of individual investors trades.
 
     It gives a daily view into retail activity and sentiment for over 9,500 US traded stocks,
-    ADRs, and ETPs."""
+    ADRs, and ETPs.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="UpcomingReleaseDays",
     examples=[APIEx(parameters={"provider": "seeking_alpha"})],
 )
@@ -182,14 +183,15 @@
 )
 async def filings(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Get the URLs to SEC filings reported to EDGAR database, such as 10-K, 10-Q, 8-K, and more. SEC
-    filings include Form 10-K, Form 10-Q, Form 8-K, the proxy statement, Forms 3, 4, and 5, Schedule 13, Form 114,
+    """Get the URLs to SEC filings reported to EDGAR database, such as 10-K, 10-Q, 8-K, and more.
+
+    SEC filings include Form 10-K, Form 10-Q, Form 8-K, the proxy statement, Forms 3, 4, and 5, Schedule 13, Form 114,
     Foreign Investment Disclosures and others. The annual 10-K report is required to be
     filed annually and includes the company's financial statements, management discussion and analysis,
     and audited financial statements.
     """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/equity_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,18 @@
 )
 async def screener(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Screen for companies meeting various criteria. These criteria include
-    market cap, price, beta, volume, and dividend yield."""
+    """Screen for companies meeting various criteria.
+
+    These criteria include market cap, price, beta, volume, and dividend yield.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="EquityInfo",
     examples=[APIEx(parameters={"symbol": "AAPL", "provider": "fmp"})],
 )
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
 )
 async def form_13f(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
+    """Get the form 13F.
+
     The Securities and Exchange Commission's (SEC) Form 13F is a quarterly report
     that is required to be filed by all institutional investment managers with at least
     $100 million in assets under management.
     Managers are required to file Form 13F within 45 days after the last day of the calendar quarter.
     Most funds wait until the end of this period in order to conceal
     their investment strategy from competitors and the public.
     """
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/index_router.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 )
 async def market(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Historical Market Indices."""
+    """Get Historical Market Indices."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="IndexConstituents",
     examples=[
         APIEx(parameters={"symbol": "dowjones", "provider": "fmp"}),
@@ -52,15 +52,15 @@
 )
 async def constituents(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Index Constituents."""
+    """Get Index Constituents."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="IndexSnapshots",
     examples=[
         APIEx(parameters={"provider": "tmx"}),
@@ -103,15 +103,15 @@
 )
 async def search(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Filters indices for rows containing the query."""
+    """Filter indices for rows containing the query."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="SP500Multiples",
     examples=[
         APIEx(parameters={"provider": "nasdaq"}),
@@ -120,23 +120,23 @@
 )
 async def sp500_multiples(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Historical S&P 500 multiples and Shiller PE ratios."""
+    """Get historical S&P 500 multiples and Shiller PE ratios."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="IndexSectors",
     examples=[APIEx(parameters={"symbol": "^TX60", "provider": "tmx"})],
 )
 async def sectors(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Index Sectors. Sector weighting of an index."""
+    """Get Index Sectors. Sector weighting of an index."""
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""OpenBB Performance Extension router."""
+
 from typing import List
 
 import numpy as np
 import pandas as pd
 from openbb_core.app.model.example import APIEx, PythonEx
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.router import Router
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,16 +372,15 @@
             }
         ),
     ],
 )
 def mean(
     data: List[Data], target: str, window: PositiveInt = 21, index: str = "date"
 ) -> OBBject[List[Data]]:
-    """
-    Calculate the rolling mean (average) of a target column within a given window size.
+    """Calculate the rolling average of a target column within a given window size.
 
     The rolling mean is a simple moving average that calculates the average of a target variable over a specified window.
     This function is widely used in financial analysis to smooth short-term fluctuations and highlight longer-term trends
     or cycles in time series data.
 
     Parameters
     ----------
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Statistics Functions"""
+"""Statistics Functions."""
 
 from typing import Union
 
 from numpy import (
     mean as mean_np,
     ndarray,
     std,
@@ -12,30 +12,36 @@
 from scipy import stats
 
 # Because python is weird and these being the same name as the fastapi router functions
 # which overwrites the function signature, we add the _ after the function name
 
 
 def kurtosis_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Kurtosis is a measure of the "tailedness" of the probability distribution of a real-valued random variable."""
+    """Get Kurtosis.
+
+    It is a measure of the "tailedness" of the probability distribution of a real-valued random variable.
+    """
     return stats.kurtosis(data)
 
 
 def skew_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Skewness is a measure of the asymmetry of the probability distribution of a
-    real-valued random variable about its mean."""
+    """Get Skewness.
+
+    It is a measure of the asymmetry of the probability distribution of a
+    real-valued random variable about its mean.
+    """
     return stats.skew(data)
 
 
 def mean_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Mean is the average of the numbers."""
+    """Get Mean which is the average of the numbers."""
     return mean_np(data)
 
 
 def std_dev_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Standard deviation is a measure of the amount of variation or dispersion of a set of values."""
+    """Get Standard deviation that is a measure of the amount of variation or dispersion of a set of values."""
     return std(data)
 
 
 def var_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Variance is a measure of the amount of variation or dispersion of a set of values."""
+    """Get Variance that is a measure of the amount of variation or dispersion of a set of values."""
     return var_np(data)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,15 @@
                     sample={"date": "2023-01-01", "close": 0.05},
                 ),
             }
         ),
     ],
 )
 def variance(data: List[Data], target: str) -> OBBject[List[Data]]:
-    """
-    Calculate the  variance of a target column.
+    """Calculate the  variance of a target column.
 
     Variance measures the dispersion of a set of data points around their mean. It is a key metric for
     assessing the volatility and stability of financial returns or other time series data.
 
     Parameters
     ----------
     data: List[Data]
@@ -146,16 +145,15 @@
                     sample={"date": "2023-01-01", "close": 0.05},
                 ),
             }
         ),
     ],
 )
 def stdev(data: List[Data], target: str) -> OBBject[List[Data]]:
-    """
-    Calculate the rolling standard deviation of a target column.
+    """Calculate the rolling standard deviation of a target column.
 
     Standard deviation is a measure of the amount of variation or dispersion of a set of values.
     It is widely used to assess the risk and volatility of financial returns or other time series data
     It is the square root of the variance.
 
     Parameters
     ----------
@@ -196,16 +194,15 @@
                     sample={"date": "2023-01-01", "close": 0.05},
                 ),
             }
         ),
     ],
 )
 def kurtosis(data: List[Data], target: str) -> OBBject[List[Data]]:
-    """
-    Calculate the rolling kurtosis of a target column.
+    """Calculate the rolling kurtosis of a target column.
 
     Kurtosis measures the "tailedness" of the probability distribution of a real-valued random variable.
     High kurtosis indicates a distribution with heavy tails (outliers), suggesting a higher risk of extreme outcomes.
     Low kurtosis indicates a distribution with lighter tails (less outliers), suggesting less risk of extreme outcomes.
     This function helps in assessing the risk of outliers in financial returns or other time series data.
 
     Parameters
@@ -251,16 +248,15 @@
     ],
 )
 def quantile(
     data: List[Data],
     target: str,
     quantile_pct: NonNegativeFloat = 0.5,
 ) -> OBBject[List[Data]]:
-    """
-    Calculate the quantile of a target column at a specified quantile percentage.
+    """Calculate the quantile of a target column at a specified quantile percentage.
 
     Quantiles are points dividing the range of a probability distribution into  intervals with equal probabilities,
     or dividing the  sample in the same way.
 
     Parameters
     ----------
     data: List[Data]
@@ -308,16 +304,15 @@
         ),
     ],
 )
 def mean(
     data: List[Data],
     target: str,
 ) -> OBBject[List[Data]]:
-    """
-    Calculate the  mean (average) of a target column.
+    """Calculate the average of a target column.
 
     The rolling mean is a simple moving average that calculates the average of a target variable.
     This function is widely used in financial analysis to smooth short-term fluctuations and highlight longer-term trends
     or cycles in time series data.
 
     Parameters
     ----------
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,9 +55,9 @@
 )
 async def cot(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Commitment of Traders Reports."""
+    """Get Commitment of Traders Reports."""
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 )
 async def schema_files(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """A tool for navigating the directory of SEC XML schema files by year."""
+    """Use tool for navigating the directory of SEC XML schema files by year."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="SymbolMap",
     examples=[APIEx(parameters={"query": "0000789019", "provider": "sec"})],
 )
@@ -104,15 +104,15 @@
 )
 async def rss_litigation(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """The RSS feed provides links to litigation releases concerning civil lawsuits brought by the Commission in federal court."""  # noqa: E501 pylint: disable=C0301
+    """Get the RSS feed that provides links to litigation releases concerning civil lawsuits brought by the Commission in federal court."""  # noqa: E501 pylint: disable=C0301
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="SicSearch",
     examples=[
         APIEx(parameters={"provider": "sec"}),
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 def standard_deviation(
     data: pd.DataFrame,
     window: int = 30,
     trading_periods: Optional[int] = None,
     is_crypto: bool = False,
     clean: bool = True,
 ) -> pd.DataFrame:
-    """Standard deviation.
+    """Calculate the Standard deviation.
 
     Measures how widely returns are dispersed from the average return.
     It is the most common (and biased) estimator of volatility.
 
     Parameters
     ----------
     data : pd.DataFrame
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/technical_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
+    Tuple,
     Union,
 )
+from warnings import warn
 
 import numpy as np
 import pandas as pd
 from openbb_core.app.model.charts.chart import Chart
 from openbb_core.app.model.extension import Extension
 from openbb_core.app.utils import basemodel_to_df, convert_to_basemodel
 from openbb_core.provider.abstract.data import Data
 
 from openbb_charting import charting_router
+from openbb_charting.core.backend import Backend, create_backend, get_backend
 from openbb_charting.core.to_chart import ChartIndicators, to_chart
 from openbb_charting.utils.helpers import get_charting_functions
 
 ext = Extension(name="charting")
 
 
 @ext.obbject_accessor
@@ -47,32 +50,38 @@
         from openbb_core.app.model.obbject import OBBject
 
         self._obbject: OBBject = obbject
         self._charting_settings = ChartingSettings(
             user_settings=self._obbject._user_settings,  # type: ignore
             system_settings=self._obbject._system_settings,  # type: ignore
         )
-        self._handle_backend()
+        self._backend: Backend = self._handle_backend()
 
     @classmethod
     def indicators(cls):
-        """Returns a list of the available indicators."""
+        """Return a list of the available indicators."""
         return ChartIndicators.get_available_indicators()
 
     @classmethod
     def functions(cls):
-        """Returns a list of the available functions."""
+        """Return a list of the available functions."""
         return get_charting_functions()
 
     def _handle_backend(self):
+        """Create and start the backend."""
         # pylint: disable=import-outside-toplevel
-        from openbb_charting.core.backend import create_backend, get_backend
+        from openbb_charting.core.backend import (  # pylint: disable=W0621, W0404
+            create_backend,  # noqa
+            get_backend,  # noqa
+        )
 
         create_backend(self._charting_settings)
-        get_backend().start(debug=self._charting_settings.debug_mode)
+        backend = get_backend()
+        backend.start(debug=self._charting_settings.debug_mode)
+        return backend
 
     @staticmethod
     def _get_chart_function(route: str) -> Callable:
         """Given a route, it returns the chart function. The module must contain the given route."""
         adjusted_route = route.replace("/", "_")[1:]
         return getattr(charting_router, adjusted_route)
 
@@ -96,14 +105,36 @@
         fig, content = charting_function(**kwargs)
         self._obbject.chart = Chart(
             fig=fig, content=content, format=charting_router.CHART_FORMAT
         )
         if render:
             fig.show(**kwargs)
 
+    def _prepare_data_as_df(
+        self, data: Optional[Union[pd.DataFrame, pd.Series]]
+    ) -> Tuple[pd.DataFrame, bool]:
+        has_data = (isinstance(data, (pd.DataFrame, pd.Series)) and not data.empty) or (
+            bool(data)
+        )
+        index = (
+            data.index.name
+            if has_data and isinstance(data, (pd.DataFrame, pd.Series))
+            else None
+        )
+        data_as_df: pd.DataFrame = (
+            basemodel_to_df(convert_to_basemodel(data), index=index)
+            if has_data
+            else self._obbject.to_dataframe()
+        )
+        if "date" in data_as_df.columns:
+            data_as_df = data_as_df.set_index("date")
+        if "provider" in data_as_df.columns:
+            data_as_df.drop(columns="provider", inplace=True)
+        return data_as_df, has_data
+
     # pylint: disable=too-many-arguments
     def to_chart(
         self,
         data: Optional[
             Union[
                 list,
                 dict,
@@ -120,16 +151,15 @@
         candles: bool = True,
         volume: bool = True,
         prepost: bool = False,
         volume_ticks_x: int = 7,
         render: bool = True,
         **kwargs,
     ):
-        """
-        Creates a OpenBBFigure with user customizations (if any) and saves it to the OBBject.
+        """Create a OpenBBFigure with user customizations (if any) and saves it to the OBBject.
 
         This function is used so it can be called at the module level and used out of the box,
         which allows some more flexibility, ease of use and doesn't require the user to know
         about the PlotlyTA class.
 
         Parameters
         ----------
@@ -169,29 +199,15 @@
         2) Get all the available indicators
         > from openbb_charting.core.plotly_ta.data_classes import ChartIndicators
         > ChartIndicators.get_available_indicators()
         or
         > from openbb_charting import Charting
         > Charting.indicators()
         """
-        has_data = (isinstance(data, (pd.DataFrame, pd.Series)) and not data.empty) or (
-            data
-        )
-        index = (
-            data.index.name
-            if has_data and isinstance(data, (pd.DataFrame, pd.Series))
-            else None
-        )
-        data_as_df: pd.DataFrame = (
-            basemodel_to_df(convert_to_basemodel(data), index=index)
-            if has_data
-            else self._obbject.to_dataframe()
-        )
-        if "date" in data_as_df.columns:
-            data_as_df = data_as_df.set_index("date")
+        data_as_df, has_data = self._prepare_data_as_df(data)  # type: ignore
         try:
             fig, content = to_chart(
                 data_as_df,
                 indicators=indicators,
                 symbol=symbol,
                 candles=candles,
                 volume=volume,
@@ -208,7 +224,48 @@
             try:
                 if has_data:
                     self.show(data=data_as_df, symbol=symbol, render=render, **kwargs)
                 else:
                     self.show(**kwargs)
             except Exception as e:
                 raise RuntimeError("Could not create chart from the OBBject.") from e
+
+    def table(
+        self,
+        data: Optional[Union[pd.DataFrame, pd.Series]] = None,
+        title: str = "",
+    ):
+        """
+        Display an interactive table.
+
+        Parameters
+        ----------
+        data : Optional[Union[pd.DataFrame, pd.Series]], optional
+            Data to be plotted, by default None.
+            If no data is provided the OBBject results will be used.
+        """
+        data_as_df, _ = self._prepare_data_as_df(data)
+        if isinstance(data_as_df.index, pd.RangeIndex):
+            data_as_df.reset_index(inplace=True, drop=True)
+        else:
+            data_as_df.reset_index(inplace=True)
+        if self._backend.isatty:
+            try:
+                self._backend.send_table(
+                    df_table=data_as_df,
+                    title=title
+                    or self._obbject._route,  # pylint: disable=protected-access
+                    theme=self._charting_settings.table_style,
+                )
+            except Exception as e:
+                warn(f"Failed to show figure with backend. {e}")
+
+        else:
+            from plotly import (  # pylint:disable=import-outside-toplevel
+                optional_imports,
+            )
+
+            ipython_display = optional_imports.get_module("IPython.display")
+            if ipython_display:
+                ipython_display.display(ipython_display.HTML(data_as_df.to_html()))
+            else:
+                warn("IPython.display is not available.")
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/charting_router.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/charting_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     def __init__(
         self,
         charting_settings: "ChartingSettings",
         daemon: bool = True,
         max_retries: int = 30,
         proc_name: str = "OpenBB Terminal",
     ):
+        """Create a new instance of the backend."""
         self.charting_settings = charting_settings
 
         has_version = hasattr(PyWry, "__version__")
         init_kwargs: Dict[str, Any] = dict(daemon=daemon, max_retries=max_retries)
 
         if has_version and version.parse(PyWry.__version__) >= version.parse("0.4.8"):
             init_kwargs.update(dict(proc_name=proc_name))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""OpenBB Charting Styles."""
+
 from typing import Any, List, Optional
 
 import pandas as pd
 
 # Vsurf Plot Settings
 PLT_3DMESH_COLORSCALE = "Jet"
 PLT_3DMESH_SCENE = dict(
@@ -149,16 +151,17 @@
 def de_increasing_color_list(
     df_column: Optional[pd.DataFrame] = None,
     text: Optional[str] = None,
     contains_str: str = "-",
     increasing_color: str = PLT_STYLE_INCREASING,
     decreasing_color: str = PLT_STYLE_DECREASING,
 ) -> List[str]:
-    """Makes a colorlist for decrease/increase if value in df_column
-    contains "{contains_str}" default is "-"
+    """Make a colorlist for decrease/increase if value in df_column.
+
+    Contains "{contains_str}" default is "-"
 
     Parameters
     ----------
     df_column : pd.DataFrame, optional
         Dataframe column to create colorlist. by default None
     text : str, optional
         Search in a string, by default None
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Dummy backend for charting to avoid import errors."""
+
 import asyncio
 import warnings
 from queue import Queue
 from typing import List
 
 import dotenv
 from openbb_core.app.constants import OPENBB_DIRECTORY
@@ -48,32 +50,32 @@
     def __new__(cls, *args, **kwargs):  # pylint: disable=W0613
         """Create a singleton instance of the backend."""
         if not hasattr(cls, "instance"):
             cls.instance = super().__new__(cls)  # pylint: disable=E1120
         return cls.instance
 
     def __init__(self, daemon: bool = True, max_retries: int = 30):
-        """Dummy init to avoid import errors."""
+        """Use cummy init to avoid import errors."""
         self.daemon = daemon
         self.max_retries = max_retries
         try:
             self.loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()
         except RuntimeError:
             self.loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self.loop)
 
         if Env().DEBUG_MODE:
             warnings.warn(pywry_missing)
         dotenv.set_key(SETTINGS_ENV_FILE, "PLOT_ENABLE_PYWRY", "0")
 
     def close(self, reset: bool = False):  # pylint: disable=W0613
-        pass
+        """Close the backend."""
 
     def start(self, debug: bool = False):  # pylint: disable=W0613
-        pass
+        """Start the backend."""
 
     def send_outgoing(self, outgoing: dict):
-        pass
+        """Send outgoing data to the backend."""
 
     async def check_backend(self):
-        """Dummy check backend method to avoid errors and revert to browser."""
+        """Check backend method to avoid errors and revert to browser."""
         raise Exception
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     to_subplot(subplot: `OpenBBFigure`, row: `int`, col: `int`, secondary_y: `bool`, ...)
         Returns the figure as a subplot of another figure
     """
 
     plotlyjs_path: Path = PLOTLYJS_PATH
 
     def __init__(self, fig: Optional[go.Figure] = None, **kwargs) -> None:
+        """Initialize the OpenBBFigure."""
         super().__init__()
         if fig:
             self.__dict__ = fig.__dict__
 
         self._charting_settings: Optional["ChartingSettings"] = kwargs.pop(
             "charting_settings", None
         )
@@ -234,16 +235,15 @@
         self,
         data: pd.DataFrame,
         row: int = 1,
         col: int = 1,
         secondary_y: bool = False,
         **kwargs,
     ):
-        """
-        Add a trend line to the figure.
+        """Add a trend line to the figure.
 
         Parameters
         ----------
         data : `pd.DataFrame`
             Data to plot
         row : `int`, optional
             Row number, by default 1
@@ -287,16 +287,15 @@
         show_curve: bool = True,
         show_rug: bool = True,
         show_hist: bool = True,
         forecast: bool = False,
         row: int = 1,
         col: int = 1,
     ) -> None:
-        """
-        Add a histogram with a curve and rug plot if desired.
+        """Add a histogram with a curve and rug plot if desired.
 
         Parameters
         ----------
         dataset : `Union[np.ndarray, pd.Series, TimeSeriesT]`
             Data to plot
         name : `Optional[Union[str, List[str]]]`, optional
             Name of the plot, by default None
@@ -556,16 +555,15 @@
         self,
         y: float,
         name: str,
         line: Optional[dict] = None,
         legendrank: Optional[int] = None,
         **kwargs,
     ) -> None:
-        """
-        Add a horizontal line with a legend label.
+        """Add a horizontal line with a legend label.
 
         Parameters
         ----------
         y : `float`
             y value of the line
         name : `str`
             Name of the to display in the legend
@@ -594,16 +592,15 @@
         self,
         x: float,
         name: str,
         line: Optional[dict] = None,
         legendrank: Optional[int] = None,
         **kwargs,
     ) -> None:
-        """
-        Add a vertical line with a legend label.
+        """Add a vertical line with a legend label.
 
         Parameters
         ----------
         x : `float`
             x value of the line
         name : `str`
             Name of the to display in the legend
@@ -663,16 +660,15 @@
             )
         )
 
     @staticmethod
     def chart_volume_scaling(
         df_volume: pd.DataFrame, volume_ticks_x: int = 7
     ) -> Dict[str, list]:
-        """
-        Takes df_volume and returns volume_ticks, tickvals for chart volume scaling.
+        """Take df_volume and returns volume_ticks, tickvals for chart volume scaling.
 
         Parameters
         ----------
         df_volume : pd.DataFrame
             Dataframe of volume (e.g. df_volume = df["volume"])
         volume_ticks_x : int, optional
             Number to multiply volume, by default 7
@@ -712,16 +708,15 @@
         df_stock: pd.DataFrame,
         close_col: Optional[str] = "close",
         volume_col: Optional[str] = "volume",
         row: Optional[int] = 1,
         col: Optional[int] = 1,
         volume_ticks_x: int = 7,
     ) -> None:
-        """
-        Add in-chart volume to a subplot.
+        """Add in-chart volume to a subplot.
 
         Parameters
         ----------
         df_stock : `pd.DataFrame`
             Dataframe of the stock
         close_col : `str`, optional
             Name of the close column, by default "close"
@@ -842,16 +837,15 @@
     def show(  # noqa: PLR0915
         self,
         *args,
         external: bool = False,
         export_image: Optional[Union[Path, str]] = "",
         **kwargs,
     ) -> "OpenBBFigure":
-        """
-        Show the figure.
+        """Show the figure.
 
         Parameters
         ----------
         external : `bool`, optional
             Whether to return the figure object instead of showing it, by default False
         export_image : `Union[Path, str]`, optional
             The path to export the figure image to, by default ""
@@ -1230,16 +1224,15 @@
             self.update_yaxes(tickfont=dict(size=13))
 
         return super().to_html(*args, **kwargs)
 
     def to_plotly_json(
         self, ndarray: bool = False, np_nan: bool = False
     ) -> Dict[str, Any]:
-        """
-        Convert figure to a JSON representation as a Python dict.
+        """Convert figure to a JSON representation as a Python dict.
 
         Parameters
         ----------
         ndarray : `bool`, optional
             If the plotly json should contain np.ndarray, by default False
 
         np_nan : `bool`, optional
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     def __init__(
         self,
         func: Callable,
         name: str = "",
         **attrs: Any,
     ) -> None:
+        """Initialize the indicator."""
         self.func = func
         self.name = name
         self.attrs = attrs
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Call the indicator function."""
         return self.func(*args, **kwargs)
@@ -81,14 +82,15 @@
 
     def __iter__(cls: Type["PluginMeta"]) -> Iterator[Indicator]:  # type: ignore
         """Iterate over the indicators."""
         return iter(cls.__indicators__)
 
     # pylint: disable=unused-argument
     def __init__(cls, *args: Any, **kwargs: Any) -> None:
+        """Initialize the class."""
         super().__init__(*args, **kwargs)
 
 
 class PltTA(metaclass=PluginMeta):
     """The base class that all Plotly plugins must inherit from."""
 
     indicators: ChartIndicators
@@ -178,27 +180,27 @@
                 delattr(self, static_method)
 
     def __iter__(self) -> Iterator[Indicator]:
         """Iterate over the indicators."""
         return iter(self.__indicators__)
 
     def get_float_precision(self) -> str:
-        """Returns f-string precision format."""
+        """Return f-string precision format."""
         price = self.df_stock[self.close_column].tail(1).values[0]
         float_precision = (
             ",.2f" if price > 1.10 else "" if len(str(price)) < 8 else ".6f"
         )
         return float_precision
 
 
 def indicator(
     name: str = "",
     **attrs: Any,
 ) -> Callable:
-    """Decorator for adding indicators to a plugin class."""
+    """Use this decorator for adding indicators to a plugin class."""
     attrs["name"] = name
 
     def decorator(func: Callable) -> Indicator:
         if not attrs.pop("name", ""):
             name = func.__name__
 
         return Indicator(func, name, **attrs)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+"""Overlap technical indicators plugin for Plotly TA."""
+
 import warnings
 
 import pandas as pd
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
     columns_regex,
 )
 
 
 class Overlap(PltTA):
-    """Overlap technical indicators"""
+    """Overlap technical indicators."""
 
     __inchart__ = ["vwap"]
     __ma_mode__ = ["sma", "ema", "wma", "hma", "zlma", "rma"]
 
     @indicator()
     def plot_ma(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
-        """Adds moving average to plotly figure"""
+        """Add moving average to plotly figure."""
         check_ma = [ma for ma in self.ma_mode if ma in self.indicators.get_active_ids()]
         if check_ma:
             for ma in check_ma:
                 column_names = columns_regex(df_ta, ma.upper())
                 try:
                     for column in column_names:
                         if df_ta[column].empty:
@@ -61,15 +63,15 @@
                 except Exception as e:
                     warnings.warn(f"Error adding {ma.upper()} to plot - {e}")
 
         return fig, inchart_index
 
     @indicator()
     def plot_vwap(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
-        """Adds vwap to plotly figure"""
+        """Add vwap to plotly figure."""
         fig.add_scatter(
             name=columns_regex(df_ta, "VWAP_")[0],
             mode="lines",
             line=dict(width=1.5, color=self.inchart_colors[inchart_index]),
             x=df_ta.index,
             y=df_ta[columns_regex(df_ta, "VWAP_")[0]].values,
             opacity=0.8,
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Trend technical indicators."""
+
 import pandas as pd
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
@@ -90,15 +92,15 @@
         )
         fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_aroon(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
-        """Adds aroon to plotly figure"""
+        """Add aroon to plotly figure."""
         aroon_up_col = columns_regex(df_ta, "AROONU")[0]
         aroon_down_col = columns_regex(df_ta, "AROOND")[0]
         aroon_osc_col = columns_regex(df_ta, "AROONOSC")[0]
         fig.add_scatter(
             name="Aroon Up",
             mode="lines",
             line=dict(width=1.5, color=fig.theme.up_color),
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+"""Volatility technical indicators plugin for Plotly TA."""
+
 import pandas as pd
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
     columns_regex,
 )
 
 
 class Volatility(PltTA):
-    """Volatility technical indicators"""
+    """Volatility technical indicators."""
 
     __inchart__ = ["bbands", "donchian", "kc"]
     __subplots__ = ["atr"]
 
     @indicator()
     def plot_atr(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
-        """Adds average true range to plotly figure"""
-
+        """Add average true range to plotly figure."""
         fig.add_scatter(
             name=f"{columns_regex(df_ta, 'ATR')[0]}",
             x=df_ta.index,
             y=df_ta[columns_regex(df_ta, "ATR")[0]].values,
             mode="lines",
             line=dict(width=1, color=fig.theme.get_colors()[1]),
             row=subplot_row,
@@ -43,16 +44,15 @@
         )
         fig["layout"][f"yaxis{subplot_row}"].update(nticks=5, autorange=True)
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_bbands(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
-        """Adds bollinger bands to plotly figure"""
-
+        """Add bollinger bands to plotly figure."""
         bbands_opacity = 0.8 if fig.theme.plt_style == "light" else 1
 
         fig.add_scatter(
             name=f"{columns_regex(df_ta, 'BBU')[0]}",
             x=df_ta.index,
             y=df_ta[columns_regex(df_ta, "BBU")[0]].values,
             opacity=bbands_opacity,
@@ -103,16 +103,15 @@
             opacity=0.9,
         )
 
         return fig, inchart_index + 1
 
     @indicator()
     def plot_donchian(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
-        """Adds donchian channels to plotly figure"""
-
+        """Add donchian channels to plotly figure."""
         if fig.theme.plt_style == "light":
             fillcolor = "rgba(239, 103, 137, 0.05)"
             donchian_opacity = 0.4
         else:
             fillcolor = "rgba(239, 103, 137, 0.05)"
             donchian_opacity = 0.4
 
@@ -162,15 +161,15 @@
             opacity=0.9,
         )
 
         return fig, inchart_index + 1
 
     @indicator()
     def plot_kc(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
-        """Adds Keltner channels to plotly figure"""
+        """Add Keltner channels to plotly figure."""
         mamode = (self.params["kc"].get_argument_values("mamode") or "ema").lower()  # type: ignore
 
         if fig.theme.plt_style == "light":
             fillcolor = "rgba(239, 103, 137, 0.05)"
             kc_opacity = 0.4
         else:
             fillcolor = "rgba(239, 103, 137, 0.05)"
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Volume technical indicators."""
+
 import pandas as pd
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
@@ -16,15 +18,15 @@
 
     # Useless super delegation
     # def __init__(self, *args, **kwargs):
     #     super().__init__(*args, **kwargs)
 
     @indicator()
     def plot_ad(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
-        """Adds ad to plotly figure"""
+        """Add ad to plotly figure."""
         ad_col = columns_regex(df_ta, "AD")[0]
         fig.add_scatter(
             name="AD",
             mode="lines",
             line=dict(width=1.5, color=fig.theme.get_colors()[1]),
             x=df_ta.index,
             y=df_ta[ad_col].values,
@@ -58,15 +60,15 @@
         )
         fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=3, autorange=True)
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_adosc(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
-        """Adds adosc to plotly figure"""
+        """Add adosc to plotly figure."""
         ad_col = columns_regex(df_ta, "ADOSC")[0]
         fig.add_scatter(
             name="ADOSC",
             mode="lines",
             line=dict(width=1.5, color=fig.theme.get_colors()[1]),
             x=df_ta.index,
             y=df_ta[ad_col].values,
@@ -88,15 +90,15 @@
             font_color=fig.theme.get_colors()[1],
         )
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_obv(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
-        """Adds obv to plotly figure"""
+        """Add obv to plotly figure."""
         obv_col = columns_regex(df_ta, "OBV")[0]
         fig.add_scatter(
             name="OBV",
             mode="lines",
             line=dict(width=1.5, color=fig.theme.get_colors()[1]),
             x=df_ta.index,
             y=df_ta[obv_col].values,
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,18 @@
     has_volume: bool = True
     show_volume: bool = True
     prepost: bool = False
     charting_settings: Optional["ChartingSettings"] = None
     theme: Optional[ChartStyle] = None
 
     def __new__(cls, *args, **kwargs):
-        """Method is overridden to create a singleton instance of the class."""
+        """Create a new instance of the class.
+
+        Method is overridden to create a singleton instance of the class.
+        """
         cls.charting_settings = kwargs.pop("charting_settings", cls.charting_settings)
         cls.theme = cls.setup_theme(
             chart_style=getattr(cls.charting_settings, "chart_style", ""),
             user_styles_directory=getattr(
                 cls.charting_settings, "user_styles_directory", ""
             ),
         )
@@ -117,24 +120,27 @@
                 getattr(cls.charting_settings, "debug_mode", False)
             )
             PLOTLY_TA.add_plugins(PLOTLY_TA.plugins)  # type: ignore[attr-defined, assignment]
 
         return PLOTLY_TA
 
     def __init__(self, *args, **kwargs):
-        """Method is overridden to do nothing, except to clear the internal data structures."""
+        """Initialize the class.
+
+        Method is overridden to do nothing, except to clear the internal data structures.
+        """
         if not args and not kwargs:
             self._clear_data()
         else:
             self.df_fib = None
             super().__init__(*args, **kwargs)
 
     @staticmethod
     def setup_theme(chart_style, user_styles_directory) -> ChartStyle:
-        """Setup theme for charting."""
+        """Set up theme for charting."""
         return ChartStyle(chart_style, user_styles_directory)
 
     @property
     def ma_mode(self) -> List[str]:
         """List of available moving average modes."""
         return list(set(self.__ma_mode__))
 
@@ -171,15 +177,18 @@
         symbol: str = "",
         candles: bool = True,
         volume: bool = True,
         prepost: bool = False,
         fig: Optional[OpenBBFigure] = None,
         volume_ticks_x: int = 7,
     ) -> OpenBBFigure:
-        """Method should not be called directly. Use the PlotlyTA.plot() static method instead."""
+        """Do not call this directly.
+
+        Use the PlotlyTA.plot() static method instead.
+        """
         if isinstance(df_stock, pd.Series):
             df_stock = df_stock.to_frame()
 
         if not isinstance(indicators, ChartIndicators):
             indicators = ChartIndicators.from_dict(indicators or {})
 
         # Apply to_datetime to the index in a way that handles daylight savings.
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+"""Helper functions for technical analysis indicators."""
+
 import re
 from typing import Optional
 
 import pandas as pd
 
 
 def check_columns(
     data: pd.DataFrame, high: bool = True, low: bool = True, close: bool = True
 ) -> Optional[str]:
-    """Returns the close columns, or None if the dataframe does not have required columns
+    """Return the close columns, or None if the dataframe does not have required columns.
 
     Parameters
     ----------
     data: pd.DataFrame
         The dataframe to check
     high: bool
         Whether to check for high column
@@ -20,15 +22,14 @@
     close: bool
         Whether to check for close column
 
     Returns
     -------
     Optional[str]
         The name of the close column, none if df is invalid
-
     """
     close_regex = r"(Adj\sClose|adj_close|Close)"
     # pylint: disable=too-many-boolean-expressions
     if (
         (re.findall(r"High", str(data.columns), re.IGNORECASE) is None and high)
         or (re.findall(r"Low", str(data.columns), re.IGNORECASE) is None and low)
         or (close_col := re.findall(close_regex, str(data.columns), re.IGNORECASE))
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     indicators: Optional[Union[ChartIndicators, Dict[str, Dict[str, Any]]]] = None,
     symbol: str = "",
     candles: bool = True,
     volume: bool = True,
     prepost: bool = False,
     volume_ticks_x: int = 7,
 ) -> Tuple[OpenBBFigure, Dict[str, Any]]:
-    """
-    Returns the plotly json representation of the chart.
+    """Return the plotly json representation of the chart.
 
     This function is used so it can be called at the module level and used out of the box,
     which allows some more flexibility, ease of use and doesn't require the user to know
     about the PlotlyTA class.
 
     Parameters
     ----------
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/obbject_extensions/charting/openbb_charting/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/assets/reference.json` & `openbb_nightly-4.1.6.dev202404100009/openbb/assets/reference.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9749954259367681%*

 * *Differences: {"'paths'": "{'/etf/holdings': {'parameters': {'intrinio': [OrderedDict([('name', 'date'), "*

 * *            "('type', 'Union[date, str]'), ('description', 'A specific date to get data for.'), "*

 * *            "('default', None), ('optional', True)])]}}}",*

 * * "'routers'": "{'/derivatives': OrderedDict([('description', 'Derivatives market data.')]), "*

 * *              "'/regulators': OrderedDict([('description', 'Financial market regulators data.')])}"}*

```diff
@@ -21360,15 +21360,23 @@
                         "default": null,
                         "description": "The CIK of the filing entity. Overrides symbol.",
                         "name": "cik",
                         "optional": true,
                         "type": "str"
                     }
                 ],
-                "intrinio": [],
+                "intrinio": [
+                    {
+                        "default": null,
+                        "description": "A specific date to get data for.",
+                        "name": "date",
+                        "optional": true,
+                        "type": "Union[date, str]"
+                    }
+                ],
                 "sec": [
                     {
                         "default": null,
                         "description": "A specific date to get data for. The date represents the period ending. The date entered will return the closest filing.",
                         "name": "date",
                         "optional": true,
                         "type": "Union[Union[str, date], str]"
@@ -27169,14 +27177,17 @@
     "routers": {
         "/crypto": {
             "description": "Cryptocurrency market data."
         },
         "/currency": {
             "description": "Foreign exchange (FX) market data."
         },
+        "/derivatives": {
+            "description": "Derivatives market data."
+        },
         "/economy": {
             "description": "Economic data."
         },
         "/equity": {
             "description": "Equity market data."
         },
         "/etf": {
@@ -27186,10 +27197,13 @@
             "description": "Fixed Income market data."
         },
         "/index": {
             "description": "Indices data."
         },
         "/news": {
             "description": "Financial market news data."
+        },
+        "/regulators": {
+            "description": "Financial market regulators data."
         }
     }
 }
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/__extensions__.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/crypto.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/crypto_price.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/currency.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/currency.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/currency_price.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/currency_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/derivatives.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives_options.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/economy.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/economy.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_compare.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_fundamental.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_price.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_shorts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/etf.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/etf.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,14 +388,15 @@
             Symbol to get data for. (ETF)
         provider : Optional[Literal['fmp', 'intrinio', 'sec']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
         date : Optional[Union[str, datetime.date]]
             A specific date to get data for. Entering a date will attempt to return the NPORT-P filing for the entered date. This needs to be _exactly_ the date of the filing. Use the holdings_date command/endpoint to find available filing dates for the ETF. (provider: fmp);
+            A specific date to get data for. (provider: intrinio);
             A specific date to get data for.  The date represents the period ending. The date entered will return the closest filing. (provider: sec)
         cik : Optional[str]
             The CIK of the filing entity. Overrides symbol. (provider: fmp)
         use_cache : bool
             Whether or not to use cache for the request. (provider: sec)
 
         Returns
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_corporate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/index.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/index.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/news.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/openbb/package/regulators_sec.py` & `openbb_nightly-4.1.6.dev202404100009/openbb/package/regulators_sec.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,26 +153,26 @@
         if "INTRADAY" in function:
             query_str += f"&interval={interval}&extended_hours={str(query.extended_hours).lower()}"
             intraday = True
 
         results = []
 
         async def callback(response, _):
-            """Callback function to process the response."""
+            """Use callback function to process the response."""
             try:
                 result = await response.json()
                 if "Information" in result:
                     warn(str(result.get("Information")))
             except Exception as _:
                 # TODO: This is hacky, find a better solution.
                 return await response.read()
             return await response.read()
 
         async def intraday_callback(response, _):
-            """Callback function to process the intraday response."""
+            """Use callback function to process the intraday response."""
             symbol = response.url.query.get("symbol", None)
             data = await response.read()
             if data:
                 df = read_csv(BytesIO(data))
                 if len(df) > 0:
                     df.rename(
                         columns={
@@ -185,15 +185,14 @@
                 results.extend(df.to_dict("records"))
             if not data:
                 warn(f"Symbol Error: No data found for {symbol}")
             return results
 
         async def get_one(symbol, intraday: bool = False):
             """Get data for one symbol."""
-
             if intraday is True:
                 adjusted = query.adjustment != "unadjusted"
                 if query.adjustment == "splits_only":
                     warn(
                         "Intraday does not support 'splits_only'. Using 'splits_and_dividends' instead."
                     )
                 url = (
@@ -294,15 +293,14 @@
         return results
 
     @staticmethod
     def transform_data(
         query: AVEquityHistoricalQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[AVEquityHistoricalData]:
         """Transform the data to the standard format."""
-
         if data == []:
             return []
         if "{" in data[0]:
             warn(str(data[0]["{"].strip()))
             return []
         return [
             AVEquityHistoricalData.model_validate(d)
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,30 @@
             <= end_date,
             data,
         )
     )
 
 
 def calculate_adjusted_prices(df: pd.DataFrame, column: str, dividends: bool = False):
-    """Calculates the split-adjusted prices, or split and dividend adjusted prices.
+    """Calculate the split-adjusted prices, or split and dividend adjusted prices.
 
     Parameters
-    ------------
+    ----------
     df: pd.DataFrame
         DataFrame with unadjusted OHLCV values + split_factor + dividend
     column: str
         The column name to adjust.
     dividends: bool
         Whether to adjust for both splits and dividends. Default is split-adjusted only.
 
     Returns
-    --------
+    -------
     pd.DataFrame
         DataFrame with adjusted prices.
     """
-
     df = df.copy()
     adj_column = "adj_" + column
 
     # Reverse the DataFrame order, sorting by date in descending order
     df.sort_index(ascending=False, inplace=True)
 
     price_col = df[column].values
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,15 @@
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="3y_stdev",
     )
 
     @field_validator("last_updated", mode="before", check_fields=False)
     @classmethod
     def validate_date(cls, v):
+        """Validate date."""
         if v:
             dt = datetime.fromtimestamp(v, UTC)
             return dt.date() if dt.time() == dt.min.time() else dt
         return v
 
     @model_validator(mode="before")
     @classmethod
@@ -336,15 +337,14 @@
     @staticmethod
     async def aextract_data(
         query: BenzingaAnalystSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the raw data."""
-
         token = credentials.get("benzinga_api_key") if credentials else ""
         querystring = get_querystring(query.model_dump(), [])
         url = f"https://api.benzinga.com/api/v2.1/calendar/ratings/analysts?{querystring}&token={token}"
         response = await amake_request(url, **kwargs)
 
         if not response:
             raise EmptyDataError()
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,96 +1,95 @@
-"""Biztoc Helpers"""
+"""Biztoc Helpers."""
 
 from datetime import timedelta
 from typing import Dict, List, Literal
 
 import requests
 import requests_cache
 from openbb_core.app.utils import get_user_cache_directory
 
+# pylint: disable=C0325
+
 cache_dir = get_user_cache_directory()
 
 biztoc_session_tags = requests_cache.CachedSession(
     f"{cache_dir}/http/biztoc_tags", expire_after=timedelta(days=1)
 )
 biztoc_session_sources = requests_cache.CachedSession(
     f"{cache_dir}/http/biztoc_sources", expire_after=timedelta(days=3)
 )
 
 
 def get_sources(api_key: str) -> List[Dict]:
-    """Valid sources for Biztoc queries."""
-
+    """Get valid sources for Biztoc queries."""
     headers = {
         "X-RapidAPI-Key": f"{api_key}",
         "X-RapidAPI-Host": "biztoc.p.rapidapi.com",
         "Accept": "application/json",
         "Accept-Encoding": "gzip",
     }
     sources = biztoc_session_sources.get(
         "https://biztoc.p.rapidapi.com/sources", headers=headers, timeout=10
     )
 
     return sources.json()
 
 
 def get_pages(api_key: str) -> List[str]:
-    """Valid pages for Biztoc queries."""
-
+    """Get valid pages for Biztoc queries."""
     headers = {
         "X-RapidAPI-Key": f"{api_key}",
         "X-RapidAPI-Host": "biztoc.p.rapidapi.com",
         "Accept": "application/json",
         "Accept-Encoding": "gzip",
     }
     pages = biztoc_session_sources.get(
         "https://biztoc.p.rapidapi.com/pages", headers=headers, timeout=10
     )
 
     return pages.json()
 
 
 def get_tags_by_page(page_id: str, api_key: str) -> List[str]:
-    """Valid tags required for Biztoc queries."""
-
+    """Get valid tags required for Biztoc queries."""
     headers = {
         "X-RapidAPI-Key": f"{api_key}",
         "X-RapidAPI-Host": "biztoc.p.rapidapi.com",
         "Accept": "application/json",
         "Accept-Encoding": "gzip",
     }
     tags = biztoc_session_tags.get(
         f"https://biztoc.p.rapidapi.com/tags/{page_id}", headers=headers, timeout=10
     )
 
     return tags.json()
 
 
 def get_all_tags(api_key) -> Dict[str, List[str]]:
+    """Get all tags for all pages."""
     tags: Dict[str, List[str]] = {}
 
     pages = get_pages(api_key)
     for page in pages:
         page_tags = get_tags_by_page(page, api_key)
-        tags.update({page: [x["tag"] for x in page_tags]})
+        tags.update({page: [x["tag"] for x in page_tags]})  # type: ignore
 
     return tags
 
 
 def get_news(
     api_key: str,
     filter_: Literal[
         "crypto", "hot", "latest", "main", "media", "source", "tag"
     ] = "latest",
     source: str = "bloomberg",
     tag: str = "",
     term: str = "",
 ) -> List[Dict]:
-    """Calls the BizToc API and returns the data."""
-
+    """Call the BizToc API and returns the data."""
     results = []
     term = term.replace(" ", "%20") if term else ""
     _tags = get_all_tags(api_key)
     pages = get_pages(api_key)
     tags = []
     tag = tag.lower() if tag else ""
     for page in pages:
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         List[CboeFuturesCurveData],
     ]
 ):
     """Transform the query, extract and transform the data from the CBOE endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> CboeFuturesCurveQueryParams:
+        """Transform the query."""
         return CboeFuturesCurveQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: CboeFuturesCurveQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the CBOE endpoint."""
-
         symbol = query.symbol.upper().split(",")[0]
         FUTURES = await get_settlement_prices(**kwargs)
         if len(FUTURES) == 0:
             raise EmptyDataError()
 
         if symbol not in FUTURES["product"].unique().tolist():
             raise RuntimeError(
@@ -64,8 +64,9 @@
 
     @staticmethod
     def transform_data(
         query: CboeFuturesCurveQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[CboeFuturesCurveData]:
+        """Transform data."""
         return [CboeFuturesCurveData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Cboe Helpers"""
+"""Cboe Helpers."""
 
 # pylint: disable=expression-not-assigned, unused-argument
 
 from datetime import date as dateType
 from io import BytesIO, StringIO
 from typing import Any, List, Literal, Optional
 
@@ -77,48 +77,47 @@
 ]
 
 cache_dir = get_user_cache_directory()
 backend = SQLiteBackend(f"{cache_dir}/http/cboe_directories", expire_after=3600 * 24)
 
 
 async def response_callback(response: ClientResponse, _: Any):
-    """Callback for HTTP Client Response."""
+    """Use callback for HTTP Client Response."""
     content_type = response.headers.get("Content-Type", "")
     if "application/json" in content_type:
         return await response.json()
     if "text" in content_type:
         return await response.text()
     return await response.read()
 
 
 async def get_cboe_data(url, use_cache: bool = True, **kwargs) -> Any:
-    """Generic Cboe HTTP request."""
+    """Use the generic Cboe HTTP request."""
     if use_cache is True:
         async with CachedSession(cache=backend) as cached_session:
             try:
                 response = await cached_session.get(url, timeout=10, **kwargs)
                 data = await response_callback(response, None)
             finally:
                 await cached_session.close()
     else:
         data = await amake_request(url, response_callback=response_callback)
 
     return data
 
 
 async def get_company_directory(use_cache: bool = True, **kwargs) -> DataFrame:
-    """
-    Get the US Company Directory for Cboe options. If use_cache is True,
-    the data will be cached for 24 hours.
+    """Get the US Company Directory for Cboe options.
+
+    If use_cache is True, the data will be cached for 24 hours.
 
     Returns
     -------
     DataFrame: Pandas DataFrame of the Cboe listings directory
     """
-
     url = "https://www.cboe.com/us/options/symboldir/equity_index_options/?download=csv"
 
     results = await get_cboe_data(url, use_cache)
 
     response = BytesIO(results)
 
     directory = read_csv(response)
@@ -132,23 +131,22 @@
         }
     ).set_index("symbol")
 
     return directory.astype(str)
 
 
 async def get_index_directory(use_cache: bool = True, **kwargs) -> DataFrame:
-    """
-    Get the Cboe Index Directory. If use_cache is True,
-    the data will be cached for 24 hours.
+    """Get the Cboe Index Directory.
+
+    If use_cache is True, the data will be cached for 24 hours.
 
     Returns
-    --------
+    -------
     List[Dict]: A list of dictionaries containing the index information.
     """
-
     url = "https://cdn.cboe.com/api/global/us_indices/definitions/all_indices.json"
 
     results = await get_cboe_data(url, use_cache=use_cache)
 
     [result.pop("featured") for result in results]
     [result.pop("featured_order") for result in results]
     [result.pop("display") for result in results]
@@ -158,19 +156,18 @@
     return results
 
 
 async def list_futures(**kwargs) -> List[dict]:
     """List of CBOE futures and their underlying symbols.
 
     Returns
-    --------
+    -------
     pd.DataFrame
         Pandas DataFrame with results.
     """
-
     r = await get_cboe_data(
         "https://cdn.cboe.com/api/global/delayed_quotes/symbol_book/futures-roots.json"
     )
     data = r.get("data")
     [d.pop("sort_order") for d in data]
 
     return data
@@ -179,18 +176,18 @@
 async def get_settlement_prices(
     settlement_date: Optional[dateType] = None,
     options: bool = False,
     archives: bool = False,
     final_settlement: bool = False,
     **kwargs,
 ) -> DataFrame:
-    """Gets the settlement prices of CBOE futures.
+    """Get the settlement prices of CBOE futures.
 
     Parameters
-    -----------
+    ----------
     settlement_date: Optional[date]
         The settlement date. Only valid for active contracts. [YYYY-MM-DD]
     options: bool
         If true, returns options on futures.
     archives: bool
         Settlement price archives for select years and products.  Overridden by other parameters.
     final_settlement: bool
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# Helper functions for FINRA API
+"""Helper functions for FINRA API."""
+
 import datetime
 from typing import List
 
 import requests
 
+# pylint: disable=W0621
+
 
 def get_finra_weeks(tier: str = "T1", is_ats: bool = True):
-    """Fetches the available weeks from FINRA that can be used."""
+    """Fetch the available weeks from FINRA that can be used."""
     request_header = {"Accept": "application/json", "Content-Type": "application/json"}
 
     request_data = {
         "compareFilters": [
             {
                 "compareType": "EQUAL",
                 "fieldName": "summaryTypeCode",
@@ -36,14 +39,15 @@
         timeout=3,
     )
 
     return response.json() if response.status_code == 200 else []
 
 
 def get_finra_data(symbol, week_start, tier: str = "T1", is_ats: bool = True):
+    """Get the data for a symbol from FINRA."""
     req_hdr = {
         "Accept": "application/json",
         "Content-Type": "application/json",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) ",
     }
 
     filters = [
@@ -89,48 +93,51 @@
         json=req_data,
         timeout=2,
     )
     return response
 
 
 def get_full_data(symbol, tier: str = "T1", is_ats: bool = True):
+    """Get the full data for a symbol from FINRA."""
     weeks = [week["weekStartDate"] for week in get_finra_weeks(tier, is_ats)]
 
     data = []
     for week in weeks:
         response = get_finra_data(symbol, week, tier, is_ats)
         r_json = response.json()
         if response.status_code == 200 and r_json:
             data.append(response.json()[0])
 
     return data
 
 
 def get_adjusted_date(year, month, day):
+    """Find the closest date if the date falls on a weekend."""
     # Get the date
     date = datetime.date(year, month, day)
 
     # If the date is a Saturday, subtract one day
     if date.weekday() == 5:
         date -= datetime.timedelta(days=1)
     # If the date is a Sunday, subtract two days
     elif date.weekday() == 6:
         date -= datetime.timedelta(days=2)
 
     return date
 
 
 def get_short_interest_dates() -> List[str]:
-    """
-    Get a list of dates for which the short interest data is available.  It is reported on the 15th and the
-    last day of each month,but if the date falls on a weekend, the date is adjusted to the closest friday.
+    """Get a list of dates for which the short interest data is available.
+
+    It is reported on the 15th and the last day of each month,but if the date falls on a weekend,
+    the date is adjusted to the closest friday.
     """
 
     def get_adjusted_date(year, month, day):
-        """If the date falls on a weekend, find the closest date"""
+        """Find the closest date if the date falls on a weekend."""
         # Get the date
         date = datetime.date(year, month, day)
 
         # If the date is a Saturday, subtract one day
         if date.weekday() == 5:
             date -= datetime.timedelta(days=1)
         # If the date is a Sunday, subtract two days
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         if v is not None and "%" in str(v):
             return float(v.replace("%", "")) / 100
         return v if v else None
 
     @field_validator("market_cap", "volume", mode="before", check_fields=False)
     @classmethod
     def validate_abbreviated_numbers(cls, v):
-        """Checks for abbreviated string values."""
+        """Check for abbreviated string values."""
         if v is not None and isinstance(v, str):
             v = (
                 v.replace("M", "e+6")
                 .replace("B", "e+9")
                 .replace("T", "e+12")
                 .replace("K", "e+3")
             )
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 )
 from pydantic import BaseModel
 
 
 async def response_callback(
     response: ClientResponse, _: ClientSession
 ) -> Union[Dict, List[Dict]]:
-    """Callback for make_request."""
-
+    """Use callback for make_request."""
     data = await response.json()
     if isinstance(data, dict) and "Error Message" in data:
         raise RuntimeError(f"FMP Error Message -> {data['Error Message']}")
 
     if isinstance(data, dict) and "error" in data:
         raise RuntimeError(
             f"FMP Error Message -> {data['error']}. Status code: {response.status}"
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""US Government Treasury Prices"""
+"""US Government Treasury Prices."""
 
 # pylint: disable=unused-argument
 import asyncio
 from datetime import datetime, timedelta
 from io import StringIO
 from typing import Any, Dict, List, Literal, Optional
 
@@ -34,20 +34,21 @@
 
 class GovernmentUSTreasuryPricesFetcher(
     Fetcher[
         GovernmentUSTreasuryPricesQueryParams,
         List[GovernmentUSTreasuryPricesData],
     ]
 ):
+    """US Government Treasury Prices Fetcher."""
+
     @staticmethod
     def transform_query(
         params: Dict[str, Any]
     ) -> GovernmentUSTreasuryPricesQueryParams:
         """Transform query params."""
-
         if params.get("date") is None:
             _date = datetime.now().date()
         else:
             _date = (
                 datetime.strptime(params["date"], "%Y-%m-%d").date()
                 if isinstance(params["date"], str)
                 else params["date"]
@@ -62,15 +63,14 @@
     @staticmethod
     async def aextract_data(
         query: GovernmentUSTreasuryPricesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> str:
         """Extract the raw data from US Treasury website."""
-
         url = "https://treasurydirect.gov/GA-FI/FedInvest/securityPriceDetail"
 
         HEADERS = {
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
             "Accept-Language": "en-CA,en-US;q=0.7,en;q=0.3",
             "Accept-Encoding": "gzip, deflate, br",
             "Referer": "https://treasurydirect.gov/",
@@ -106,15 +106,14 @@
     @staticmethod
     def transform_data(
         query: GovernmentUSTreasuryPricesQueryParams,
         data: str,
         **kwargs: Any,
     ) -> List[GovernmentUSTreasuryPricesData]:
         """Transform the data."""
-
         try:
             if not data:
                 raise EmptyDataError("Data not found")
             results = read_csv(StringIO(data), header=0)
             results.columns = Index(
                 [
                     "cusip",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     # pylint: disable=W0613:unused-argument
     @staticmethod
     def transform_data(
         query: IntrinioEquityInfoQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioEquityInfoData]:
-        """Transforms the data."""
+        """Transform the data."""
         return [IntrinioEquityInfoData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_holdings import (
     EtfHoldingsData,
     EtfHoldingsQueryParams,
 )
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_request,
 )
 from pydantic import Field, model_validator
 
@@ -21,14 +22,20 @@
 class IntrinioEtfHoldingsQueryParams(EtfHoldingsQueryParams):
     """
     Intrinio ETF Holdings Query Params.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_holdings_v2
     """
 
+    __alias_dict__ = {"date": "as_of_date"}
+
+    date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("date", "")
+    )
+
 
 class IntrinioEtfHoldingsData(EtfHoldingsData):
     """Intrinio ETF Holdings Data."""
 
     __alias_dict__ = {
         "symbol": "ticker",
         "security_type": "type",
@@ -141,21 +148,19 @@
     @staticmethod
     async def aextract_data(
         query: IntrinioEtfHoldingsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
-
         api_key = credentials.get("intrinio_api_key") if credentials else ""
-
         symbol = query.symbol + ":US" if ":" not in query.symbol else query.symbol
-
         URL = f"https://api-v2.intrinio.com/etfs/{symbol}/holdings?page_size=10000&api_key={api_key}"
-
+        if query.date:
+            URL += f"&as_of_date={query.date}"
         data = []
 
         async def response_callback(response: ClientResponse, session: ClientSession):
             """Async response callback."""
             results = await response.json()
 
             if results.get("error"):  # type: ignore
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                     results.extend(new_data)
 
         if symbols:
             await asyncio.gather(*[get_one(symbol) for symbol in symbols])
             return results
 
         async def fetch_callback(response, session):
-            """Callback for pagination."""
+            """Use callback for pagination."""
             data = await response.json()
             messages = data.get("messages", None)
             if messages:
                 raise RuntimeError(str(messages))
             if data.get("estimates") and len(data.get("estimates")) > 0:  # type: ignore
                 results.extend(data.get("estimates"))  # type: ignore
                 while data.get("next_page"):  # type: ignore
@@ -192,15 +192,14 @@
     @staticmethod
     def transform_data(
         query: IntrinioForwardEpsEstimatesQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioForwardEpsEstimatesData]:
         """Transform the raw data into the standard format."""
-
         symbols = query.symbol.split(",") if query.symbol else []
         results: List[IntrinioForwardEpsEstimatesData] = []
         for item in sorted(
             data,
             key=lambda item: (  # type: ignore
                 (
                     symbols.index(item.get("symbol")) if item.get("symbol") in symbols else len(symbols),  # type: ignore
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                     results.extend(new_data)
 
         if symbols:
             await asyncio.gather(*[get_one(symbol) for symbol in symbols])
             return results
 
         async def fetch_callback(response, session):
-            """Callback for pagination."""
+            """Use callback for pagination."""
             data = await response.json()
             messages = data.get("messages")
             if messages:
                 raise RuntimeError(str(messages))
             if data.get("estimates") and len(data.get("estimates")) > 0:  # type: ignore
                 results.extend(data.get("estimates"))  # type: ignore
                 while data.get("next_page"):  # type: ignore
@@ -211,15 +211,14 @@
     @staticmethod
     def transform_data(
         query: IntrinioForwardSalesEstimatesQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioForwardSalesEstimatesData]:
         """Transform the raw data into the standard format."""
-
         symbols = query.symbol.split(",") if query.symbol else []
         results: List[IntrinioForwardSalesEstimatesData] = []
         for item in sorted(
             data,
             key=lambda item: (  # type: ignore
                 (
                     symbols.index(item.get("symbol")) if item.get("symbol") in symbols else len(symbols),  # type: ignore
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Intrinio Historical Attributes Model."""
 
+# pylint: disable = unused-argument
+
 import warnings
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.app.model.abstract.warning import OpenBBWarning
 from openbb_core.provider.abstract.fetcher import Fetcher
@@ -58,79 +60,85 @@
         if params.get("end_date") is None:
             transformed_params["end_date"] = now
 
         return IntrinioHistoricalAttributesQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
-        query: IntrinioHistoricalAttributesQueryParams,  # pylint: disable=unused-argument
+        query: IntrinioHistoricalAttributesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
 
         base_url = "https://api-v2.intrinio.com"
         query_str = get_querystring(query.model_dump(by_alias=True), ["symbol", "tag"])
 
         def generate_url(symbol: str, tag: str) -> str:
-            """Returns the url for the given symbol and tag."""
+            """Return the url for the given symbol and tag."""
             url_params = f"{symbol}/{tag}?{query_str}&api_key={api_key}"
             url = f"{base_url}/historical_data/{url_params}"
             return url
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             """Return the response."""
             init_response = await response.json()
 
-            if message := init_response.get("error") or init_response.get("message"):
-                warnings.warn(message=message, category=OpenBBWarning)
+            if message := init_response.get(  # type: ignore
+                "error"
+            ) or init_response.get(  # type: ignore
+                "message"
+            ):
+                warnings.warn(message=str(message), category=OpenBBWarning)
                 return []
 
-            symbol = response.url.parts[-2]
-            tag = response.url.parts[-1]
+            symbol = response.url.parts[-2]  # type: ignore
+            tag = response.url.parts[-1]  # type: ignore
 
-            all_data: list = init_response.get("historical_data", [])
+            all_data: List = init_response.get("historical_data", [])  # type: ignore
             all_data = [{**item, "symbol": symbol, "tag": tag} for item in all_data]
 
-            next_page = init_response.get("next_page", None)
+            next_page = init_response.get("next_page", None)  # type: ignore
             while next_page:
-                url = response.url.update_query(next_page=next_page).human_repr()
+                url = response.url.update_query(  # type: ignore
+                    next_page=next_page
+                ).human_repr()
                 response_data = await session.get_json(url)
 
-                if message := response_data.get("error") or response_data.get(
+                if message := response_data.get("error") or response_data.get(  # type: ignore
                     "message"
                 ):
                     warnings.warn(message=message, category=OpenBBWarning)
                     return []
 
-                symbol = response.url.parts[-2]
-                tag = response_data.url.parts[-1]
+                symbol = response.url.parts[-2]  # type: ignore
+                tag = response_data.url.parts[-1]  # type: ignore
 
-                response_data = response_data.get("historical_data", [])
+                response_data = response_data.get("historical_data", [])  # type: ignore
                 response_data = [
                     {**item, "symbol": symbol, "tag": tag} for item in response_data
                 ]
 
                 all_data.extend(response_data)
-                next_page = response_data.get("next_page", None)
+                next_page = response_data.get("next_page", None)  # type: ignore
 
             return all_data
 
         urls = [
             generate_url(symbol, tag)
             for symbol in query.symbol.split(",")
             for tag in query.tag.split(",")
         ]
 
         return await amake_requests(urls, callback, **kwargs)
 
     @staticmethod
     def transform_data(
-        query: IntrinioHistoricalAttributesQueryParams,  # pylint: disable=unused-argument
+        query: IntrinioHistoricalAttributesQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioHistoricalAttributesData]:
         """Return the transformed data."""
         return [IntrinioHistoricalAttributesData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,26 +53,27 @@
     ) -> Dict:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
 
         base_url = "https://api-v2.intrinio.com/companies"
 
         def generate_url(symbol: str, tag: str) -> str:
-            """Returns the url for the given symbol and tag."""
+            """Return the url for the given symbol and tag."""
             return f"{base_url}/{symbol}/data_point/{tag}?api_key={api_key}"
 
         async def callback(response: ClientResponse, _: Any) -> Dict:
             """Return the response."""
             response_data = await response.json()
 
             if isinstance(response_data, Dict) and (
                 "error" in response_data or "message" in response_data
             ):
                 warnings.warn(
-                    message=response_data.get("error") or response_data.get("message"),
+                    message=str(response_data.get("error"))
+                    or str(response_data.get("message")),
                     category=OpenBBWarning,
                 )
                 return {}
             if not response_data:
                 return {}
 
             tag = response.url.parts[-1]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                     results.extend(new_data)
 
         if symbols:
             await asyncio.gather(*[get_one(symbol) for symbol in symbols])
             return results
 
         async def fetch_callback(response, session):
-            """Callback for pagination."""
+            """Use callback for pagination."""
             data = await response.json()
             messages = data.get("messages")
             if messages:
                 raise RuntimeError(str(messages))
             _data = data.get("target_price_consensuses")
             if _data and len(_data) > 0:
                 results.extend(_data)  # type: ignore
@@ -158,15 +158,14 @@
     @staticmethod
     def transform_data(
         query: IntrinioPriceTargetConsensusQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioPriceTargetConsensusData]:
         """Transform the raw data into the standard format."""
-
         symbols = query.symbol.split(",") if query.symbol else []
         results: List[IntrinioPriceTargetConsensusData] = []
         for item in sorted(  # type: ignore
             sorted(  # type: ignore
                 data,
                 key=lambda item: item.get("most_recent_date"),  # type: ignore
                 reverse=True,
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     response = open_url(url)
     return BasicResponse(response)
 
 
 async def response_callback(
     response: ClientResponse, _: ClientSession
 ) -> Union[dict, List[dict]]:
-    """Callback for async_request."""
+    """Use callback for async_request."""
     data = await response.json()
 
     if isinstance(data, dict) and response.status != 200:
         if message := data.get("error", None) or data.get("message", None):
             raise RuntimeError(f"Error in Intrinio request -> {message}")
 
         if error := data.get("Error Message", None):
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         "payment_date",
         "declaration_date",
         mode="before",
         check_fields=False,
     )
     @classmethod
     def validate_date(cls, v: str):
+        """Validate the date."""
         v = v.replace("N/A", "")
         return datetime.strptime(v, "%m/%d/%Y").date() if v else None
 
 
 class NasdaqCalendarDividendFetcher(
     Fetcher[
         NasdaqCalendarDividendQueryParams,
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,32 +81,33 @@
 
 
 class NasdaqCotData(COTData):
     """Nasdaq CFTC Commitment of Traders Reports Data."""
 
     @field_validator("date", mode="before", check_fields=False)
     def date_validate(cls, v):  # pylint: disable=E0213
-        """Return the datetime object from the date string"""
-
+        """Return the datetime object from the date string."""
         return datetime.strptime(v, "%Y-%m-%d").date()
 
 
 class NasdaqCotFetcher(Fetcher[NasdaqCotQueryParams, List[NasdaqCotData]]):
     """Transform the query, extract and transform the data from the Nasdaq endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqCotQueryParams:
+        """Transform the query parameters."""
         return NasdaqCotQueryParams(**params)
 
     @staticmethod
     def extract_data(
         query: NasdaqCotQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
+        """Extract the data from the Nasdaq Data Link API."""
         api_key = credentials.get("nasdaq_api_key") if credentials else ""
 
         # The "code" can be an exact name, a symbol, or a CFTC series code.
         series_id: str = ""
         series_ids = pd.DataFrame(CFTC).transpose().reset_index(drop=True)
         series_ids.columns = series_ids.columns.str.lower()
 
@@ -170,8 +171,9 @@
 
     @staticmethod
     def transform_data(
         query: NasdaqCotQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[NasdaqCotData]:
+        """Transform the data."""
         return [NasdaqCotData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cot_search import (
     CotSearchData,
     CotSearchQueryParams,
 )
 from openbb_nasdaq.utils.series_ids import CFTC
 
+# pylint: disable=W0613
+
 
 class NasdaqCotSearchQueryParams(CotSearchQueryParams):
     """Nasdaq CFTC Commitment of Traders Reports Search Query.
 
     Source: https://data.nasdaq.com/data/CFTC-commodity-futures-trading-commission-reports/documentation
     """
 
@@ -27,14 +29,15 @@
 ):
     """Transform the query, extract and transform the data from the Nasdaq endpoints."""
 
     require_credentials = False
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqCotSearchQueryParams:
+        """Transform the query params."""
         return NasdaqCotSearchQueryParams(**params)
 
     @staticmethod
     def extract_data(
         query: NasdaqCotSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
@@ -56,8 +59,9 @@
 
     @staticmethod
     def transform_data(
         query: CotSearchQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[NasdaqCotSearchData]:
+        """Transform the data."""
         return [NasdaqCotSearchData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""OECD helper functions."""
+
 import ssl
 from datetime import date
 from io import StringIO
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import requests
@@ -16,35 +18,37 @@
 Path(cache).mkdir(parents=True, exist_ok=True)
 
 # OECD does not play well with newer python.  This code block from stackoverflow helps
 # to create a custom session:
 
 
 class CustomHttpAdapter(requests.adapters.HTTPAdapter):
-    # "Transport adapter" that allows us to use custom ssl_context.
+    """Transport adapter" that allows us to use custom ssl_context."""
 
     def __init__(self, ssl_context=None, **kwargs):
+        """Initialize the adapter with a custom ssl_context."""
         self.ssl_context = ssl_context
         super().__init__(**kwargs)
 
     # pylint: disable=arguments-differ
     def init_poolmanager(self, connections, maxsize, block=False):
+        """Initialize the poolmanager with a custom ssl_context."""
         self.poolmanager = urllib3.poolmanager.PoolManager(  # pylint: disable=attribute-defined-outside-init
             num_pools=connections,
             maxsize=maxsize,
             block=block,
             ssl_context=self.ssl_context,
         )
 
 
 # pylint: enable=arguments-differ
 
 
 def get_legacy_session():
-    """Stackoverflow code to create a custom session."""
+    """Create a custom session."""
     ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
     ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
     session = requests.Session()
     session.mount("https://", CustomHttpAdapter(ctx))
     return session
 
 
@@ -60,17 +64,17 @@
     return data
 
 
 ### The functions below are for using the new oecd data-explorer instead of the stats.oecd
 
 
 def oecd_xml_to_df(xml_string: str) -> DataFrame:
-    """Helper function to parse the OECD XML and return a dataframe.
+    """Parse the OECD XML and return a dataframe.
 
-     Parameters
+    Parameters
     ----------
     xml_string : str
         A string containing the OECD XML data.
 
     Returns
     -------
     DataFrame
@@ -104,15 +108,15 @@
             data.append(obs_data)
 
     # Create a DataFrame
     return DataFrame(data)
 
 
 def parse_url(url: str) -> DataFrame:
-    """Helper function to parse the SDMX url and return a dataframe.
+    """Parse the SDMX url and return a dataframe.
 
     Parameters
     ----------
     url:str
         URL to parse
 
     Returns
@@ -189,29 +193,28 @@
         with open(f"{cache_str}.timestamp", "w") as f:
             f.write(str(date.today()))
     else:
         raise NotImplementedError
 
 
 def query_dict_to_path(query_dict: dict) -> str:
-    """Convert the query dict into something usable for writing file"""
+    """Convert the query dict into something usable for writing file."""
     items = sorted(query_dict.items())
     key_parts = [f"{key}_{value}" for key, value in items]
     return "-".join(key_parts).replace("/", "_").replace(" ", "_")
 
 
 def get_possibly_cached_data(
     url: str,
     function: Optional[str] = None,
     query_dict: Optional[dict] = None,
     cache_method: str = "csv",
     skip_cache: bool = False,
 ) -> DataFrame:
-    """
-    Retrieve data from a given URL or from the cache if available and valid.
+    """Retrieve data from a given URL or from the cache if available and valid.
 
     Parameters
     ----------
     url : str
         The URL from which to fetch the data if it's not available in the cache.
     function : Optional[str], optional
         The name of the function for which data is being fetched or cached.
@@ -221,16 +224,17 @@
         The method used for caching the data (default is 'csv').
 
     Returns
     -------
     DataFrame
         A Pandas DataFrame containing the fetched or cached data.
     """
-
-    base_cache = f"{cache}/{function}_{query_dict_to_path(query_dict)}"
+    base_cache = (
+        f"{cache}/{function}_{query_dict_to_path(query_dict if query_dict else {})}"
+    )
     if cache_method == "parquet":
         cache_path = base_cache + ".parquet"
     elif cache_method == "csv":
         cache_path = base_cache + ".csv"
 
     use_cache = check_cache_exists_and_valid(
         cache_str=base_cache, cache_method=cache_method
@@ -244,15 +248,15 @@
         data = parse_url(url)
         if not skip_cache:
             write_to_cache(cache_str=base_cache, data=data, cache_method=cache_method)
     return data
 
 
 def oecd_date_to_python_date(input_date: Union[str, int]) -> date:
-    """Darrens good idea to make the dates filterable"""
+    """Use Darrens good idea to make the dates filterable."""
     input_date = str(input_date)
     if "Q" in input_date:
         return to_datetime(input_date).to_period("Q").to_timestamp("Q").date()
     if len(input_date) == 4:
         return date(int(input_date), 12, 31)
     if len(input_date) == 7:
         return to_datetime(input_date).to_period("M").to_timestamp("M").date()
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Polygon Helpers Module."""
 
 import json
 from io import StringIO
-from typing import Any, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union
 
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_request,
 )
@@ -27,39 +27,40 @@
 
     def json(self) -> dict:
         """Return the response as a dictionary."""
         return json.loads(self.text)
 
 
 def request(url: str) -> BasicResponse:
-    """
-    Request function for PyScript. Pass in Method and make sure to await.
+    """Request function for PyScript.
+
+    Pass in Method and make sure to await.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     url: str
         URL to make request to
 
-    Return:
-    -------
+    Return
+    ------
     response: BasicRequest
         BasicRequest object with status_code and text attributes
     """
     # pylint: disable=import-outside-toplevel
     from pyodide.http import open_url  # type: ignore
 
     response = open_url(url)
     return BasicResponse(response)
 
 
 async def response_callback(
     response: ClientResponse, _: ClientSession
 ) -> Union[dict, List[dict]]:
-    """Callback for make_request."""
-    data: dict = await response.json()
+    """Use callback for make_request."""
+    data: Dict = await response.json()  # type: ignore
 
     if response.status != 200:
         message = data.get("error", None) or data.get("message", None)
         raise RuntimeError(f"Error in Polygon request -> {message}")
 
     keys_in_data = "results" in data or "tickers" in data
 
@@ -75,23 +76,23 @@
 
 
 async def get_data_many(
     url: str, sub_dict: Optional[str] = None, **kwargs: Any
 ) -> List[dict]:
     """Get data from Polygon endpoint and convert to list of schemas.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     url: str
         The URL to get the data from.
     sub_dict: Optional[str]
         The sub-dictionary to use.
 
-    Returns:
-    --------
+    Returns
+    -------
     List[dict]
         Dictionary of data.
     """
     data = await get_data(url, **kwargs)
     if sub_dict and isinstance(data, dict):
         data = data.get(sub_dict, [])
     if isinstance(data, dict):
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/company_filings.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,31 +141,31 @@
 
     @staticmethod
     def extract_data(
         query: SecCompanyFilingsQueryParams,  # pylint: disable=unused-argument
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Extracts the data from the SEC endpoint."""
+        """Extract the data from the SEC endpoint."""
         filings = pd.DataFrame()
 
         if query.symbol and not query.cik:
             query.cik = symbol_map(query.symbol.lower(), use_cache=query.use_cache)
             if not query.cik:
                 return []
         if query.cik is None:
             return []
 
         # The leading 0s need to be inserted but are typically removed from the data to store as an integer.
-        if len(query.cik) != 10:
+        if len(query.cik) != 10:  # type: ignore
             cik_: str = ""
-            temp = 10 - len(query.cik)
+            temp = 10 - len(query.cik)  # type: ignore
             for i in range(temp):
                 cik_ = cik_ + "0"
-            query.cik = cik_ + query.cik
+            query.cik = cik_ + str(query.cik)  # type: ignore
 
         url = f"https://data.sec.gov/submissions/CIK{query.cik}.json"
         r = (
             requests.get(url, headers=HEADERS, timeout=5)
             if query.use_cache is False
             else sec_session_company_filings.get(url, headers=HEADERS, timeout=5)
         )
@@ -232,9 +232,9 @@
 
         return filings.to_dict("records")
 
     @staticmethod
     def transform_data(
         query: SecCompanyFilingsQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecCompanyFilingsData]:
-        """Transforms the data."""
+        """Transform the data."""
         return [SecCompanyFilingsData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_ftd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     @staticmethod
     def extract_data(
         query: SecEquityFtdQueryParams,  # pylint: disable=unused-argument
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Extracts the data from the SEC website."""
+        """Extract the data from the SEC website."""
         results = []
         limit = query.limit if query.limit is not None and query.limit > 0 else 0
         symbol = query.symbol.upper()
 
         urls_data = get_ftd_urls()
         urls = list(urls_data.values())
         if limit > 0:
@@ -79,9 +79,9 @@
 
         return results
 
     @staticmethod
     def transform_data(
         query: SecEquityFtdQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecEquityFtdData]:
-        """Transforms the data to the standard format."""
+        """Transform the data to the standard format."""
         return [SecEquityFtdData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""SEC Helpers module"""
+"""SEC Helpers module."""
 
 # pylint: skip-file
 from datetime import timedelta
 from io import BytesIO
 from typing import Dict, List, Optional
 from zipfile import ZipFile
 
@@ -26,42 +26,41 @@
 
 sec_session_company_filings = requests_cache.CachedSession(
     f"{cache_dir}/http/sec_company_filings", expire_after=timedelta(days=1)
 )
 
 
 def get_all_companies(use_cache: bool = True) -> pd.DataFrame:
-    """Gets all company names, tickers, and CIK numbers registered with the SEC.
+    """Get all company names, tickers, and CIK numbers registered with the SEC.
+
     Companies are sorted by market cap.
 
     Returns
     -------
     pd.DataFrame: Pandas DataFrame with columns for Symbol, Company Name, and CIK Number.
 
     Example
     -------
     >>> tickers = get_all_companies()
     """
-
     url = "https://www.sec.gov/files/company_tickers.json"
 
     r = (
         sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
         if use_cache is True
         else requests.get(url, headers=SEC_HEADERS, timeout=5)
     )
     df = pd.DataFrame(r.json()).transpose()
     cols = ["cik", "symbol", "name"]
     df.columns = cols
     return df.astype(str)
 
 
 def get_all_ciks(use_cache: bool = True) -> pd.DataFrame:
-    """Gets a list of entity names and their CIK number."""
-
+    """Get a list of entity names and their CIK number."""
     HEADERS = {
         "User-Agent": "my real company name definitelynot@fakecompany.com",
         "Accept-Encoding": "gzip, deflate",
         "Host": "www.sec.gov",
     }
     url = "https://www.sec.gov/Archives/edgar/cik-lookup-data.txt"
     r = (
@@ -82,16 +81,15 @@
     df.columns = cols
     df = df.dropna()
 
     return df
 
 
 def get_mf_and_etf_map(use_cache: bool = True) -> pd.DataFrame:
-    """Returns the CIK number of a ticker symbol for querying the SEC API."""
-
+    """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbols = pd.DataFrame()
 
     url = "https://www.sec.gov/files/company_tickers_mf.json"
     r = (
         sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
         if use_cache is True
         else requests.get(url, headers=SEC_HEADERS, timeout=5)
@@ -106,16 +104,15 @@
     """Search for an institution by name.  It is case-insensitive."""
     institutions = get_all_ciks(use_cache=use_cache)
     hp = institutions["Institution"].str.contains(keyword, case=False)
     return institutions[hp].astype(str)
 
 
 def symbol_map(symbol: str, use_cache: bool = True) -> str:
-    """Returns the CIK number of a ticker symbol for querying the SEC API."""
-
+    """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbol = symbol.upper().replace(".", "-")
     symbols = get_all_companies(use_cache=use_cache)
 
     if symbol not in symbols["symbol"].to_list():
         symbols = get_mf_and_etf_map(use_cache=use_cache).astype(str)
         if symbol not in symbols["symbol"].to_list():
             return ""
@@ -126,16 +123,15 @@
     for i in range(temp):
         cik_ = cik_ + "0"
 
     return str(cik_ + cik)
 
 
 def cik_map(cik: int, use_cache: bool = True) -> str:
-    """
-    Converts a CIK number to a ticker symbol.  Enter CIK as an integer with no leading zeros.
+    """Convert a CIK number to a ticker symbol.  Enter CIK as an integer with no leading zeros.
 
     Function is not meant for funds.
 
     Parameters
     ----------
     cik : int
         The CIK number to convert to a ticker symbol.
@@ -160,15 +156,16 @@
     quarter: Optional[QUARTERS] = None,
     taxonomy: TAXONOMIES = "us-gaap",
     units: str = "USD",
     fact: str = "Revenues",
     instantaneous: bool = False,
     use_cache: bool = True,
 ) -> Dict:
-    """
+    """Get a frame of data for a given fact.
+
     The xbrl/frames API aggregates one fact for each reporting entity
     that is last filed that most closely fits the calendrical period requested.
 
     This API supports for annual, quarterly and instantaneous data:
 
     https://data.sec.gov/api/xbrl/frames/us-gaap/AccountsPayableCurrent/USD/CY2019Q1I.json
 
@@ -193,15 +190,14 @@
     InterestAndDebtExpense
     IncomeTaxExpenseBenefit
     NetIncomeLoss
 
     Facts where units are, "shares":
     WeightedAverageNumberOfDilutedSharesOutstanding
     """
-
     if fact in ["WeightedAverageNumberOfDilutedSharesOutstanding"]:
         units = "shares"
 
     url = f"https://data.sec.gov/api/xbrl/frames/{taxonomy}/{fact}/{units}/CY{year}"
 
     if quarter:
         url = url + f"Q{quarter}"
@@ -233,14 +229,15 @@
 
     results = {"metadata": metadata, "data": data}
 
     return results
 
 
 def get_schema_filelist(query: str = "", url: str = "") -> List:
+    """Get a list of schema files from the SEC website."""
     results: List = []
     url = url if url else f"https://xbrl.fasb.org/us-gaap/{query}"
     _url = url
     _url = url + "/" if query else _url
     r = sec_session_companies.get(_url, headers=HEADERS, timeout=5)
 
     if r.status_code != 200:
@@ -296,15 +293,14 @@
             results["price"] = results["price"].astype(float)
 
     return results.reset_index(drop=True).to_dict("records")
 
 
 def get_ftd_urls() -> Dict:
     """Get Fails-to-Deliver Data URLs."""
-
     results = {}
     position = None
     key = "title"
     value = "Fails-to-Deliver Data"
 
     r = requests.get("https://www.sec.gov/data.json", timeout=5, headers=SEC_HEADERS)
     if r.status_code != 200:
@@ -326,16 +322,16 @@
 
     return results
 
 
 def get_series_id(
     symbol: Optional[str] = None, cik: Optional[str] = None, use_cache: bool = True
 ):
-    """
-    This function maps the fund to the series and class IDs for validating the correct filing.
+    """Map the fund to the series and class IDs for validating the correct filing.
+
     For an exact match, use a symbol.
     """
     symbol = symbol if symbol else ""
     cik = cik if cik else ""
 
     results = pd.DataFrame()
     if not symbol and not cik:
@@ -355,16 +351,15 @@
     if len(results) > 0:
         results = results[results[choice if not symbol else choice] == target]
 
         return results
 
 
 def get_nport_candidates(symbol: str, use_cache: bool = True) -> List[Dict]:
-    """Gets a list of all NPORT-P filings for a given fund's symbol."""
-
+    """Get a list of all NPORT-P filings for a given fund's symbol."""
     results = []
     _series_id = get_series_id(symbol, use_cache=use_cache)
     try:
         series_id = (
             symbol_map(symbol, use_cache)
             if _series_id is None or len(_series_id) == 0
             else _series_id["seriesId"].iloc[0]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Utility functions for parsing SEC Form 13F-HR."""
 
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
 
 import xmltodict
 from bs4 import BeautifulSoup
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_sec.models.company_filings import SecCompanyFilingsFetcher
 from openbb_sec.utils.definitions import HEADERS
 from pandas import DataFrame, offsets, to_datetime
@@ -18,15 +18,15 @@
         .strftime("%Y-%m-%d")
     )
 
 
 def get_13f_candidates(symbol: Optional[str] = None, cik: Optional[str] = None):
     """Get the 13F-HR filings for a given symbol or CIK."""
     fetcher = SecCompanyFilingsFetcher()
-    params = {}
+    params: Dict[str, Any] = {}
     if cik is not None:
         params["cik"] = str(cik)
     if symbol is not None:
         params["symbol"] = symbol
     if cik is None and symbol is None:
         raise ValueError("Either symbol or cik must be provided.")
 
@@ -42,15 +42,15 @@
         DataFrame(data=filings)
         .query("`reportDate` >= '2013-06-30'")
         .set_index("reportDate")["completeSubmissionUrl"]
     )
 
 
 async def complete_submission_callback(response, _):
-    """Callback function for processing the response object."""
+    """Use callback function for processing the response object."""
     if response.status == 200:
         return await response.text()
     raise RuntimeError(f"Request failed with status code {response.status}")
 
 
 async def get_complete_submission(url: str):
     """Get the Complete Submission TXT file string from the SEC API."""
@@ -102,15 +102,15 @@
     raise ValueError(
         "Failed to get the period of report from the form header."
         + " Check the response from `parse_header`."
     )
 
 
 async def parse_13f_hr(filing: str):
-    """Parses a 13F-HR filing from the Complete Submission TXT file string."""
+    """Parse a 13F-HR filing from the Complete Submission TXT file string."""
     data = DataFrame()
 
     # Check if the input string is a URL
     if filing.startswith("https://"):
         filing = await get_complete_submission(filing)  # type: ignore
 
     # Validate the submission so we know that we can parse it.
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Earnings Calendar Model"""
+"""TMX Earnings Calendar Model."""
 
 # pylint: disable=unused-argument
 import asyncio
 import json
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Optional
 
@@ -81,22 +81,20 @@
     @staticmethod
     async def aextract_data(
         query: TmxCalendarEarningsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
-        results = []
-        dates = []
+        results: List[Dict] = []
         user_agent = get_random_agent()
         dates = date_range(query.start_date, end=query.end_date)
 
         async def create_task(date, results):
-            """Creates a task for a single date in the range."""
+            """Create a task for a single date in the range."""
             data = []
             date = date.strftime("%Y-%m-%d")
             payload = gql.get_earnings_date_payload.copy()
             payload["variables"]["date"] = date
             url = "https://app-money.tmx.com/graphql"
             r = await get_data_from_gql(
                 method="POST",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,25 @@
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
     page: Optional[int] = Field(
         default=1, description="The page number to start from. Use with limit."
     )
 
+    @field_validator("symbol", mode="before")
+    @classmethod
+    def symbols_validate(cls, v):
+        """Validate the symbols."""
+        if v is None:
+            raise ValueError("Symbol is a required field for TMX.")
+        return v
+
 
 class TmxCompanyNewsData(CompanyNewsData):
-    """TMX Stock News Data"""
+    """TMX Stock News Data."""
 
     __alias_dict__ = {
         "date": "datetime",
         "title": "headline",
     }
 
     source: Optional[str] = Field(description="Source of the news.", default=None)
@@ -59,30 +67,29 @@
     async def aextract_data(
         query: TmxCompanyNewsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
         user_agent = get_random_agent()
-        symbols = query.symbol.split(",")
-        results = []
+        symbols = query.symbol.split(",")  # type: ignore
+        results: List[Dict] = []
 
         async def create_task(symbol, results):
-            """Makes a POST request to the TMX GraphQL endpoint for a single symbol."""
-
+            """Make a POST request to the TMX GraphQL endpoint for a single symbol."""
             symbol = (
                 symbol.upper().replace(".TO", "").replace(".TSX", "").replace("-", ".")
             )
             payload = gql.get_company_news_events_payload
             payload["variables"]["symbol"] = symbol
             payload["variables"]["page"] = query.page
             payload["variables"]["limit"] = query.limit
             payload["variables"]["locale"] = "en"
             url = "https://app-money.tmx.com/graphql"
-            data = {}
+            data: Dict = {}
             response = await get_data_from_gql(
                 method="POST",
                 url=url,
                 data=json.dumps(payload),
                 headers={
                     "authority": "app-money.tmx.com",
                     "referer": f"https://money.tmx.com/en/quote/{symbol}",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     source: https://money.tmx.com
     """
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
     interval: Union[
         Literal["1m", "2m", "5m", "15m", "30m", "60m", "1h", "1d", "1W", "1M"], str, int
-    ] = Field(
+    ] = Field(  # type: ignore
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " Or, any integer (entered as a string) representing the number of minutes."
         + " Default is daily data."
         + " There is no extended hours data, and intraday data is limited to after April 12 2022.",
         default="day",
     )
     adjustment: Literal["splits_only", "splits_and_dividends", "unadjusted"] = Field(
@@ -142,20 +142,19 @@
     @staticmethod
     async def aextract_data(
         query: TmxEquityHistoricalQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         results: List[Dict] = []
         symbols = query.symbol.split(",")
 
         async def create_task(symbol, results):
-            """Makes a POST request to the TMX GraphQL endpoint for a single ticker."""
+            """Make a POST request to the TMX GraphQL endpoint for a single ticker."""
             data: List[Dict] = []
             # A different request is used for each type of interval.
             if query.interval == "day":
                 data = await get_daily_price_history(
                     symbol,
                     start_date=query.start_date,
                     end_date=query.end_date,
@@ -195,15 +194,14 @@
     @staticmethod
     def transform_data(
         query: TmxEquityHistoricalQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TmxEquityHistoricalData]:
         """Return the transformed data."""
-
         results = DataFrame(data)
         if results.empty or len(results) == 0:
             raise EmptyDataError()
 
         # Handle the date formatting differences.
         results = results.rename(columns={"dateTime": "datetime"})
         if query.interval != "day":
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Equity Profile fetcher"""
+"""TMX Equity Profile fetcher."""
 
 # pylint: disable=unused-argument
 import asyncio
 import json
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
@@ -80,26 +80,24 @@
     @staticmethod
     async def aextract_data(
         query: TmxEquityProfileQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         symbols = query.symbol.split(",")
 
         # The list where the results will be stored and appended to.
-        results = []
+        results: List[Dict] = []
         user_agent = get_random_agent()
 
         url = "https://app-money.tmx.com/graphql"
 
         async def create_task(symbol: str, results) -> None:
-            """Makes a POST request to the TMX GraphQL endpoint for a single symbol."""
-
+            """Make a POST request to the TMX GraphQL endpoint for a single symbol."""
             symbol = (
                 symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
             )
 
             payload = gql.stock_info_payload.copy()
             payload["variables"]["symbol"] = symbol
 
@@ -129,15 +127,14 @@
     @staticmethod
     def transform_data(
         query: TmxEquityProfileQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TmxEquityProfileData]:
         """Return the transformed data."""
-
         # Get only the items associated with `equity.profile()`.
         items_list = [
             "shortDescription",
             "longDescription",
             "website",
             "phoneNumber",
             "fullAddress",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Equity Profile fetcher"""
+"""TMX Equity Profile fetcher."""
 
 # pylint: disable=unused-argument
 
 import asyncio
 import json
 import warnings
 from datetime import (
@@ -233,15 +233,15 @@
         "div_ex_date",
         "div_pay_date",
         mode="before",
         check_fields=False,
     )
     @classmethod
     def date_validate(cls, v):  # pylint: disable=E0213
-        """Return the datetime object from the date string"""
+        """Return the datetime object from the date string."""
         if v:
             try:
                 return datetime.strptime(v, "%Y-%m-%d").date()
             except ValueError:
                 return datetime.strptime(v, "%Y-%m-%d %H:%M:%S.%f").date()
         return None
 
@@ -277,26 +277,24 @@
     @staticmethod
     async def aextract_data(
         query: TmxEquityQuoteQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         symbols = query.symbol.split(",")
 
         # The list where the results will be stored and appended to.
-        results = []
+        results: List[Dict] = []
         user_agent = get_random_agent()
 
         url = "https://app-money.tmx.com/graphql"
 
         async def create_task(symbol: str, results) -> None:
-            """Makes a POST request to the TMX GraphQL endpoint for a single symbol."""
-
+            """Make a POST request to the TMX GraphQL endpoint for a single symbol."""
             symbol = (
                 symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
             )
 
             payload = gql.stock_info_payload.copy()
             payload["variables"]["symbol"] = symbol
 
@@ -328,15 +326,14 @@
     @staticmethod
     def transform_data(
         query: TmxEquityQuoteQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TmxEquityQuoteData]:
         """Return the transformed data."""
-
         # Remove the items associated with `equity.profile()`.
         items_list = [
             "shortDescription",
             "longDescription",
             "website",
             "phoneNumber",
             "fullAddress",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     def normalize_percent(cls, v):
         """Return percents as normalized percentage points."""
         return float(v) / 100 if v else 0
 
     @model_validator(mode="before")
     @classmethod
     def check_metric(cls, values):
+        """Check for missing metrics."""
         for k, v in values.items():
             if v is None or v == "-":
                 values[k] = 0
             if k in ["Dividend Yield"]:
                 values[k] = float(v) / 100 if v else None
         return values
 
@@ -100,15 +101,14 @@
     @staticmethod
     async def aextract_data(
         query: TmxGainersQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[TmxGainersData]:
         """Return the raw data from the TMX endpoint."""
-
         user_agent = get_random_agent()
         payload = gql.get_stock_list_payload.copy()
         payload["variables"]["stockListId"] = STOCK_LISTS_DICT[query.category]
 
         url = "https://app-money.tmx.com/graphql"
         response = await get_data_from_gql(
             method="POST",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Index Constituents Model"""
+"""TMX Index Constituents Model."""
 
 # pylint: disable=unused-argument
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.index_constituents import (
     IndexConstituentsData,
@@ -45,27 +45,28 @@
 
 class TmxIndexConstituentsFetcher(
     Fetcher[
         TmxIndexConstituentsQueryParams,
         List[TmxIndexConstituentsData],
     ]
 ):
+    """TMX Index Constituents Fetcher."""
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TmxIndexConstituentsQueryParams:
         """Transform the query."""
         return TmxIndexConstituentsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: TmxIndexConstituentsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the TMX endpoint."""
-
         url = "https://tmxinfoservices.com/files/indices/sptsx-indices.json"
 
         data = await get_data_from_url(
             url,
             use_cache=query.use_cache,
             backend=tmx_indices_backend,
         )
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Index Snapshots Model"""
+"""TMX Index Snapshots Model."""
 
 # pylint: disable=unused-argument
 import json
 from typing import Any, Dict, List, Literal, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.index_snapshots import (
@@ -20,15 +20,15 @@
 )
 from pydantic import Field, field_validator
 
 
 class TmxIndexSnapshotsQueryParams(IndexSnapshotsQueryParams):
     """TMX Index Snapshots Query Params."""
 
-    region: Literal[None, "ca", "us"] = Field(default="ca")
+    region: Literal[None, "ca", "us"] = Field(default="ca")  # type: ignore
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request."
         + " Index data is from a single JSON file, updated each day after close."
         + " It is cached for one day. To bypass, set to False.",
     )
 
@@ -147,14 +147,16 @@
 
 class TmxIndexSnapshotsFetcher(
     Fetcher[
         TmxIndexSnapshotsQueryParams,
         List[TmxIndexSnapshotsData],
     ]
 ):
+    """TMX Index Snapshots Fetcher."""
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TmxIndexSnapshotsQueryParams:
         """Transform the query."""
         return TmxIndexSnapshotsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Insider Trading Model"""
+"""TMX Insider Trading Model."""
 
 # pylint: disable=unused-argument
 import json
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.insider_trading import (
@@ -13,24 +13,24 @@
 from openbb_core.provider.utils.helpers import to_snake_case
 from openbb_tmx.utils import gql
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, field_validator
 
 
 class TmxInsiderTradingQueryParams(InsiderTradingQueryParams):
-    """TMX Insider Trading Query Params"""
+    """TMX Insider Trading Query Params."""
 
     summary: bool = Field(
         default=False,
         description="Return a summary of the insider activity instead of the individuals.",
     )
 
 
 class TmxInsiderTradingData(InsiderTradingData):
-    """TMX Insider Trading Data"""
+    """TMX Insider Trading Data."""
 
     period: str = Field(
         description="The period of the activity. Bucketed by three, six, and twelve months."
     )
     owner_name: Optional[str] = Field(
         default=None, description="The name of the insider."
     )
@@ -62,14 +62,15 @@
         default=None,
         description="The total net activity by all insiders over the period.",
     )
 
     @field_validator("period", mode="before", check_fields=False)
     @classmethod
     def period_to_snake_case(cls, v):
+        """Convert the period to snake case."""
         return to_snake_case(v) if v else None
 
 
 class TmxInsiderTradingFetcher(
     Fetcher[
         TmxInsiderTradingQueryParams,
         List[TmxInsiderTradingData],
@@ -85,15 +86,14 @@
     @staticmethod
     async def aextract_data(
         query: TmxInsiderTradingQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         results = []
         user_agent = get_random_agent()
         symbol = (
             query.symbol.upper()
             .replace("-", ".")
             .replace(".TO", "")
             .replace(".TSX", "")
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import (
     date as dateType,
     datetime,
     time,
     timedelta,
 )
 from io import StringIO
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional, Union
 
 import exchange_calendars as xcals
 import pandas as pd
 import pytz
 from aiohttp_client_cache import SQLiteBackend
 from aiohttp_client_cache.session import CachedSession
 from dateutil import rrule
@@ -261,15 +261,15 @@
     "^XCM": "PHLX Chemicals Sector",
     "^XEX": "PHLX Europe Sector",
     "^XND": "Nasdaq-100 Micro Index",
 }
 
 
 async def response_callback(response, _: Any):
-    """Callback for HTTP Client Response."""
+    """Use callback for HTTP Client Response."""
     content_type = response.headers.get("Content-Type", "")
     if "application/json" in content_type:
         return await response.json()
     if "text" in content_type:
         return await response.text()
     return await response.read()
 
@@ -292,29 +292,28 @@
         data = await amake_request(url, response_callback=response_callback, timeout=20)
 
     return data
 
 
 async def get_data_from_gql(url: str, headers, data, **kwargs: Any) -> Any:
     """Make an asynchronous GraphQL request."""
-
     response = await amake_request(
         url=url,
         method="POST",
         response_callback=response_callback,
         headers=headers,
         data=data,
         timeout=30,
     )
 
     return response
 
 
 def replace_values_in_list_of_dicts(data):
-    """Helper function to replace "NA" and "-" with None in a list of dictionaries."""
+    """Replace "NA" and "-" with None in a list of dictionaries."""
     for d in data:
         for k, v in d.items():
             if isinstance(v, dict):
                 replace_values_in_list_of_dicts([v])  # Recurse into nested dictionary
             elif isinstance(v, list):
                 for i in range(len(v)):  # pylint: disable=C0200
                     if isinstance(v[i], dict):
@@ -325,52 +324,47 @@
                         v[i] = None  # Replace "NA" and "-" with None
             elif v in ("NA", "-"):
                 d[k] = None  # Replace "NA" and "-" with None
     return data
 
 
 def check_weekday(date) -> str:
-    """Helper function to check if the input date is a weekday, and if not, returns the next weekday.
+    """Check if the input date is a weekday, and if not, returns the next weekday.
 
     Parameters
     ----------
     date: str
         The date to check in YYYY-MM-DD format.
 
     Returns
     -------
     str
         Date in YYYY-MM-DD format.  If the date is a weekend, returns the date of the next weekday.
     """
-
     if pd.to_datetime(date).weekday() > 4:
         return next_workday(pd.to_datetime(date)).strftime("%Y-%m-%d")
     return date
 
 
 async def get_all_etfs(use_cache: bool = True) -> List[Dict]:
-    """
-    Gets a summary of the TMX ETF universe.
+    """Get a summary of the TMX ETF universe.
 
     Returns
     -------
     Dict
         Dictionary with all TMX-listed ETFs.
     """
-
     url = "https://dgr53wu9i7rmp.cloudfront.net/etfs/etfs.json"
 
     response = await get_data_from_url(
         url, use_cache=use_cache, backend=tmx_etfs_backend
     )
 
-    if response is None:
-        raise RuntimeError(
-            f"There was a problem with the request. Could not get ETFs.  -> {response.status_code}"
-        )
+    if not response or response is None:
+        raise RuntimeError("There was a problem with the request. Could not get ETFs.")
 
     response = replace_values_in_list_of_dicts(response)
 
     etfs = pd.DataFrame(response).rename(columns=COLUMNS_DICT)
 
     etfs = etfs.drop(
         columns=[
@@ -399,16 +393,15 @@
 
     return etfs.to_dict(orient="records")
 
 
 async def get_tmx_tickers(
     exchange: Literal["tsx", "tsxv"] = "tsx", use_cache: bool = True
 ) -> Dict:
-    """Gets a dictionary of either TSX or TSX-V symbols and names."""
-
+    """Get a dictionary of either TSX or TSX-V symbols and names."""
     tsx_json_url = "https://www.tsx.com/json/company-directory/search"
     url = f"{tsx_json_url}/{exchange}/*"
     response = await get_data_from_url(
         url, use_cache=use_cache, backend=tmx_companies_backend
     )
     data = (
         pd.DataFrame.from_records(response["results"])[["symbol", "name"]]
@@ -416,32 +409,31 @@
         .sort_index()
     )
     results = data.to_dict()["name"]
     return results
 
 
 async def get_all_tmx_companies(use_cache: bool = True) -> Dict:
-    """Merges TSX and TSX-V listings into a single dictionary."""
+    """Merge TSX and TSX-V listings into a single dictionary."""
     all_tmx = {}
     tsx_tickers = await get_tmx_tickers(use_cache=use_cache)
     tsxv_tickers = await get_tmx_tickers("tsxv", use_cache=use_cache)
     all_tmx.update(tsxv_tickers)
     all_tmx.update(tsx_tickers)
     return all_tmx
 
 
 async def get_all_options_tickers(use_cache: bool = True) -> pd.DataFrame:
-    """Returns a DataFrame with all valid ticker symbols."""
-
+    """Return a DataFrame with all valid ticker symbols."""
     url = "https://www.m-x.ca/en/trading/data/options-list"
 
     r = await get_data_from_url(url, use_cache=use_cache, backend=tmx_companies_backend)
 
-    if r is None:
-        raise RuntimeError(f"Error with the request:  {r.status_code}")
+    if r is None or r == []:
+        raise RuntimeError("Error with the request")  # mypy: ignore
 
     options_listings = pd.read_html(StringIO(r))
     listings = pd.concat(options_listings)
     listings = listings.set_index("Option Symbol").drop_duplicates().sort_index()
     symbols = listings[:-1]
     symbols = symbols.fillna(value="")
     symbols["Underlying Symbol"] = (
@@ -452,16 +444,15 @@
         to_snake_case(col).replace("name_of_", "") for col in symbols.columns
     ]
 
     return symbols.set_index("option_symbol")
 
 
 async def get_current_options(symbol: str, use_cache: bool = True) -> pd.DataFrame:
-    """Gets the current quotes for the complete options chain."""
-
+    """Get the current quotes for the complete options chain."""
     SYMBOLS = await get_all_options_tickers(use_cache=use_cache)
     data = pd.DataFrame()
     symbol = symbol.upper()
 
     # Remove exchange  identifiers from the symbol.
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
     # Underlying symbol may have a different ticker symbol than the ticker used to lookup options.
@@ -554,16 +545,15 @@
 
     return chains
 
 
 async def download_eod_chains(
     symbol: str, date: Optional[dateType] = None, use_cache: bool = False
 ) -> pd.DataFrame:
-    """Downloads EOD chains data for a given symbol and date."""
-
+    """Download EOD chains data for a given symbol and date."""
     symbol = symbol.upper()
     SYMBOLS = await get_all_options_tickers(use_cache=False)
     # Remove echange  identifiers from the symbol.
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
 
     # Underlying symbol may have a different ticker symbol than the ticker used to lookup options.
     if len(SYMBOLS[SYMBOLS["underlying_symbol"].str.contains(symbol)]) == 1:
@@ -578,18 +568,18 @@
 
     cal = xcals.get_calendar("XTSE")
 
     if date is None:
         EOD_URL = BASE_URL + f"{symbol}" "&dnld=1#quotes"
     if date is not None:
         date = check_weekday(date)  # type: ignore
-        if cal.is_session(date) is False:
+        if cal.is_session(date) is False:  # type: ignore
             date = (pd.to_datetime(date) + timedelta(days=1)).strftime("%Y-%m-%d")  # type: ignore
         date = check_weekday(date)  # type: ignore
-        if cal.is_session(date=date) is False:
+        if cal.is_session(date=date) is False:  # type: ignore
             date = (pd.to_datetime(date) + timedelta(days=1)).strftime("%Y-%m-%d")  # type: ignore
 
         EOD_URL = (
             BASE_URL + f"{symbol}" "&from=" f"{date}" "&to=" f"{date}" "&dnld=1#quotes"
         )
 
     r = await get_data_from_url(EOD_URL, use_cache=use_cache)  # type: ignore
@@ -713,16 +703,16 @@
     results = r.get("data").get("filings")
 
     return results
 
 
 async def get_daily_price_history(
     symbol: str,
-    start_date: Optional[dateType] = None,
-    end_date: Optional[dateType] = None,
+    start_date: Optional[Union[str, dateType]] = None,
+    end_date: Optional[Union[str, dateType]] = None,
     adjustment: Literal[
         "splits_only", "unadjusted", "splits_and_dividends"
     ] = "splits_only",
 ):
     """Get historical price data."""
     start_date = (
         datetime.strptime(start_date, "%Y-%m-%d")
@@ -830,29 +820,31 @@
     results = [d for d in results if d["openPrice"] is not None]
 
     return sorted(results, key=lambda x: x["datetime"], reverse=False)
 
 
 async def get_weekly_or_monthly_price_history(
     symbol: str,
-    start_date: Optional[dateType] = None,
-    end_date: Optional[dateType] = None,
+    start_date: Optional[Union[str, dateType]] = None,
+    end_date: Optional[Union[str, dateType]] = None,
     interval: Literal["month", "week"] = "month",
 ):
     """Get historical price data."""
-    start_date = (
-        datetime.strptime(start_date, "%Y-%m-%d")
-        if isinstance(start_date, str)
-        else start_date
-    )
-    end_date = (
-        datetime.strptime(end_date, "%Y-%m-%d")
-        if isinstance(end_date, str)
-        else end_date
-    )
+    if start_date:
+        start_date = (
+            datetime.strptime(start_date, "%Y-%m-%d")
+            if isinstance(start_date, str)
+            else start_date
+        )
+    if end_date:
+        end_date = (
+            datetime.strptime(end_date, "%Y-%m-%d")
+            if isinstance(end_date, str)
+            else end_date
+        )
     user_agent = get_random_agent()
     results: List[Dict] = []
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
     start_date = (
         (datetime.now() - timedelta(weeks=52 * 100)).date()
         if start_date is None
         else start_date
@@ -864,16 +856,22 @@
         payload["variables"].pop("interval")
     if "startDateTime" in payload["variables"]:
         payload["variables"].pop("startDateTime")
     if "endDateTime" in payload["variables"]:
         payload["variables"].pop("endDateTime")
     payload["variables"]["symbol"] = symbol
     payload["variables"]["freq"] = interval
-    payload["variables"]["end"] = end_date.strftime("%Y-%m-%d")
-    payload["variables"]["start"] = start_date.strftime("%Y-%m-%d")
+    payload["variables"]["end"] = (
+        end_date.strftime("%Y-%m-%d") if isinstance(end_date, dateType) else end_date
+    )
+    payload["variables"]["start"] = (
+        start_date.strftime("%Y-%m-%d")
+        if isinstance(start_date, dateType)
+        else start_date
+    )
     url = "https://app-money.tmx.com/graphql"
     data = await get_data_from_gql(
         method="POST",
         url=url,
         data=json.dumps(payload),
         headers={
             "authority": "app-money.tmx.com",
@@ -910,46 +908,48 @@
         results = data["data"].get("getTimeSeriesData")
         results = sorted(results, key=lambda x: x["dateTime"], reverse=False)
     return results
 
 
 async def get_intraday_price_history(
     symbol: str,
-    start_date: Optional[dateType] = None,
-    end_date: Optional[dateType] = None,
+    start_date: Optional[Union[str, dateType]] = None,
+    end_date: Optional[Union[str, dateType]] = None,
     interval: Optional[int] = 1,
 ):
     """Get historical price data."""
-    start_date = (
-        datetime.strptime(start_date, "%Y-%m-%d")
-        if isinstance(start_date, str)
-        else start_date
-    )
-    end_date = (
-        datetime.strptime(end_date, "%Y-%m-%d")
-        if isinstance(end_date, str)
-        else end_date
-    )
+    if start_date:
+        start_date = (
+            datetime.strptime(start_date, "%Y-%m-%d")
+            if isinstance(start_date, str)
+            else start_date
+        )
+    if end_date:
+        end_date = (
+            datetime.strptime(end_date, "%Y-%m-%d")
+            if isinstance(end_date, str)
+            else end_date
+        )
     user_agent = get_random_agent()
     results: List[Dict] = []
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
     start_date = (
         (datetime.now() - timedelta(weeks=4)).date()
         if start_date is None
         else start_date
     )
     end_date = datetime.now().date() if end_date is None else end_date
     # This is the first date of available intraday data.
     date_check = datetime(2022, 4, 12).date()
     start_date = max(start_date, date_check)
-    if end_date < date_check:
+    if end_date < date_check:  # type: ignore
         end_date = datetime.now().date()
     # Generate a list of dates from start_date to end_date with a frequency of 3 weeks
     dates = list(
-        rrule.rrule(rrule.WEEKLY, interval=4, dtstart=start_date, until=end_date)
+        rrule.rrule(rrule.WEEKLY, interval=4, dtstart=start_date, until=end_date)  # type: ignore
     )
 
     if dates[-1] != end_date:
         dates.append(end_date)  # type: ignore
 
     # Create a list of 4-week chunks
     chunks = [
@@ -1035,16 +1035,18 @@
     if len(results) > 0 and "dateTime" in results[0]:
         results = sorted(results, key=lambda x: x["dateTime"], reverse=False)
 
     return results
 
 
 async def get_all_bonds(use_cache: bool = True) -> pd.DataFrame:
-    """Gets all bonds reference data published by CIRO. The complete list is approximately 70-100K securities."""
+    """Get all bonds reference data published by CIRO.
 
+    The complete list is approximately 70-100K securities.
+    """
     url = "https://bondtradedata.iiroc.ca/debtip/designatedbonds/list"
     response = await get_data_from_url(
         url, use_cache=use_cache, timeout=30, backend=tmx_bonds_backend
     )
 
     # Convert the response to a DataFrame and set the types for proper filtering in-fetcher.
     # This is done here because multiple functions might share this response object.
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tradier Options Chains Model"""
+"""Tradier Options Chains Model."""
 
 # pylint: disable = unused-argument
 
 import asyncio
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
@@ -16,26 +16,25 @@
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
 class TradierOptionsChainsQueryParams(OptionsChainsQueryParams):
-    """
-    Tradier Options Chains Query.
+    """Tradier Options Chains Query.
 
     Source: https://documentation.tradier.com/brokerage-api/markets/get-options-chains
 
     Greeks/IV data is updated once per hour.
     This data is calculated using the ORATS APIs and is supplied directly from them.
     """
 
 
 class TradierOptionsChainsData(OptionsChainsData):
-    """Tradier Options Chains Data"""
+    """Tradier Options Chains Data."""
 
     __alias_dict__ = {
         "expiration": "expiration_date",
         "contract_symbol": "symbol",
         "last_trade_price": "last",
         "bid_size": "bidsize",
         "ask_size": "asksize",
@@ -173,24 +172,24 @@
 class TradierOptionsChainsFetcher(
     Fetcher[TradierOptionsChainsQueryParams, List[TradierOptionsChainsData]]
 ):
     """Tradier Options Chains Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TradierOptionsChainsQueryParams:
+        """Transform the query parameters."""
         return TradierOptionsChainsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: TradierOptionsChainsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Return the raw data from the Tradier endpoint"""
-
+        """Return the raw data from the Tradier endpoint."""
         api_key = credentials.get("tradier_api_key") if credentials else ""
         sandbox = True
 
         if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
             raise ValueError(
                 "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
             )
@@ -212,15 +211,14 @@
             "Authorization": f"Bearer {api_key}",
             "Accept": "application/json",
         }
 
         # Get the expiration dates for the symbol so we can gather the chains data.
         async def get_expirations(symbol):
             """Get the expiration dates for the given symbol."""
-
             url = (
                 f"{BASE_URL}expirations?symbol={symbol}&includeAllRoots=true"
                 "&strikes=false&contractSize=false&expirationType=false"
             )
             response = await amake_request(url, headers=HEADERS)
             if response.get("expirations") and isinstance(response["expirations"].get("date"), list):  # type: ignore
                 expirations = response["expirations"].get("date")  # type: ignore
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
             check_item(v.lower(), COUNTRIES)
             result.append(v.lower())
         return ",".join(result)
 
     @field_validator("importance")
     @classmethod
     def importance_to_number(cls, v):
+        """Convert importance to number."""
         string_to_value = {"Low": 1, "Medium": 2, "High": 3}
         return string_to_value.get(v, None)
 
 
 class TEEconomicCalendarData(EconomicCalendarData):
     """Trading Economics Economic Calendar Data."""
 
@@ -89,14 +90,15 @@
         "previous": "Previous",
         "revised": "Revised",
     }
 
     @field_validator("date", mode="before")
     @classmethod
     def validate_date(cls, v: str) -> datetime:
+        """Validate the date."""
         return to_datetime(v, utc=True)
 
 
 class TEEconomicCalendarFetcher(
     Fetcher[
         TEEconomicCalendarQueryParams,
         List[TEEconomicCalendarData],
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Countries list for Trading Economics API."""
+
 country_dict = {
     "G20": [
         "United States",
         "Euro Area",
         "China",
         "Japan",
         "Germany",
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from datetime import date
 from typing import Dict, List
 from urllib.parse import quote, urlencode
 
 
 def check_args(query_args: Dict, to_include: List[str]):
+    """Check if all fields in to_include are present in query_args."""
     available_args = ["country", "start_date", "end_date", "importance", "group"]
 
     # Check if all fields in to_include are present in query_args
     # and elements in available_args that are not in to_include are not present in query_args
     return all(field in query_args for field in to_include) and all(
         field not in query_args for field in available_args if field not in to_include
     )
 
 
 def generate_url(in_query):
-    """
-    Generate the url for trading economimcs.  There is not a single api endpoint to hit so these are
-    generated based on the combinations.  There are also some combinations that return no data so that will return ""
+    """Generate the url for trading economimcs.
+
+    There is not a single api endpoint to hit so these are generated based on the combinations.
+    There are also some combinations that return no data so that will return an empty string.
     """
     # Converting the input query to a dict of params that are not None
     query = {k: v for k, v in in_query.dict().items() if v is not None}
 
     # Nothing -- just a snapshot
     if not query:
         return "https://api.tradingeconomics.com/calendar?c="
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> YFinanceAvailableIndicesQueryParams:
         """Transform the query params."""
         return YFinanceAvailableIndicesQueryParams(**params)
 
     @staticmethod
     def extract_data(
-        query: YFinanceAvailableIndicesQueryParams,
+        query: YFinanceAvailableIndicesQueryParams,  # pylint disable=unused-argument
         credentials: Optional[Dict[str, str]],
-        **kwargs: Any,
     ) -> List[Dict]:
+        """Extract the data."""
         indices = pd.DataFrame(INDICES).transpose().reset_index()
         indices.columns = ["code", "name", "ticker"]
 
         return indices.to_dict("records")
 
     @staticmethod
     def transform_data(
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404090009/pyproject.toml` & `openbb_nightly-4.1.6.dev202404100009/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.6.dev202404090009"
+version = "4.1.6.dev202404100009"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
```

### Comparing `openbb_nightly-4.1.6.dev202404090009/PKG-INFO` & `openbb_nightly-4.1.6.dev202404100009/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.6.dev202404090009
+Version: 4.1.6.dev202404100009
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


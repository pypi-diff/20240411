# Comparing `tmp/grimoire_elk-1.0.0rc1.tar.gz` & `tmp/grimoire_elk-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoire_elk-1.0.0rc1.tar", max compression
+gzip compressed data, was "grimoire_elk-1.0.0rc2.tar", max compression
```

## Comparing `grimoire_elk-1.0.0rc1.tar` & `grimoire_elk-1.0.0rc2.tar`

### file list

```diff
@@ -1,248 +1,248 @@
--rw-r--r--   0        0        0      468 2024-04-09 16:28:32.315883 grimoire_elk-1.0.0rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0    27832 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/NEWS
--rw-r--r--   0        0        0    14186 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/README.md
--rw-r--r--   0        0        0      894 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/__init__.py
--rw-r--r--   0        0        0       91 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/_version.py
--rw-r--r--   0        0        0    23287 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic.py
--rw-r--r--   0        0        0     1642 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic_analyzer.py
--rw-r--r--   0        0        0    15494 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic_items.py
--rw-r--r--   0        0        0     1653 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic_mapping.py
--rwxr-xr-x   0        0        0    36859 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elk.py
--rw-r--r--   0        0        0        0 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/__init__.py
--rw-r--r--   0        0        0    14023 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/askbot.py
--rw-r--r--   0        0        0     7751 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzilla.py
--rw-r--r--   0        0        0     6067 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzillarest.py
--rw-r--r--   0        0        0    12774 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/ceres_base.py
--rw-r--r--   0        0        0    15605 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/cocom.py
--rw-r--r--   0        0        0    16481 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/colic.py
--rw-r--r--   0        0        0     5141 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/confluence.py
--rw-r--r--   0        0        0     5296 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/crates.py
--rw-r--r--   0        0        0    12597 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/discourse.py
--rw-r--r--   0        0        0     4956 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerdeps.py
--rw-r--r--   0        0        0     6144 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerhub.py
--rw-r--r--   0        0        0     5187 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockersmells.py
--rw-r--r--   0        0        0    97698 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/enrich.py
--rw-r--r--   0        0        0     6242 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/functest.py
--rw-r--r--   0        0        0    32547 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gerrit.py
--rw-r--r--   0        0        0    46730 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/git.py
--rw-r--r--   0        0        0    36818 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github.py
--rw-r--r--   0        0        0    28496 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github2.py
--rw-r--r--   0        0        0     5505 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github_study_evolution.py
--rw-r--r--   0        0        0    33292 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/githubql.py
--rw-r--r--   0        0        0    16523 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitlab.py
--rw-r--r--   0        0        0     5673 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitter.py
--rw-r--r--   0        0        0     1670 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/google_hits.py
--rw-r--r--   0        0        0     5648 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/graal_study_evolution.py
--rw-r--r--   0        0        0      897 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/groupsio.py
--rw-r--r--   0        0        0      908 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/hyperkitty.py
--rw-r--r--   0        0        0     8614 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jenkins.py
--rw-r--r--   0        0        0    18534 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jira.py
--rw-r--r--   0        0        0     9440 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/kitsune.py
--rw-r--r--   0        0        0     8062 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/launchpad.py
--rw-r--r--   0        0        0     2552 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc.json
--rw-r--r--   0        0        0     2295 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc_es7.json
--rw-r--r--   0        0        0      981 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion.json
--rw-r--r--   0        0        0      961 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion_es7.json
--rw-r--r--   0        0        0     9237 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mattermost.py
--rw-r--r--   0        0        0     8409 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox.py
--rw-r--r--   0        0        0    16606 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox_study_kip.py
--rw-r--r--   0        0        0     9113 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mediawiki.py
--rw-r--r--   0        0        0    13622 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/meetup.py
--rw-r--r--   0        0        0     6172 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mozillaclub.py
--rw-r--r--   0        0        0     1052 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/nntp.py
--rw-r--r--   0        0        0    13120 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pagure.py
--rw-r--r--   0        0        0    16022 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/phabricator.py
--rw-r--r--   0        0        0      907 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pipermail.py
--rw-r--r--   0        0        0     6687 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/puppetforge.py
--rw-r--r--   0        0        0     5566 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/redmine.py
--rw-r--r--   0        0        0     8301 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/remo.py
--rw-r--r--   0        0        0     6787 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rocketchat.py
--rw-r--r--   0        0        0     3481 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rss.py
--rw-r--r--   0        0        0    23552 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/slack.py
--rw-r--r--   0        0        0    19794 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/sortinghat_gelk.py
--rw-r--r--   0        0        0    10011 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/stackexchange.py
--rw-r--r--   0        0        0     8795 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_aoc.py
--rw-r--r--   0        0        0    16420 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_onion.py
--rw-r--r--   0        0        0     3362 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/supybot.py
--rw-r--r--   0        0        0     5328 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/telegram.py
--rw-r--r--   0        0        0     5431 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/twitter.py
--rwxr-xr-x   0        0        0     8567 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/utils.py
--rw-r--r--   0        0        0     6565 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/weblate.py
--rw-r--r--   0        0        0     1309 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/errors.py
--rw-r--r--   0        0        0        0 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/git.py
--rw-r--r--   0        0        0     2712 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/github.py
--rw-r--r--   0        0        0     1722 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/gitlab.py
--rw-r--r--   0        0        0     1237 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/identities.py
--rw-r--r--   0        0        0     1835 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/meetup.py
--rw-r--r--   0        0        0     1916 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/stackexchange.py
--rw-r--r--   0        0        0        0 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/__init__.py
--rw-r--r--   0        0        0     2181 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/askbot.py
--rw-r--r--   0        0        0     2450 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzilla.py
--rw-r--r--   0        0        0     4458 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzillarest.py
--rw-r--r--   0        0        0     2831 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/confluence.py
--rw-r--r--   0        0        0     1836 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/crates.py
--rw-r--r--   0        0        0     3488 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/discourse.py
--rw-r--r--   0        0        0     2036 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/dockerhub.py
--rw-r--r--   0        0        0    11185 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/elastic.py
--rw-r--r--   0        0        0     2341 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/functest.py
--rw-r--r--   0        0        0     3017 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/gerrit.py
--rw-r--r--   0        0        0     2728 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/git.py
--rw-r--r--   0        0        0     4828 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/github.py
--rw-r--r--   0        0        0     1853 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/githubql.py
--rw-r--r--   0        0        0     3448 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitlab.py
--rw-r--r--   0        0        0     1831 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitter.py
--rw-r--r--   0        0        0      903 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/google_hits.py
--rw-r--r--   0        0        0     2327 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/graal.py
--rw-r--r--   0        0        0      882 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/groupsio.py
--rw-r--r--   0        0        0     1831 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/hyperkitty.py
--rw-r--r--   0        0        0     5603 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/jenkins.py
--rw-r--r--   0        0        0     3442 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/jira.py
--rw-r--r--   0        0        0     2407 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/kitsune.py
--rw-r--r--   0        0        0     1870 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/launchpad.py
--rw-r--r--   0        0        0     5204 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mattermost.py
--rw-r--r--   0        0        0     2249 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mbox.py
--rw-r--r--   0        0        0     2128 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mediawiki.py
--rw-r--r--   0        0        0     2666 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/meetup.py
--rw-r--r--   0        0        0     1882 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mozillaclub.py
--rw-r--r--   0        0        0     2113 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/nntp.py
--rw-r--r--   0        0        0     1921 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/pagure.py
--rw-r--r--   0        0        0     3052 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/phabricator.py
--rw-r--r--   0        0        0      892 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/pipermail.py
--rw-r--r--   0        0        0      874 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/puppetforge.py
--rw-r--r--   0        0        0     2088 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/redmine.py
--rw-r--r--   0        0        0     1788 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/remo.py
--rw-r--r--   0        0        0     1863 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/rocketchat.py
--rw-r--r--   0        0        0     2023 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/rss.py
--rw-r--r--   0        0        0     3084 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/slack.py
--rw-r--r--   0        0        0     2613 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/stackexchange.py
--rw-r--r--   0        0        0     1044 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/supybot.py
--rw-r--r--   0        0        0      877 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/telegram.py
--rw-r--r--   0        0        0     3815 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/twitter.py
--rw-r--r--   0        0        0     1899 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/weblate.py
--rwxr-xr-x   0        0        0    20183 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/utils.py
--rw-r--r--   0        0        0     2144 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      775 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/README.md
--rw-r--r--   0        0        0        0 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0    16169 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/base.py
--rw-r--r--   0        0        0   317579 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/data/askbot.json
--rw-r--r--   0        0        0     1262 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_1.json
--rw-r--r--   0        0        0     1262 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_2.json
--rw-r--r--   0        0        0      282 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_empty.json
--rw-r--r--   0        0        0   123043 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzilla.json
--rw-r--r--   0        0        0    13208 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzillarest-item-bulgarian.json
--rw-r--r--   0        0        0      189 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzillarest-projects.json
--rw-r--r--   0        0        0   742238 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzillarest.json
--rw-r--r--   0        0        0    12691 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/cocom.json
--rw-r--r--   0        0        0    16260 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/colic.json
--rw-r--r--   0        0        0    66663 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/confluence.json
--rw-r--r--   0        0        0     8772 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/confluence_with_credentials.json
--rw-r--r--   0        0        0   155992 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/crates.json
--rw-r--r--   0        0        0   544021 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/discourse.json
--rw-r--r--   0        0        0    37574 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/dockerdeps.json
--rw-r--r--   0        0        0   115251 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/dockerhub.json
--rw-r--r--   0        0        0    11347 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/dockersmells.json
--rw-r--r--   0        0        0    53387 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/functest.json
--rw-r--r--   0        0        0   279521 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/functest_wrong.json
--rw-r--r--   0        0        0   843001 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/gerrit.json
--rw-r--r--   0        0        0    15713 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/git.json
--rw-r--r--   0        0        0   244775 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/github.json
--rw-r--r--   0        0        0   234447 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/github2.json
--rw-r--r--   0        0        0    75664 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/githubql.json
--rw-r--r--   0        0        0   672068 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/gitlab.json
--rw-r--r--   0        0        0    12297 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/gitter.json
--rw-r--r--   0        0        0   330892 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/gmane.json
--rw-r--r--   0        0        0     2025 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/google_hits.json
--rw-r--r--   0        0        0   346405 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/groupsio.json
--rw-r--r--   0        0        0     8313 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/hyperkitty.json
--rw-r--r--   0        0        0   384247 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jenkins.json
--rw-r--r--   0        0        0   185733 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jira.json
--rw-r--r--   0        0        0      649 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jira_enriched_fields.json
--rw-r--r--   0        0        0    20498 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jira_new.json
--rw-r--r--   0        0        0   378857 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/jira_raw_fields.json
--rw-r--r--   0        0        0    17761 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/kitsune.json
--rw-r--r--   0        0        0    79536 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/launchpad.json
--rw-r--r--   0        0        0   210275 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mattermost.json
--rw-r--r--   0        0        0   269992 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mbox.json
--rw-r--r--   0        0        0    57533 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mediawiki.json
--rw-r--r--   0        0        0   324979 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/meetup.json
--rw-r--r--   0        0        0   296278 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mozillaclub.json
--rw-r--r--   0        0        0   115901 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/nntp.json
--rw-r--r--   0        0        0    54714 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/pagure.json
--rw-r--r--   0        0        0   112410 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/phabricator.json
--rw-r--r--   0        0        0   298460 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/pipermail.json
--rw-r--r--   0        0        0      101 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/projects-release-mediawiki-uc2.json
--rw-r--r--   0        0        0     3760 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/projects-release.json
--rw-r--r--   0        0        0    44809 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/puppetforge.json
--rw-r--r--   0        0        0   103516 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/redmine.json
--rw-r--r--   0        0        0   105975 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/remo.json
--rw-r--r--   0        0        0    50742 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/rocketchat.json
--rw-r--r--   0        0        0   131368 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/rss.json
--rw-r--r--   0        0        0    43442 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/slack.json
--rw-r--r--   0        0        0    92013 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/stackexchange.json
--rw-r--r--   0        0        0     8311 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/supybot.json
--rw-r--r--   0        0        0     2032 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/task-identities-data.json
--rw-r--r--   0        0        0    12597 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/telegram.json
--rw-r--r--   0        0        0    44540 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/data/twitter.json
--rw-r--r--   0        0        0     8339 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/data/weblate.json
--rw-r--r--   0        0        0    11214 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/model.py
--rwxr-xr-x   0        0        0      992 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/run_tests.py
--rw-r--r--   0        0        0     4180 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_askbot.py
--rw-r--r--   0        0        0     4678 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_bugzilla.py
--rw-r--r--   0        0        0     5330 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_bugzillarest.py
--rw-r--r--   0        0        0     7455 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_cocom.py
--rw-r--r--   0        0        0     6691 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_colic.py
--rw-r--r--   0        0        0     9722 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_confluence.py
--rw-r--r--   0        0        0     4466 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_crates.py
--rw-r--r--   0        0        0    10044 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_discourse.py
--rw-r--r--   0        0        0     4687 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_dockerdeps.py
--rw-r--r--   0        0        0     4082 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_dockerhub.py
--rw-r--r--   0        0        0     5813 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_dockersmells.py
--rw-r--r--   0        0        0    32434 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elastic.py
--rw-r--r--   0        0        0    20552 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elastic_items.py
--rw-r--r--   0        0        0     2791 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elastic_ocean.py
--rw-r--r--   0        0        0     4636 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elk.py
--rw-r--r--   0        0        0    34090 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_enrich.py
--rw-r--r--   0        0        0     1906 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_enrich_jira.py
--rw-r--r--   0        0        0     2451 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_errors.py
--rw-r--r--   0        0        0     4776 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_functest.py
--rw-r--r--   0        0        0    17512 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_gerrit.py
--rw-r--r--   0        0        0    41064 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_git.py
--rw-r--r--   0        0        0    21320 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_github.py
--rw-r--r--   0        0        0    15209 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_github2.py
--rw-r--r--   0        0        0    23121 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_githubql.py
--rw-r--r--   0        0        0    15573 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_gitlab.py
--rw-r--r--   0        0        0    10355 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_gitter.py
--rw-r--r--   0        0        0     3353 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_google_hits.py
--rw-r--r--   0        0        0     4398 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_groupsio.py
--rw-r--r--   0        0        0     4700 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_hyperkitty.py
--rw-r--r--   0        0        0     5747 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_jenkins.py
--rw-r--r--   0        0        0     8950 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_jira.py
--rw-r--r--   0        0        0     5503 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_kitsune.py
--rw-r--r--   0        0        0    15777 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_launchpad.py
--rw-r--r--   0        0        0     4677 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_load_identities.py
--rw-r--r--   0        0        0    10822 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mattermost.py
--rw-r--r--   0        0        0     8469 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mbox.py
--rw-r--r--   0        0        0    12014 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mediawiki.py
--rw-r--r--   0        0        0     7827 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_meetup.py
--rw-r--r--   0        0        0     4818 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mozillaclub.py
--rw-r--r--   0        0        0     5533 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_nntp.py
--rw-r--r--   0        0        0    11163 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_pagure.py
--rw-r--r--   0        0        0     4439 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_phabricator.py
--rw-r--r--   0        0        0     4549 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_pipermail.py
--rw-r--r--   0        0        0     4950 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_projects.sql
--rw-r--r--   0        0        0     4189 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_puppetforge.py
--rw-r--r--   0        0        0     5116 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_redmine.py
--rw-r--r--   0        0        0     4170 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_remo.py
--rw-r--r--   0        0        0     5900 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_rocketchat.py
--rw-r--r--   0        0        0     4173 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_rss.py
--rw-r--r--   0        0        0     5681 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_slack.py
--rw-r--r--   0        0        0    14524 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_sortinghat_gelk.py
--rw-r--r--   0        0        0     6478 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_stackexchange.py
--rw-r--r--   0        0        0     4697 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_supybot.py
--rw-r--r--   0        0        0     5967 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_telegram.py
--rw-r--r--   0        0        0     4178 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_twitter.py
--rw-r--r--   0        0        0    11146 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_weblate.py
--rw-r--r--   0        0        0      137 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/tests.conf
--rw-r--r--   0        0        0    15901 1970-01-01 00:00:00.000000 grimoire_elk-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      468 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    27832 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/NEWS
+-rw-r--r--   0        0        0    14186 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/README.md
+-rw-r--r--   0        0        0      894 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/_version.py
+-rw-r--r--   0        0        0    23287 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/elastic.py
+-rw-r--r--   0        0        0     1642 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/elastic_analyzer.py
+-rw-r--r--   0        0        0    15494 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/elastic_items.py
+-rw-r--r--   0        0        0     1653 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/elastic_mapping.py
+-rwxr-xr-x   0        0        0    36859 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/elk.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/__init__.py
+-rw-r--r--   0        0        0    14023 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/askbot.py
+-rw-r--r--   0        0        0     7751 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/bugzilla.py
+-rw-r--r--   0        0        0     6067 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/bugzillarest.py
+-rw-r--r--   0        0        0    12774 2024-04-11 11:01:52.071354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/ceres_base.py
+-rw-r--r--   0        0        0    15605 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/cocom.py
+-rw-r--r--   0        0        0    16481 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/colic.py
+-rw-r--r--   0        0        0     5141 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/confluence.py
+-rw-r--r--   0        0        0     5296 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/crates.py
+-rw-r--r--   0        0        0    12597 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/discourse.py
+-rw-r--r--   0        0        0     4956 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/dockerdeps.py
+-rw-r--r--   0        0        0     6144 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/dockerhub.py
+-rw-r--r--   0        0        0     5187 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/dockersmells.py
+-rw-r--r--   0        0        0    97698 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/enrich.py
+-rw-r--r--   0        0        0     6242 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/functest.py
+-rw-r--r--   0        0        0    32547 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/gerrit.py
+-rw-r--r--   0        0        0    46730 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/git.py
+-rw-r--r--   0        0        0    36818 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/github.py
+-rw-r--r--   0        0        0    28496 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/github2.py
+-rw-r--r--   0        0        0     5505 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/github_study_evolution.py
+-rw-r--r--   0        0        0    33292 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/githubql.py
+-rw-r--r--   0        0        0    16523 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/gitlab.py
+-rw-r--r--   0        0        0     5673 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/gitter.py
+-rw-r--r--   0        0        0     1670 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/google_hits.py
+-rw-r--r--   0        0        0     5648 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/graal_study_evolution.py
+-rw-r--r--   0        0        0      897 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/groupsio.py
+-rw-r--r--   0        0        0      908 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/hyperkitty.py
+-rw-r--r--   0        0        0     8614 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/jenkins.py
+-rw-r--r--   0        0        0    18534 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/jira.py
+-rw-r--r--   0        0        0     9440 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/kitsune.py
+-rw-r--r--   0        0        0     8062 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/launchpad.py
+-rw-r--r--   0        0        0     2552 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/git_aoc.json
+-rw-r--r--   0        0        0     2295 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/git_aoc_es7.json
+-rw-r--r--   0        0        0      981 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/onion.json
+-rw-r--r--   0        0        0      961 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/onion_es7.json
+-rw-r--r--   0        0        0     9237 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mattermost.py
+-rw-r--r--   0        0        0     8409 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mbox.py
+-rw-r--r--   0        0        0    16606 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mbox_study_kip.py
+-rw-r--r--   0        0        0     9113 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mediawiki.py
+-rw-r--r--   0        0        0    13622 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/meetup.py
+-rw-r--r--   0        0        0     6172 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mozillaclub.py
+-rw-r--r--   0        0        0     1052 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/nntp.py
+-rw-r--r--   0        0        0    13120 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/pagure.py
+-rw-r--r--   0        0        0    16022 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/phabricator.py
+-rw-r--r--   0        0        0      907 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/pipermail.py
+-rw-r--r--   0        0        0     6687 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/puppetforge.py
+-rw-r--r--   0        0        0     5566 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/redmine.py
+-rw-r--r--   0        0        0     8301 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/remo.py
+-rw-r--r--   0        0        0     6787 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/rocketchat.py
+-rw-r--r--   0        0        0     3481 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/rss.py
+-rw-r--r--   0        0        0    23552 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/slack.py
+-rw-r--r--   0        0        0    19794 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/sortinghat_gelk.py
+-rw-r--r--   0        0        0    10011 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/stackexchange.py
+-rw-r--r--   0        0        0     8795 2024-04-11 11:01:52.075354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/study_ceres_aoc.py
+-rw-r--r--   0        0        0    16420 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/study_ceres_onion.py
+-rw-r--r--   0        0        0     3362 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/supybot.py
+-rw-r--r--   0        0        0     5328 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/telegram.py
+-rw-r--r--   0        0        0     5431 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/twitter.py
+-rwxr-xr-x   0        0        0     8567 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/utils.py
+-rw-r--r--   0        0        0     6565 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/enriched/weblate.py
+-rw-r--r--   0        0        0     1309 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/errors.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/identities/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/identities/git.py
+-rw-r--r--   0        0        0     2712 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/identities/github.py
+-rw-r--r--   0        0        0     1722 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/identities/gitlab.py
+-rw-r--r--   0        0        0     1237 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/identities/identities.py
+-rw-r--r--   0        0        0     1835 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/identities/meetup.py
+-rw-r--r--   0        0        0     1916 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/identities/stackexchange.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/__init__.py
+-rw-r--r--   0        0        0     2181 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/askbot.py
+-rw-r--r--   0        0        0     2450 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/bugzilla.py
+-rw-r--r--   0        0        0     4458 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/bugzillarest.py
+-rw-r--r--   0        0        0     2831 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/confluence.py
+-rw-r--r--   0        0        0     1836 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/crates.py
+-rw-r--r--   0        0        0     3488 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/discourse.py
+-rw-r--r--   0        0        0     2036 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/dockerhub.py
+-rw-r--r--   0        0        0    11185 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/elastic.py
+-rw-r--r--   0        0        0     2341 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/functest.py
+-rw-r--r--   0        0        0     3017 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/gerrit.py
+-rw-r--r--   0        0        0     2728 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/git.py
+-rw-r--r--   0        0        0     4828 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/github.py
+-rw-r--r--   0        0        0     1853 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/githubql.py
+-rw-r--r--   0        0        0     3448 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/gitlab.py
+-rw-r--r--   0        0        0     1831 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/gitter.py
+-rw-r--r--   0        0        0      903 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/google_hits.py
+-rw-r--r--   0        0        0     2327 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/graal.py
+-rw-r--r--   0        0        0      882 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/groupsio.py
+-rw-r--r--   0        0        0     1831 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/hyperkitty.py
+-rw-r--r--   0        0        0     5603 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/jenkins.py
+-rw-r--r--   0        0        0     3442 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/jira.py
+-rw-r--r--   0        0        0     2407 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/kitsune.py
+-rw-r--r--   0        0        0     1870 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/launchpad.py
+-rw-r--r--   0        0        0     5204 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/mattermost.py
+-rw-r--r--   0        0        0     2435 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/mbox.py
+-rw-r--r--   0        0        0     2128 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/mediawiki.py
+-rw-r--r--   0        0        0     2666 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/meetup.py
+-rw-r--r--   0        0        0     1882 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/mozillaclub.py
+-rw-r--r--   0        0        0     2113 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/nntp.py
+-rw-r--r--   0        0        0     1921 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/pagure.py
+-rw-r--r--   0        0        0     3052 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/phabricator.py
+-rw-r--r--   0        0        0      892 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/pipermail.py
+-rw-r--r--   0        0        0      874 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/puppetforge.py
+-rw-r--r--   0        0        0     2088 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/redmine.py
+-rw-r--r--   0        0        0     1788 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/remo.py
+-rw-r--r--   0        0        0     1863 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/rocketchat.py
+-rw-r--r--   0        0        0     2023 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/rss.py
+-rw-r--r--   0        0        0     3084 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/slack.py
+-rw-r--r--   0        0        0     2613 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/stackexchange.py
+-rw-r--r--   0        0        0     1044 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/supybot.py
+-rw-r--r--   0        0        0      877 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/telegram.py
+-rw-r--r--   0        0        0     3815 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/twitter.py
+-rw-r--r--   0        0        0     1899 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/raw/weblate.py
+-rwxr-xr-x   0        0        0    20183 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/grimoire_elk/utils.py
+-rw-r--r--   0        0        0     2144 2024-04-11 11:01:52.079354 grimoire_elk-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      775 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0    16169 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/base.py
+-rw-r--r--   0        0        0   317579 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/data/askbot.json
+-rw-r--r--   0        0        0     1262 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/data/author_min_max_dates_1.json
+-rw-r--r--   0        0        0     1262 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/data/author_min_max_dates_2.json
+-rw-r--r--   0        0        0      282 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/data/author_min_max_dates_empty.json
+-rw-r--r--   0        0        0   123043 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/data/bugzilla.json
+-rw-r--r--   0        0        0    13208 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/data/bugzillarest-item-bulgarian.json
+-rw-r--r--   0        0        0      189 2024-04-11 11:01:52.087354 grimoire_elk-1.0.0rc2/tests/data/bugzillarest-projects.json
+-rw-r--r--   0        0        0   742238 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/bugzillarest.json
+-rw-r--r--   0        0        0    12691 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/cocom.json
+-rw-r--r--   0        0        0    16260 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/colic.json
+-rw-r--r--   0        0        0    66663 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/confluence.json
+-rw-r--r--   0        0        0     8772 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/confluence_with_credentials.json
+-rw-r--r--   0        0        0   155992 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/crates.json
+-rw-r--r--   0        0        0   544021 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/discourse.json
+-rw-r--r--   0        0        0    37574 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/dockerdeps.json
+-rw-r--r--   0        0        0   115251 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/dockerhub.json
+-rw-r--r--   0        0        0    11347 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/dockersmells.json
+-rw-r--r--   0        0        0    53387 2024-04-11 11:01:52.091354 grimoire_elk-1.0.0rc2/tests/data/functest.json
+-rw-r--r--   0        0        0   279521 2024-04-11 11:01:52.095354 grimoire_elk-1.0.0rc2/tests/data/functest_wrong.json
+-rw-r--r--   0        0        0   843001 2024-04-11 11:01:52.095354 grimoire_elk-1.0.0rc2/tests/data/gerrit.json
+-rw-r--r--   0        0        0    15713 2024-04-11 11:01:52.095354 grimoire_elk-1.0.0rc2/tests/data/git.json
+-rw-r--r--   0        0        0   244775 2024-04-11 11:01:52.095354 grimoire_elk-1.0.0rc2/tests/data/github.json
+-rw-r--r--   0        0        0   234447 2024-04-11 11:01:52.095354 grimoire_elk-1.0.0rc2/tests/data/github2.json
+-rw-r--r--   0        0        0    75664 2024-04-11 11:01:52.099354 grimoire_elk-1.0.0rc2/tests/data/githubql.json
+-rw-r--r--   0        0        0   672068 2024-04-11 11:01:52.099354 grimoire_elk-1.0.0rc2/tests/data/gitlab.json
+-rw-r--r--   0        0        0    12297 2024-04-11 11:01:52.099354 grimoire_elk-1.0.0rc2/tests/data/gitter.json
+-rw-r--r--   0        0        0   330892 2024-04-11 11:01:52.099354 grimoire_elk-1.0.0rc2/tests/data/gmane.json
+-rw-r--r--   0        0        0     2025 2024-04-11 11:01:52.099354 grimoire_elk-1.0.0rc2/tests/data/google_hits.json
+-rw-r--r--   0        0        0   346405 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/groupsio.json
+-rw-r--r--   0        0        0     8313 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/hyperkitty.json
+-rw-r--r--   0        0        0   384247 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/jenkins.json
+-rw-r--r--   0        0        0   185733 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/jira.json
+-rw-r--r--   0        0        0      649 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/jira_enriched_fields.json
+-rw-r--r--   0        0        0    20498 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/jira_new.json
+-rw-r--r--   0        0        0   378857 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/jira_raw_fields.json
+-rw-r--r--   0        0        0    17761 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/kitsune.json
+-rw-r--r--   0        0        0    79536 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/launchpad.json
+-rw-r--r--   0        0        0   210275 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/mattermost.json
+-rw-r--r--   0        0        0   269992 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/mbox.json
+-rw-r--r--   0        0        0    57533 2024-04-11 11:01:52.103354 grimoire_elk-1.0.0rc2/tests/data/mediawiki.json
+-rw-r--r--   0        0        0   324979 2024-04-11 11:01:52.107354 grimoire_elk-1.0.0rc2/tests/data/meetup.json
+-rw-r--r--   0        0        0   296278 2024-04-11 11:01:52.107354 grimoire_elk-1.0.0rc2/tests/data/mozillaclub.json
+-rw-r--r--   0        0        0   115901 2024-04-11 11:01:52.107354 grimoire_elk-1.0.0rc2/tests/data/nntp.json
+-rw-r--r--   0        0        0    54714 2024-04-11 11:01:52.107354 grimoire_elk-1.0.0rc2/tests/data/pagure.json
+-rw-r--r--   0        0        0   112410 2024-04-11 11:01:52.107354 grimoire_elk-1.0.0rc2/tests/data/phabricator.json
+-rw-r--r--   0        0        0   298460 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/pipermail.json
+-rw-r--r--   0        0        0      101 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/projects-release-mediawiki-uc2.json
+-rw-r--r--   0        0        0     3760 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/projects-release.json
+-rw-r--r--   0        0        0    44809 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/puppetforge.json
+-rw-r--r--   0        0        0   103516 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/redmine.json
+-rw-r--r--   0        0        0   105975 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/remo.json
+-rw-r--r--   0        0        0    50742 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/rocketchat.json
+-rw-r--r--   0        0        0   131368 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/rss.json
+-rw-r--r--   0        0        0    43442 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/slack.json
+-rw-r--r--   0        0        0    92013 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/stackexchange.json
+-rw-r--r--   0        0        0     8311 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/supybot.json
+-rw-r--r--   0        0        0     2032 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/task-identities-data.json
+-rw-r--r--   0        0        0    12597 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/telegram.json
+-rw-r--r--   0        0        0    44540 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/twitter.json
+-rw-r--r--   0        0        0     8339 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/data/weblate.json
+-rw-r--r--   0        0        0    11214 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/model.py
+-rwxr-xr-x   0        0        0      992 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/run_tests.py
+-rw-r--r--   0        0        0     4180 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_askbot.py
+-rw-r--r--   0        0        0     4678 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_bugzilla.py
+-rw-r--r--   0        0        0     5330 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_bugzillarest.py
+-rw-r--r--   0        0        0     7455 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_cocom.py
+-rw-r--r--   0        0        0     6691 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_colic.py
+-rw-r--r--   0        0        0     9722 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_confluence.py
+-rw-r--r--   0        0        0     4466 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_crates.py
+-rw-r--r--   0        0        0    10044 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_discourse.py
+-rw-r--r--   0        0        0     4687 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_dockerdeps.py
+-rw-r--r--   0        0        0     4082 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_dockerhub.py
+-rw-r--r--   0        0        0     5813 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_dockersmells.py
+-rw-r--r--   0        0        0    32434 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_elastic.py
+-rw-r--r--   0        0        0    20552 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_elastic_items.py
+-rw-r--r--   0        0        0     2791 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_elastic_ocean.py
+-rw-r--r--   0        0        0     4636 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_elk.py
+-rw-r--r--   0        0        0    34090 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_enrich.py
+-rw-r--r--   0        0        0     1906 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_enrich_jira.py
+-rw-r--r--   0        0        0     2451 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_errors.py
+-rw-r--r--   0        0        0     4776 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_functest.py
+-rw-r--r--   0        0        0    17512 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_gerrit.py
+-rw-r--r--   0        0        0    41064 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_git.py
+-rw-r--r--   0        0        0    21320 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_github.py
+-rw-r--r--   0        0        0    15209 2024-04-11 11:01:52.111354 grimoire_elk-1.0.0rc2/tests/test_github2.py
+-rw-r--r--   0        0        0    23121 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_githubql.py
+-rw-r--r--   0        0        0    15573 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_gitlab.py
+-rw-r--r--   0        0        0    10355 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_gitter.py
+-rw-r--r--   0        0        0     3353 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_google_hits.py
+-rw-r--r--   0        0        0     4398 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_groupsio.py
+-rw-r--r--   0        0        0     4700 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_hyperkitty.py
+-rw-r--r--   0        0        0     5747 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_jenkins.py
+-rw-r--r--   0        0        0     8950 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_jira.py
+-rw-r--r--   0        0        0     5503 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_kitsune.py
+-rw-r--r--   0        0        0    15777 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_launchpad.py
+-rw-r--r--   0        0        0     4677 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_load_identities.py
+-rw-r--r--   0        0        0    10822 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_mattermost.py
+-rw-r--r--   0        0        0     8469 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_mbox.py
+-rw-r--r--   0        0        0    12014 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_mediawiki.py
+-rw-r--r--   0        0        0     7827 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_meetup.py
+-rw-r--r--   0        0        0     4818 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_mozillaclub.py
+-rw-r--r--   0        0        0     5533 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_nntp.py
+-rw-r--r--   0        0        0    11163 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_pagure.py
+-rw-r--r--   0        0        0     4439 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_phabricator.py
+-rw-r--r--   0        0        0     4549 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_pipermail.py
+-rw-r--r--   0        0        0     4950 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_projects.sql
+-rw-r--r--   0        0        0     4189 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_puppetforge.py
+-rw-r--r--   0        0        0     5116 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_redmine.py
+-rw-r--r--   0        0        0     4170 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_remo.py
+-rw-r--r--   0        0        0     5900 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_rocketchat.py
+-rw-r--r--   0        0        0     4173 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_rss.py
+-rw-r--r--   0        0        0     5681 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_slack.py
+-rw-r--r--   0        0        0    14524 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_sortinghat_gelk.py
+-rw-r--r--   0        0        0     6478 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_stackexchange.py
+-rw-r--r--   0        0        0     4697 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_supybot.py
+-rw-r--r--   0        0        0     5967 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_telegram.py
+-rw-r--r--   0        0        0     4178 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_twitter.py
+-rw-r--r--   0        0        0    11146 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/test_weblate.py
+-rw-r--r--   0        0        0      137 2024-04-11 11:01:52.115354 grimoire_elk-1.0.0rc2/tests/tests.conf
+-rw-r--r--   0        0        0    15901 1970-01-01 00:00:00.000000 grimoire_elk-1.0.0rc2/PKG-INFO
```

### Comparing `grimoire_elk-1.0.0rc1/LICENSE` & `grimoire_elk-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/NEWS` & `grimoire_elk-1.0.0rc2/NEWS`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/README.md` & `grimoire_elk-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/__init__.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/__init__.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/elastic.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/elastic.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/elastic_analyzer.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/elastic_analyzer.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/elastic_items.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/elastic_items.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/elastic_mapping.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/elastic_mapping.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/elk.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/elk.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/askbot.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/askbot.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzilla.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/bugzilla.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzillarest.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/bugzillarest.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/ceres_base.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/ceres_base.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/cocom.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/cocom.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/colic.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/colic.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/confluence.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/confluence.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/crates.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/crates.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/discourse.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/discourse.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerdeps.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/dockerdeps.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerhub.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/dockerhub.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockersmells.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/dockersmells.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/enrich.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/enrich.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/functest.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/functest.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gerrit.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/gerrit.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/git.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/git.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/github.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github2.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/github2.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github_study_evolution.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/github_study_evolution.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/githubql.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/githubql.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitlab.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/gitlab.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitter.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/gitter.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/google_hits.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/google_hits.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/graal_study_evolution.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/graal_study_evolution.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/groupsio.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/groupsio.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/hyperkitty.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/hyperkitty.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jenkins.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/jenkins.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jira.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/jira.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/kitsune.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/kitsune.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/launchpad.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/launchpad.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc.json` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/git_aoc.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc_es7.json` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/git_aoc_es7.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion.json` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/onion.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion_es7.json` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mappings/onion_es7.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mattermost.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mattermost.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mbox.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox_study_kip.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mbox_study_kip.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mediawiki.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mediawiki.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/meetup.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/meetup.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mozillaclub.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/mozillaclub.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/nntp.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/nntp.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pagure.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/pagure.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/phabricator.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/phabricator.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pipermail.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/pipermail.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/puppetforge.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/puppetforge.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/redmine.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/redmine.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/remo.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/remo.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rocketchat.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/rocketchat.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rss.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/rss.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/slack.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/slack.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/sortinghat_gelk.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/sortinghat_gelk.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/stackexchange.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/stackexchange.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_aoc.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/study_ceres_aoc.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_onion.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/study_ceres_onion.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/supybot.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/supybot.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/telegram.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/telegram.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/twitter.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/twitter.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/utils.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/utils.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/weblate.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/enriched/weblate.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/errors.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/errors.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/identities/git.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/identities/git.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/identities/github.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/identities/github.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/identities/gitlab.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/identities/gitlab.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/identities/identities.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/identities/identities.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/identities/meetup.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/identities/meetup.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/identities/stackexchange.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/identities/stackexchange.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/askbot.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/askbot.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzilla.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/bugzilla.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzillarest.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/bugzillarest.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/confluence.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/confluence.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/crates.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/crates.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/discourse.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/discourse.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/dockerhub.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/dockerhub.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/elastic.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/elastic.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/functest.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/functest.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/gerrit.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/gerrit.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/git.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/git.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/github.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/github.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/githubql.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/githubql.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitlab.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/gitlab.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitter.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/gitter.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/google_hits.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/google_hits.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/graal.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/graal.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/groupsio.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/groupsio.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/hyperkitty.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/hyperkitty.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/jenkins.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/jenkins.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/jira.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/jira.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/kitsune.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/kitsune.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/launchpad.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/launchpad.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mattermost.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/mattermost.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mbox.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/mozillaclub.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,67 +15,48 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
-import logging
-
-from .elastic import ElasticOcean
+from grimoire_elk.raw.elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
-logger = logging.getLogger(__name__)
-
-
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
-        Non dynamic discovery of type for:
-            * data.body (inmense field)
-
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
          {
             "dynamic":true,
                 "properties": {
                     "data": {
                         "properties": {
-                            "body": {
-                                "dynamic":false,
-                                "properties": {}
+                            "Event Creations": {
+                                "type": "text",
+                                "index": true
+                            },
+                            "Event Description": {
+                                "type": "text",
+                                "index": true
                             }
                         }
                     }
                 }
         }
         '''
 
         return {"items": mapping}
 
 
-class MBoxOcean(ElasticOcean):
-    """MBox Ocean feeder"""
+class MozillaClubOcean(ElasticOcean):
+    """MozillaClub Ocean feeder"""
 
     mapping = Mapping
-
-    @classmethod
-    def get_perceval_params_from_url(cls, url):
-        # In the url the uri and the data dir are included
-        params = url.split()
-
-        return params
-
-    def _fix_item(self, item):
-        # Remove all custom fields to avoid the 1000 fields limit in ES
-
-        fields = list(item["data"].keys())
-        for field in fields:
-            if field.lower().startswith("x-"):
-                item["data"].pop(field)
```

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mediawiki.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/mediawiki.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/meetup.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/meetup.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mozillaclub.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/redmine.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,48 +15,55 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
-from grimoire_elk.raw.elastic import ElasticOcean
+from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
+        Non dynamic discovery of type for:
+            * data.journals
+
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
          {
             "dynamic":true,
                 "properties": {
                     "data": {
                         "properties": {
-                            "Event Creations": {
+                            "journals": {
+                                "dynamic": false,
+                                "properties": {}
+                            },
+                            "subject": {
                                 "type": "text",
                                 "index": true
                             },
-                            "Event Description": {
+                            "description": {
                                 "type": "text",
                                 "index": true
                             }
                         }
                     }
                 }
         }
         '''
 
         return {"items": mapping}
 
 
-class MozillaClubOcean(ElasticOcean):
-    """MozillaClub Ocean feeder"""
+class RedmineOcean(ElasticOcean):
+    """Redmine Ocean feeder"""
 
     mapping = Mapping
```

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/nntp.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/nntp.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/pagure.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/pagure.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/phabricator.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/phabricator.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/pipermail.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/pipermail.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/puppetforge.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/puppetforge.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/redmine.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/remo.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,44 +26,37 @@
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
         Non dynamic discovery of type for:
-            * data.journals
+            * data.answers.answered_by
+            * data.author
 
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
          {
             "dynamic":true,
                 "properties": {
                     "data": {
                         "properties": {
-                            "journals": {
-                                "dynamic": false,
-                                "properties": {}
-                            },
-                            "subject": {
-                                "type": "text",
-                                "index": true
-                            },
                             "description": {
                                 "type": "text",
                                 "index": true
                             }
                         }
                     }
                 }
         }
         '''
 
         return {"items": mapping}
 
 
-class RedmineOcean(ElasticOcean):
-    """Redmine Ocean feeder"""
+class ReMoOcean(ElasticOcean):
+    """ReMo API v2 Ocean feeder"""
 
     mapping = Mapping
```

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/remo.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/rocketchat.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,51 +12,56 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Alvaro del Castillo San Felix <acs@bitergia.com>
+#   Animesh Kumar<animuz111@gmail.com>
 #
 
 from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
-        Non dynamic discovery of type for:
-            * data.answers.answered_by
-            * data.author
-
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
-         {
-            "dynamic":true,
+             {
+                "dynamic":true,
                 "properties": {
                     "data": {
-                        "properties": {
-                            "description": {
-                                "type": "text",
-                                "index": true
-                            }
-                        }
+                        "dynamic":false,
+                        "properties": {}
                     }
                 }
-        }
-        '''
+            }
+            '''
 
         return {"items": mapping}
 
 
-class ReMoOcean(ElasticOcean):
-    """ReMo API v2 Ocean feeder"""
+class RocketChatOcean(ElasticOcean):
+    """RocketChat Ocean feeder"""
 
     mapping = Mapping
+
+    @classmethod
+    def get_perceval_params_from_url(cls, url):
+        """ Get the perceval params given a URL for the data source """
+
+        params = []
+
+        tokens = url.split(' ')
+        server = tokens[0]
+        channel = tokens[1]
+        params.append(server)
+        params.append(channel)
+        return params
```

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/rocketchat.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/weblate.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Animesh Kumar<animuz111@gmail.com>
+#   Quan Zhou <quan@bitergia.com>
 #
 
 from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
         :param es_major: major version of Elasticsearch, as string
-        :returns:        dictionary with a key, 'items', with the mapping
+        :returns: dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
              {
                 "dynamic":true,
                 "properties": {
                     "data": {
@@ -44,24 +44,24 @@
                 }
             }
             '''
 
         return {"items": mapping}
 
 
-class RocketChatOcean(ElasticOcean):
-    """RocketChat Ocean feeder"""
+class WeblateOcean(ElasticOcean):
+    """Weblate Ocean feeder"""
 
     mapping = Mapping
 
-    @classmethod
-    def get_perceval_params_from_url(cls, url):
-        """ Get the perceval params given a URL for the data source """
-
-        params = []
-
-        tokens = url.split(' ')
-        server = tokens[0]
-        channel = tokens[1]
-        params.append(server)
-        params.append(channel)
-        return params
+    def _fix_item(self, item):
+        change = item['data']
+        if change.get('author_data', None) or not change['author']:
+            return
+
+        name = change['author'].split('api/users/')[1].split('/')[0]
+        author_data = {
+            'username': name,
+            'full_name': None,
+            'email': None
+        }
+        change['author_data'] = author_data
```

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/rss.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/rss.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/slack.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/slack.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/stackexchange.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/stackexchange.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/supybot.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/supybot.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/telegram.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/telegram.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/raw/twitter.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/raw/twitter.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/grimoire_elk/utils.py` & `grimoire_elk-1.0.0rc2/grimoire_elk/utils.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/pyproject.toml` & `grimoire_elk-1.0.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoire-elk"
-version = "1.0.0-rc.1"
+version = "1.0.0-rc.2"
 description = "GrimoireELK processes and stores software development data to ElasticSearch"
 readme = "README.md"
 authors = [
    "Bitergia <grimoirelab-discussions@lists.linuxfoundation.org>"
 ]
 repository = "https://github.com/chaoss/grimoirelab-elk"
 keywords = ["development repositories analytics"]
```

### Comparing `grimoire_elk-1.0.0rc1/tests/README.md` & `grimoire_elk-1.0.0rc2/tests/README.md`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/base.py` & `grimoire_elk-1.0.0rc2/tests/base.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/askbot.json` & `grimoire_elk-1.0.0rc2/tests/data/askbot.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_1.json` & `grimoire_elk-1.0.0rc2/tests/data/author_min_max_dates_1.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_2.json` & `grimoire_elk-1.0.0rc2/tests/data/author_min_max_dates_2.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/bugzilla.json` & `grimoire_elk-1.0.0rc2/tests/data/bugzilla.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/bugzillarest-item-bulgarian.json` & `grimoire_elk-1.0.0rc2/tests/data/bugzillarest-item-bulgarian.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/bugzillarest.json` & `grimoire_elk-1.0.0rc2/tests/data/bugzillarest.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/cocom.json` & `grimoire_elk-1.0.0rc2/tests/data/cocom.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/colic.json` & `grimoire_elk-1.0.0rc2/tests/data/colic.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/confluence.json` & `grimoire_elk-1.0.0rc2/tests/data/confluence.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/confluence_with_credentials.json` & `grimoire_elk-1.0.0rc2/tests/data/confluence_with_credentials.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/crates.json` & `grimoire_elk-1.0.0rc2/tests/data/crates.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/discourse.json` & `grimoire_elk-1.0.0rc2/tests/data/discourse.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/dockerdeps.json` & `grimoire_elk-1.0.0rc2/tests/data/dockerdeps.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/dockerhub.json` & `grimoire_elk-1.0.0rc2/tests/data/dockerhub.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/dockersmells.json` & `grimoire_elk-1.0.0rc2/tests/data/dockersmells.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/functest.json` & `grimoire_elk-1.0.0rc2/tests/data/functest.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/functest_wrong.json` & `grimoire_elk-1.0.0rc2/tests/data/functest_wrong.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/gerrit.json` & `grimoire_elk-1.0.0rc2/tests/data/gerrit.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/git.json` & `grimoire_elk-1.0.0rc2/tests/data/git.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/github.json` & `grimoire_elk-1.0.0rc2/tests/data/github.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/github2.json` & `grimoire_elk-1.0.0rc2/tests/data/github2.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/githubql.json` & `grimoire_elk-1.0.0rc2/tests/data/githubql.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/gitlab.json` & `grimoire_elk-1.0.0rc2/tests/data/gitlab.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/gitter.json` & `grimoire_elk-1.0.0rc2/tests/data/gitter.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/gmane.json` & `grimoire_elk-1.0.0rc2/tests/data/gmane.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/google_hits.json` & `grimoire_elk-1.0.0rc2/tests/data/google_hits.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/groupsio.json` & `grimoire_elk-1.0.0rc2/tests/data/groupsio.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/hyperkitty.json` & `grimoire_elk-1.0.0rc2/tests/data/hyperkitty.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/jenkins.json` & `grimoire_elk-1.0.0rc2/tests/data/jenkins.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/jira.json` & `grimoire_elk-1.0.0rc2/tests/data/jira.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/jira_enriched_fields.json` & `grimoire_elk-1.0.0rc2/tests/data/jira_enriched_fields.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/jira_new.json` & `grimoire_elk-1.0.0rc2/tests/data/jira_new.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/jira_raw_fields.json` & `grimoire_elk-1.0.0rc2/tests/data/jira_raw_fields.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/kitsune.json` & `grimoire_elk-1.0.0rc2/tests/data/kitsune.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/launchpad.json` & `grimoire_elk-1.0.0rc2/tests/data/launchpad.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/mattermost.json` & `grimoire_elk-1.0.0rc2/tests/data/mattermost.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/mbox.json` & `grimoire_elk-1.0.0rc2/tests/data/mbox.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/mediawiki.json` & `grimoire_elk-1.0.0rc2/tests/data/mediawiki.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/meetup.json` & `grimoire_elk-1.0.0rc2/tests/data/meetup.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/mozillaclub.json` & `grimoire_elk-1.0.0rc2/tests/data/mozillaclub.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/nntp.json` & `grimoire_elk-1.0.0rc2/tests/data/nntp.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/pagure.json` & `grimoire_elk-1.0.0rc2/tests/data/pagure.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/phabricator.json` & `grimoire_elk-1.0.0rc2/tests/data/phabricator.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/pipermail.json` & `grimoire_elk-1.0.0rc2/tests/data/pipermail.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/projects-release.json` & `grimoire_elk-1.0.0rc2/tests/data/projects-release.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/puppetforge.json` & `grimoire_elk-1.0.0rc2/tests/data/puppetforge.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/redmine.json` & `grimoire_elk-1.0.0rc2/tests/data/redmine.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/remo.json` & `grimoire_elk-1.0.0rc2/tests/data/remo.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/rocketchat.json` & `grimoire_elk-1.0.0rc2/tests/data/rocketchat.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/rss.json` & `grimoire_elk-1.0.0rc2/tests/data/rss.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/slack.json` & `grimoire_elk-1.0.0rc2/tests/data/slack.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/stackexchange.json` & `grimoire_elk-1.0.0rc2/tests/data/stackexchange.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/supybot.json` & `grimoire_elk-1.0.0rc2/tests/data/supybot.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/task-identities-data.json` & `grimoire_elk-1.0.0rc2/tests/data/task-identities-data.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/telegram.json` & `grimoire_elk-1.0.0rc2/tests/data/telegram.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/twitter.json` & `grimoire_elk-1.0.0rc2/tests/data/twitter.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/data/weblate.json` & `grimoire_elk-1.0.0rc2/tests/data/weblate.json`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/model.py` & `grimoire_elk-1.0.0rc2/tests/model.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/run_tests.py` & `grimoire_elk-1.0.0rc2/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_askbot.py` & `grimoire_elk-1.0.0rc2/tests/test_askbot.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_bugzilla.py` & `grimoire_elk-1.0.0rc2/tests/test_bugzilla.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_bugzillarest.py` & `grimoire_elk-1.0.0rc2/tests/test_bugzillarest.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_cocom.py` & `grimoire_elk-1.0.0rc2/tests/test_cocom.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_colic.py` & `grimoire_elk-1.0.0rc2/tests/test_colic.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_confluence.py` & `grimoire_elk-1.0.0rc2/tests/test_confluence.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_crates.py` & `grimoire_elk-1.0.0rc2/tests/test_crates.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_discourse.py` & `grimoire_elk-1.0.0rc2/tests/test_discourse.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_dockerdeps.py` & `grimoire_elk-1.0.0rc2/tests/test_dockerdeps.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_dockerhub.py` & `grimoire_elk-1.0.0rc2/tests/test_dockerhub.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_dockersmells.py` & `grimoire_elk-1.0.0rc2/tests/test_dockersmells.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_elastic.py` & `grimoire_elk-1.0.0rc2/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_elastic_items.py` & `grimoire_elk-1.0.0rc2/tests/test_elastic_items.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_elastic_ocean.py` & `grimoire_elk-1.0.0rc2/tests/test_elastic_ocean.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_elk.py` & `grimoire_elk-1.0.0rc2/tests/test_elk.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_enrich.py` & `grimoire_elk-1.0.0rc2/tests/test_enrich.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_enrich_jira.py` & `grimoire_elk-1.0.0rc2/tests/test_enrich_jira.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_errors.py` & `grimoire_elk-1.0.0rc2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_functest.py` & `grimoire_elk-1.0.0rc2/tests/test_functest.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_gerrit.py` & `grimoire_elk-1.0.0rc2/tests/test_gerrit.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_git.py` & `grimoire_elk-1.0.0rc2/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_github.py` & `grimoire_elk-1.0.0rc2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_github2.py` & `grimoire_elk-1.0.0rc2/tests/test_github2.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_githubql.py` & `grimoire_elk-1.0.0rc2/tests/test_githubql.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_gitlab.py` & `grimoire_elk-1.0.0rc2/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_gitter.py` & `grimoire_elk-1.0.0rc2/tests/test_gitter.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_google_hits.py` & `grimoire_elk-1.0.0rc2/tests/test_google_hits.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_groupsio.py` & `grimoire_elk-1.0.0rc2/tests/test_groupsio.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_hyperkitty.py` & `grimoire_elk-1.0.0rc2/tests/test_hyperkitty.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_jenkins.py` & `grimoire_elk-1.0.0rc2/tests/test_jenkins.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_jira.py` & `grimoire_elk-1.0.0rc2/tests/test_jira.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_kitsune.py` & `grimoire_elk-1.0.0rc2/tests/test_kitsune.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_launchpad.py` & `grimoire_elk-1.0.0rc2/tests/test_launchpad.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_load_identities.py` & `grimoire_elk-1.0.0rc2/tests/test_load_identities.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_mattermost.py` & `grimoire_elk-1.0.0rc2/tests/test_mattermost.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_mbox.py` & `grimoire_elk-1.0.0rc2/tests/test_mbox.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_mediawiki.py` & `grimoire_elk-1.0.0rc2/tests/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_meetup.py` & `grimoire_elk-1.0.0rc2/tests/test_meetup.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_mozillaclub.py` & `grimoire_elk-1.0.0rc2/tests/test_mozillaclub.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_nntp.py` & `grimoire_elk-1.0.0rc2/tests/test_nntp.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_pagure.py` & `grimoire_elk-1.0.0rc2/tests/test_pagure.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_phabricator.py` & `grimoire_elk-1.0.0rc2/tests/test_phabricator.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_pipermail.py` & `grimoire_elk-1.0.0rc2/tests/test_pipermail.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_projects.sql` & `grimoire_elk-1.0.0rc2/tests/test_projects.sql`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_puppetforge.py` & `grimoire_elk-1.0.0rc2/tests/test_puppetforge.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_redmine.py` & `grimoire_elk-1.0.0rc2/tests/test_redmine.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_remo.py` & `grimoire_elk-1.0.0rc2/tests/test_remo.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_rocketchat.py` & `grimoire_elk-1.0.0rc2/tests/test_rocketchat.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_rss.py` & `grimoire_elk-1.0.0rc2/tests/test_rss.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_slack.py` & `grimoire_elk-1.0.0rc2/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_sortinghat_gelk.py` & `grimoire_elk-1.0.0rc2/tests/test_sortinghat_gelk.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_stackexchange.py` & `grimoire_elk-1.0.0rc2/tests/test_stackexchange.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_supybot.py` & `grimoire_elk-1.0.0rc2/tests/test_supybot.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_telegram.py` & `grimoire_elk-1.0.0rc2/tests/test_telegram.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_twitter.py` & `grimoire_elk-1.0.0rc2/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/tests/test_weblate.py` & `grimoire_elk-1.0.0rc2/tests/test_weblate.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk-1.0.0rc1/PKG-INFO` & `grimoire_elk-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoire-elk
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: GrimoireELK processes and stores software development data to ElasticSearch
 Home-page: https://github.com/chaoss/grimoirelab-elk
 License: GPL-3.0-or-later
 Keywords: development repositories analytics
 Author: Bitergia
 Author-email: grimoirelab-discussions@lists.linuxfoundation.org
 Requires-Python: >=3.8,<4.0
```


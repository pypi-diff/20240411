# Comparing `tmp/perceval-1.0.0rc1.tar.gz` & `tmp/perceval-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval-1.0.0rc1.tar", max compression
+gzip compressed data, was "perceval-1.0.0rc2.tar", max compression
```

## Comparing `perceval-1.0.0rc1.tar` & `perceval-1.0.0rc2.tar`

### file list

```diff
@@ -1,421 +1,421 @@
--rw-r--r--   0        0        0      372 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0    27830 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/NEWS
--rw-r--r--   0        0        0    14910 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/README.md
--rw-r--r--   0        0        0       91 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/_version.py
--rw-r--r--   0        0        0    16644 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/archive.py
--rw-r--r--   0        0        0    48005 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backend.py
--rw-r--r--   0        0        0      913 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/__init__.py
--rw-r--r--   0        0        0    20584 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/askbot.py
--rw-r--r--   0        0        0    19635 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/bugzilla.py
--rw-r--r--   0        0        0    17429 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/bugzillarest.py
--rw-r--r--   0        0        0    18002 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/confluence.py
--rw-r--r--   0        0        0    14960 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/discourse.py
--rw-r--r--   0        0        0     7067 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/dockerhub.py
--rw-r--r--   0        0        0    18878 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/gerrit.py
--rw-r--r--   0        0        0    52424 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/git.py
--rw-r--r--   0        0        0    43434 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/github.py
--rw-r--r--   0        0        0    17649 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/githubql.py
--rw-r--r--   0        0        0    27653 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/gitlab.py
--rw-r--r--   0        0        0    12438 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/gitter.py
--rw-r--r--   0        0        0     8489 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/googlehits.py
--rw-r--r--   0        0        0    12010 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/groupsio.py
--rw-r--r--   0        0        0    10438 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/hyperkitty.py
--rw-r--r--   0        0        0    11676 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/jenkins.py
--rw-r--r--   0        0        0    15703 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/jira.py
--rw-r--r--   0        0        0    17102 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/launchpad.py
--rw-r--r--   0        0        0    17731 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/mattermost.py
--rw-r--r--   0        0        0    14322 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/mbox.py
--rw-r--r--   0        0        0    21374 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/mediawiki.py
--rw-r--r--   0        0        0    16238 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/meetup.py
--rw-r--r--   0        0        0    11554 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/nntp.py
--rw-r--r--   0        0        0    14905 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/pagure.py
--rw-r--r--   0        0        0    20949 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/phabricator.py
--rw-r--r--   0        0        0    10892 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/pipermail.py
--rw-r--r--   0        0        0    14273 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/redmine.py
--rw-r--r--   0        0        0    13851 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/rocketchat.py
--rw-r--r--   0        0        0     5761 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/rss.py
--rw-r--r--   0        0        0    15998 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/slack.py
--rw-r--r--   0        0        0    12685 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/stackexchange.py
--rw-r--r--   0        0        0    13727 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/supybot.py
--rw-r--r--   0        0        0    12519 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/telegram.py
--rw-r--r--   0        0        0    15640 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/twitter.py
--rw-r--r--   0        0        0    11883 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/client.py
--rw-r--r--   0        0        0     2350 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/errors.py
--rwxr-xr-x   0        0        0     7223 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/perceval.py
--rw-r--r--   0        0        0     8559 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/utils.py
--rw-r--r--   0        0        0     1762 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0     1880 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/base.py
--rw-r--r--   0        0        0     5757 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/api_24396_openstack.json
--rw-r--r--   0        0        0     6055 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_2481_multicomments.json
--rw-r--r--   0        0        0     1007 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_api_questions.json
--rw-r--r--   0        0        0     2758 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_api_questions_2.json
--rw-r--r--   0        0        0    82758 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question.html
--rw-r--r--   0        0        0    15771 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question_empty.html
--rw-r--r--   0        0        0   150456 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question_multipage_1.html
--rw-r--r--   0        0        0    81766 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question_multipage_2.html
--rw-r--r--   0        0        0   133477 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_148_comments_answer_2_openstack.html
--rw-r--r--   0        0        0    94749 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_16_multicomment_answer_1_openstack.html
--rw-r--r--   0        0        0   153064 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_2_openstack.html
--rw-r--r--   0        0        0   157831 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_3_openstack.html
--rw-r--r--   0        0        0    81807 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_4_openstack.html
--rw-r--r--   0        0        0   146501 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_openstack.html
--rw-r--r--   0        0        0   107008 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_26830_comments_question_openstack.html
--rw-r--r--   0        0        0   155552 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/askbot/html_7893_answer_3_updated.html
--rw-r--r--   0        0        0    71587 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/askbot/html_country_and_website.html
--rw-r--r--   0        0        0     4140 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug.xml
--rw-r--r--   0        0        0    10630 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity.html
--rw-r--r--   0        0        0    11983 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_empty.html
--rw-r--r--   0        0        0    11985 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_empty_alt.html
--rw-r--r--   0        0        0    11924 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_not_valid.html
--rw-r--r--   0        0        0      753 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_buglist.csv
--rw-r--r--   0        0        0      304 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_buglist_next.csv
--rw-r--r--   0        0        0    11373 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details.xml
--rw-r--r--   0        0        0     4475 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details_next.xml
--rw-r--r--   0        0        0     4850 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details_not_valid.xml
--rw-r--r--   0        0        0    14409 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_invalid_chars.xml
--rw-r--r--   0        0        0      246 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_no_version.xml
--rw-r--r--   0        0        0     5666 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs.json
--rw-r--r--   0        0        0      769 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_attachments.json
--rw-r--r--   0        0        0       68 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_attachments_empty.json
--rw-r--r--   0        0        0     5818 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_comments.json
--rw-r--r--   0        0        0       83 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_comments_empty.json
--rw-r--r--   0        0        0       19 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_empty.json
--rw-r--r--   0        0        0     3530 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_history.json
--rw-r--r--   0        0        0      123 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_history_empty.json
--rw-r--r--   0        0        0     6003 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_next.json
--rw-r--r--   0        0        0      165 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_error.json
--rw-r--r--   0        0        0      273 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_version.xml
--rw-r--r--   0        0        0     3785 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v1.json
--rw-r--r--   0        0        0     6573 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v2.json
--rw-r--r--   0        0        0     2287 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v3.json
--rw-r--r--   0        0        0    11007 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_2_v1.json
--rw-r--r--   0        0        0     2658 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_3.json
--rw-r--r--   0        0        0     2196 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_att_v1.json
--rw-r--r--   0        0        0     2698 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_space.json
--rw-r--r--   0        0        0     3548 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_contents.json
--rw-r--r--   0        0        0      275 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_contents_empty.json
--rw-r--r--   0        0        0     1175 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_contents_next.json
--rw-r--r--   0        0        0     2265 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_post.json
--rw-r--r--   0        0        0    10341 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_posts.json
--rw-r--r--   0        0        0    91062 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1148.json
--rw-r--r--   0        0        0    42932 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1149.json
--rw-r--r--   0        0        0    42931 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1150.json
--rw-r--r--   0        0        0     4029 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics.json
--rw-r--r--   0        0        0      199 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics_empty.json
--rw-r--r--   0        0        0     3528 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics_last_posted_at_null.json
--rw-r--r--   0        0        0     5902 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics_pinned.json
--rw-r--r--   0        0        0     8371 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/dockerhub/dockerhub_repository_1.json
--rw-r--r--   0        0        0    19166 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_1
--rw-r--r--   0        0        0    11082 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_2
--rw-r--r--   0        0        0    11073 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_3
--rw-r--r--   0        0        0       36 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_version_214
--rw-r--r--   0        0        0       20 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_version_313
--rw-r--r--   0        0        0       33 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_version_unknown
--rw-r--r--   0        0        0      412 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_bad_cr.txt
--rw-r--r--   0        0        0      828 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_bad_encoding.txt
--rw-r--r--   0        0        0     4635 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log.txt
--rw-r--r--   0        0        0        1 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_empty.txt
--rw-r--r--   0        0        0      874 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_incompleted.txt
--rw-r--r--   0        0        0     1098 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_merge.txt
--rw-r--r--   0        0        0     1616 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_trailers.txt
--rw-r--r--   0        0        0     9235 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gitalternates.tar.gz
--rw-r--r--   0        0        0    14520 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gitdetached.tar.gz
--rw-r--r--   0        0        0    16064 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gittest-sub.tar.gz
--rw-r--r--   0        0        0    30758 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gittest-top-sub.tar.gz
--rw-r--r--   0        0        0    14464 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gittest.tar.gz
--rw-r--r--   0        0        0     7232 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/git/gittest_no_refs.tar.gz
--rw-r--r--   0        0        0     6108 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/git/gittestempty.tar.gz
--rw-r--r--   0        0        0      192 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/abuse_rate_limit
--rw-r--r--   0        0        0        3 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_empty_request
--rw-r--r--   0        0        0      998 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_enterprise_request_requested_reviewers
--rw-r--r--   0        0        0      253 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_error
--rw-r--r--   0        0        0     1911 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_page_1
--rw-r--r--   0        0        0     2419 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_page_2
--rw-r--r--   0        0        0     1408 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_page_3
--rw-r--r--   0        0        0     3609 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_pull_request_review
--rw-r--r--   0        0        0     4727 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_1
--rw-r--r--   0        0        0     2678 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_2
--rw-r--r--   0        0        0     2574 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_2_reactions
--rw-r--r--   0        0        0     2992 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_2_with_pr
--rw-r--r--   0        0        0     2389 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comment_1_reactions
--rw-r--r--   0        0        0        3 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comment_2_reactions
--rw-r--r--   0        0        0     1761 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comments_1
--rw-r--r--   0        0        0     1762 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comments_2
--rw-r--r--   0        0        0     1310 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_login
--rw-r--r--   0        0        0     1103 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_orgs
--rw-r--r--   0        0        0     7135 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_repo
--rw-r--r--   0        0        0     4819 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request
--rw-r--r--   0        0        0     2172 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_from_2016_03_01
--rw-r--r--   0        0        0    25995 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1
--rw-r--r--   0        0        0     5751 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_comment_2_reactions
--rw-r--r--   0        0        0     7951 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_comments
--rw-r--r--   0        0        0     4408 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_commits
--rw-r--r--   0        0        0     2499 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_reviews
--rw-r--r--   0        0        0    23553 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2
--rw-r--r--   0        0        0    11230 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_comments
--rw-r--r--   0        0        0     4408 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_commits
--rw-r--r--   0        0        0     1773 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_reviews
--rw-r--r--   0        0        0     1150 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_requested_reviewers
--rw-r--r--   0        0        0     1163 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_requested_reviewers_ghost
--rw-r--r--   0        0        0      883 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/private.pem
--rw-r--r--   0        0        0      484 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/rate_limit
--rw-r--r--   0        0        0      480 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/rate_limit_aaa
--rw-r--r--   0        0        0      484 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/rate_limit_bbb
--rw-r--r--   0        0        0     1534 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/commits_1
--rw-r--r--   0        0        0      581 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/commits_2
--rw-r--r--   0        0        0      617 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/commits_3
--rw-r--r--   0        0        0     1233 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/emoji
--rw-r--r--   0        0        0        2 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/empty_emoji
--rw-r--r--   0        0        0        2 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/empty_response
--rw-r--r--   0        0        0     2379 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_1
--rw-r--r--   0        0        0     1311 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_2
--rw-r--r--   0        0        0     1164 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_3
--rw-r--r--   0        0        0     1411 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_4
--rw-r--r--   0        0        0     3708 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_page_1
--rw-r--r--   0        0        0     3378 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_page_2
--rw-r--r--   0        0        0     1735 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1
--rw-r--r--   0        0        0     3454 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1_version_1
--rw-r--r--   0        0        0     1001 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1_version_2
--rw-r--r--   0        0        0      778 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1_versions
--rw-r--r--   0        0        0     1872 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_2
--rw-r--r--   0        0        0     2786 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_2_version_1
--rw-r--r--   0        0        0      388 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_2_versions
--rw-r--r--   0        0        0     2493 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_3
--rw-r--r--   0        0        0     4320 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_3_version_1
--rw-r--r--   0        0        0      388 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_3_versions
--rw-r--r--   0        0        0      868 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_1
--rw-r--r--   0        0        0      683 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_2
--rw-r--r--   0        0        0      868 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_outdated
--rw-r--r--   0        0        0      868 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_updated
--rw-r--r--   0        0        0     1316 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_1
--rw-r--r--   0        0        0      672 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_2
--rw-r--r--   0        0        0      626 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_3
--rw-r--r--   0        0        0      626 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_4
--rw-r--r--   0        0        0     2283 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/project
--rw-r--r--   0        0        0        2 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/message_empty
--rw-r--r--   0        0        0      721 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/message_page_1
--rw-r--r--   0        0        0      721 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/message_page_2
--rw-r--r--   0        0        0     1316 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/rooms
--rw-r--r--   0        0        0    78598 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/googlehits/hits_bitergia
--rw-r--r--   0        0        0    69900 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/googlehits/hits_bitergia_grimoirelab
--rw-r--r--   0        0        0    38721 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/googlehits/hits_zero
--rw-r--r--   0        0        0      145 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/empty.zip
--rw-r--r--   0        0        0     1518 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/login
--rw-r--r--   0        0        0    33111 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/messages.zip
--rw-r--r--   0        0        0     3757 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/subscriptions_page_1
--rw-r--r--   0        0        0     3751 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/subscriptions_page_2
--rw-r--r--   0        0        0     6511 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/hyperkitty/hyperkitty_2016_april.mbox
--rw-r--r--   0        0        0      875 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/hyperkitty/hyperkitty_2016_march.mbox
--rw-r--r--   0        0        0     6547 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_build.json
--rw-r--r--   0        0        0   190490 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_builds.json
--rw-r--r--   0        0        0        3 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_builds_empty.json
--rw-r--r--   0        0        0    42326 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_no_builds.json
--rw-r--r--   0        0        0      890 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_jobs.json
--rw-r--r--   0        0        0        3 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_jobs_empty.json
--rw-r--r--   0        0        0    97205 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_workflow_job_builds.json
--rw-r--r--   0        0        0     1941 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_workflow_jobs.json
--rw-r--r--   0        0        0       77 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_empty.json
--rw-r--r--   0        0        0     7209 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_page_1.json
--rw-r--r--   0        0        0     7207 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_page_2.json
--rw-r--r--   0        0        0    14567 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_fields.json
--rw-r--r--   0        0        0    13217 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_page_1.json
--rw-r--r--   0        0        0     6584 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_page_2.json
--rw-r--r--   0        0        0       76 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_page_empty.json
--rw-r--r--   0        0        0    12054 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_parse_expected.json
--rw-r--r--   0        0        0      159 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issue_activities
--rw-r--r--   0        0        0      162 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issue_attachments
--rw-r--r--   0        0        0      154 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issue_comments
--rw-r--r--   0        0        0       46 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issues
--rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1
--rw-r--r--   0        0        0      827 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities
--rw-r--r--   0        0        0     1610 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_next_1
--rw-r--r--   0        0        0     1509 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_next_2
--rw-r--r--   0        0        0      117 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_no_entries
--rw-r--r--   0        0        0     2571 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments
--rw-r--r--   0        0        0     1865 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_next_1
--rw-r--r--   0        0        0     1769 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_next_2
--rw-r--r--   0        0        0      117 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_no_entries
--rw-r--r--   0        0        0     1925 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments
--rw-r--r--   0        0        0     2039 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_next_1
--rw-r--r--   0        0        0     1916 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_next_2
--rw-r--r--   0        0        0      117 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_no_entries
--rw-r--r--   0        0        0    28963 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_expected
--rw-r--r--   0        0        0     3981 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_expected_no_entries
--rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_no_entries
--rw-r--r--   0        0        0     2297 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2
--rw-r--r--   0        0        0      831 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_activities
--rw-r--r--   0        0        0     1041 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_comments
--rw-r--r--   0        0        0    17790 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_expected
--rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_3
--rw-r--r--   0        0        0     7538 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_3_expected
--rw-r--r--   0        0        0     2208 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1
--rw-r--r--   0        0        0     1639 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1_no_entries
--rw-r--r--   0        0        0     1707 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1_no_next
--rw-r--r--   0        0        0     2309 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_2
--rw-r--r--   0        0        0     1791 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_3
--rw-r--r--   0        0        0     3379 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_user_1
--rw-r--r--   0        0        0      485 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_channel.json
--rw-r--r--   0        0        0      205 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_erros.json
--rw-r--r--   0        0        0     4014 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts.json
--rw-r--r--   0        0        0       37 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts_empty.json
--rw-r--r--   0        0        0     2812 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts_next.json
--rw-r--r--   0        0        0      507 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_user_sduenas.json
--rw-r--r--   0        0        0      892 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_user_valcos.json
--rw-r--r--   0        0        0     8584 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_complex.mbox
--rw-r--r--   0        0        0      953 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_iso8859_encoding.mbox
--rw-r--r--   0        0        0     9610 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_multipart.mbox
--rw-r--r--   0        0        0     1788 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_no_fields.mbox
--rw-r--r--   0        0        0      330 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_single.mbox
--rw-r--r--   0        0        0     2412 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_unixfrom_encoding.mbox
--rw-r--r--   0        0        0     1688 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_unknown_encoding.mbox
--rw-r--r--   0        0        0     9282 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_namespaces.json
--rw-r--r--   0        0        0   166125 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_476583_revisions.json
--rw-r--r--   0        0        0      339 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_476589_revisions.json
--rw-r--r--   0        0        0      339 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_476590_revisions.json
--rw-r--r--   0        0        0      921 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_592384_revisions.json
--rw-r--r--   0        0        0      555 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_all.json
--rw-r--r--   0        0        0      104 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_all_empty.json
--rw-r--r--   0        0        0     1823 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_allrevisions.json
--rw-r--r--   0        0        0      217 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_allrevisions_empty.json
--rw-r--r--   0        0        0     1831 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_recent_changes.json
--rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_siteinfo_1.23.json
--rw-r--r--   0        0        0     3108 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_siteinfo_1.28.json
--rw-r--r--   0        0        0     1670 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_comments.json
--rw-r--r--   0        0        0    16033 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events.json
--rw-r--r--   0        0        0        3 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events_empty.json
--rw-r--r--   0        0        0    12659 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events_next.json
--rw-r--r--   0        0        0    11156 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events_range.json
--rw-r--r--   0        0        0     5071 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_rsvps.json
--rw-r--r--   0        0        0     5405 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/nntp/nntp_1.txt
--rw-r--r--   0        0        0     9233 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/nntp/nntp_2.txt
--rw-r--r--   0        0        0     4113 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/nntp/nntp_parsing_error.txt
--rw-r--r--   0        0        0        3 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_empty_request
--rw-r--r--   0        0        0     3348 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_namespace_issue_2
--rw-r--r--   0        0        0     1647 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_1
--rw-r--r--   0        0        0     3216 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_2
--rw-r--r--   0        0        0     2126 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_from_2020_03_07
--rw-r--r--   0        0        0     2173 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_only_issue_2
--rw-r--r--   0        0        0      300 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_error.json
--rw-r--r--   0        0        0      420 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_phid_herald.json
--rw-r--r--   0        0        0      759 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_phids.json
--rw-r--r--   0        0        0      417 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_project_bugreport.json
--rw-r--r--   0        0        0      419 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_project_devel.json
--rw-r--r--   0        0        0     4029 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks.json
--rw-r--r--   0        0        0      320 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks_empty.json
--rw-r--r--   0        0        0     1730 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks_next.json
--rw-r--r--   0        0        0    25354 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_transactions.json
--rw-r--r--   0        0        0     9874 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_transactions_next.json
--rw-r--r--   0        0        0      466 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jane.json
--rw-r--r--   0        0        0      453 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_janesmith.json
--rw-r--r--   0        0        0      466 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jdoe.json
--rw-r--r--   0        0        0      441 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jrae.json
--rw-r--r--   0        0        0       69 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jsmith.json
--rw-r--r--   0        0        0     1601 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_users.json
--rw-r--r--   0        0        0     6495 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_2015_november.mbox
--rw-r--r--   0        0        0     6511 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_2016_april.mbox
--rw-r--r--   0        0        0      875 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_2016_march.mbox
--rw-r--r--   0        0        0     2170 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_apache_index.html
--rw-r--r--   0        0        0     1867 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_index.html
--rw-r--r--   0        0        0      593 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_index_empty.html
--rw-r--r--   0        0        0     1414 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_2.json
--rw-r--r--   0        0        0     1426 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_5.json
--rw-r--r--   0        0        0    13221 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_7311.json
--rw-r--r--   0        0        0     1425 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_9.json
--rw-r--r--   0        0        0     2830 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issues.json
--rw-r--r--   0        0        0       76 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issues_empty.json
--rw-r--r--   0        0        0     1061 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issues_next.json
--rw-r--r--   0        0        0      292 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_24.json
--rw-r--r--   0        0        0      292 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_25.json
--rw-r--r--   0        0        0      291 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_3.json
--rw-r--r--   0        0        0      291 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_4.json
--rw-r--r--   0        0        0      896 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/channel_info.json
--rw-r--r--   0        0        0       82 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_empty_2020_05_10.json
--rw-r--r--   0        0        0     1408 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_page_1.json
--rw-r--r--   0        0        0     1017 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_page_2.json
--rw-r--r--   0        0        0      448 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_page_2020_05_03.json
--rw-r--r--   0        0        0    18134 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rss/rss_entries.xml
--rw-r--r--   0        0        0       54 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_error.json
--rw-r--r--   0        0        0     1752 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history.json
--rw-r--r--   0        0        0     1013 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history_20150323.json
--rw-r--r--   0        0        0       97 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history_empty.json
--rw-r--r--   0        0        0      393 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history_next.json
--rw-r--r--   0        0        0     1064 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_info.json
--rw-r--r--   0        0        0     1063 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_info_archived.json
--rw-r--r--   0        0        0     2225 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_members1.json
--rw-r--r--   0        0        0     1445 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_members2.json
--rw-r--r--   0        0        0     1252 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0001.json
--rw-r--r--   0        0        0     1170 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0002.json
--rw-r--r--   0        0        0     1060 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0003.json
--rw-r--r--   0        0        0       51 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0004_private.json
--rw-r--r--   0        0        0     2676 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question
--rw-r--r--   0        0        0     5189 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_backoff_page
--rw-r--r--   0        0        0     5171 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_page
--rw-r--r--   0        0        0     5172 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_page_2
--rw-r--r--   0        0        0     4638 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_parse
--rw-r--r--   0        0        0      883 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/supybot/supybot_2012_10_17.log
--rw-r--r--   0        0        0      660 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_2012_10_18.log
--rw-r--r--   0        0        0      181 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_date_without_tz.log
--rw-r--r--   0        0        0      820 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_invalid_date.log
--rw-r--r--   0        0        0      818 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_invalid_msg.log
--rw-r--r--   0        0        0     7571 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_valid.log
--rw-r--r--   0        0        0     1612 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/telegram/telegram_messages.json
--rw-r--r--   0        0        0       27 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/telegram/telegram_messages_empty.json
--rw-r--r--   0        0        0     1587 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/telegram/telegram_messages_next.json
--rw-r--r--   0        0        0   731129 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets.json
--rw-r--r--   0        0        0    21985 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets_page_1.json
--rw-r--r--   0        0        0    24147 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets_page_2.json
--rw-r--r--   0        0        0      381 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets_page_3.json
--rw-r--r--   0        0        0     4140 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/bugzilla_bug.xml
--rw-r--r--   0        0        0    14409 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/bugzilla_bugs_invalid_chars.xml
--rw-r--r--   0        0        0     5429 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/email_multipart_encoding.txt
--rw-r--r--   0        0        0     4180 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/email_multipart_no_encoding.txt
--rw-r--r--   0        0        0      329 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/email_single.txt
--rw-r--r--   0        0        0      330 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/mbox_single.mbox
--rw-r--r--   0        0        0      420 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/xml_invalid.xml
--rw-r--r--   0        0        0        0 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/__init__.py
--rw-r--r--   0        0        0     1270 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/backend.py
--rw-r--r--   0        0        0        0 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/nested_package/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/nested_package/nested_backend_b.py
--rw-r--r--   0        0        0     1241 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/mocked_package/nested_package/nested_backend_c.py
--rwxr-xr-x   0        0        0     1180 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/run_tests.py
--rw-r--r--   0        0        0    18694 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_archive.py
--rw-r--r--   0        0        0    29194 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_askbot.py
--rw-r--r--   0        0        0    89739 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_backend.py
--rw-r--r--   0        0        0    45401 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_bugzilla.py
--rw-r--r--   0        0        0    34723 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_bugzillarest.py
--rw-r--r--   0        0        0    19093 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_client.py
--rw-r--r--   0        0        0    28276 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_confluence.py
--rw-r--r--   0        0        0    46790 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_discourse.py
--rw-r--r--   0        0        0     9175 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_dockerhub.py
--rw-r--r--   0        0        0     4320 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_errors.py
--rw-r--r--   0        0        0    21716 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_gerrit.py
--rw-r--r--   0        0        0    82928 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_git.py
--rw-r--r--   0        0        0   216577 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_github.py
--rw-r--r--   0        0        0    38701 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_githubql.py
--rw-r--r--   0        0        0    83197 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_gitlab.py
--rw-r--r--   0        0        0    19906 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_gitter.py
--rw-r--r--   0        0        0    13003 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_googlehits.py
--rw-r--r--   0        0        0    21109 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_groupsio.py
--rw-r--r--   0        0        0    18362 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_hyperkitty.py
--rw-r--r--   0        0        0    38356 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_jenkins.py
--rw-r--r--   0        0        0    40029 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_jira.py
--rw-r--r--   0        0        0    54602 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_launchpad.py
--rw-r--r--   0        0        0    31185 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_mattermost.py
--rw-r--r--   0        0        0    27864 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_mbox.py
--rw-r--r--   0        0        0    28609 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_mediawiki.py
--rw-r--r--   0        0        0    37724 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_meetup.py
--rw-r--r--   0        0        0    30330 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_pagure.py
--rw-r--r--   0        0        0    45588 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_phabricator.py
--rw-r--r--   0        0        0    27472 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_pipermail.py
--rw-r--r--   0        0        0    23487 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_redmine.py
--rw-r--r--   0        0        0    25298 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_rocketchat.py
--rw-r--r--   0        0        0    10139 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_rss.py
--rw-r--r--   0        0        0    35971 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_slack.py
--rw-r--r--   0        0        0    22342 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_stackexchange.py
--rw-r--r--   0        0        0    22836 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_supybot.py
--rw-r--r--   0        0        0    18086 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_telegram.py
--rw-r--r--   0        0        0    17146 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_twitter.py
--rw-r--r--   0        0        0    11254 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_utils.py
--rw-r--r--   0        0        0    16471 1970-01-01 00:00:00.000000 perceval-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      372 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    27830 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/NEWS
+-rw-r--r--   0        0        0    14910 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/README.md
+-rw-r--r--   0        0        0       91 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/_version.py
+-rw-r--r--   0        0        0    16644 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/archive.py
+-rw-r--r--   0        0        0    48005 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backend.py
+-rw-r--r--   0        0        0      913 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/__init__.py
+-rw-r--r--   0        0        0    20584 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/askbot.py
+-rw-r--r--   0        0        0    19635 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/bugzilla.py
+-rw-r--r--   0        0        0    17429 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/bugzillarest.py
+-rw-r--r--   0        0        0    18002 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/confluence.py
+-rw-r--r--   0        0        0    14960 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/discourse.py
+-rw-r--r--   0        0        0     7067 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/dockerhub.py
+-rw-r--r--   0        0        0    18878 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/gerrit.py
+-rw-r--r--   0        0        0    52424 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/git.py
+-rw-r--r--   0        0        0    43434 2024-04-11 10:42:47.177317 perceval-1.0.0rc2/perceval/backends/core/github.py
+-rw-r--r--   0        0        0    17649 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/githubql.py
+-rw-r--r--   0        0        0    27653 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/gitlab.py
+-rw-r--r--   0        0        0    12438 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/gitter.py
+-rw-r--r--   0        0        0     8489 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/googlehits.py
+-rw-r--r--   0        0        0    12010 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/groupsio.py
+-rw-r--r--   0        0        0    10438 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/hyperkitty.py
+-rw-r--r--   0        0        0    11676 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/jenkins.py
+-rw-r--r--   0        0        0    15703 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/jira.py
+-rw-r--r--   0        0        0    17102 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/launchpad.py
+-rw-r--r--   0        0        0    17731 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/mattermost.py
+-rw-r--r--   0        0        0    14322 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/mbox.py
+-rw-r--r--   0        0        0    21374 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/mediawiki.py
+-rw-r--r--   0        0        0    16238 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/meetup.py
+-rw-r--r--   0        0        0    11554 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/nntp.py
+-rw-r--r--   0        0        0    14905 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/pagure.py
+-rw-r--r--   0        0        0    20949 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/phabricator.py
+-rw-r--r--   0        0        0    10892 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/pipermail.py
+-rw-r--r--   0        0        0    14273 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/redmine.py
+-rw-r--r--   0        0        0    13851 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/rocketchat.py
+-rw-r--r--   0        0        0     5761 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/rss.py
+-rw-r--r--   0        0        0    15998 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/slack.py
+-rw-r--r--   0        0        0    12685 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/stackexchange.py
+-rw-r--r--   0        0        0    13727 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/supybot.py
+-rw-r--r--   0        0        0    12519 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/telegram.py
+-rw-r--r--   0        0        0    15640 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/backends/core/twitter.py
+-rw-r--r--   0        0        0    11883 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/client.py
+-rw-r--r--   0        0        0     2350 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/errors.py
+-rwxr-xr-x   0        0        0     7223 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/perceval.py
+-rw-r--r--   0        0        0     8559 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/perceval/utils.py
+-rw-r--r--   0        0        0     1762 2024-04-11 10:42:47.181317 perceval-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0     1880 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/base.py
+-rw-r--r--   0        0        0     5757 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/api_24396_openstack.json
+-rw-r--r--   0        0        0     6055 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/askbot_2481_multicomments.json
+-rw-r--r--   0        0        0     1007 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/askbot_api_questions.json
+-rw-r--r--   0        0        0     2758 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/askbot_api_questions_2.json
+-rw-r--r--   0        0        0    82758 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/askbot_question.html
+-rw-r--r--   0        0        0    15771 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/askbot_question_empty.html
+-rw-r--r--   0        0        0   150456 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/askbot_question_multipage_1.html
+-rw-r--r--   0        0        0    81766 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/askbot_question_multipage_2.html
+-rw-r--r--   0        0        0   133477 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/html_148_comments_answer_2_openstack.html
+-rw-r--r--   0        0        0    94749 2024-04-11 10:42:47.185317 perceval-1.0.0rc2/tests/data/askbot/html_16_multicomment_answer_1_openstack.html
+-rw-r--r--   0        0        0   153064 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_2_openstack.html
+-rw-r--r--   0        0        0   157831 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_3_openstack.html
+-rw-r--r--   0        0        0    81807 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_4_openstack.html
+-rw-r--r--   0        0        0   146501 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_openstack.html
+-rw-r--r--   0        0        0   107008 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/askbot/html_26830_comments_question_openstack.html
+-rw-r--r--   0        0        0   155552 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/askbot/html_7893_answer_3_updated.html
+-rw-r--r--   0        0        0    71587 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/askbot/html_country_and_website.html
+-rw-r--r--   0        0        0     4140 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug.xml
+-rw-r--r--   0        0        0    10630 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity.html
+-rw-r--r--   0        0        0    11983 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity_empty.html
+-rw-r--r--   0        0        0    11985 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity_empty_alt.html
+-rw-r--r--   0        0        0    11924 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity_not_valid.html
+-rw-r--r--   0        0        0      753 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_buglist.csv
+-rw-r--r--   0        0        0      304 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_buglist_next.csv
+-rw-r--r--   0        0        0    11373 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_details.xml
+-rw-r--r--   0        0        0     4475 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_details_next.xml
+-rw-r--r--   0        0        0     4850 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_details_not_valid.xml
+-rw-r--r--   0        0        0    14409 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_invalid_chars.xml
+-rw-r--r--   0        0        0      246 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_no_version.xml
+-rw-r--r--   0        0        0     5666 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs.json
+-rw-r--r--   0        0        0      769 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_attachments.json
+-rw-r--r--   0        0        0       68 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_attachments_empty.json
+-rw-r--r--   0        0        0     5818 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_comments.json
+-rw-r--r--   0        0        0       83 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_comments_empty.json
+-rw-r--r--   0        0        0       19 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_empty.json
+-rw-r--r--   0        0        0     3530 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_history.json
+-rw-r--r--   0        0        0      123 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_history_empty.json
+-rw-r--r--   0        0        0     6003 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_next.json
+-rw-r--r--   0        0        0      165 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_error.json
+-rw-r--r--   0        0        0      273 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_version.xml
+-rw-r--r--   0        0        0     3785 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_content_1_v1.json
+-rw-r--r--   0        0        0     6573 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_content_1_v2.json
+-rw-r--r--   0        0        0     2287 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_content_1_v3.json
+-rw-r--r--   0        0        0    11007 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_content_2_v1.json
+-rw-r--r--   0        0        0     2658 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_content_3.json
+-rw-r--r--   0        0        0     2196 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_content_att_v1.json
+-rw-r--r--   0        0        0     2698 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_content_space.json
+-rw-r--r--   0        0        0     3548 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_contents.json
+-rw-r--r--   0        0        0      275 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_contents_empty.json
+-rw-r--r--   0        0        0     1175 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/confluence/confluence_contents_next.json
+-rw-r--r--   0        0        0     2265 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/discourse/discourse_post.json
+-rw-r--r--   0        0        0    10341 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/discourse/discourse_posts.json
+-rw-r--r--   0        0        0    91062 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/discourse/discourse_topic_1148.json
+-rw-r--r--   0        0        0    42932 2024-04-11 10:42:47.189317 perceval-1.0.0rc2/tests/data/discourse/discourse_topic_1149.json
+-rw-r--r--   0        0        0    42931 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/discourse/discourse_topic_1150.json
+-rw-r--r--   0        0        0     4029 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/discourse/discourse_topics.json
+-rw-r--r--   0        0        0      199 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/discourse/discourse_topics_empty.json
+-rw-r--r--   0        0        0     3528 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/discourse/discourse_topics_last_posted_at_null.json
+-rw-r--r--   0        0        0     5902 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/discourse/discourse_topics_pinned.json
+-rw-r--r--   0        0        0     8371 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/dockerhub/dockerhub_repository_1.json
+-rw-r--r--   0        0        0    19166 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gerrit/gerrit_reviews_page_1
+-rw-r--r--   0        0        0    11082 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gerrit/gerrit_reviews_page_2
+-rw-r--r--   0        0        0    11073 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gerrit/gerrit_reviews_page_3
+-rw-r--r--   0        0        0       36 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gerrit/gerrit_version_214
+-rw-r--r--   0        0        0       20 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gerrit/gerrit_version_313
+-rw-r--r--   0        0        0       33 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gerrit/gerrit_version_unknown
+-rw-r--r--   0        0        0      412 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/git_bad_cr.txt
+-rw-r--r--   0        0        0      828 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/git_bad_encoding.txt
+-rw-r--r--   0        0        0     4635 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/git_log.txt
+-rw-r--r--   0        0        0        1 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/git_log_empty.txt
+-rw-r--r--   0        0        0      874 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/git_log_incompleted.txt
+-rw-r--r--   0        0        0     1098 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/git_log_merge.txt
+-rw-r--r--   0        0        0     1616 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/git_log_trailers.txt
+-rw-r--r--   0        0        0     9235 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/gitalternates.tar.gz
+-rw-r--r--   0        0        0    14520 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/gitdetached.tar.gz
+-rw-r--r--   0        0        0    16064 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/gittest-sub.tar.gz
+-rw-r--r--   0        0        0    30758 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/gittest-top-sub.tar.gz
+-rw-r--r--   0        0        0    14464 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/gittest.tar.gz
+-rw-r--r--   0        0        0     7232 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/gittest_no_refs.tar.gz
+-rw-r--r--   0        0        0     6108 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/git/gittestempty.tar.gz
+-rw-r--r--   0        0        0      192 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/abuse_rate_limit
+-rw-r--r--   0        0        0        3 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_empty_request
+-rw-r--r--   0        0        0      998 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_enterprise_request_requested_reviewers
+-rw-r--r--   0        0        0      253 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_events_error
+-rw-r--r--   0        0        0     1911 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_events_page_1
+-rw-r--r--   0        0        0     2419 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_events_page_2
+-rw-r--r--   0        0        0     1408 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_events_page_3
+-rw-r--r--   0        0        0     3609 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_events_pull_request_review
+-rw-r--r--   0        0        0     4727 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_1
+-rw-r--r--   0        0        0     2678 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_2
+-rw-r--r--   0        0        0     2574 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_2_reactions
+-rw-r--r--   0        0        0     2992 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_2_with_pr
+-rw-r--r--   0        0        0     2389 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_comment_1_reactions
+-rw-r--r--   0        0        0        3 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_comment_2_reactions
+-rw-r--r--   0        0        0     1761 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_comments_1
+-rw-r--r--   0        0        0     1762 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_issue_comments_2
+-rw-r--r--   0        0        0     1310 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_login
+-rw-r--r--   0        0        0     1103 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_orgs
+-rw-r--r--   0        0        0     7135 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_repo
+-rw-r--r--   0        0        0     4819 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request
+-rw-r--r--   0        0        0     2172 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_from_2016_03_01
+-rw-r--r--   0        0        0    25995 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1
+-rw-r--r--   0        0        0     5751 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_comment_2_reactions
+-rw-r--r--   0        0        0     7951 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_comments
+-rw-r--r--   0        0        0     4408 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_commits
+-rw-r--r--   0        0        0     2499 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_reviews
+-rw-r--r--   0        0        0    23553 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2
+-rw-r--r--   0        0        0    11230 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2_comments
+-rw-r--r--   0        0        0     4408 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2_commits
+-rw-r--r--   0        0        0     1773 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2_reviews
+-rw-r--r--   0        0        0     1150 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_requested_reviewers
+-rw-r--r--   0        0        0     1163 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/github_request_requested_reviewers_ghost
+-rw-r--r--   0        0        0      883 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/private.pem
+-rw-r--r--   0        0        0      484 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/rate_limit
+-rw-r--r--   0        0        0      480 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/rate_limit_aaa
+-rw-r--r--   0        0        0      484 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/github/rate_limit_bbb
+-rw-r--r--   0        0        0     1534 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/commits_1
+-rw-r--r--   0        0        0      581 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/commits_2
+-rw-r--r--   0        0        0      617 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/commits_3
+-rw-r--r--   0        0        0     1233 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/emoji
+-rw-r--r--   0        0        0        2 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/empty_emoji
+-rw-r--r--   0        0        0        2 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/empty_response
+-rw-r--r--   0        0        0     2379 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/issue_1
+-rw-r--r--   0        0        0     1311 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/issue_2
+-rw-r--r--   0        0        0     1164 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/issue_3
+-rw-r--r--   0        0        0     1411 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/issue_4
+-rw-r--r--   0        0        0     3708 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/issue_page_1
+-rw-r--r--   0        0        0     3378 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/issue_page_2
+-rw-r--r--   0        0        0     1735 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_1
+-rw-r--r--   0        0        0     3454 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_1_version_1
+-rw-r--r--   0        0        0     1001 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_1_version_2
+-rw-r--r--   0        0        0      778 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_1_versions
+-rw-r--r--   0        0        0     1872 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_2
+-rw-r--r--   0        0        0     2786 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_2_version_1
+-rw-r--r--   0        0        0      388 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_2_versions
+-rw-r--r--   0        0        0     2493 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_3
+-rw-r--r--   0        0        0     4320 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_3_version_1
+-rw-r--r--   0        0        0      388 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_3_versions
+-rw-r--r--   0        0        0      868 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_page_1
+-rw-r--r--   0        0        0      683 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_page_2
+-rw-r--r--   0        0        0      868 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_page_outdated
+-rw-r--r--   0        0        0      868 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/merge_page_updated
+-rw-r--r--   0        0        0     1316 2024-04-11 10:42:47.193317 perceval-1.0.0rc2/tests/data/gitlab/notes_1
+-rw-r--r--   0        0        0      672 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitlab/notes_2
+-rw-r--r--   0        0        0      626 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitlab/notes_3
+-rw-r--r--   0        0        0      626 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitlab/notes_4
+-rw-r--r--   0        0        0     2283 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitlab/project
+-rw-r--r--   0        0        0        2 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitter/message_empty
+-rw-r--r--   0        0        0      721 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitter/message_page_1
+-rw-r--r--   0        0        0      721 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitter/message_page_2
+-rw-r--r--   0        0        0     1316 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/gitter/rooms
+-rw-r--r--   0        0        0    78598 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/googlehits/hits_bitergia
+-rw-r--r--   0        0        0    69900 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/googlehits/hits_bitergia_grimoirelab
+-rw-r--r--   0        0        0    38721 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/googlehits/hits_zero
+-rw-r--r--   0        0        0      145 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/groupsio/empty.zip
+-rw-r--r--   0        0        0     1518 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/groupsio/login
+-rw-r--r--   0        0        0    33111 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/groupsio/messages.zip
+-rw-r--r--   0        0        0     3757 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/groupsio/subscriptions_page_1
+-rw-r--r--   0        0        0     3751 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/groupsio/subscriptions_page_2
+-rw-r--r--   0        0        0     6511 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/hyperkitty/hyperkitty_2016_april.mbox
+-rw-r--r--   0        0        0      875 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/hyperkitty/hyperkitty_2016_march.mbox
+-rw-r--r--   0        0        0     6547 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_build.json
+-rw-r--r--   0        0        0   190490 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_job_builds.json
+-rw-r--r--   0        0        0        3 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_job_builds_empty.json
+-rw-r--r--   0        0        0    42326 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_job_no_builds.json
+-rw-r--r--   0        0        0      890 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_jobs.json
+-rw-r--r--   0        0        0        3 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_jobs_empty.json
+-rw-r--r--   0        0        0    97205 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_workflow_job_builds.json
+-rw-r--r--   0        0        0     1941 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jenkins/jenkins_workflow_jobs.json
+-rw-r--r--   0        0        0       77 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_comments_issue_empty.json
+-rw-r--r--   0        0        0     7209 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_comments_issue_page_1.json
+-rw-r--r--   0        0        0     7207 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_comments_issue_page_2.json
+-rw-r--r--   0        0        0    14567 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_fields.json
+-rw-r--r--   0        0        0    13217 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_issues_page_1.json
+-rw-r--r--   0        0        0     6584 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_issues_page_2.json
+-rw-r--r--   0        0        0       76 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_issues_page_empty.json
+-rw-r--r--   0        0        0    12054 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/jira/jira_issues_parse_expected.json
+-rw-r--r--   0        0        0      159 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_empty_issue_activities
+-rw-r--r--   0        0        0      162 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_empty_issue_attachments
+-rw-r--r--   0        0        0      154 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_empty_issue_comments
+-rw-r--r--   0        0        0       46 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_empty_issues
+-rw-r--r--   0        0        0     2139 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1
+-rw-r--r--   0        0        0      827 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_activities
+-rw-r--r--   0        0        0     1610 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_activities_next_1
+-rw-r--r--   0        0        0     1509 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_activities_next_2
+-rw-r--r--   0        0        0      117 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_activities_no_entries
+-rw-r--r--   0        0        0     2571 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_attachments
+-rw-r--r--   0        0        0     1865 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_attachments_next_1
+-rw-r--r--   0        0        0     1769 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_attachments_next_2
+-rw-r--r--   0        0        0      117 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_attachments_no_entries
+-rw-r--r--   0        0        0     1925 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_comments
+-rw-r--r--   0        0        0     2039 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_comments_next_1
+-rw-r--r--   0        0        0     1916 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_comments_next_2
+-rw-r--r--   0        0        0      117 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_comments_no_entries
+-rw-r--r--   0        0        0    28963 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_expected
+-rw-r--r--   0        0        0     3981 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_expected_no_entries
+-rw-r--r--   0        0        0     2139 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_no_entries
+-rw-r--r--   0        0        0     2297 2024-04-11 10:42:47.197317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2
+-rw-r--r--   0        0        0      831 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2_activities
+-rw-r--r--   0        0        0     1041 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2_comments
+-rw-r--r--   0        0        0    17790 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2_expected
+-rw-r--r--   0        0        0     2139 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_3
+-rw-r--r--   0        0        0     7538 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_3_expected
+-rw-r--r--   0        0        0     2208 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_1
+-rw-r--r--   0        0        0     1639 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_1_no_entries
+-rw-r--r--   0        0        0     1707 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_1_no_next
+-rw-r--r--   0        0        0     2309 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_2
+-rw-r--r--   0        0        0     1791 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_3
+-rw-r--r--   0        0        0     3379 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/launchpad/launchpad_user_1
+-rw-r--r--   0        0        0      485 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mattermost/mattermost_channel.json
+-rw-r--r--   0        0        0      205 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mattermost/mattermost_erros.json
+-rw-r--r--   0        0        0     4014 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mattermost/mattermost_posts.json
+-rw-r--r--   0        0        0       37 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mattermost/mattermost_posts_empty.json
+-rw-r--r--   0        0        0     2812 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mattermost/mattermost_posts_next.json
+-rw-r--r--   0        0        0      507 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mattermost/mattermost_user_sduenas.json
+-rw-r--r--   0        0        0      892 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mattermost/mattermost_user_valcos.json
+-rw-r--r--   0        0        0     8584 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mbox/mbox_complex.mbox
+-rw-r--r--   0        0        0      953 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mbox/mbox_iso8859_encoding.mbox
+-rw-r--r--   0        0        0     9610 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mbox/mbox_multipart.mbox
+-rw-r--r--   0        0        0     1788 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mbox/mbox_no_fields.mbox
+-rw-r--r--   0        0        0      330 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mbox/mbox_single.mbox
+-rw-r--r--   0        0        0     2412 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mbox/mbox_unixfrom_encoding.mbox
+-rw-r--r--   0        0        0     1688 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mbox/mbox_unknown_encoding.mbox
+-rw-r--r--   0        0        0     9282 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_namespaces.json
+-rw-r--r--   0        0        0   166125 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_page_476583_revisions.json
+-rw-r--r--   0        0        0      339 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_page_476589_revisions.json
+-rw-r--r--   0        0        0      339 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_page_476590_revisions.json
+-rw-r--r--   0        0        0      921 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_page_592384_revisions.json
+-rw-r--r--   0        0        0      555 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_all.json
+-rw-r--r--   0        0        0      104 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_all_empty.json
+-rw-r--r--   0        0        0     1823 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_allrevisions.json
+-rw-r--r--   0        0        0      217 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_allrevisions_empty.json
+-rw-r--r--   0        0        0     1831 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_recent_changes.json
+-rw-r--r--   0        0        0     2139 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_siteinfo_1.23.json
+-rw-r--r--   0        0        0     3108 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_siteinfo_1.28.json
+-rw-r--r--   0        0        0     1670 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/meetup/meetup_comments.json
+-rw-r--r--   0        0        0    16033 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/meetup/meetup_events.json
+-rw-r--r--   0        0        0        3 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/meetup/meetup_events_empty.json
+-rw-r--r--   0        0        0    12659 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/meetup/meetup_events_next.json
+-rw-r--r--   0        0        0    11156 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/meetup/meetup_events_range.json
+-rw-r--r--   0        0        0     5071 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/meetup/meetup_rsvps.json
+-rw-r--r--   0        0        0     5405 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/nntp/nntp_1.txt
+-rw-r--r--   0        0        0     9233 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/nntp/nntp_2.txt
+-rw-r--r--   0        0        0     4113 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/nntp/nntp_parsing_error.txt
+-rw-r--r--   0        0        0        3 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pagure/pagure_empty_request
+-rw-r--r--   0        0        0     3348 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pagure/pagure_namespace_issue_2
+-rw-r--r--   0        0        0     1647 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pagure/pagure_repo_issue_1
+-rw-r--r--   0        0        0     3216 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pagure/pagure_repo_issue_2
+-rw-r--r--   0        0        0     2126 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pagure/pagure_repo_issue_from_2020_03_07
+-rw-r--r--   0        0        0     2173 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pagure/pagure_repo_only_issue_2
+-rw-r--r--   0        0        0      300 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_error.json
+-rw-r--r--   0        0        0      420 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_phid_herald.json
+-rw-r--r--   0        0        0      759 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_phids.json
+-rw-r--r--   0        0        0      417 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_project_bugreport.json
+-rw-r--r--   0        0        0      419 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_project_devel.json
+-rw-r--r--   0        0        0     4029 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_tasks.json
+-rw-r--r--   0        0        0      320 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_tasks_empty.json
+-rw-r--r--   0        0        0     1730 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_tasks_next.json
+-rw-r--r--   0        0        0    25354 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_transactions.json
+-rw-r--r--   0        0        0     9874 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_transactions_next.json
+-rw-r--r--   0        0        0      466 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_user_jane.json
+-rw-r--r--   0        0        0      453 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_user_janesmith.json
+-rw-r--r--   0        0        0      466 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_user_jdoe.json
+-rw-r--r--   0        0        0      441 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_user_jrae.json
+-rw-r--r--   0        0        0       69 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_user_jsmith.json
+-rw-r--r--   0        0        0     1601 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/phabricator/phabricator_users.json
+-rw-r--r--   0        0        0     6495 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pipermail/pipermail_2015_november.mbox
+-rw-r--r--   0        0        0     6511 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pipermail/pipermail_2016_april.mbox
+-rw-r--r--   0        0        0      875 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pipermail/pipermail_2016_march.mbox
+-rw-r--r--   0        0        0     2170 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pipermail/pipermail_apache_index.html
+-rw-r--r--   0        0        0     1867 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pipermail/pipermail_index.html
+-rw-r--r--   0        0        0      593 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/pipermail/pipermail_index_empty.html
+-rw-r--r--   0        0        0     1414 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/redmine/redmine_issue_2.json
+-rw-r--r--   0        0        0     1426 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/redmine/redmine_issue_5.json
+-rw-r--r--   0        0        0    13221 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/redmine/redmine_issue_7311.json
+-rw-r--r--   0        0        0     1425 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/redmine/redmine_issue_9.json
+-rw-r--r--   0        0        0     2830 2024-04-11 10:42:47.201317 perceval-1.0.0rc2/tests/data/redmine/redmine_issues.json
+-rw-r--r--   0        0        0       76 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/redmine/redmine_issues_empty.json
+-rw-r--r--   0        0        0     1061 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/redmine/redmine_issues_next.json
+-rw-r--r--   0        0        0      292 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/redmine/redmine_user_24.json
+-rw-r--r--   0        0        0      292 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/redmine/redmine_user_25.json
+-rw-r--r--   0        0        0      291 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/redmine/redmine_user_3.json
+-rw-r--r--   0        0        0      291 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/redmine/redmine_user_4.json
+-rw-r--r--   0        0        0      896 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/rocketchat/channel_info.json
+-rw-r--r--   0        0        0       82 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/rocketchat/message_empty_2020_05_10.json
+-rw-r--r--   0        0        0     1408 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/rocketchat/message_page_1.json
+-rw-r--r--   0        0        0     1017 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/rocketchat/message_page_2.json
+-rw-r--r--   0        0        0      448 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/rocketchat/message_page_2020_05_03.json
+-rw-r--r--   0        0        0    18134 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/rss/rss_entries.xml
+-rw-r--r--   0        0        0       54 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_error.json
+-rw-r--r--   0        0        0     1752 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_history.json
+-rw-r--r--   0        0        0     1013 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_history_20150323.json
+-rw-r--r--   0        0        0       97 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_history_empty.json
+-rw-r--r--   0        0        0      393 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_history_next.json
+-rw-r--r--   0        0        0     1064 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_info.json
+-rw-r--r--   0        0        0     1063 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_info_archived.json
+-rw-r--r--   0        0        0     2225 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_members1.json
+-rw-r--r--   0        0        0     1445 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_members2.json
+-rw-r--r--   0        0        0     1252 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_user_U0001.json
+-rw-r--r--   0        0        0     1170 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_user_U0002.json
+-rw-r--r--   0        0        0     1060 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_user_U0003.json
+-rw-r--r--   0        0        0       51 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/slack/slack_user_U0004_private.json
+-rw-r--r--   0        0        0     2676 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question
+-rw-r--r--   0        0        0     5189 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_backoff_page
+-rw-r--r--   0        0        0     5171 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_page
+-rw-r--r--   0        0        0     5172 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_page_2
+-rw-r--r--   0        0        0     4638 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_parse
+-rw-r--r--   0        0        0      883 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/supybot/supybot_2012_10_17.log
+-rw-r--r--   0        0        0      660 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/supybot/supybot_2012_10_18.log
+-rw-r--r--   0        0        0      181 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/supybot/supybot_date_without_tz.log
+-rw-r--r--   0        0        0      820 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/supybot/supybot_invalid_date.log
+-rw-r--r--   0        0        0      818 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/supybot/supybot_invalid_msg.log
+-rw-r--r--   0        0        0     7571 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/supybot/supybot_valid.log
+-rw-r--r--   0        0        0     1612 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/telegram/telegram_messages.json
+-rw-r--r--   0        0        0       27 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/telegram/telegram_messages_empty.json
+-rw-r--r--   0        0        0     1587 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/telegram/telegram_messages_next.json
+-rw-r--r--   0        0        0   731129 2024-04-11 10:42:47.205317 perceval-1.0.0rc2/tests/data/twitter/tweets.json
+-rw-r--r--   0        0        0    21985 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/twitter/tweets_page_1.json
+-rw-r--r--   0        0        0    24147 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/twitter/tweets_page_2.json
+-rw-r--r--   0        0        0      381 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/twitter/tweets_page_3.json
+-rw-r--r--   0        0        0     4140 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/utils/bugzilla_bug.xml
+-rw-r--r--   0        0        0    14409 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/utils/bugzilla_bugs_invalid_chars.xml
+-rw-r--r--   0        0        0     5429 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/utils/email_multipart_encoding.txt
+-rw-r--r--   0        0        0     4180 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/utils/email_multipart_no_encoding.txt
+-rw-r--r--   0        0        0      329 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/utils/email_single.txt
+-rw-r--r--   0        0        0      330 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/utils/mbox_single.mbox
+-rw-r--r--   0        0        0      420 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/data/utils/xml_invalid.xml
+-rw-r--r--   0        0        0        0 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/mocked_package/__init__.py
+-rw-r--r--   0        0        0     1270 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/mocked_package/backend.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/mocked_package/nested_package/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/mocked_package/nested_package/nested_backend_b.py
+-rw-r--r--   0        0        0     1241 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/mocked_package/nested_package/nested_backend_c.py
+-rwxr-xr-x   0        0        0     1180 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/run_tests.py
+-rw-r--r--   0        0        0    18694 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_archive.py
+-rw-r--r--   0        0        0    29194 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_askbot.py
+-rw-r--r--   0        0        0    89739 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_backend.py
+-rw-r--r--   0        0        0    45401 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_bugzilla.py
+-rw-r--r--   0        0        0    34723 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_bugzillarest.py
+-rw-r--r--   0        0        0    19093 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_client.py
+-rw-r--r--   0        0        0    28276 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_confluence.py
+-rw-r--r--   0        0        0    46790 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_discourse.py
+-rw-r--r--   0        0        0     9175 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_dockerhub.py
+-rw-r--r--   0        0        0     4320 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_errors.py
+-rw-r--r--   0        0        0    21716 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_gerrit.py
+-rw-r--r--   0        0        0    82928 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_git.py
+-rw-r--r--   0        0        0   216577 2024-04-11 10:42:47.209317 perceval-1.0.0rc2/tests/test_github.py
+-rw-r--r--   0        0        0    38701 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_githubql.py
+-rw-r--r--   0        0        0    83197 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_gitlab.py
+-rw-r--r--   0        0        0    19906 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_gitter.py
+-rw-r--r--   0        0        0    13003 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_googlehits.py
+-rw-r--r--   0        0        0    21109 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_groupsio.py
+-rw-r--r--   0        0        0    18362 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_hyperkitty.py
+-rw-r--r--   0        0        0    38356 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_jenkins.py
+-rw-r--r--   0        0        0    40029 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_jira.py
+-rw-r--r--   0        0        0    54602 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_launchpad.py
+-rw-r--r--   0        0        0    31185 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_mattermost.py
+-rw-r--r--   0        0        0    27864 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_mbox.py
+-rw-r--r--   0        0        0    28609 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_mediawiki.py
+-rw-r--r--   0        0        0    37724 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_meetup.py
+-rw-r--r--   0        0        0    30330 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_pagure.py
+-rw-r--r--   0        0        0    45588 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_phabricator.py
+-rw-r--r--   0        0        0    27472 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_pipermail.py
+-rw-r--r--   0        0        0    23487 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_redmine.py
+-rw-r--r--   0        0        0    25298 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_rocketchat.py
+-rw-r--r--   0        0        0    10139 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_rss.py
+-rw-r--r--   0        0        0    35971 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_slack.py
+-rw-r--r--   0        0        0    22342 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_stackexchange.py
+-rw-r--r--   0        0        0    22836 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_supybot.py
+-rw-r--r--   0        0        0    18086 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_telegram.py
+-rw-r--r--   0        0        0    17146 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_twitter.py
+-rw-r--r--   0        0        0    11254 2024-04-11 10:42:47.213317 perceval-1.0.0rc2/tests/test_utils.py
+-rw-r--r--   0        0        0    16471 1970-01-01 00:00:00.000000 perceval-1.0.0rc2/PKG-INFO
```

### Comparing `perceval-1.0.0rc1/LICENSE` & `perceval-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/NEWS` & `perceval-1.0.0rc2/NEWS`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/README.md` & `perceval-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/archive.py` & `perceval-1.0.0rc2/perceval/archive.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backend.py` & `perceval-1.0.0rc2/perceval/backend.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/__init__.py` & `perceval-1.0.0rc2/perceval/backends/core/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/askbot.py` & `perceval-1.0.0rc2/perceval/backends/core/askbot.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/bugzilla.py` & `perceval-1.0.0rc2/perceval/backends/core/bugzilla.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/bugzillarest.py` & `perceval-1.0.0rc2/perceval/backends/core/bugzillarest.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/confluence.py` & `perceval-1.0.0rc2/perceval/backends/core/confluence.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/discourse.py` & `perceval-1.0.0rc2/perceval/backends/core/discourse.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/dockerhub.py` & `perceval-1.0.0rc2/perceval/backends/core/dockerhub.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/gerrit.py` & `perceval-1.0.0rc2/perceval/backends/core/gerrit.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/git.py` & `perceval-1.0.0rc2/perceval/backends/core/git.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/github.py` & `perceval-1.0.0rc2/perceval/backends/core/github.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/githubql.py` & `perceval-1.0.0rc2/perceval/backends/core/githubql.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/gitlab.py` & `perceval-1.0.0rc2/perceval/backends/core/gitlab.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/gitter.py` & `perceval-1.0.0rc2/perceval/backends/core/gitter.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/googlehits.py` & `perceval-1.0.0rc2/perceval/backends/core/googlehits.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/groupsio.py` & `perceval-1.0.0rc2/perceval/backends/core/groupsio.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/hyperkitty.py` & `perceval-1.0.0rc2/perceval/backends/core/hyperkitty.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/jenkins.py` & `perceval-1.0.0rc2/perceval/backends/core/jenkins.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/jira.py` & `perceval-1.0.0rc2/perceval/backends/core/jira.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/launchpad.py` & `perceval-1.0.0rc2/perceval/backends/core/launchpad.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/mattermost.py` & `perceval-1.0.0rc2/perceval/backends/core/mattermost.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/mbox.py` & `perceval-1.0.0rc2/perceval/backends/core/mbox.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/mediawiki.py` & `perceval-1.0.0rc2/perceval/backends/core/mediawiki.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/meetup.py` & `perceval-1.0.0rc2/perceval/backends/core/meetup.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/nntp.py` & `perceval-1.0.0rc2/perceval/backends/core/nntp.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/pagure.py` & `perceval-1.0.0rc2/perceval/backends/core/pagure.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/phabricator.py` & `perceval-1.0.0rc2/perceval/backends/core/phabricator.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/pipermail.py` & `perceval-1.0.0rc2/perceval/backends/core/pipermail.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/redmine.py` & `perceval-1.0.0rc2/perceval/backends/core/redmine.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/rocketchat.py` & `perceval-1.0.0rc2/perceval/backends/core/rocketchat.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/rss.py` & `perceval-1.0.0rc2/perceval/backends/core/rss.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/slack.py` & `perceval-1.0.0rc2/perceval/backends/core/slack.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/stackexchange.py` & `perceval-1.0.0rc2/perceval/backends/core/stackexchange.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/supybot.py` & `perceval-1.0.0rc2/perceval/backends/core/supybot.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/telegram.py` & `perceval-1.0.0rc2/perceval/backends/core/telegram.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/backends/core/twitter.py` & `perceval-1.0.0rc2/perceval/backends/core/twitter.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/client.py` & `perceval-1.0.0rc2/perceval/client.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/errors.py` & `perceval-1.0.0rc2/perceval/errors.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/perceval.py` & `perceval-1.0.0rc2/perceval/perceval.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/perceval/utils.py` & `perceval-1.0.0rc2/perceval/utils.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/pyproject.toml` & `perceval-1.0.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval"
-version = "1.0.0-rc.1"
+version = "1.0.0-rc.2"
 description = "Send Sir Perceval on a quest to fetch and gather data from software repositories."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval-1.0.0rc1/tests/base.py` & `perceval-1.0.0rc2/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/api_24396_openstack.json` & `perceval-1.0.0rc2/tests/data/askbot/api_24396_openstack.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/askbot_2481_multicomments.json` & `perceval-1.0.0rc2/tests/data/askbot/askbot_2481_multicomments.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/askbot_api_questions.json` & `perceval-1.0.0rc2/tests/data/askbot/askbot_api_questions.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/askbot_api_questions_2.json` & `perceval-1.0.0rc2/tests/data/askbot/askbot_api_questions_2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/askbot_question.html` & `perceval-1.0.0rc2/tests/data/askbot/askbot_question.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/askbot_question_empty.html` & `perceval-1.0.0rc2/tests/data/askbot/askbot_question_empty.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/askbot_question_multipage_1.html` & `perceval-1.0.0rc2/tests/data/askbot/askbot_question_multipage_1.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/askbot_question_multipage_2.html` & `perceval-1.0.0rc2/tests/data/askbot/askbot_question_multipage_2.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_148_comments_answer_2_openstack.html` & `perceval-1.0.0rc2/tests/data/askbot/html_148_comments_answer_2_openstack.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_16_multicomment_answer_1_openstack.html` & `perceval-1.0.0rc2/tests/data/askbot/html_16_multicomment_answer_1_openstack.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_2_openstack.html` & `perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_2_openstack.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_3_openstack.html` & `perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_3_openstack.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_4_openstack.html` & `perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_4_openstack.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_openstack.html` & `perceval-1.0.0rc2/tests/data/askbot/html_24396_multipage_openstack.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_26830_comments_question_openstack.html` & `perceval-1.0.0rc2/tests/data/askbot/html_26830_comments_question_openstack.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_7893_answer_3_updated.html` & `perceval-1.0.0rc2/tests/data/askbot/html_7893_answer_3_updated.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/askbot/html_country_and_website.html` & `perceval-1.0.0rc2/tests/data/askbot/html_country_and_website.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug.xml` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity.html` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_empty.html` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity_empty.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_empty_alt.html` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity_empty_alt.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_not_valid.html` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bug_activity_not_valid.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_buglist.csv` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_buglist.csv`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details.xml` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_details.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details_next.xml` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_details_next.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details_not_valid.xml` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_details_not_valid.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_invalid_chars.xml` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_bugs_invalid_chars.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs.json` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_attachments.json` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_attachments.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_comments.json` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_comments.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_history.json` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_history.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_next.json` & `perceval-1.0.0rc2/tests/data/bugzilla/bugzilla_rest_bugs_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v1.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_content_1_v1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v2.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_content_1_v2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v3.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_content_1_v3.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_content_2_v1.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_content_2_v1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_content_3.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_content_3.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_content_att_v1.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_content_att_v1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_content_space.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_content_space.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_contents.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_contents.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/confluence/confluence_contents_next.json` & `perceval-1.0.0rc2/tests/data/confluence/confluence_contents_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_post.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_post.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_posts.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_posts.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1148.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_topic_1148.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1149.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_topic_1149.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1150.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_topic_1150.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_topics.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_topics.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_topics_last_posted_at_null.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_topics_last_posted_at_null.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/discourse/discourse_topics_pinned.json` & `perceval-1.0.0rc2/tests/data/discourse/discourse_topics_pinned.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/dockerhub/dockerhub_repository_1.json` & `perceval-1.0.0rc2/tests/data/dockerhub/dockerhub_repository_1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_1` & `perceval-1.0.0rc2/tests/data/gerrit/gerrit_reviews_page_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_2` & `perceval-1.0.0rc2/tests/data/gerrit/gerrit_reviews_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_3` & `perceval-1.0.0rc2/tests/data/gerrit/gerrit_reviews_page_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/git_bad_encoding.txt` & `perceval-1.0.0rc2/tests/data/git/git_bad_encoding.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/git_log.txt` & `perceval-1.0.0rc2/tests/data/git/git_log.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/git_log_incompleted.txt` & `perceval-1.0.0rc2/tests/data/git/git_log_incompleted.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/git_log_merge.txt` & `perceval-1.0.0rc2/tests/data/git/git_log_merge.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/git_log_trailers.txt` & `perceval-1.0.0rc2/tests/data/git/git_log_trailers.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/gitalternates.tar.gz` & `perceval-1.0.0rc2/tests/data/git/gitalternates.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/gitdetached.tar.gz` & `perceval-1.0.0rc2/tests/data/git/gitdetached.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/gittest-sub.tar.gz` & `perceval-1.0.0rc2/tests/data/git/gittest-sub.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/gittest-top-sub.tar.gz` & `perceval-1.0.0rc2/tests/data/git/gittest-top-sub.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/gittest.tar.gz` & `perceval-1.0.0rc2/tests/data/git/gittest.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/gittest_no_refs.tar.gz` & `perceval-1.0.0rc2/tests/data/git/gittest_no_refs.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/git/gittestempty.tar.gz` & `perceval-1.0.0rc2/tests/data/git/gittestempty.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_enterprise_request_requested_reviewers` & `perceval-1.0.0rc2/tests/data/github/github_enterprise_request_requested_reviewers`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_events_page_1` & `perceval-1.0.0rc2/tests/data/github/github_events_page_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_events_page_2` & `perceval-1.0.0rc2/tests/data/github/github_events_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_events_page_3` & `perceval-1.0.0rc2/tests/data/github/github_events_page_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_events_pull_request_review` & `perceval-1.0.0rc2/tests/data/github/github_events_pull_request_review`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_issue_1` & `perceval-1.0.0rc2/tests/data/github/github_issue_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_issue_2` & `perceval-1.0.0rc2/tests/data/github/github_issue_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_issue_2_reactions` & `perceval-1.0.0rc2/tests/data/github/github_issue_2_reactions`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_issue_2_with_pr` & `perceval-1.0.0rc2/tests/data/github/github_issue_2_with_pr`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_issue_comment_1_reactions` & `perceval-1.0.0rc2/tests/data/github/github_issue_comment_1_reactions`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_issue_comments_1` & `perceval-1.0.0rc2/tests/data/github/github_issue_comments_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_issue_comments_2` & `perceval-1.0.0rc2/tests/data/github/github_issue_comments_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_login` & `perceval-1.0.0rc2/tests/data/github/github_login`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_orgs` & `perceval-1.0.0rc2/tests/data/github/github_orgs`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_repo` & `perceval-1.0.0rc2/tests/data/github/github_repo`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request` & `perceval-1.0.0rc2/tests/data/github/github_request`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_from_2016_03_01` & `perceval-1.0.0rc2/tests/data/github/github_request_from_2016_03_01`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_comment_2_reactions` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_comment_2_reactions`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_comments` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_comments`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_commits` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_commits`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_reviews` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_1_reviews`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_comments` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2_comments`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_commits` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2_commits`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_reviews` & `perceval-1.0.0rc2/tests/data/github/github_request_pull_request_2_reviews`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_requested_reviewers` & `perceval-1.0.0rc2/tests/data/github/github_request_requested_reviewers`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/github_request_requested_reviewers_ghost` & `perceval-1.0.0rc2/tests/data/github/github_request_requested_reviewers_ghost`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/github/private.pem` & `perceval-1.0.0rc2/tests/data/github/private.pem`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/commits_1` & `perceval-1.0.0rc2/tests/data/gitlab/commits_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/commits_2` & `perceval-1.0.0rc2/tests/data/gitlab/commits_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/commits_3` & `perceval-1.0.0rc2/tests/data/gitlab/commits_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/emoji` & `perceval-1.0.0rc2/tests/data/gitlab/emoji`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/issue_1` & `perceval-1.0.0rc2/tests/data/gitlab/issue_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/issue_2` & `perceval-1.0.0rc2/tests/data/gitlab/issue_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/issue_3` & `perceval-1.0.0rc2/tests/data/gitlab/issue_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/issue_4` & `perceval-1.0.0rc2/tests/data/gitlab/issue_4`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/issue_page_1` & `perceval-1.0.0rc2/tests/data/gitlab/issue_page_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/issue_page_2` & `perceval-1.0.0rc2/tests/data/gitlab/issue_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_1` & `perceval-1.0.0rc2/tests/data/gitlab/merge_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_1_version_1` & `perceval-1.0.0rc2/tests/data/gitlab/merge_1_version_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_1_version_2` & `perceval-1.0.0rc2/tests/data/gitlab/merge_1_version_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_1_versions` & `perceval-1.0.0rc2/tests/data/gitlab/merge_1_versions`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_2` & `perceval-1.0.0rc2/tests/data/gitlab/merge_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_2_version_1` & `perceval-1.0.0rc2/tests/data/gitlab/merge_2_version_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_3` & `perceval-1.0.0rc2/tests/data/gitlab/merge_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_3_version_1` & `perceval-1.0.0rc2/tests/data/gitlab/merge_3_version_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_page_1` & `perceval-1.0.0rc2/tests/data/gitlab/merge_page_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_page_2` & `perceval-1.0.0rc2/tests/data/gitlab/merge_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_page_outdated` & `perceval-1.0.0rc2/tests/data/gitlab/merge_page_outdated`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/merge_page_updated` & `perceval-1.0.0rc2/tests/data/gitlab/merge_page_updated`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/notes_1` & `perceval-1.0.0rc2/tests/data/gitlab/notes_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/notes_2` & `perceval-1.0.0rc2/tests/data/gitlab/notes_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/notes_3` & `perceval-1.0.0rc2/tests/data/gitlab/notes_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/notes_4` & `perceval-1.0.0rc2/tests/data/gitlab/notes_4`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitlab/project` & `perceval-1.0.0rc2/tests/data/gitlab/project`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitter/message_page_1` & `perceval-1.0.0rc2/tests/data/gitter/message_page_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitter/message_page_2` & `perceval-1.0.0rc2/tests/data/gitter/message_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/gitter/rooms` & `perceval-1.0.0rc2/tests/data/gitter/rooms`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/googlehits/hits_bitergia` & `perceval-1.0.0rc2/tests/data/googlehits/hits_bitergia`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/googlehits/hits_bitergia_grimoirelab` & `perceval-1.0.0rc2/tests/data/googlehits/hits_bitergia_grimoirelab`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/googlehits/hits_zero` & `perceval-1.0.0rc2/tests/data/googlehits/hits_zero`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/groupsio/login` & `perceval-1.0.0rc2/tests/data/groupsio/login`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/groupsio/messages.zip` & `perceval-1.0.0rc2/tests/data/groupsio/messages.zip`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/groupsio/subscriptions_page_1` & `perceval-1.0.0rc2/tests/data/groupsio/subscriptions_page_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/groupsio/subscriptions_page_2` & `perceval-1.0.0rc2/tests/data/groupsio/subscriptions_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/hyperkitty/hyperkitty_2016_april.mbox` & `perceval-1.0.0rc2/tests/data/hyperkitty/hyperkitty_2016_april.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/hyperkitty/hyperkitty_2016_march.mbox` & `perceval-1.0.0rc2/tests/data/hyperkitty/hyperkitty_2016_march.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jenkins/jenkins_build.json` & `perceval-1.0.0rc2/tests/data/jenkins/jenkins_build.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_builds.json` & `perceval-1.0.0rc2/tests/data/jenkins/jenkins_job_builds.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_no_builds.json` & `perceval-1.0.0rc2/tests/data/jenkins/jenkins_job_no_builds.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jenkins/jenkins_jobs.json` & `perceval-1.0.0rc2/tests/data/jenkins/jenkins_jobs.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jenkins/jenkins_workflow_job_builds.json` & `perceval-1.0.0rc2/tests/data/jenkins/jenkins_workflow_job_builds.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jenkins/jenkins_workflow_jobs.json` & `perceval-1.0.0rc2/tests/data/jenkins/jenkins_workflow_jobs.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_page_1.json` & `perceval-1.0.0rc2/tests/data/jira/jira_comments_issue_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_page_2.json` & `perceval-1.0.0rc2/tests/data/jira/jira_comments_issue_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jira/jira_fields.json` & `perceval-1.0.0rc2/tests/data/jira/jira_fields.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jira/jira_issues_page_1.json` & `perceval-1.0.0rc2/tests/data/jira/jira_issues_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jira/jira_issues_page_2.json` & `perceval-1.0.0rc2/tests/data/jira/jira_issues_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/jira/jira_issues_parse_expected.json` & `perceval-1.0.0rc2/tests/data/jira/jira_issues_parse_expected.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_activities`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_next_1` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_activities_next_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_next_2` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_activities_next_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_attachments`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_next_1` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_attachments_next_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_next_2` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_attachments_next_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_comments`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_next_1` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_comments_next_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_next_2` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_comments_next_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_expected` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_expected`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_expected_no_entries` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_expected_no_entries`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_no_entries` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_1_no_entries`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_activities` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2_activities`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_comments` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2_comments`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_expected` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_2_expected`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_3` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_3_expected` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issue_3_expected`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1_no_entries` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_1_no_entries`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1_no_next` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_1_no_next`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_2` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_3` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_issues_page_3`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/launchpad/launchpad_user_1` & `perceval-1.0.0rc2/tests/data/launchpad/launchpad_user_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts.json` & `perceval-1.0.0rc2/tests/data/mattermost/mattermost_posts.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts_next.json` & `perceval-1.0.0rc2/tests/data/mattermost/mattermost_posts_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mattermost/mattermost_user_valcos.json` & `perceval-1.0.0rc2/tests/data/mattermost/mattermost_user_valcos.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mbox/mbox_complex.mbox` & `perceval-1.0.0rc2/tests/data/mbox/mbox_complex.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mbox/mbox_iso8859_encoding.mbox` & `perceval-1.0.0rc2/tests/data/mbox/mbox_iso8859_encoding.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mbox/mbox_multipart.mbox` & `perceval-1.0.0rc2/tests/data/mbox/mbox_multipart.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mbox/mbox_no_fields.mbox` & `perceval-1.0.0rc2/tests/data/mbox/mbox_no_fields.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mbox/mbox_unixfrom_encoding.mbox` & `perceval-1.0.0rc2/tests/data/mbox/mbox_unixfrom_encoding.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mbox/mbox_unknown_encoding.mbox` & `perceval-1.0.0rc2/tests/data/mbox/mbox_unknown_encoding.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_namespaces.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_namespaces.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_476583_revisions.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_page_476583_revisions.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_592384_revisions.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_page_592384_revisions.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_all.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_all.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_allrevisions.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_allrevisions.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_recent_changes.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_pages_recent_changes.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_siteinfo_1.23.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_siteinfo_1.23.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_siteinfo_1.28.json` & `perceval-1.0.0rc2/tests/data/mediawiki/mediawiki_siteinfo_1.28.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/meetup/meetup_comments.json` & `perceval-1.0.0rc2/tests/data/meetup/meetup_comments.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/meetup/meetup_events.json` & `perceval-1.0.0rc2/tests/data/meetup/meetup_events.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/meetup/meetup_events_next.json` & `perceval-1.0.0rc2/tests/data/meetup/meetup_events_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/meetup/meetup_events_range.json` & `perceval-1.0.0rc2/tests/data/meetup/meetup_events_range.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/meetup/meetup_rsvps.json` & `perceval-1.0.0rc2/tests/data/meetup/meetup_rsvps.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/nntp/nntp_1.txt` & `perceval-1.0.0rc2/tests/data/nntp/nntp_1.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/nntp/nntp_2.txt` & `perceval-1.0.0rc2/tests/data/nntp/nntp_2.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/nntp/nntp_parsing_error.txt` & `perceval-1.0.0rc2/tests/data/nntp/nntp_parsing_error.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pagure/pagure_namespace_issue_2` & `perceval-1.0.0rc2/tests/data/pagure/pagure_namespace_issue_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_1` & `perceval-1.0.0rc2/tests/data/pagure/pagure_repo_issue_1`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_2` & `perceval-1.0.0rc2/tests/data/pagure/pagure_repo_issue_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_from_2020_03_07` & `perceval-1.0.0rc2/tests/data/pagure/pagure_repo_issue_from_2020_03_07`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pagure/pagure_repo_only_issue_2` & `perceval-1.0.0rc2/tests/data/pagure/pagure_repo_only_issue_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/phabricator/phabricator_phids.json` & `perceval-1.0.0rc2/tests/data/phabricator/phabricator_phids.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks.json` & `perceval-1.0.0rc2/tests/data/phabricator/phabricator_tasks.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks_next.json` & `perceval-1.0.0rc2/tests/data/phabricator/phabricator_tasks_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/phabricator/phabricator_transactions.json` & `perceval-1.0.0rc2/tests/data/phabricator/phabricator_transactions.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/phabricator/phabricator_transactions_next.json` & `perceval-1.0.0rc2/tests/data/phabricator/phabricator_transactions_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/phabricator/phabricator_users.json` & `perceval-1.0.0rc2/tests/data/phabricator/phabricator_users.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pipermail/pipermail_2015_november.mbox` & `perceval-1.0.0rc2/tests/data/pipermail/pipermail_2015_november.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pipermail/pipermail_2016_april.mbox` & `perceval-1.0.0rc2/tests/data/pipermail/pipermail_2016_april.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pipermail/pipermail_2016_march.mbox` & `perceval-1.0.0rc2/tests/data/pipermail/pipermail_2016_march.mbox`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pipermail/pipermail_apache_index.html` & `perceval-1.0.0rc2/tests/data/pipermail/pipermail_apache_index.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pipermail/pipermail_index.html` & `perceval-1.0.0rc2/tests/data/pipermail/pipermail_index.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/pipermail/pipermail_index_empty.html` & `perceval-1.0.0rc2/tests/data/pipermail/pipermail_index_empty.html`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/redmine/redmine_issue_2.json` & `perceval-1.0.0rc2/tests/data/redmine/redmine_issue_2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/redmine/redmine_issue_5.json` & `perceval-1.0.0rc2/tests/data/redmine/redmine_issue_5.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/redmine/redmine_issue_7311.json` & `perceval-1.0.0rc2/tests/data/redmine/redmine_issue_7311.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/redmine/redmine_issue_9.json` & `perceval-1.0.0rc2/tests/data/redmine/redmine_issue_9.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/redmine/redmine_issues.json` & `perceval-1.0.0rc2/tests/data/redmine/redmine_issues.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/redmine/redmine_issues_next.json` & `perceval-1.0.0rc2/tests/data/redmine/redmine_issues_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/rocketchat/channel_info.json` & `perceval-1.0.0rc2/tests/data/rocketchat/channel_info.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/rocketchat/message_page_1.json` & `perceval-1.0.0rc2/tests/data/rocketchat/message_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/rocketchat/message_page_2.json` & `perceval-1.0.0rc2/tests/data/rocketchat/message_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/rss/rss_entries.xml` & `perceval-1.0.0rc2/tests/data/rss/rss_entries.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_history.json` & `perceval-1.0.0rc2/tests/data/slack/slack_history.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_history_20150323.json` & `perceval-1.0.0rc2/tests/data/slack/slack_history_20150323.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_info.json` & `perceval-1.0.0rc2/tests/data/slack/slack_info.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_info_archived.json` & `perceval-1.0.0rc2/tests/data/slack/slack_info_archived.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_members1.json` & `perceval-1.0.0rc2/tests/data/slack/slack_members1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_members2.json` & `perceval-1.0.0rc2/tests/data/slack/slack_members2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_user_U0001.json` & `perceval-1.0.0rc2/tests/data/slack/slack_user_U0001.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_user_U0002.json` & `perceval-1.0.0rc2/tests/data/slack/slack_user_U0002.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/slack/slack_user_U0003.json` & `perceval-1.0.0rc2/tests/data/slack/slack_user_U0003.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question` & `perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_backoff_page` & `perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_backoff_page`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_page` & `perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_page`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_page_2` & `perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_page_2`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_parse` & `perceval-1.0.0rc2/tests/data/stackexchange/stackexchange_question_parse`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/supybot/supybot_2012_10_17.log` & `perceval-1.0.0rc2/tests/data/supybot/supybot_2012_10_17.log`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/supybot/supybot_2012_10_18.log` & `perceval-1.0.0rc2/tests/data/supybot/supybot_2012_10_18.log`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/supybot/supybot_invalid_date.log` & `perceval-1.0.0rc2/tests/data/supybot/supybot_invalid_date.log`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/supybot/supybot_invalid_msg.log` & `perceval-1.0.0rc2/tests/data/supybot/supybot_invalid_msg.log`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/supybot/supybot_valid.log` & `perceval-1.0.0rc2/tests/data/supybot/supybot_valid.log`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/telegram/telegram_messages.json` & `perceval-1.0.0rc2/tests/data/telegram/telegram_messages.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/telegram/telegram_messages_next.json` & `perceval-1.0.0rc2/tests/data/telegram/telegram_messages_next.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/twitter/tweets.json` & `perceval-1.0.0rc2/tests/data/twitter/tweets.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/twitter/tweets_page_1.json` & `perceval-1.0.0rc2/tests/data/twitter/tweets_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/twitter/tweets_page_2.json` & `perceval-1.0.0rc2/tests/data/twitter/tweets_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/utils/bugzilla_bug.xml` & `perceval-1.0.0rc2/tests/data/utils/bugzilla_bug.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/utils/bugzilla_bugs_invalid_chars.xml` & `perceval-1.0.0rc2/tests/data/utils/bugzilla_bugs_invalid_chars.xml`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/utils/email_multipart_encoding.txt` & `perceval-1.0.0rc2/tests/data/utils/email_multipart_encoding.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/data/utils/email_multipart_no_encoding.txt` & `perceval-1.0.0rc2/tests/data/utils/email_multipart_no_encoding.txt`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/mocked_package/backend.py` & `perceval-1.0.0rc2/tests/mocked_package/backend.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/mocked_package/nested_package/nested_backend_b.py` & `perceval-1.0.0rc2/tests/mocked_package/nested_package/nested_backend_b.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/mocked_package/nested_package/nested_backend_c.py` & `perceval-1.0.0rc2/tests/mocked_package/nested_package/nested_backend_c.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/run_tests.py` & `perceval-1.0.0rc2/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_archive.py` & `perceval-1.0.0rc2/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_askbot.py` & `perceval-1.0.0rc2/tests/test_askbot.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_backend.py` & `perceval-1.0.0rc2/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_bugzilla.py` & `perceval-1.0.0rc2/tests/test_bugzilla.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_bugzillarest.py` & `perceval-1.0.0rc2/tests/test_bugzillarest.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_client.py` & `perceval-1.0.0rc2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_confluence.py` & `perceval-1.0.0rc2/tests/test_confluence.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_discourse.py` & `perceval-1.0.0rc2/tests/test_discourse.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_dockerhub.py` & `perceval-1.0.0rc2/tests/test_dockerhub.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_errors.py` & `perceval-1.0.0rc2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_gerrit.py` & `perceval-1.0.0rc2/tests/test_gerrit.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_git.py` & `perceval-1.0.0rc2/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_github.py` & `perceval-1.0.0rc2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_githubql.py` & `perceval-1.0.0rc2/tests/test_githubql.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_gitlab.py` & `perceval-1.0.0rc2/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_gitter.py` & `perceval-1.0.0rc2/tests/test_gitter.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_googlehits.py` & `perceval-1.0.0rc2/tests/test_googlehits.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_groupsio.py` & `perceval-1.0.0rc2/tests/test_groupsio.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_hyperkitty.py` & `perceval-1.0.0rc2/tests/test_hyperkitty.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_jenkins.py` & `perceval-1.0.0rc2/tests/test_jenkins.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_jira.py` & `perceval-1.0.0rc2/tests/test_jira.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_launchpad.py` & `perceval-1.0.0rc2/tests/test_launchpad.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_mattermost.py` & `perceval-1.0.0rc2/tests/test_mattermost.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_mbox.py` & `perceval-1.0.0rc2/tests/test_mbox.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_mediawiki.py` & `perceval-1.0.0rc2/tests/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_meetup.py` & `perceval-1.0.0rc2/tests/test_meetup.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_pagure.py` & `perceval-1.0.0rc2/tests/test_pagure.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_phabricator.py` & `perceval-1.0.0rc2/tests/test_phabricator.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_pipermail.py` & `perceval-1.0.0rc2/tests/test_pipermail.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_redmine.py` & `perceval-1.0.0rc2/tests/test_redmine.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_rocketchat.py` & `perceval-1.0.0rc2/tests/test_rocketchat.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_rss.py` & `perceval-1.0.0rc2/tests/test_rss.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_slack.py` & `perceval-1.0.0rc2/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_stackexchange.py` & `perceval-1.0.0rc2/tests/test_stackexchange.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_supybot.py` & `perceval-1.0.0rc2/tests/test_supybot.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_telegram.py` & `perceval-1.0.0rc2/tests/test_telegram.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_twitter.py` & `perceval-1.0.0rc2/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/tests/test_utils.py` & `perceval-1.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `perceval-1.0.0rc1/PKG-INFO` & `perceval-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Send Sir Perceval on a quest to fetch and gather data from software repositories.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


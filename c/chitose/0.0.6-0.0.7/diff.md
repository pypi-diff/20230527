# Comparing `tmp/chitose-0.0.6.tar.gz` & `tmp/chitose-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chitose-0.0.6.tar", max compression
+gzip compressed data, was "chitose-0.0.7.tar", max compression
```

## Comparing `chitose-0.0.6.tar` & `chitose-0.0.7.tar`

### file list

```diff
@@ -1,143 +1,144 @@
--rw-r--r--   0        0        0     1073 2023-05-21 03:09:41.620752 chitose-0.0.6/LICENSE
--rw-r--r--   0        0        0     3483 2023-05-21 03:09:41.620752 chitose-0.0.6/README.md
--rw-r--r--   0        0        0      221 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/__init__.py
--rw-r--r--   0        0        0     7877 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/agent.py
--rw-r--r--   0        0        0      478 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/__init__.py
--rw-r--r--   0        0        0     1207 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     5314 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      314 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      286 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      297 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      453 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      682 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      466 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0      467 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      435 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      372 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1717 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1343 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2511 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1145 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0     3748 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     6930 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1037 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/describe_feed_generator.py
--rw-r--r--   0        0        0      926 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/generator.py
--rw-r--r--   0        0        0      462 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_actor_feeds.py
--rw-r--r--   0        0        0      439 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      461 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed.py
--rw-r--r--   0        0        0      387 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed_generator.py
--rw-r--r--   0        0        0      353 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed_generators.py
--rw-r--r--   0        0        0      463 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed_skeleton.py
--rw-r--r--   0        0        0      902 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      352 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      310 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0      453 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      477 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      480 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2470 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/post.py
--rw-r--r--   0        0        0      484 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/repost.py
--rw-r--r--   0        0        0     3094 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      398 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2637 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      400 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      415 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0      437 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      433 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      420 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0      428 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0      448 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      398 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      969 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/list.py
--rw-r--r--   0        0        0      459 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      345 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      342 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      351 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      348 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0     1200 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      343 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1641 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      379 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      375 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1327 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      719 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      497 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      373 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/blob.py
--rw-r--r--   0        0        0      490 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/__init__.py
--rw-r--r--   0        0        0     1186 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/__init__.py
--rw-r--r--   0        0        0     5949 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    13162 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      438 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      516 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      399 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0      494 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      338 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      504 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      338 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0      785 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      369 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      309 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      489 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      438 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      538 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1061 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      478 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      414 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      935 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      466 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      362 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0     1030 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1096 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/defs.py
--rw-r--r--   0        0        0      810 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      820 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      931 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      735 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      740 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0     5687 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1929 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0      923 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      884 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      410 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0      693 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1418 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1066 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      568 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      392 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      355 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0     4551 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      607 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      767 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      447 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0      827 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      521 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1191 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/defs.py
--rw-r--r--   0        0        0      433 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      293 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      782 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      496 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      304 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      634 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      302 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      324 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      390 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      407 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      372 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0     4350 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      430 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      387 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      500 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      591 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      356 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      574 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      618 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      593 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      686 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      530 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      440 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2945 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      170 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/link.py
--rw-r--r--   0        0        0      136 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/object.py
--rw-r--r--   0        0        0      136 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/record.py
--rw-r--r--   0        0        0     1379 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/xrpc.py
--rw-r--r--   0        0        0      801 2023-05-21 03:09:41.624752 chitose-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4286 1970-01-01 00:00:00.000000 chitose-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-27 13:16:49.683080 chitose-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3483 2023-05-27 13:16:49.683080 chitose-0.0.7/README.md
+-rw-r--r--   0        0        0      221 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/__init__.py
+-rw-r--r--   0        0        0     8972 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/agent.py
+-rw-r--r--   0        0        0      443 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/__init__.py
+-rw-r--r--   0        0        0     1070 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/__init__.py
+-rw-r--r--   0        0        0     2061 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     5314 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      276 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      248 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      259 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      415 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      682 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      428 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0      429 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      397 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      354 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1717 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1343 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2511 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1145 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0     3583 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     6930 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0      999 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/describe_feed_generator.py
+-rw-r--r--   0        0        0      926 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/generator.py
+-rw-r--r--   0        0        0      424 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_actor_feeds.py
+-rw-r--r--   0        0        0      401 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      423 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed.py
+-rw-r--r--   0        0        0      349 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed_generator.py
+-rw-r--r--   0        0        0      315 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed_generators.py
+-rw-r--r--   0        0        0      425 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed_skeleton.py
+-rw-r--r--   0        0        0      864 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      389 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      272 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0      415 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      439 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      480 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2470 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      484 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0     2889 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2642 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      400 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      377 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0      399 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      395 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      382 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      390 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0      410 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      360 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      969 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      459 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      307 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      304 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      313 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      310 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0     1131 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      305 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1603 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      341 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      357 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1327 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      930 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      307 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/unspecced/get_popular_feed_generators.py
+-rw-r--r--   0        0        0      373 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/blob.py
+-rw-r--r--   0        0        0      455 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/__init__.py
+-rw-r--r--   0        0        0     1049 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/__init__.py
+-rw-r--r--   0        0        0     5659 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    13162 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      400 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      478 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      361 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0      456 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      300 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      466 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      300 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0      747 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      331 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      271 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      451 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      400 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      500 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1023 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      440 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      376 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      794 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      339 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      324 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      995 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1096 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/defs.py
+-rw-r--r--   0        0        0      772 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0      820 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      896 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      697 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      740 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0     5516 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1896 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0      885 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      846 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      372 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0      655 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1380 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1028 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      530 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      392 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      317 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0     4261 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      729 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      409 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0      789 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      483 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1191 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      395 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      255 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      744 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      458 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      266 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      596 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      264 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      286 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      352 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      369 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      334 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0     4145 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      349 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      462 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      553 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      318 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      536 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      580 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      555 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      648 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      492 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      402 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2945 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      170 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/link.py
+-rw-r--r--   0        0        0      136 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/object.py
+-rw-r--r--   0        0        0      136 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/record.py
+-rw-r--r--   0        0        0     1642 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/xrpc.py
+-rw-r--r--   0        0        0      801 2023-05-27 13:16:49.687080 chitose-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4286 1970-01-01 00:00:00.000000 chitose-0.0.7/PKG-INFO
```

### Comparing `chitose-0.0.6/LICENSE` & `chitose-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/README.md` & `chitose-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/agent.py` & `chitose-0.0.7/chitose/agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,74 @@
 from __future__ import annotations
 from datetime import datetime
 from datetime import timezone
 import typing
 import json
+import urllib
 
 from chitose.app.bsky.feed.like import Like
 from chitose.app.bsky.feed.post import Post
 from chitose.app.bsky.feed.repost import Repost
 from chitose.app.bsky.graph.follow import Follow
 from chitose.com.atproto.repo.strong_ref import StrongRef
 
 from .app import App_
 from .com import Com_
+from .xrpc import call
+from .xrpc import XrpcParams
+from .xrpc import XrpcData
+from .xrpc import XrpcHeaders
 
 
 class BskyAgent:
     def __init__(self, service: str) -> None:
         self.service = service
-        self.headers: dict[str, str] = {}
-        self.session: dict = {}
+        self.session: dict[str, str] = {}
+
+    def _add_auth_header(self, headers: dict[str, str]):
+        if 'authorization' not in headers and 'accessJwt' in self.session:
+            return headers | {
+                'authorization': f'Bearer {self.session["accessJwt"]}'
+            }
+
+        return headers
+
+    def _refresh_session(self, e: urllib.error.HTTPError):
+        if 'refreshJwt' not in self.session:
+            raise e
+
+        error = json.loads(e.read().decode())['error']
+        if error != 'ExpiredToken':
+            raise e
+
+        self.session = json.loads(
+            call('com.atproto.server.refreshSession',
+                 [], {}, self.service,
+                 {'authorization':
+                  f'Bearer {self.session["refreshJwt"]}'})
+        )
+
+    def _call(self, method: str, params: XrpcParams,
+              d: XrpcData, headers: XrpcHeaders) -> bytes:
+        try:
+            return call(method, params, d, self.service,
+                        self._add_auth_header(headers))
+        except urllib.error.HTTPError as e:
+            self._refresh_session(e)
+
+            return call(method, params, d, self.service,
+                        self._add_auth_header(headers))
 
     @property
     def app(self):
-        return App_(self.service, self.headers)
+        return App_(self._call)
 
     @property
     def com(self):
-        return Com_(self.service, self.headers)
+        return Com_(self._call)
 
     def get_timeline(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
         return self.app.bsky.feed.get_timeline(**kwargs)
 
     def get_author_feed(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
@@ -195,11 +233,7 @@
 
         return self.app.bsky.notification.update_seen(seen_at=seen_at)
 
     def login(self, identifier: str, password: str) -> None:
         self.session = json.loads(
             self.com.atproto.server.create_session(
                 identifier=identifier, password=password))
-
-        if 'accessJwt' in self.session:
-            self.headers['authorization'] \
-                = f'Bearer {self.session["accessJwt"]}'
```

### Comparing `chitose-0.0.6/chitose/app/bsky/__init__.py` & `chitose-0.0.7/chitose/com/atproto/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .actor import Actor_
-from .embed import Embed_
-from .feed import Feed_
-from .graph import Graph_
-from .notification import Notification_
-from .richtext import Richtext_
-from .unspecced import Unspecced_
+from chitose.xrpc import XrpcCallable
+from .admin import Admin_
+from .identity import Identity_
+from .label import Label_
+from .moderation import Moderation_
+from .repo import Repo_
+from .server import Server_
+from .sync import Sync_
 
-class Bsky_:
+class Atproto_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     @property
-    def actor(self):
-        return Actor_(self.service, self.headers)
+    def admin(self):
+        return Admin_(self.call)
 
     @property
-    def embed(self):
-        return Embed_(self.service, self.headers)
+    def identity(self):
+        return Identity_(self.call)
 
     @property
-    def feed(self):
-        return Feed_(self.service, self.headers)
+    def label(self):
+        return Label_(self.call)
 
     @property
-    def graph(self):
-        return Graph_(self.service, self.headers)
+    def moderation(self):
+        return Moderation_(self.call)
 
     @property
-    def notification(self):
-        return Notification_(self.service, self.headers)
+    def repo(self):
+        return Repo_(self.call)
 
     @property
-    def richtext(self):
-        return Richtext_(self.service, self.headers)
+    def server(self):
+        return Server_(self.call)
 
     @property
-    def unspecced(self):
-        return Unspecced_(self.service, self.headers)
+    def sync(self):
+        return Sync_(self.call)
```

### Comparing `chitose-0.0.6/chitose/app/bsky/actor/__init__.py` & `chitose-0.0.7/chitose/app/bsky/actor/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from chitose.xrpc import XrpcCallable
 from .get_preferences import _get_preferences
 from .get_profile import _get_profile
 from .get_profiles import _get_profiles
 from .get_suggestions import _get_suggestions
 from .put_preferences import _put_preferences
 from .search_actors import _search_actors
 from .search_actors_typeahead import _search_actors_typeahead
 import chitose.app.bsky.actor.defs
 import typing
 
 class Actor_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     def search_actors_typeahead(self, term: typing.Optional[str]=None, limit: typing.Optional[int]=None) -> bytes:
         """Find actor suggestions for a search term."""
-        return _search_actors_typeahead(self.service, self.headers, term, limit)
+        return _search_actors_typeahead(self.call, term, limit)
 
     def put_preferences(self, preferences: chitose.app.bsky.actor.defs.Preferences) -> bytes:
         """Sets the private preferences attached to the account."""
-        return _put_preferences(self.service, self.headers, preferences)
+        return _put_preferences(self.call, preferences)
 
     def get_profile(self, actor: str) -> bytes:
         """"""
-        return _get_profile(self.service, self.headers, actor)
+        return _get_profile(self.call, actor)
 
     def get_suggestions(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Get a list of actors suggested for following. Used in discovery UIs."""
-        return _get_suggestions(self.service, self.headers, limit, cursor)
+        return _get_suggestions(self.call, limit, cursor)
 
     def search_actors(self, term: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Find actors matching search criteria."""
-        return _search_actors(self.service, self.headers, term, limit, cursor)
+        return _search_actors(self.call, term, limit, cursor)
 
     def get_profiles(self, actors: list[str]) -> bytes:
         """"""
-        return _get_profiles(self.service, self.headers, actors)
+        return _get_profiles(self.call, actors)
 
     def get_preferences(self) -> bytes:
         """Get private preferences attached to the account."""
-        return _get_preferences(self.service, self.headers)
+        return _get_preferences(self.call)
```

### Comparing `chitose-0.0.6/chitose/app/bsky/actor/defs.py` & `chitose-0.0.7/chitose/app/bsky/actor/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/actor/profile.py` & `chitose-0.0.7/chitose/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/embed/external.py` & `chitose-0.0.7/chitose/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/embed/images.py` & `chitose-0.0.7/chitose/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/embed/record.py` & `chitose-0.0.7/chitose/app/bsky/embed/record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/embed/record_with_media.py` & `chitose-0.0.7/chitose/app/bsky/embed/record_with_media.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/feed/__init__.py` & `chitose-0.0.7/chitose/app/bsky/feed/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from chitose.xrpc import XrpcCallable
 from .describe_feed_generator import _describe_feed_generator
 from .get_actor_feeds import _get_actor_feeds
 from .get_author_feed import _get_author_feed
 from .get_feed import _get_feed
 from .get_feed_generator import _get_feed_generator
 from .get_feed_generators import _get_feed_generators
 from .get_feed_skeleton import _get_feed_skeleton
@@ -14,58 +15,57 @@
 from .get_timeline import _get_timeline
 import chitose.app.bsky.actor.defs
 import typing
 
 class Feed_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     def get_feed_generators(self, feeds: list[str]) -> bytes:
         """Get information about a list of feed generators"""
-        return _get_feed_generators(self.service, self.headers, feeds)
+        return _get_feed_generators(self.call, feeds)
 
     def get_timeline(self, algorithm: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A view of the user's home timeline."""
-        return _get_timeline(self.service, self.headers, algorithm, limit, cursor)
+        return _get_timeline(self.call, algorithm, limit, cursor)
 
     def get_feed_generator(self, feed: str) -> bytes:
         """Get information about a specific feed offered by a feed generator, such as its online status"""
-        return _get_feed_generator(self.service, self.headers, feed)
+        return _get_feed_generator(self.call, feed)
 
     def get_author_feed(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A view of an actor's feed."""
-        return _get_author_feed(self.service, self.headers, actor, limit, cursor)
+        return _get_author_feed(self.call, actor, limit, cursor)
 
     def get_likes(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """"""
-        return _get_likes(self.service, self.headers, uri, cid, limit, cursor)
+        return _get_likes(self.call, uri, cid, limit, cursor)
 
-    def get_post_thread(self, uri: str, depth: typing.Optional[int]=None) -> bytes:
+    def get_post_thread(self, uri: str, depth: typing.Optional[int]=None, parent_height: typing.Optional[int]=None) -> bytes:
         """"""
-        return _get_post_thread(self.service, self.headers, uri, depth)
+        return _get_post_thread(self.call, uri, depth, parent_height)
 
     def get_reposted_by(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """"""
-        return _get_reposted_by(self.service, self.headers, uri, cid, limit, cursor)
+        return _get_reposted_by(self.call, uri, cid, limit, cursor)
 
     def describe_feed_generator(self) -> bytes:
         """Returns information about a given feed generator including TOS & offered feed URIs"""
-        return _describe_feed_generator(self.service, self.headers)
+        return _describe_feed_generator(self.call)
 
     def get_posts(self, uris: list[str]) -> bytes:
         """A view of an actor's feed."""
-        return _get_posts(self.service, self.headers, uris)
+        return _get_posts(self.call, uris)
 
     def get_feed(self, feed: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Compose and hydrate a feed from a user's selected feed generator"""
-        return _get_feed(self.service, self.headers, feed, limit, cursor)
+        return _get_feed(self.call, feed, limit, cursor)
 
     def get_feed_skeleton(self, feed: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A skeleton of a feed provided by a feed generator"""
-        return _get_feed_skeleton(self.service, self.headers, feed, limit, cursor)
+        return _get_feed_skeleton(self.call, feed, limit, cursor)
 
     def get_actor_feeds(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Retrieve a list of feeds created by a given actor"""
-        return _get_actor_feeds(self.service, self.headers, actor, limit, cursor)
+        return _get_actor_feeds(self.call, actor, limit, cursor)
```

### Comparing `chitose-0.0.6/chitose/app/bsky/feed/defs.py` & `chitose-0.0.7/chitose/app/bsky/feed/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/feed/describe_feed_generator.py` & `chitose-0.0.7/chitose/app/bsky/feed/describe_feed_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _describe_feed_generator(service: str, headers: dict[str, str]) -> bytes:
+def _describe_feed_generator(call: chitose.xrpc.XrpcCallable) -> bytes:
     """Returns information about a given feed generator including TOS & offered feed URIs"""
-    return chitose.xrpc.call('app.bsky.feed.describeFeedGenerator', [], None, service, {} | headers)
+    return call('app.bsky.feed.describeFeedGenerator', [], None, {})
 
 class Feed(chitose.Object):
     """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
```

### Comparing `chitose-0.0.6/chitose/app/bsky/feed/generator.py` & `chitose-0.0.7/chitose/app/bsky/feed/generator.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/feed/get_likes.py` & `chitose-0.0.7/chitose/app/bsky/feed/get_likes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import typing
 
-def _get_likes(service: str, headers: dict[str, str], uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _get_likes(call: chitose.xrpc.XrpcCallable, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """"""
-    return chitose.xrpc.call('app.bsky.feed.getLikes', [('uri', uri), ('cid', cid), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
+    return call('app.bsky.feed.getLikes', [('uri', uri), ('cid', cid), ('limit', limit), ('cursor', cursor)], None, {})
 
 class Like(chitose.Object):
     """"""
 
     def __init__(self, indexed_at: str, created_at: str, actor: chitose.app.bsky.actor.defs.ProfileView) -> None:
         self.indexed_at = indexed_at
         self.created_at = created_at
```

### Comparing `chitose-0.0.6/chitose/app/bsky/feed/post.py` & `chitose-0.0.7/chitose/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/graph/__init__.py` & `chitose-0.0.7/chitose/app/bsky/graph/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from chitose.xrpc import XrpcCallable
 from .get_blocks import _get_blocks
 from .get_followers import _get_followers
 from .get_follows import _get_follows
 from .get_list import _get_list
 from .get_list_mutes import _get_list_mutes
 from .get_lists import _get_lists
 from .get_mutes import _get_mutes
@@ -12,54 +13,53 @@
 from .unmute_actor import _unmute_actor
 from .unmute_actor_list import _unmute_actor_list
 import typing
 
 class Graph_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     def unmute_actor_list(self, list: str) -> bytes:
         """Unmute a list of actors."""
-        return _unmute_actor_list(self.service, self.headers, list)
+        return _unmute_actor_list(self.call, list)
 
     def mute_actor_list(self, list: str) -> bytes:
         """Mute a list of actors."""
-        return _mute_actor_list(self.service, self.headers, list)
+        return _mute_actor_list(self.call, list)
 
     def get_lists(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Fetch a list of lists that belong to an actor"""
-        return _get_lists(self.service, self.headers, actor, limit, cursor)
+        return _get_lists(self.call, actor, limit, cursor)
 
     def get_followers(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is following an actor?"""
-        return _get_followers(self.service, self.headers, actor, limit, cursor)
+        return _get_followers(self.call, actor, limit, cursor)
 
     def mute_actor(self, actor: str) -> bytes:
         """Mute an actor by did or handle."""
-        return _mute_actor(self.service, self.headers, actor)
+        return _mute_actor(self.call, actor)
 
     def get_mutes(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who does the viewer mute?"""
-        return _get_mutes(self.service, self.headers, limit, cursor)
+        return _get_mutes(self.call, limit, cursor)
 
     def get_list_mutes(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Which lists is the requester's account muting?"""
-        return _get_list_mutes(self.service, self.headers, limit, cursor)
+        return _get_list_mutes(self.call, limit, cursor)
 
     def get_follows(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is an actor following?"""
-        return _get_follows(self.service, self.headers, actor, limit, cursor)
+        return _get_follows(self.call, actor, limit, cursor)
 
     def get_blocks(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is the requester's account blocking?"""
-        return _get_blocks(self.service, self.headers, limit, cursor)
+        return _get_blocks(self.call, limit, cursor)
 
     def unmute_actor(self, actor: str) -> bytes:
         """Unmute an actor by did or handle."""
-        return _unmute_actor(self.service, self.headers, actor)
+        return _unmute_actor(self.call, actor)
 
     def get_list(self, list: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Fetch a list of actors"""
-        return _get_list(self.service, self.headers, list, limit, cursor)
+        return _get_list(self.call, list, limit, cursor)
```

### Comparing `chitose-0.0.6/chitose/app/bsky/graph/defs.py` & `chitose-0.0.7/chitose/app/bsky/graph/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import chitose.app.bsky.graph.defs
 import chitose.app.bsky.richtext.facet
 import typing
 
 class ListViewBasic(chitose.Object):
     """"""
 
-    def __init__(self, uri: str, name: str, purpose: chitose.app.bsky.graph.defs.ListPurpose, avatar: typing.Optional[str], viewer: typing.Optional[chitose.app.bsky.graph.defs.ListViewerState]=None, indexed_at: typing.Optional[str]=None) -> None:
+    def __init__(self, uri: str, name: str, purpose: chitose.app.bsky.graph.defs.ListPurpose, avatar: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.graph.defs.ListViewerState]=None, indexed_at: typing.Optional[str]=None) -> None:
         self.uri = uri
         self.name = name
         self.purpose = purpose
         self.avatar = avatar
         self.viewer = viewer
         self.indexed_at = indexed_at
```

### Comparing `chitose-0.0.6/chitose/app/bsky/graph/list.py` & `chitose-0.0.7/chitose/app/bsky/graph/list.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/app/bsky/notification/list_notifications.py` & `chitose-0.0.7/chitose/app/bsky/notification/list_notifications.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 """"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.com.atproto.label.defs
 import typing
 
-def _list_notifications(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None) -> bytes:
+def _list_notifications(call: chitose.xrpc.XrpcCallable, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None) -> bytes:
     """"""
-    return chitose.xrpc.call('app.bsky.notification.listNotifications', [('limit', limit), ('cursor', cursor), ('seenAt', seen_at)], None, service, {} | headers)
+    return call('app.bsky.notification.listNotifications', [('limit', limit), ('cursor', cursor), ('seenAt', seen_at)], None, {})
 
 class Notification(chitose.Object):
     """
 
 
     :param reason: Expected values are 'like', 'repost', 'follow', 'mention', 'reply', and 'quote'.
     """
```

### Comparing `chitose-0.0.6/chitose/app/bsky/richtext/facet.py` & `chitose-0.0.7/chitose/app/bsky/richtext/facet.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/com/atproto/admin/defs.py` & `chitose-0.0.7/chitose/com/atproto/admin/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/com/atproto/admin/get_moderation_reports.py` & `chitose-0.0.7/chitose/com/atproto/admin/get_moderation_reports.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _get_moderation_reports(call: chitose.xrpc.XrpcCallable, subject: typing.Optional[str]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """List moderation reports related to a subject."""
-    return chitose.xrpc.call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
+    return call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor)], None, {})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/admin/take_moderation_action.py` & `chitose-0.0.7/chitose/com/atproto/admin/take_moderation_action.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
-def _take_moderation_action(service: str, headers: dict[str, str], action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
+def _take_moderation_action(call: chitose.xrpc.XrpcCallable, action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
     """Take a moderation action on a repo."""
-    return chitose.xrpc.call('com.atproto.admin.takeModerationAction', [], {'action': action, 'subject': subject, 'subjectBlobCids': subject_blob_cids, 'createLabelVals': create_label_vals, 'negateLabelVals': negate_label_vals, 'reason': reason, 'createdBy': created_by}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.admin.takeModerationAction', [], {'action': action, 'subject': subject, 'subjectBlobCids': subject_blob_cids, 'createLabelVals': create_label_vals, 'negateLabelVals': negate_label_vals, 'reason': reason, 'createdBy': created_by}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/identity/__init__.py` & `chitose-0.0.7/chitose/com/atproto/identity/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from chitose.xrpc import XrpcCallable
 from .resolve_handle import _resolve_handle
 from .update_handle import _update_handle
-import typing
 
 class Identity_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     def update_handle(self, handle: str) -> bytes:
         """Updates the handle of the account"""
-        return _update_handle(self.service, self.headers, handle)
+        return _update_handle(self.call, handle)
 
-    def resolve_handle(self, handle: typing.Optional[str]=None) -> bytes:
+    def resolve_handle(self, handle: str) -> bytes:
         """Provides the DID of a repo.
 
 
-        :param handle: The handle to resolve. If not supplied, will resolve the host's own handle.
+        :param handle: The handle to resolve.
         """
-        return _resolve_handle(self.service, self.headers, handle)
+        return _resolve_handle(self.call, handle)
```

### Comparing `chitose-0.0.6/chitose/com/atproto/label/defs.py` & `chitose-0.0.7/chitose/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/com/atproto/label/query_labels.py` & `chitose-0.0.7/chitose/com/atproto/label/query_labels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _query_labels(service: str, headers: dict[str, str], uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _query_labels(call: chitose.xrpc.XrpcCallable, uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """Find labels relevant to the provided URI patterns.
 
 
     :param uri_patterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI
 
     :param sources: Optional list of label sources (DIDs) to filter on
     """
-    return chitose.xrpc.call('com.atproto.label.queryLabels', [('uriPatterns', uri_patterns), ('sources', sources), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
+    return call('com.atproto.label.queryLabels', [('uriPatterns', uri_patterns), ('sources', sources), ('limit', limit), ('cursor', cursor)], None, {})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/label/subscribe_labels.py` & `chitose-0.0.7/chitose/com/atproto/label/subscribe_labels.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/com/atproto/moderation/__init__.py` & `chitose-0.0.7/chitose/com/atproto/moderation/create_report.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
-from .create_report import _create_report
+import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.moderation.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
-class Moderation_:
-    """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
-
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
-
-    def create_report(self, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None) -> bytes:
-        """Report a repo or a record."""
-        return _create_report(self.service, self.headers, reason_type, subject, reason)
+def _create_report(call: chitose.xrpc.XrpcCallable, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None) -> bytes:
+    """Report a repo or a record."""
+    return call('com.atproto.moderation.createReport', [], {'reasonType': reason_type, 'reason': reason, 'subject': subject}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/moderation/defs.py` & `chitose-0.0.7/chitose/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/com/atproto/repo/__init__.py` & `chitose-0.0.7/chitose/com/atproto/repo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from chitose.xrpc import XrpcCallable
 from .apply_writes import _apply_writes
 from .create_record import _create_record
 from .delete_record import _delete_record
 from .describe_repo import _describe_repo
 from .get_record import _get_record
 from .list_records import _list_records
 from .put_record import _put_record
@@ -11,17 +12,16 @@
 from .upload_blob import _upload_blob
 import chitose.com.atproto.repo.apply_writes
 import typing
 
 class Repo_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     def create_record(self, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Create a new record.
 
 
         :param repo: The handle or DID of the repo.
 
@@ -31,15 +31,15 @@
 
         :param rkey: The key of the record.
 
         :param validate: Validate the record?
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
-        return _create_record(self.service, self.headers, repo, collection, record, rkey, validate, swap_commit)
+        return _create_record(self.call, repo, collection, record, rkey, validate, swap_commit)
 
     def delete_record(self, repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Delete a record, or ensure it doesn't exist.
 
 
         :param repo: The handle or DID of the repo.
 
@@ -47,15 +47,15 @@
 
         :param rkey: The key of the record.
 
         :param swap_record: Compare and swap with the previous record by cid.
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
-        return _delete_record(self.service, self.headers, repo, collection, rkey, swap_record, swap_commit)
+        return _delete_record(self.call, repo, collection, rkey, swap_record, swap_commit)
 
     def put_record(self, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[bool]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Write a record, creating or updating it as needed.
 
 
         :param repo: The handle or DID of the repo.
 
@@ -67,61 +67,61 @@
 
         :param validate: Validate the record?
 
         :param swap_record: Compare and swap with the previous record by cid.
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
-        return _put_record(self.service, self.headers, repo, collection, rkey, record, validate, swap_record, swap_commit)
+        return _put_record(self.call, repo, collection, rkey, record, validate, swap_record, swap_commit)
 
     def rebase_repo(self, repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
         """Simple rebase of repo that deletes history
 
 
         :param repo: The handle or DID of the repo.
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
-        return _rebase_repo(self.service, self.headers, repo, swap_commit)
+        return _rebase_repo(self.call, repo, swap_commit)
 
     def upload_blob(self, input_: bytes) -> bytes:
         """Upload a new blob to be added to repo in a later request."""
-        return _upload_blob(self.service, self.headers, input_)
+        return _upload_blob(self.call, input_)
 
     def describe_repo(self, repo: str) -> bytes:
         """Get information about the repo, including the list of collections.
 
 
         :param repo: The handle or DID of the repo.
         """
-        return _describe_repo(self.service, self.headers, repo)
+        return _describe_repo(self.call, repo)
 
     def get_record(self, repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None) -> bytes:
         """Get a record.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record collection.
 
         :param rkey: The key of the record.
 
         :param cid: The CID of the version of the record. If not specified, then return the most recent version.
         """
-        return _get_record(self.service, self.headers, repo, collection, rkey, cid)
+        return _get_record(self.call, repo, collection, rkey, cid)
 
     def apply_writes(self, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Apply a batch transaction of creates, updates, and deletes.
 
 
         :param repo: The handle or DID of the repo.
 
         :param validate: Validate the records?
         """
-        return _apply_writes(self.service, self.headers, repo, writes, validate, swap_commit)
+        return _apply_writes(self.call, repo, writes, validate, swap_commit)
 
     def list_records(self, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
         """List a range of records in a collection.
 
 
         :param repo: The handle or DID of the repo.
 
@@ -131,8 +131,8 @@
 
         :param rkey_start: DEPRECATED: The lowest sort-ordered rkey to start from (exclusive)
 
         :param rkey_end: DEPRECATED: The highest sort-ordered rkey to stop at (exclusive)
 
         :param reverse: Reverse the order of the returned records?
         """
-        return _list_records(self.service, self.headers, repo, collection, limit, cursor, rkey_start, rkey_end, reverse)
+        return _list_records(self.call, repo, collection, limit, cursor, rkey_start, rkey_end, reverse)
```

### Comparing `chitose-0.0.6/chitose/com/atproto/repo/apply_writes.py` & `chitose-0.0.7/chitose/com/atproto/repo/apply_writes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.repo.apply_writes
 import typing
 
-def _apply_writes(service: str, headers: dict[str, str], repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _apply_writes(call: chitose.xrpc.XrpcCallable, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Apply a batch transaction of creates, updates, and deletes.
 
 
     :param repo: The handle or DID of the repo.
 
     :param validate: Validate the records?
     """
-    return chitose.xrpc.call('com.atproto.repo.applyWrites', [], {'repo': repo, 'validate': validate, 'writes': writes, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.repo.applyWrites', [], {'repo': repo, 'validate': validate, 'writes': writes, 'swapCommit': swap_commit}, {'Content-Type': 'application/json'})
 
 class Create(chitose.Object):
     """"""
 
-    def __init__(self, collection: str, value: typing.Any, rkey: typing.Optional[str]) -> None:
+    def __init__(self, collection: str, value: typing.Any, rkey: typing.Optional[str]=None) -> None:
         self.collection = collection
         self.value = value
         self.rkey = rkey
 
     def to_dict(self) -> dict:
         return {'collection': self.collection, 'value': self.value, 'rkey': self.rkey, '$type': 'com.atproto.repo.applyWrites#create'}
```

### Comparing `chitose-0.0.6/chitose/com/atproto/repo/create_record.py` & `chitose-0.0.7/chitose/com/atproto/repo/put_record.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_record(service: str, headers: dict[str, str], repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
-    """Create a new record.
+def _put_record(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[bool]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+    """Write a record, creating or updating it as needed.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
 
-    :param record: The record to create.
-
     :param rkey: The key of the record.
 
+    :param record: The record to write.
+
     :param validate: Validate the record?
 
+    :param swap_record: Compare and swap with the previous record by cid.
+
     :param swap_commit: Compare and swap with the previous commit by cid.
     """
-    return chitose.xrpc.call('com.atproto.repo.createRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'validate': validate, 'record': record, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.repo.putRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'validate': validate, 'record': record, 'swapRecord': swap_record, 'swapCommit': swap_commit}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/repo/delete_record.py` & `chitose-0.0.7/chitose/com/atproto/repo/delete_record.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _delete_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _delete_record(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Delete a record, or ensure it doesn't exist.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
 
     :param rkey: The key of the record.
 
     :param swap_record: Compare and swap with the previous record by cid.
 
     :param swap_commit: Compare and swap with the previous commit by cid.
     """
-    return chitose.xrpc.call('com.atproto.repo.deleteRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'swapRecord': swap_record, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.repo.deleteRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'swapRecord': swap_record, 'swapCommit': swap_commit}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/repo/get_record.py` & `chitose-0.0.7/chitose/com/atproto/repo/get_record.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None) -> bytes:
+def _get_record(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None) -> bytes:
     """Get a record.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
 
     :param rkey: The key of the record.
 
     :param cid: The CID of the version of the record. If not specified, then return the most recent version.
     """
-    return chitose.xrpc.call('com.atproto.repo.getRecord', [('repo', repo), ('collection', collection), ('rkey', rkey), ('cid', cid)], None, service, {} | headers)
+    return call('com.atproto.repo.getRecord', [('repo', repo), ('collection', collection), ('rkey', rkey), ('cid', cid)], None, {})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/repo/list_records.py` & `chitose-0.0.7/chitose/com/atproto/repo/list_records.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_records(service: str, headers: dict[str, str], repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
+def _list_records(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
     """List a range of records in a collection.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record type.
 
@@ -16,15 +16,15 @@
 
     :param rkey_start: DEPRECATED: The lowest sort-ordered rkey to start from (exclusive)
 
     :param rkey_end: DEPRECATED: The highest sort-ordered rkey to stop at (exclusive)
 
     :param reverse: Reverse the order of the returned records?
     """
-    return chitose.xrpc.call('com.atproto.repo.listRecords', [('repo', repo), ('collection', collection), ('limit', limit), ('cursor', cursor), ('rkeyStart', rkey_start), ('rkeyEnd', rkey_end), ('reverse', reverse)], None, service, {} | headers)
+    return call('com.atproto.repo.listRecords', [('repo', repo), ('collection', collection), ('limit', limit), ('cursor', cursor), ('rkeyStart', rkey_start), ('rkeyEnd', rkey_end), ('reverse', reverse)], None, {})
 
 class Record(chitose.Object):
     """"""
 
     def __init__(self, uri: str, cid: str, value: typing.Any) -> None:
         self.uri = uri
         self.cid = cid
```

### Comparing `chitose-0.0.6/chitose/com/atproto/repo/rebase_repo.py` & `chitose-0.0.7/chitose/com/atproto/repo/rebase_repo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _rebase_repo(service: str, headers: dict[str, str], repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
+def _rebase_repo(call: chitose.xrpc.XrpcCallable, repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
     """Simple rebase of repo that deletes history
 
 
     :param repo: The handle or DID of the repo.
 
     :param swap_commit: Compare and swap with the previous commit by cid.
     """
-    return chitose.xrpc.call('com.atproto.repo.rebaseRepo', [], {'repo': repo, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.repo.rebaseRepo', [], {'repo': repo, 'swapCommit': swap_commit}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/server/__init__.py` & `chitose-0.0.7/chitose/com/atproto/server/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from chitose.xrpc import XrpcCallable
 from .create_account import _create_account
 from .create_app_password import _create_app_password
 from .create_invite_code import _create_invite_code
 from .create_invite_codes import _create_invite_codes
 from .create_session import _create_session
 from .delete_account import _delete_account
 from .delete_session import _delete_session
@@ -17,78 +18,77 @@
 from .reset_password import _reset_password
 from .revoke_app_password import _revoke_app_password
 import typing
 
 class Server_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     def get_account_invite_codes(self, include_used: typing.Optional[bool]=None, create_available: typing.Optional[bool]=None) -> bytes:
         """Get all invite codes for a given account"""
-        return _get_account_invite_codes(self.service, self.headers, include_used, create_available)
+        return _get_account_invite_codes(self.call, include_used, create_available)
 
     def create_session(self, identifier: str, password: str) -> bytes:
         """Create an authentication session.
 
 
         :param identifier: Handle or other identifier supported by the server for the authenticating user.
         """
-        return _create_session(self.service, self.headers, identifier, password)
+        return _create_session(self.call, identifier, password)
 
     def list_app_passwords(self) -> bytes:
         """List all app-specific passwords."""
-        return _list_app_passwords(self.service, self.headers)
+        return _list_app_passwords(self.call)
 
     def create_invite_codes(self, code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
         """Create an invite code."""
-        return _create_invite_codes(self.service, self.headers, code_count, use_count, for_accounts)
+        return _create_invite_codes(self.call, code_count, use_count, for_accounts)
 
     def delete_session(self) -> bytes:
         """Delete the current session."""
-        return _delete_session(self.service, self.headers)
+        return _delete_session(self.call)
 
     def revoke_app_password(self, name: str) -> bytes:
         """Revoke an app-specific password by name."""
-        return _revoke_app_password(self.service, self.headers, name)
+        return _revoke_app_password(self.call, name)
 
     def create_app_password(self, name: str) -> bytes:
         """Create an app-specific password."""
-        return _create_app_password(self.service, self.headers, name)
+        return _create_app_password(self.call, name)
 
     def describe_server(self) -> bytes:
         """Get a document describing the service's accounts configuration."""
-        return _describe_server(self.service, self.headers)
+        return _describe_server(self.call)
 
     def get_session(self) -> bytes:
         """Get information about the current session."""
-        return _get_session(self.service, self.headers)
+        return _get_session(self.call)
 
     def refresh_session(self) -> bytes:
         """Refresh an authentication session."""
-        return _refresh_session(self.service, self.headers)
+        return _refresh_session(self.call)
 
     def reset_password(self, token: str, password: str) -> bytes:
         """Reset a user account password using a token."""
-        return _reset_password(self.service, self.headers, token, password)
+        return _reset_password(self.call, token, password)
 
     def request_password_reset(self, email: str) -> bytes:
         """Initiate a user account password reset via email."""
-        return _request_password_reset(self.service, self.headers, email)
+        return _request_password_reset(self.call, email)
 
     def request_account_delete(self) -> bytes:
         """Initiate a user account deletion via email."""
-        return _request_account_delete(self.service, self.headers)
+        return _request_account_delete(self.call)
 
     def create_account(self, email: str, handle: str, password: str, did: typing.Optional[str]=None, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
         """Create an account."""
-        return _create_account(self.service, self.headers, email, handle, password, did, invite_code, recovery_key)
+        return _create_account(self.call, email, handle, password, did, invite_code, recovery_key)
 
     def delete_account(self, did: str, password: str, token: str) -> bytes:
         """Delete a user account with a token and password."""
-        return _delete_account(self.service, self.headers, did, password, token)
+        return _delete_account(self.call, did, password, token)
 
     def create_invite_code(self, use_count: int, for_account: typing.Optional[str]=None) -> bytes:
         """Create an invite code."""
-        return _create_invite_code(self.service, self.headers, use_count, for_account)
+        return _create_invite_code(self.call, use_count, for_account)
```

### Comparing `chitose-0.0.6/chitose/com/atproto/server/create_account.py` & `chitose-0.0.7/chitose/com/atproto/server/create_account.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_account(service: str, headers: dict[str, str], email: str, handle: str, password: str, did: typing.Optional[str]=None, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
+def _create_account(call: chitose.xrpc.XrpcCallable, email: str, handle: str, password: str, did: typing.Optional[str]=None, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
     """Create an account."""
-    return chitose.xrpc.call('com.atproto.server.createAccount', [], {'email': email, 'handle': handle, 'did': did, 'inviteCode': invite_code, 'password': password, 'recoveryKey': recovery_key}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.server.createAccount', [], {'email': email, 'handle': handle, 'did': did, 'inviteCode': invite_code, 'password': password, 'recoveryKey': recovery_key}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/server/create_app_password.py` & `chitose-0.0.7/chitose/com/atproto/server/create_app_password.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 
-def _create_app_password(service: str, headers: dict[str, str], name: str) -> bytes:
+def _create_app_password(call: chitose.xrpc.XrpcCallable, name: str) -> bytes:
     """Create an app-specific password."""
-    return chitose.xrpc.call('com.atproto.server.createAppPassword', [], {'name': name}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.server.createAppPassword', [], {'name': name}, {'Content-Type': 'application/json'})
 
 class AppPassword(chitose.Object):
     """"""
 
     def __init__(self, name: str, password: str, created_at: str) -> None:
         self.name = name
         self.password = password
```

### Comparing `chitose-0.0.6/chitose/com/atproto/server/create_invite_codes.py` & `chitose-0.0.7/chitose/com/atproto/server/create_invite_codes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_invite_codes(service: str, headers: dict[str, str], code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
+def _create_invite_codes(call: chitose.xrpc.XrpcCallable, code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
     """Create an invite code."""
-    return chitose.xrpc.call('com.atproto.server.createInviteCodes', [], {'codeCount': code_count, 'useCount': use_count, 'forAccounts': for_accounts}, service, {'Content-Type': 'application/json'} | headers)
+    return call('com.atproto.server.createInviteCodes', [], {'codeCount': code_count, 'useCount': use_count, 'forAccounts': for_accounts}, {'Content-Type': 'application/json'})
 
 class AccountCodes(chitose.Object):
     """"""
 
     def __init__(self, account: str, codes: list[str]) -> None:
         self.account = account
         self.codes = codes
```

### Comparing `chitose-0.0.6/chitose/com/atproto/server/defs.py` & `chitose-0.0.7/chitose/com/atproto/server/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/com/atproto/server/describe_server.py` & `chitose-0.0.7/chitose/com/atproto/server/describe_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _describe_server(service: str, headers: dict[str, str]) -> bytes:
+def _describe_server(call: chitose.xrpc.XrpcCallable) -> bytes:
     """Get a document describing the service's accounts configuration."""
-    return chitose.xrpc.call('com.atproto.server.describeServer', [], None, service, {} | headers)
+    return call('com.atproto.server.describeServer', [], None, {})
 
 class Links(chitose.Object):
     """"""
 
     def __init__(self, privacy_policy: typing.Optional[str]=None, terms_of_service: typing.Optional[str]=None) -> None:
         self.privacy_policy = privacy_policy
         self.terms_of_service = terms_of_service
```

### Comparing `chitose-0.0.6/chitose/com/atproto/sync/__init__.py` & `chitose-0.0.7/chitose/com/atproto/sync/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from chitose.xrpc import XrpcCallable
 from .get_blob import _get_blob
 from .get_blocks import _get_blocks
 from .get_checkout import _get_checkout
 from .get_commit_path import _get_commit_path
 from .get_head import _get_head
 from .get_record import _get_record
 from .get_repo import _get_repo
@@ -12,112 +13,111 @@
 from .notify_of_update import _notify_of_update
 from .request_crawl import _request_crawl
 import typing
 
 class Sync_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]) -> None:
-        self.service = service
-        self.headers = headers
+    def __init__(self, call: XrpcCallable) -> None:
+        self.call = call
 
     def get_head(self, did: str) -> bytes:
         """Gets the current HEAD CID of a repo.
 
 
         :param did: The DID of the repo.
         """
-        return _get_head(self.service, self.headers, did)
+        return _get_head(self.call, did)
 
     def get_blob(self, did: str, cid: str) -> bytes:
         """Get a blob associated with a given repo.
 
 
         :param did: The DID of the repo.
 
         :param cid: The CID of the blob to fetch
         """
-        return _get_blob(self.service, self.headers, did, cid)
+        return _get_blob(self.call, did, cid)
 
     def get_repo(self, did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None) -> bytes:
         """Gets the repo state.
 
 
         :param did: The DID of the repo.
 
         :param earliest: The earliest commit in the commit range (not inclusive)
 
         :param latest: The latest commit in the commit range (inclusive)
         """
-        return _get_repo(self.service, self.headers, did, earliest, latest)
+        return _get_repo(self.call, did, earliest, latest)
 
     def notify_of_update(self, hostname: str) -> bytes:
         """Notify a crawling service of a recent update. Often when a long break between updates causes the connection with the crawling service to break.
 
 
         :param hostname: Hostname of the service that is notifying of update.
         """
-        return _notify_of_update(self.service, self.headers, hostname)
+        return _notify_of_update(self.call, hostname)
 
     def request_crawl(self, hostname: str) -> bytes:
         """Request a service to persistently crawl hosted repos.
 
 
         :param hostname: Hostname of the service that is requesting to be crawled.
         """
-        return _request_crawl(self.service, self.headers, hostname)
+        return _request_crawl(self.call, hostname)
 
     def list_blobs(self, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
         """List blob cids for some range of commits
 
 
         :param did: The DID of the repo.
 
         :param latest: The most recent commit
 
         :param earliest: The earliest commit to start from
         """
-        return _list_blobs(self.service, self.headers, did, latest, earliest)
+        return _list_blobs(self.call, did, latest, earliest)
 
     def get_record(self, did: str, collection: str, rkey: str, commit: typing.Optional[str]=None) -> bytes:
         """Gets blocks needed for existence or non-existence of record.
 
 
         :param did: The DID of the repo.
 
         :param commit: An optional past commit CID.
         """
-        return _get_record(self.service, self.headers, did, collection, rkey, commit)
+        return _get_record(self.call, did, collection, rkey, commit)
 
     def list_repos(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """List dids and root cids of hosted repos"""
-        return _list_repos(self.service, self.headers, limit, cursor)
+        return _list_repos(self.call, limit, cursor)
 
     def get_commit_path(self, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
         """Gets the path of repo commits
 
 
         :param did: The DID of the repo.
 
         :param latest: The most recent commit
 
         :param earliest: The earliest commit to start from
         """
-        return _get_commit_path(self.service, self.headers, did, latest, earliest)
+        return _get_commit_path(self.call, did, latest, earliest)
 
     def get_blocks(self, did: str, cids: list[str]) -> bytes:
         """Gets blocks from a given repo.
 
 
         :param did: The DID of the repo.
         """
-        return _get_blocks(self.service, self.headers, did, cids)
+        return _get_blocks(self.call, did, cids)
 
     def get_checkout(self, did: str, commit: typing.Optional[str]=None) -> bytes:
         """Gets the repo state.
 
 
         :param did: The DID of the repo.
 
         :param commit: The commit to get the checkout from. Defaults to current HEAD.
         """
-        return _get_checkout(self.service, self.headers, did, commit)
+        return _get_checkout(self.call, did, commit)
```

### Comparing `chitose-0.0.6/chitose/com/atproto/sync/get_commit_path.py` & `chitose-0.0.7/chitose/com/atproto/sync/list_blobs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_commit_path(service: str, headers: dict[str, str], did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
-    """Gets the path of repo commits
+def _list_blobs(call: chitose.xrpc.XrpcCallable, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
+    """List blob cids for some range of commits
 
 
     :param did: The DID of the repo.
 
     :param latest: The most recent commit
 
     :param earliest: The earliest commit to start from
     """
-    return chitose.xrpc.call('com.atproto.sync.getCommitPath', [('did', did), ('latest', latest), ('earliest', earliest)], None, service, {} | headers)
+    return call('com.atproto.sync.listBlobs', [('did', did), ('latest', latest), ('earliest', earliest)], None, {})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/sync/get_record.py` & `chitose-0.0.7/chitose/com/atproto/sync/get_record.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_record(service: str, headers: dict[str, str], did: str, collection: str, rkey: str, commit: typing.Optional[str]=None) -> bytes:
+def _get_record(call: chitose.xrpc.XrpcCallable, did: str, collection: str, rkey: str, commit: typing.Optional[str]=None) -> bytes:
     """Gets blocks needed for existence or non-existence of record.
 
 
     :param did: The DID of the repo.
 
     :param commit: An optional past commit CID.
     """
-    return chitose.xrpc.call('com.atproto.sync.getRecord', [('did', did), ('collection', collection), ('rkey', rkey), ('commit', commit)], None, service, {} | headers)
+    return call('com.atproto.sync.getRecord', [('did', did), ('collection', collection), ('rkey', rkey), ('commit', commit)], None, {})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/sync/get_repo.py` & `chitose-0.0.7/chitose/com/atproto/sync/get_repo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_repo(service: str, headers: dict[str, str], did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None) -> bytes:
+def _get_repo(call: chitose.xrpc.XrpcCallable, did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None) -> bytes:
     """Gets the repo state.
 
 
     :param did: The DID of the repo.
 
     :param earliest: The earliest commit in the commit range (not inclusive)
 
     :param latest: The latest commit in the commit range (inclusive)
     """
-    return chitose.xrpc.call('com.atproto.sync.getRepo', [('did', did), ('earliest', earliest), ('latest', latest)], None, service, {} | headers)
+    return call('com.atproto.sync.getRepo', [('did', did), ('earliest', earliest), ('latest', latest)], None, {})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/sync/list_blobs.py` & `chitose-0.0.7/chitose/com/atproto/sync/get_commit_path.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_blobs(service: str, headers: dict[str, str], did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
-    """List blob cids for some range of commits
+def _get_commit_path(call: chitose.xrpc.XrpcCallable, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
+    """Gets the path of repo commits
 
 
     :param did: The DID of the repo.
 
     :param latest: The most recent commit
 
     :param earliest: The earliest commit to start from
     """
-    return chitose.xrpc.call('com.atproto.sync.listBlobs', [('did', did), ('latest', latest), ('earliest', earliest)], None, service, {} | headers)
+    return call('com.atproto.sync.getCommitPath', [('did', did), ('latest', latest), ('earliest', earliest)], None, {})
```

### Comparing `chitose-0.0.6/chitose/com/atproto/sync/list_repos.py` & `chitose-0.0.7/chitose/com/atproto/sync/list_repos.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_repos(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _list_repos(call: chitose.xrpc.XrpcCallable, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """List dids and root cids of hosted repos"""
-    return chitose.xrpc.call('com.atproto.sync.listRepos', [('limit', limit), ('cursor', cursor)], None, service, {} | headers)
+    return call('com.atproto.sync.listRepos', [('limit', limit), ('cursor', cursor)], None, {})
 
 class Repo(chitose.Object):
     """"""
 
     def __init__(self, did: str, head: str) -> None:
         self.did = did
         self.head = head
```

### Comparing `chitose-0.0.6/chitose/com/atproto/sync/subscribe_repos.py` & `chitose-0.0.7/chitose/com/atproto/sync/subscribe_repos.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.6/chitose/xrpc.py` & `chitose-0.0.7/chitose/xrpc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+from typing import Callable
 from typing import Optional
 from typing import Union
 import json
 import urllib.parse
 import urllib.request
 
+XrpcParams = list[tuple[str, Union[str,
+                                   Optional[str], Optional[int], list[str]]]]
+XrpcData = Union[bytes, Optional[dict]]
+XrpcHeaders = dict[str, str]
+XrpcCallable = Callable[[str, XrpcParams, XrpcData, XrpcHeaders], bytes]
 
-def call(method: str,
-         params: list[tuple[str, Union[str, Optional[str],
-                                       Optional[int], list[str]]]],
-         d: Union[bytes, Optional[dict]], service: str, headers: dict[str, str]) -> bytes:
+
+def call(method: str, params: XrpcParams,
+         d: XrpcData, service: str, headers: XrpcHeaders) -> bytes:
     url = f'{service}/xrpc/{method}'
 
     query: list[tuple[str, Union[str, int]]] = []
     for key, val in params:
         if val is None:
             continue
 
@@ -38,12 +43,16 @@
                 key: val for key, val in d.items()
                 if val is not None
             }
             data = json.dumps(d, default=lambda obj: {
                               key: val for key, val in obj.to_dict().items()
                               if val is not None
                               }).encode()
-    else:
+    elif d is None:
+        # d = None => data = None
         data = None
+    else:
+        # d = {} => data = b''
+        data = b''
 
     r = urllib.request.urlopen(req, data)
     return r.read()
```

### Comparing `chitose-0.0.6/pyproject.toml` & `chitose-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chitose"
-version = "0.0.6"
+version = "0.0.7"
 description = "A client library for the AT Protocol (Bluesky) "
 license = "MIT"
 authors = [
     "Muneyuki Noguchi <nogu.dev@gmail.com>",
 ]
 readme = "README.md"
 homepage = "https://github.com/mnogu/chitose"
```

### Comparing `chitose-0.0.6/PKG-INFO` & `chitose-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitose
-Version: 0.0.6
+Version: 0.0.7
 Summary: A client library for the AT Protocol (Bluesky) 
 Home-page: https://github.com/mnogu/chitose
 License: MIT
 Author: Muneyuki Noguchi
 Author-email: nogu.dev@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
```


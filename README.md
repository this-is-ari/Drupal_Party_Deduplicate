# Drupal_Party_Deduplicate
A Drupal module to prevent the creation of duplicate parties. Enable by going to party settings (/admin/community/party/primary-fields/email) and checking "Merge Parties with the same email"


This module relies on hook_entity_update to be called in order to deduplicate - unfortunately that hook is not always called resulting in deduplication not always occuring. Need to solve this issue for this module to be useful - should look at alternatives using hook_entity_insert, hook_entity_presave, or might want to build on top of https://www.drupal.org/project/hook_post_action to fix the issue.

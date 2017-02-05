# Drupal_Party_Deduplicate
A Drupal module to prevent the creation of duplicate parties. Enable by going to party settings (/admin/community/party/primary-fields/email) and checking "Merge Parties with the same email"
There is currently a known issue with this module not firing whenever a party is created - need to diagnose why, might want to build on top of https://www.drupal.org/project/hook_post_action to fix the issue.

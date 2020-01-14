---
rank: 6
related_endpoints:
  - delete_users_id
related_guides:
  - users/deprovision/user
  - users/deprovision/transfer-folders
related_pages: []
required_guides: []
related_resources: []
alias_paths: []
category_id: users
subcategory_id: null
id: users/delete-user
type: guide
is_index: false
total_steps: 3
sibling_id: users
parent_id: users
next_page_id: users
previous_page_id: users/create-app-user
---

# Delete User

The process for deleting both app and managed users is the same. To delete a
user account, supply the user ID for the account that should be
removed.

<Samples id='delete_users_id' >

</Samples>

There are also two optional parameters that may be set when deleting a user
account:

* force: Whether the user should be deleted even if the account still has
content in it.
* notify: Whether the user will receive a notification that the account was
deleted.

<Message type='notice'>

The delete user request will fail if the user account still has content in
it. To resolve this, either
[transfer all files or folders](g://users/deprovision/transfer-folders)
to another account or use the optional `force` parameter.

</Message>
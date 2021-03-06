---
layout: "opsgenie"
page_title: "OpsGenie: opsgenie_user"
sidebar_current: "docs-opsgenie-datasource-user"
description: |-
  Gets information about a specific user within OpsGenie
---

# opsgenie\_user

Use this data source to get information about a specific user within OpsGenie.

## Example Usage

```
data "opsgenie_user" "me" {
  username = "me@cookie-monster.com"
}

resource "opsgenie_team" "test" {
  TODO: example
}
```

## Argument Reference

The following arguments are supported:

* `username` - (Required) The username (email) to use to find a user in OpsGenie.

## Attributes Reference
* `full_name` - The full name of the found user.
* `role` - The role of the found user.

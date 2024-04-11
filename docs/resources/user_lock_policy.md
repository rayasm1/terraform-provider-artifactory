---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "artifactory_user_lock_policy Resource - terraform-provider-artifactory"
subcategory: "Security"
description: |-
  Provides an Artifactory User Lock Policy resource.
---

# artifactory_user_lock_policy (Resource)

Provides an Artifactory User Lock Policy resource.

## Example Usage

```terraform
resource "artifactory_user_lock_policy" "my-user-lock-policy" {
  name = "my-user-lock-policy"
  enabled = true
  login_attempts = 10
}
```

## Argument reference

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `enabled` (Boolean) Enable User Lock Policy. Lock user after exceeding max failed login attempts.
- `login_attempts` (Number) Max failed login attempts.
- `name` (String) Name of the resource. Only used for importing.

## Import

Import is supported using the following syntax:

```shell
terraform import artifactory_user_lock_policy.my-user-lock-policy my-user-lock-policy
```
[//]: # (START/LATEST)
# Latest

## Features
  * A user-friendly description of a new feature. {issue-number}

## Fixes
 * A user-friendly description of a fix. {issue-number}

## Security
 * A user-friendly description of a security fix. {issue-number}

---

[//]: # (START/v1.0.0)
# v1.0.0

## Features:
* Option to automatically deploy 1Password Connect via the operator
* Ignore restart annotation when looking for 1Password annotations
* Release Automation
* Upgrading apiextensions.k8s.io/v1beta apiversion from the operator custom resource
* Adding configuration for auto rolling restart on deployments
* Configure Auto Restarts for a OnePasswordItem Custom Resource
* Update Connect Dependencies to latest
* Add Github action for building and testing operator
## Fixes:
* Fix spec field example for OnePasswordItem in readme
* Casing of annotations are now consistent

---

[//]: # (START/v0.0.2)
# v0.0.2

## Features:
* Items can now be accessed by either `vaults/<vault_id>/items/<item_id>` or `vaults/<vault_title>/items/<item_title>`

---

[//]: # (START/v0.0.1)

# v0.0.1

Initial 1Password Operator release

## Features
* watches for deployment creations with `onepassword` annotations and creates an associated kubernetes secret
* watches for `onepasswordsecret` crd creations and creates an associated kubernetes secrets
* watches for changes to 1Password secrets associated with kubernetes secrets and updates the kubernetes secret with changes
* restart pods when secret has been updated
* cleanup of kubernetes secrets when deployment or `onepasswordsecret` is deleted

---
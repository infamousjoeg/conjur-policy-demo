# Conjur Policy Demo

An example policy structure to be used for testing Role-Based Access Controls and policy as code within CyberArk Conjur for demonstrations and proof of concepts.

**This policy structure is for Conjur Enterprise Edition v4 ONLY.**

## Master Branch Policy

On the `master` branch is the policy that grants entitlements and members to roles, as well as establishes privilege permits to allow access to secrets using RBAC.  This policy can be loaded using the Conjur CLI.

`$ conjur policy load --as-group security_admin master-policy.yml`

## Deny-All Branch Policy

On the `deny-all` branch is the policy that denies access to all secrets within the policies.  This branch's policies may be loaded using the same means as above in the case of breach, suspected compromise, or any malicious attempt to gain access to the secrets.
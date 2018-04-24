# Conjur Policy Demo

An example policy structure to be used for testing Role-Based Access Controls and policy as code within CyberArk Conjur for demonstrations and proof of concepts.

**This policy structure is for Conjur Enterprise Edition v4 ONLY.**

## Deny All - Fail-Safe Policies

In the case of breach, suspected compromise, or any other malicious attempt to gain access to secrets, this branch may be loaded via Conjur CLI to immediately deny access to all secrets associated with this master policy.

`$ conjur policy load --as-group security_admin master-policy.yml`
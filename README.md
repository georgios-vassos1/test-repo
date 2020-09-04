# Deploy application with secrets

First, read carefully [this post!](https://maersk-analytics.atlassian.net/wiki/spaces/P/pages/813006876/Vault+access+and+manage+secrets).

Connect to [vault.maersk-digital.net!](https://vault.maersk-digital.net)

Sign in with *OIDC provider*; you can also do that through your cli tool 
with the command: 

`vault login -method=oidc`

This will prompt you to `vault.maersk-digital.net/ui/vault/secrets` where you must
be able to see an entry for each resource group that you are a member of. If the 
desired resource group does not appear you must request access from the admin. 

All in all, you should be able to view a list of directories named after
`resourcegroupname-kv/`, e.g. `dsai-kv/`, etc.

If you enter one such directory you will be able to see at least two subdirectories, one
called `kubernetes/` and the other `readable/`.




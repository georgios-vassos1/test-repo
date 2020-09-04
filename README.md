# Deploy application with secrets

Consider reading carefully this post: https://maersk-analytics.atlassian.net/wiki/spaces/P/pages/813006876/Vault+access+and+manage+secrets

Connect to vault.maersk-digital.net

Sign in with OIDC provider; you can also do that through your cli tool 
with vault login -method=oidc

This will prompt you to vault.maersk-digital.net/ui/vault/secrets where you must
be able to see an option for every resource group that you are part of. If the
desired resource group does not appear you must request access from the admin. 

All in all, you should be able to view a list of directories named after
resourcegroupname-kv/

If you enter one such directory you will be able to see two subdirectories, one
called kubernetes/ and the other readable/




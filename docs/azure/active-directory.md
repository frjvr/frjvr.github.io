# Azure Active Directory

## App Administration with Active Directory Graph

### az ad app create
```
az ad app create --display-name
                 [--app-roles]
                 [--enable-access-token-issuance {false, true}]
                 [--enable-id-token-issuance {false, true}]
                 [--end-date]
                 [--identifier-uris]
                 [--is-fallback-public-client {false, true}]
                 [--key-display-name]
                 [--key-type {AsymmetricX509Cert, Password, Symmetric}]
                 [--key-usage {Sign, Verify}]
                 [--key-value]
                 [--optional-claims]
                 [--public-client-redirect-uris]
                 [--required-resource-accesses]
                 [--sign-in-audience {AzureADMultipleOrgs, AzureADMyOrg, AzureADandPersonalMicrosoftAccount, PersonalMicrosoftAccount}]
                 [--start-date]
                 [--web-home-page-url]
                 [--web-redirect-uris]
```

### az ad app delete
```
az ad app delete --id
```

### az ad app list
```
az ad app list [--all]
               [--app-id]
               [--display-name]
               [--filter]
               [--identifier-uri]
               [--show-mine]
```

### az ad app show
```
az ad app show --id
```

### az ad app update
```
az ad app update --id
                 [--add]
                 [--app-roles]
                 [--display-name]
                 [--enable-access-token-issuance {false, true}]
                 [--enable-id-token-issuance {false, true}]
                 [--end-date]
                 [--force-string]
                 [--identifier-uris]
                 [--is-fallback-public-client {false, true}]
                 [--key-display-name]
                 [--key-type {AsymmetricX509Cert, Password, Symmetric}]
                 [--key-usage {Sign, Verify}]
                 [--key-value]
                 [--optional-claims]
                 [--public-client-redirect-uris]
                 [--remove]
                 [--required-resource-accesses]
                 [--set]
                 [--sign-in-audience {AzureADMultipleOrgs, AzureADMyOrg, AzureADandPersonalMicrosoftAccount, PersonalMicrosoftAccount}]
                 [--start-date]
                 [--web-home-page-url]
                 [--web-redirect-uris]
```

## Azure Active Directory App Credentials

### az ad app credential delete
```
az ad app credential delete --id
                            --key-id
                            [--cert]
```

### az ad app credential list
```
az ad app credential list --id
                          [--cert]
```

### az ad app credential reset
```
az ad app credential reset --id
                           [--append]
                           [--cert]
                           [--create-cert]
                           [--display-name]
                           [--end-date]
                           [--keyvault]
                           [--years]
```

## Azure Active Directory App Federated Credentials

### az ad app federated-credential create
```
az ad app federated-credential create --id
                                      --parameters
```

### az ad app federated-credential delete
```
az ad app federated-credential delete --federated-credential-id
                                      --id
```

### az ad app federated-credential list
```
az ad app federated-credential list --id
```

### az ad app federated-credential show
```
az ad app federated-credential show --federated-credential-id
                                    --id
```

### az ad app federated-credential update
```
az ad app federated-credential update --federated-credential-id
                                      --id
                                      --parameters
```

## Azure Active Directory App Owner

### az ad app owner add
```
az ad app owner add --id
                    --owner-object-id
```

### az ad app owner list
```
az ad app owner list --id
```

### az ad app owner remove
```
az ad app owner remove --id
                       --owner-object-id
```

### Azure Active Directory App Permissions

### az ad app permission add
```
az ad app permission add --api
                         --api-permissions
                         --id
```

### az ad app permission admin-consent
```
az ad app permission admin-consent --id
```

### az ad app permission delete
```
az ad app permission delete --api
                            --id
                            [--api-permissions]
```

### az ad app permission grant
```
az ad app permission grant --api,
                           --id,
                           --scope
                           [--consent-type {AllPrincipals, Principal}]
                           [--principal-id]
```

### az ad app permission list
```
az ad app permission list --id
```

### az ad app permission list-grants
```
az ad app permission list-grants [--filter]
                                 [--id]
                                 [--show-resource-name {false, true}]
```

## Azure Active Directory Domain Service

### az ad ds create
```
az ad ds create --domain
                --name
                --replica-sets
                --resource-group
                [--domain-config-type {FullySynced, ResourceTrusting}]
                [--external-access {Disabled, Enabled}]
                [--filtered-sync {Disabled, Enabled}]
                [--ldaps {Disabled, Enabled}]
                [--no-wait]
                [--notify-dc-admins {Disabled, Enabled}]
                [--notify-global-admins {Disabled, Enabled}]
                [--notify-others]
                [--ntlm-v1 {Disabled, Enabled}]
                [--pfx-cert]
                [--pfx-cert-pwd]
                [--resource-forest {Disabled, Enabled}]
                [--settings]
                [--sku {Enterprise, Premium, Standard}]
                [--sync-kerberos-pwd {Disabled, Enabled}]
                [--sync-ntlm-pwd {Disabled, Enabled}]
                [--sync-on-prem-pwd {Disabled, Enabled}]
                [--tags]
                [--tls-v1 {Disabled, Enabled}]
```

### az ad ds delete
```
az ad ds delete [--ids]
                [--name]
                [--no-wait]
                [--resource-group]
                [--yes]
```

### az ad ds list
```
az ad ds list [--resource-group]
```

### az ad ds show
```
az ad ds show [--ids]
              [--name]
              [--resource-group]
```

### az ad ds update
```
az ad ds update [--domain-config-type {FullySynced, ResourceTrusting}]
                [--external-access {Disabled, Enabled}]
                [--filtered-sync {Disabled, Enabled}]
                [--ids]
                [--ldaps {Disabled, Enabled}]
                [--name]
                [--no-wait]
                [--notify-dc-admins {Disabled, Enabled}]
                [--notify-global-admins {Disabled, Enabled}]
                [--notify-others]
                [--ntlm-v1 {Disabled, Enabled}]
                [--pfx-cert]
                [--pfx-cert-pwd]
                [--replica-sets]
                [--resource-forest {Disabled, Enabled}]
                [--resource-group]
                [--settings]
                [--sku {Enterprise, Premium, Standard}]
                [--sync-kerberos-pwd {Disabled, Enabled}]
                [--sync-ntlm-pwd {Disabled, Enabled}]
                [--sync-on-prem-pwd {Disabled, Enabled}]
                [--tags]
                [--tls-v1 {Disabled, Enabled}]
```

### az ad ds wait
```
az ad ds wait [--created]
              [--custom]
              [--deleted]
              [--exists]
              [--ids]
              [--interval]
              [--name]
              [--resource-group]
              [--timeout]
              [--updated]
```

## Azure Active Directory Groups

### az ad group create
```
az ad group create --display-name
                   --mail-nickname
                   [--description]
                   [--force {false, true}]
```

### az ad group delete
```
az ad group delete --group
```

### az ad group get-member-groups
```
az ad group get-member-groups --group
                              [--security-enabled-only {false, true}]
```

### az ad group list
```
az ad group list [--display-name]
                 [--filter]
```

### az ad group show
```
az ad group show --group
```

## Azure Active Directory Group Member

### az ad group member add
```
az ad group member add --group
                       --member-id
```

### az ad group member check
```
az ad group member check --group
                         --member-id
```

### az ad group member list
```
az ad group member list --group
```

### az ad group member remove
```
az ad group member remove --group
                          --member-id
```

## Azure Active Directory Group Owner

### az ad group owner add
```
az ad group owner add --group
                      --owner-object-id
```

### az ad group owner list
```
az ad group owner list --group
```

### az ad group owner remove
```
az ad group owner remove --group
                         --owner-object-id
```

## Azure Active Directory Signed-in User

### az ad signed-in-user list-owned-objects
```
az ad signed-in-user list-owned-objects [--type]
```

### az ad signed-in-user show
```
az ad signed-in-user show
```

## Azure Active Directory Service Principals

### az ad sp create
```
az ad sp create --id
```

### az ad sp create-for-rbac
```
az ad sp create-for-rbac [--cert]
                         [--create-cert]
                         [--display-name]
                         [--keyvault]
                         [--role]
                         [--scopes]
                         [--sdk-auth {false, true}]
                         [--skip-assignment {false, true}]
                         [--years]
```

### az ad sp delete
```
az ad sp delete --id
```

### az ad sp list
```
az ad sp list [--all]
              [--display-name]
              [--filter]
              [--show-mine]
              [--spn]
```

### az ad sp owner list
```
az ad sp owner list --id
```

### az ad sp show
```
az ad sp show --id
```

### az ad sp update
```
az ad sp update --id
                [--add]
                [--force-string]
                [--remove]
                [--set]
```

## Azure Active Directory Service Principals Credentials

### az ad sp credential delete
```
az ad sp credential delete --id
                           --key-id
                           [--cert]
```

### az ad sp credential list
```
az ad sp credential list --id
                         [--cert]
```

### az ad sp credential reset
```
az ad sp credential reset --id
                          [--append]
                          [--cert]
                          [--create-cert]
                          [--display-name]
                          [--end-date]
                          [--keyvault]
                          [--years]
```

## Azure Active Directory Service Principals User

### az ad sp user create
```
az ad user create --display-name
                  --password
                  --user-principal-name
                  [--force-change-password-next-sign-in {false, true}]
                  [--immutable-id]
                  [--mail-nickname]
```

### az ad sp user delete
```
az ad user delete --id
```

### az ad sp user get-member-groups
```
az ad user get-member-groups --id
                             [--security-enabled-only {false, true}]
```

### az ad sp user list
```
az ad user list [--display-name]
                [--filter]
                [--upn]
```

### az ad sp user show
```
az ad user show --id
```

### az ad sp user update
```
az ad user update --id
                  [--account-enabled {false, true}]
                  [--display-name]
                  [--force-change-password-next-sign-in {false, true}]
                  [--mail-nickname]
                  [--password]
```



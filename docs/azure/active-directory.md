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


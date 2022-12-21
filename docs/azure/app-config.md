# Azure App Configuration

### az appconfig create
```
az appconfig create --location
                    --name
                    --resource-group
                    [--assign-identity]
                    [--disable-local-auth {false, true}]
                    [--enable-public-network {false, true}]
                    [--enable-purge-protection {false, true}]
                    [--retention-days]
                    [--sku {Free, Standard}]
                    [--tags]
```

### az appconfig delete
```
az appconfig delete --name
                    [--resource-group]
                    [--yes]
```

### az appconfig list
```
az appconfig list [--resource-group]
```

### az appconfig list-deleted
```
az appconfig list-deleted
```

### az appconfig purge
```
az appconfig purge --name
                   [--location]
                   [--yes]
```

### az appconfig recover
```
az appconfig recover --name
                     [--location]
                     [--resource-group]
                     [--yes]
```

### az appconfig show
```
az appconfig show --name
                  [--resource-group]
```

### az appconfig show-deleted
```
az appconfig show-deleted --name
                          [--location]
```

### az appconfig update
```
az appconfig update --name
                    [--disable-local-auth {false, true}]
                    [--enable-public-network {false, true}]
                    [--enable-purge-protection {false, true}]
                    [--encryption-key-name]
                    [--encryption-key-vault]
                    [--encryption-key-version]
                    [--identity-client-id]
                    [--resource-group]
                    [--sku {Free, Standard}]
                    [--tags]
```

## Azure App Configuration Credentials

### az appconfig credential list
```
az appconfig credential list --name
                             [--resource-group]
```

### az appconfig credential regenerate
```
az appconfig credential regenerate --id
                                   --name
                                   [--resource-group]
```

## Azure App Configuration Feature

### az appconfig feature
```
az appconfig feature delete [--auth-mode {key, login}]
                            [--connection-string]
                            [--endpoint]
                            [--feature]
                            [--key]
                            [--label]
                            [--name]
                            [--yes]
```

### az appconfig feature disable
```
az appconfig feature disable [--auth-mode {key, login}]
                             [--connection-string]
                             [--endpoint]
                             [--feature]
                             [--key]
                             [--label]
                             [--name]
                             [--yes]
```

### az appconfig feature enable
```
az appconfig feature enable [--auth-mode {key, login}]
                            [--connection-string]
                            [--endpoint]
                            [--feature]
                            [--key]
                            [--label]
                            [--name]
                            [--yes]
```

### az appconfig feature list
```
az appconfig feature list [--all]
                          [--auth-mode {key, login}]
                          [--connection-string]
                          [--endpoint]
                          [--feature]
                          [--fields {conditions, description, key, label, last_modified, locked, name, state}]
                          [--key]
                          [--label]
                          [--name]
                          [--top]
```

### az appconfig feature lock
```
az appconfig feature lock [--auth-mode {key, login}]
                          [--connection-string]
                          [--endpoint]
                          [--feature]
                          [--key]
                          [--label]
                          [--name]
                          [--yes]
```

### az appconfig feature set
```
az appconfig feature set [--auth-mode {key, login}]
                         [--connection-string]
                         [--description]
                         [--endpoint]
                         [--feature]
                         [--key]
                         [--label]
                         [--name]
                         [--yes]
```

### az appconfig feature show
```
az appconfig feature show [--auth-mode {key, login}]
                          [--connection-string]
                          [--endpoint]
                          [--feature]
                          [--fields {conditions, description, key, label, last_modified, locked, name, state}]
                          [--key]
                          [--label]
                          [--name]
```
### az appconfig feature unlock
```
az appconfig feature unlock [--auth-mode {key, login}]
                            [--connection-string]
                            [--endpoint]
                            [--feature]
                            [--key]
                            [--label]
                            [--name]
                            [--yes]
```

## Azure App Configuration Feature Filter

### az appconfig feature filter add
```
az appconfig feature filter add --filter-name
                                [--auth-mode {key, login}]
                                [--connection-string]
                                [--endpoint]
                                [--feature]
                                [--filter-parameters]
                                [--index]
                                [--key]
                                [--label]
                                [--name]
                                [--yes]
```

### az appconfig feature filter delete
```
az appconfig feature filter delete [--all]
                                   [--auth-mode {key, login}]
                                   [--connection-string]
                                   [--endpoint]
                                   [--feature]
                                   [--filter-name]
                                   [--index]
                                   [--key]
                                   [--label]
                                   [--name]
                                   [--yes]
```

### az appconfig feature filter list
```
az appconfig feature filter list [--all]
                                 [--auth-mode {key, login}]
                                 [--connection-string]
                                 [--endpoint]
                                 [--feature]
                                 [--key]
                                 [--label]
                                 [--name]
                                 [--top]
```

### az appconfig feature filter show
```
az appconfig feature filter show --filter-name
                                 [--auth-mode {key, login}]
                                 [--connection-string]
                                 [--endpoint]
                                 [--feature]
                                 [--index]
                                 [--key]
                                 [--label]
                                 [--name]
```

### az appconfig feature filter update
```
az appconfig feature filter update --filter-name
                                   [--auth-mode {key, login}]
                                   [--connection-string]
                                   [--endpoint]
                                   [--feature]
                                   [--filter-parameters]
                                   [--index]
                                   [--key]
                                   [--label]
                                   [--name]
                                   [--yes]
```

## Azure App Configuration Identity

### az appconfig identity assign
```
az appconfig identity assign --name
                             [--identities]
                             [--resource-group]
```

### az appconfig identity remove
```
az appconfig identity remove --name
                             [--identities]
                             [--resource-group]
```

### az appconfig identity show
```
az appconfig identity show --name
                           [--resource-group]
```

## Azure App Configuration Key-Values

### az appconfig kv delete
```
az appconfig kv delete --key
                       [--auth-mode {key, login}]
                       [--connection-string]
                       [--endpoint]
                       [--label]
                       [--name]
                       [--yes]
```

### az appconfig kv export
```
az appconfig kv export --destination {appconfig, appservice, file}
                       [--appservice-account]
                       [--auth-mode {key, login}]
                       [--connection-string]
                       [--dest-auth-mode {key, login}]
                       [--dest-connection-string]
                       [--dest-endpoint]
                       [--dest-label]
                       [--dest-name]
                       [--endpoint]
                       [--export-as-reference {false, true}]
                       [--format {json, properties, yaml}]
                       [--key]
                       [--label]
                       [--name]
                       [--naming-convention {camel, hyphen, pascal, underscore}]
                       [--path]
                       [--prefix]
                       [--preserve-labels {false, true}]
                       [--profile {appconfig/default, appconfig/kvset}]
                       [--resolve-keyvault {false, true}]
                       [--separator]
                       [--skip-features {false, true}]
                       [--skip-keyvault {false, true}]
                       [--yes]
```

### az appconfig kv import
```
az appconfig kv import --source {appconfig, appservice, file}
                       [--appservice-account]
                       [--auth-mode {key, login}]
                       [--connection-string]
                       [--content-type]
                       [--depth]
                       [--endpoint]
                       [--format {json, properties, yaml}]
                       [--label]
                       [--name]
                       [--path]
                       [--prefix]
                       [--preserve-labels {false, true}]
                       [--profile {appconfig/default, appconfig/kvset}]
                       [--separator]
                       [--skip-features {false, true}]
                       [--src-auth-mode {key, login}]
                       [--src-connection-string]
                       [--src-endpoint]
                       [--src-key]
                       [--src-label]
                       [--src-name]
                       [--strict {false, true}]
                       [--yes]
```

### az appconfig kv list
```
az appconfig kv import --source {appconfig, appservice, file}
                       [--appservice-account]
                       [--auth-mode {key, login}]
                       [--connection-string]
                       [--content-type]
                       [--depth]
                       [--endpoint]
                       [--format {json, properties, yaml}]
                       [--label]
                       [--name]
                       [--path]
                       [--prefix]
                       [--preserve-labels {false, true}]
                       [--profile {appconfig/default, appconfig/kvset}]
                       [--separator]
                       [--skip-features {false, true}]
                       [--src-auth-mode {key, login}]
                       [--src-connection-string]
                       [--src-endpoint]
                       [--src-key]
                       [--src-label]
                       [--src-name]
                       [--strict {false, true}]
                       [--yes]
```

### az appconfig kv lock
```
az appconfig kv lock --key
                     [--auth-mode {key, login}]
                     [--connection-string]
                     [--endpoint]
                     [--label]
                     [--name]
                     [--yes]
```

### az appconfig kv restore
```
az appconfig kv restore --datetime
                        [--auth-mode {key, login}]
                        [--connection-string]
                        [--endpoint]
                        [--key]
                        [--label]
                        [--name]
                        [--yes]
```

### az appconfig kv set
```
az appconfig kv set --key
                    [--auth-mode {key, login}]
                    [--connection-string]
                    [--content-type]
                    [--endpoint]
                    [--label]
                    [--name]
                    [--tags]
                    [--value]
                    [--yes]
```

### az appconfig kv set-keyvault
```
az appconfig kv set-keyvault --key
                             --secret-identifier
                             [--auth-mode {key, login}]
                             [--connection-string]
                             [--endpoint]
                             [--label]
                             [--name]
                             [--tags]
                             [--yes]
```

### az appconfig kv show
```
az appconfig kv show --key
                     [--auth-mode {key, login}]
                     [--connection-string]
                     [--datetime]
                     [--endpoint]
                     [--label]
                     [--name]
```

### az appconfig kv unlock
```
az appconfig kv unlock --key
                       [--auth-mode {key, login}]
                       [--connection-string]
                       [--endpoint]
                       [--label]
                       [--name]
                       [--yes]
```

### az appconfig revision list
```
az appconfig revision list [--all]
                           [--auth-mode {key, login}]
                           [--connection-string]
                           [--datetime]
                           [--endpoint]
                           [--fields {content_type, etag, key, label, last_modified, locked, tags, value}]
                           [--key]
                           [--label]
                           [--name]
                           [--top]
```                           

## Azure App Configuration Replica

### az appconfig replica create
```
az appconfig replica create --location
                            --name
                            --store-name
                            [--resource-group]
```

### az appconfig replica delete
```
az appconfig replica delete --name
                            --store-name
                            [--resource-group]
                            [--yes]
```

### az appconfig replica list
```
az appconfig replica list --store-name
                          [--resource-group]
```

### az appconfig replica show
```
az appconfig replica show --name
                          --store-name
                          [--resource-group]
```

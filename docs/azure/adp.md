## Autonomous Development Platform

### az adp check-name-availability
```
az adp check-name-availability --name
                               --type {Microsoft.AutonomousDevelopmentPlatform/accounts, Microsoft.AutonomousDevelopmentPlatform/workspaces}
```

## Autonomous Development Platform Account

### az adp account create
```
az adp account create --account-name
                      --resource-group
                      [--location]
                      [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                      [--tags]
```

### az adp account delete
```
az adp account delete [--account-name]
                      [--ids]
                      [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                      [--resource-group]
                      [--subscription]
                      [--yes]
```

### az adp account list
```
az adp account list [--resource-group]
```

### az adp account show
```
az adp account show [--account-name]
                    [--ids]
                    [--resource-group]
                    [--subscription]
```

### az adp account update
```
az adp account update [--account-name]
                      [--add]
                      [--force-string {0, 1, f, false, n, no, t, true, y, yes}]
                      [--ids]
                      [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                      [--remove]
                      [--resource-group]
                      [--set]
                      [--subscription]
                      [--tags]
```

### az adp account wait
```
az adp account wait [--account-name]
                    [--created]
                    [--custom]
                    [--deleted]
                    [--exists]
                    [--ids]
                    [--interval]
                    [--resource-group]
                    [--subscription]
                    [--timeout]
                    [--updated]
```

## Autonomous Development Platform Data Pool

### az adp account data-pool create
```
az adp account data-pool create --account-name
                                --data-pool-name
                                --resource-group
                                [--locations]
                                [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                                [--tags]
```

### az adp account data-pool delete
```
az adp account data-pool delete [--account-name]
                                [--data-pool-name]
                                [--ids]
                                [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                                [--resource-group]
                                [--subscription]
                                [--yes]
```

### az adp account data-pool list
```
az adp account data-pool list --account-name
                              --resource-group
```

### az adp account data-pool show
```
az adp account data-pool show [--account-name]
                              [--data-pool-name]
                              [--ids]
                              [--resource-group]
                              [--subscription]
```

### az adp account data-pool update
```
az adp account data-pool update [--account-name]
                                [--add]
                                [--data-pool-name]
                                [--force-string {0, 1, f, false, n, no, t, true, y, yes}]
                                [--ids]
                                [--locations]
                                [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                                [--remove]
                                [--resource-group]
                                [--set]
                                [--subscription]
                                [--tags]
```

### az adp account data-pool wait
```
az adp account data-pool wait [--account-name]
                              [--created]
                              [--custom]
                              [--data-pool-name]
                              [--deleted]
                              [--exists]
                              [--ids]
                              [--interval]
                              [--resource-group]
                              [--subscription]
                              [--timeout]
                              [--updated]
```

## Autonomous Development Platform Workspace

### az adp workspace create
```
az adp workspace create --name
                        --resource-group
                        [--data-location]
                        [--direct-read-access {Disabled, Enabled}]
                        [--domain-name-scope {NoReuse, ResourceGroupReuse, SubscriptionReuse, TenantReuse}]
                        [--encryption]
                        [--identity]
                        [--location]
                        [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                        [--source-resource-id]
                        [--storage-account-count]
                        [--storage-sku]
                        [--tags]
```

### az adp workspace delete
```
az adp workspace delete [--ids]
                        [--name]
                        [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                        [--resource-group]
                        [--subscription]
                        [--yes]
```

### az adp workspace list
```
az adp workspace list [--resource-group]
```

### az adp workspace show
```
az adp workspace show [--ids]
                      [--name]
                      [--resource-group]
                      [--subscription]
```

### az adp workspace update
```
az adp workspace update [--add]
                        [--force-string {0, 1, f, false, n, no, t, true, y, yes}]
                        [--identity]
                        [--ids]
                        [--name]
                        [--no-wait {0, 1, f, false, n, no, t, true, y, yes}]
                        [--remove]
                        [--resource-group]
                        [--set]
                        [--subscription]
                        [--tags]
```

### az adp workspace wait
```
az adp workspace wait [--created]
                      [--custom]
                      [--deleted]
                      [--exists]
                      [--ids]
                      [--interval]
                      [--name]
                      [--resource-group]
                      [--subscription]
                      [--timeout]
                      [--updated]
```



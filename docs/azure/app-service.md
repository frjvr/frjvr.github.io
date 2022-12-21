# Azure App Service

### az appservice list-location
```
az appservice list-locations --sku {B1, B2, B3, D1, F1, FREE, I1, I1v2, I2, I2v2, I3, I3v2, I4v2, I5v2, I6v2, P1V2, P1V3, P2V2, P2V3, P3V2, P3V3, S1, S2, S3, SHARED, WS1, WS2, WS3}
                             [--linux-workers-enabled]
```

## Azure App Service Environments

### az appservice ase create
```
az appservice ase create --name
                         --resource-group
                         --subnet
                         [--force-network-security-group {false, true}]
                         [--force-route-table {false, true}]
                         [--front-end-scale-factor]
                         [--front-end-sku {I1, I2, I3}]
                         [--ignore-network-security-group {false, true}]
                         [--ignore-route-table {false, true}]
                         [--ignore-subnet-size-validation {false, true}]
                         [--kind {ASEv2, ASEv3}]
                         [--location]
                         [--no-wait]
                         [--os-preference {Linux, Windows}]
                         [--virtual-ip-type {External, Internal}]
                         [--vnet-name]
                         [--zone-redundant {false, true}]
```

### az appservice ase create-inbound-services
```
az appservice ase create-inbound-services --name
                                          --resource-group
                                          --subnet
                                          [--skip-dns {false, true}]
                                          [--vnet-name]
```

### az appservice ase delete
```
az appservice ase delete --name
                         [--no-wait]
                         [--resource-group]
                         [--yes]
```

### az appservice ase list
```
az appservice ase list [--resource-group]
```

### az appservice ase list-addresses
```
az appservice ase list-addresses --name
                                 [--resource-group]
```

### az appservice ase list-plans
```
az appservice ase list-plans --name
                             [--resource-group]
```

### az appservice ase show
```
az appservice ase show --name
                       [--resource-group]
```

### az appservice ase update
```
az appservice ase update --name
                         [--allow-new-private-endpoint-connections {false, true}]
                         [--front-end-scale-factor]
                         [--front-end-sku {I1, I2, I3}]
                         [--no-wait]
                         [--resource-group]
```

## Azure App Service Custom Domain

### az appservice domain create
```
az appservice domain create --contact-info
                            --hostname
                            --resource-group
                            [--accept-terms]
                            [--auto-renew]
                            [--dryrun]
                            [--privacy]
                            [--tags]
```

### az appservice domain show-terms
```
az appservice domain show-terms --hostname
```

## Azure App Service Hybrid Connection Key

### az appservice hybrid-connection set-key
```
az appservice hybrid-connection set-key --hybrid-connection
                                        --key-type
                                        --namespace
                                        --plan
                                        --resource-group
```

## Azure App Service Kubernetes

### az appservice kube create
```
az appservice kube create --custom-location
                          --name
                          --resource-group
                          [--location]
                          [--no-wait]
                          [--static-ip]
                          [--tags]
```

### az appservice kube delete
```
az appservice kube delete --name
                          --resource-group
                          [--no-wait]
                          [--yes]
```

### az appservice kube list
```
az appservice kube list [--resource-group]
```

### az appservice kube show
```
az appservice kube show --name
                        --resource-group
```

### az appservice kube update
```
az appservice kube update --name
                          --resource-group
                          [--custom-location]
                          [--no-wait]
                          [--static-ip]
                          [--tags]
```

### az appservice kube wait
```
az appservice kube wait --name
                        --resource-group
                        [--created]
                        [--custom]
                        [--deleted]
                        [--exists]
                        [--interval]
                        [--timeout]
                        [--updated]
```

## Azure App Service Plan

### az appservice plan create
```
az appservice plan create --name
                          --resource-group
                          [--app-service-environment]
                          [--hyper-v]
                          [--is-linux]
                          [--location]
                          [--no-wait]
                          [--number-of-workers]
                          [--per-site-scaling]
                          [--sku {B1, B2, B3, D1, F1, FREE, I1, I1v2, I2, I2v2, I3, I3v2, I4v2, I5v2, I6v2, P1V2, P1V3, P2V2, P2V3, P3V2, P3V3, S1, S2, S3, SHARED, WS1, WS2, WS3}]
                          [--tags]
                          [--zone-redundant]
```

### az appservice plan delete
```
az appservice plan delete [--ids]
                          [--name]
                          [--resource-group]
                          [--subscription]
                          [--yes]
```

### az appservice plan list
```
az appservice plan list [--resource-group]
```

### az appservice plan show
```
az appservice plan show [--ids]
                        [--name]
                        [--resource-group]
                        [--subscription]
```

### az appservice plan update
```
az appservice plan update [--add]
                          [--elastic-scale {false, true}]
                          [--force-string]
                          [--ids]
                          [--max-elastic-worker-count]
                          [--name]
                          [--no-wait]
                          [--number-of-workers]
                          [--remove]
                          [--resource-group]
                          [--set]
                          [--sku {B1, B2, B3, D1, F1, FREE, I1, I1v2, I2, I2v2, I3, I3v2, I4v2, I5v2, I6v2, P1V2, P1V3, P2V2, P2V3, P3V2, P3V3, S1, S2, S3, SHARED, WS1, WS2, WS3}]
                          [--subscription]
```

## Azure App Service Virtual Network Integration

### az appservice vnet-integration list
```
az appservice vnet-integration list --plan
                                    --resource-group
```




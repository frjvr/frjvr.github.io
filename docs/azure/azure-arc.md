# Azure Arc

## Azure Arc Appliance

### az arcappliance get-credentials
```
az arcappliance get-credentials --name
                                --resource-group
```

### az arcappliance list
```
az arcappliance list [--resource-group]
```

### az arcappliance notice
```
az arcappliance notice
```

### az arcappliance show
```
az arcappliance show --name
                     --resource-group
```

## Azure Arc Appliance Create

### az arcappliance create hci
```
az arcappliance create hci --config-file
                           --kubeconfig
                           [--location]
                           [--name]
                           [--resource-group]
                           [--tags]
```

### az arcappliance create kubevirt
```
az arcappliance create kubevirt --config-file
                                --kubeconfig
                                [--location]
                                [--name]
                                [--resource-group]
                                [--tags]
```

### az arcappliance create scvmm
```
az arcappliance create scvmm --config-file
                             --kubeconfig
                             [--location]
                             [--name]
                             [--resource-group]
                             [--tags]
```

### az arcappliance create vmware
```
az arcappliance create vmware --config-file
                              --kubeconfig
                              [--location]
                              [--name]
                              [--resource-group]
                              [--tags]
```

## Azure Arc Configuration Files

### az arcappliance createconfig hci
```
az arcappliance createconfig hci --location
                                 --name
                                 --resource-group
                                 [--authenticationport]
                                 [--certificateFilePath]
                                 [--cloudagent]
                                 [--controlPlaneEndpoint]
                                 [--dnsservers]
                                 [--gateway]
                                 [--http]
                                 [--https]
                                 [--ipaddressprefix]
                                 [--k8snodeippoolend]
                                 [--k8snodeippoolstart]
                                 [--loginconfigfile]
                                 [--noproxy]
                                 [--out-dir]
                                 [--overwrite-existing]
                                 [--port]
                                 [--storagecontainer]
                                 [--vlanid]
                                 [--vswitchname]
                                 [--working-dir]
```

### az arcappliance createconfig kubevirt
```
az arcappliance createconfig kubevirt --location
                                      --name
                                      --resource-group
                                      [--fabric-kubeconfig]
                                      [--out-dir]
                                      [--overwrite-existing]
                                      [--vmsize]
                                      [--working-dir]
```

### az arcappliance createconfig svcmm
```
az arcappliance createconfig scvmm --location
                                   --name
                                   --resource-group
                                   [--address]
                                   [--certificateFilePath]
                                   [--cloudname]
                                   [--controlPlaneEndpoint]
                                   [--dnsservers]
                                   [--gateway]
                                   [--highlyavailable]
                                   [--http]
                                   [--https]
                                   [--ipaddressprefix]
                                   [--ippool]
                                   [--k8snodeippoolend]
                                   [--k8snodeippoolstart]
                                   [--libshare]
                                   [--macaddress]
                                   [--memorymib]
                                   [--network]
                                   [--noproxy]
                                   [--numcpus]
                                   [--out-dir]
                                   [--overwrite-existing]
                                   [--password]
                                   [--port]
                                   [--username]
                                   [--working-dir]
```

### az arcappliance createconfig vmware
```
az arcappliance createconfig vmware --location
                                    --name
                                    --resource-group
                                    [--address]
                                    [--certificateFilePath]
                                    [--controlPlaneEndpoint]
                                    [--datacenter]
                                    [--datastore]
                                    [--disksizegib]
                                    [--dnsservers]
                                    [--folder]
                                    [--gateway]
                                    [--http]
                                    [--https]
                                    [--ipaddressprefix]
                                    [--k8snodeippoolend]
                                    [--k8snodeippoolstart]
                                    [--memorymib]
                                    [--network]
                                    [--noproxy]
                                    [--numcpus]
                                    [--out-dir]
                                    [--overwrite-existing]
                                    [--password]
                                    [--resourcepool]
                                    [--username]
                                    [--working-dir]
```

## Azure Arc Appliance Delete

### az arcappliance delete hci
```
az arcappliance delete hci --config-file
                           [--location]
                           [--name]
                           [--resource-group]
                           [--yes]
```

## az arcappliance delete kubevirt
```
az arcappliance delete kubevirt --config-file
                                [--location]
                                [--name]
                                [--resource-group]
                                [--yes]
```

### az arcappliance delete scvmm
```
az arcappliance delete scvmm --config-file
                             [--location]
                             [--name]
                             [--resource-group]
                             [--yes]
```

### az arcappliance delete vmware
```
az arcappliance delete vmware --config-file
                              [--location]
                              [--name]
                              [--resource-group]
                              [--yes]
```

## Azure Arc Appliance Deploy

### az arcappliance deploy hci
```
az arcappliance deploy hci --config-file
                           [--location]
                           [--name]
                           [--outfile]
                           [--resource-group]
```

### az arcappliance deploy kubevirt
```
az arcappliance deploy kubevirt --config-file
                                [--location]
                                [--name]
                                [--outfile]
                                [--resource-group]
```

### az arcappliance deploy scvmm
```
az arcappliance deploy scvmm --config-file
                             [--location]
                             [--name]
                             [--outfile]
                             [--resource-group]
```

### az arcappliance deploy vmware
```
az arcappliance deploy vmware --config-file
                              [--location]
                              [--name]
                              [--outfile]
                              [--resource-group]
```

## Azure Arc Appliance Logs

### az arcappliance logs hci
```
az arcappliance logs hci [--cloudagent]
                         [--ip]
                         [--kubeconfig]
                         [--loginconfigfile]
                         [--out-dir]
```

### az arcappliance logs kubevirt
```
az arcappliance logs kubevirt [--ip]
                              [--kubeconfig]
                              [--out-dir]
```

### az arcappliance logs scvmm
```
az arcappliance logs scvmm [--ip]
                           [--kubeconfig]
                           [--out-dir]
```

### az arcappliance logs vmware
```
az arcappliance logs vmware [--address]
                            [--ip]
                            [--kubeconfig]
                            [--out-dir]
                            [--password]
                            [--username]
```

## Azure Arc Appliance Prepare

### az arcappliance prepare hci
```
az arcappliance prepare hci --config-file
                            [--location]
                            [--name]
                            [--resource-group]
```

### az arcappliance prepare kubevirt
```
az arcappliance prepare kubevirt --config-file
                                 [--location]
                                 [--name]
                                 [--resource-group]
```

### az arcappliance prepare scvmm
```
az arcappliance prepare scvmm --config-file
                              [--location]
                              [--name]
                              [--resource-group]
```

### az arcappliance prepare vmware
```
az arcappliance prepare vmware --config-file
                               [--location]
                               [--name]
                               [--resource-group]
```

## Azure Arc Appliance Run

### az arcappliance run hci
```
az arcappliance run hci --location
                        --name
                        --resource-group
                        [--force]
                        [--out-dir]
                        [--tags]
                        [--working-dir]
```

### az arcappliance run kubevirt
```
az arcappliance run kubevirt --location
                             --name
                             --resource-group
                             [--force]
                             [--out-dir]
                             [--tags]
                             [--working-dir]
```

### az arcappliance run scvmm
```
az arcappliance run scvmm --location
                          --name
                          --resource-group
                          [--force]
                          [--out-dir]
                          [--tags]
                          [--working-dir]
```

### az arcappliance run vmware
```
az arcappliance run vmware --location
                           --name
                           --resource-group
                           [--force]
                           [--out-dir]
                           [--tags]
                           [--working-dir]
```

## Azure Arc Appliance Credentials

### az arcappliance update-infracredentials hci
```
az arcappliance update-infracredentials hci --kubeconfig
```

### az arcappliance update-infracredentials scvmm
```
az arcappliance update-infracredentials scvmm --kubeconfig
```

### az arcappliance update-infracredentials vmware
```
az arcappliance update-infracredentials vmware --kubeconfig
```

## Azure Arc Appliance Validate

### az arcappliance validate hci
```
az arcappliance validate hci --config-file
                             [--location]
                             [--name]
                             [--resource-group]
```

### az arcappliance validate kubevirt
```
az arcappliance validate kubevirt --config-file
                                  [--location]
                                  [--name]
                                  [--resource-group]
```

### az arcappliance validate scvmm
```
az arcappliance validate scvmm --config-file
                               [--location]
                               [--name]
                               [--resource-group]
```

### az arcappliance validate vmware
```
az arcappliance validate vmware --config-file
                                [--location]
                                [--name]
                                [--resource-group]
```

## Azure Arc Data Service

## Azure Arc Data Service Active Directory Connector

### az arcdata ad-connector create
```
az arcdata ad-connector create --account-provisioning
                               --name
                               --nameserver-addresses
                               --realm
                               [--data-controller-name]
                               [--dns-domain-name]
                               [--dns-replicas]
                               [--domain-service-account-secret]
                               [--k8s-namespace]
                               [--netbios-domain-name]
                               [--no-wait]
                               [--ou-distinguished-name]
                               [--prefer-k8s-dns]
                               [--primary-ad-dc-hostname]
                               [--resource-group]
                               [--secondary-ad-dc-hostnames]
                               [--use-k8s]
```

### az arcdata ad-connector delete
```
az arcdata ad-connector delete --name
                               [--data-controller-name]
                               [--k8s-namespace]
                               [--no-wait]
                               [--resource-group]
                               [--use-k8s]
```

### az arcdata ad-connector list
```
az arcdata ad-connector list [--data-controller-name]
                             [--k8s-namespace]
                             [--resource-group]
                             [--use-k8s]
```

### az arcdata ad-connector show
```
az arcdata ad-connector show --name
                             [--data-controller-name]
                             [--k8s-namespace]
                             [--resource-group]
                             [--use-k8s]
```

### az arcdata ad-connector update
```
az arcdata ad-connector update --name
                               [--data-controller-name]
                               [--dns-replicas]
                               [--domain-service-account-secret]
                               [--k8s-namespace]
                               [--nameserver-addresses]
                               [--no-wait]
                               [--prefer-k8s-dns]
                               [--primary-ad-dc-hostname]
                               [--resource-group]
                               [--secondary-ad-dc-hostnames]
                               [--use-k8s]
```

## Azure Arc Data Controllers

### az arcdata dc create
```
az arcdata dc create --connectivity-mode
                     --name
                     --resource-group
                     [--annotations]
                     [--auto-upload-logs {false, true}]
                     [--auto-upload-metrics {false, true}]
                     [--cluster-name]
                     [--custom-location]
                     [--infrastructure]
                     [--k8s-namespace]
                     [--labels]
                     [--location]
                     [--logs-ui-private-key-file]
                     [--logs-ui-public-key-file]
                     [--metrics-ui-private-key-file]
                     [--metrics-ui-public-key-file]
                     [--no-wait]
                     [--path]
                     [--profile-name]
                     [--service-annotations]
                     [--service-labels]
                     [--storage-annotations]
                     [--storage-class]
                     [--storage-labels]
                     [--use-k8s]
```

### az arcdata dc delete
```
az arcdata dc delete --name
                     [--force]
                     [--k8s-namespace]
                     [--no-wait]
                     [--resource-group]
                     [--use-k8s]
                     [--yes]
```

### az arcdata dc export
```
az arcdata dc export --k8s-namespace
                     --path
                     --type
                     [--force]
                     [--use-k8s]
```

### az arcdata dc list-upgrades
```
az arcdata dc list-upgrades --k8s-namespace
                            [--use-k8s]
```

### az arcdata dc update
```
az arcdata dc update [--auto-upload-logs {false, true}]
                     [--auto-upload-metrics {false, true}]
                     [--desired-version]
                     [--k8s-namespace]
                     [--maintenance-duration]
                     [--maintenance-enabled {false, true}]
                     [--maintenance-recurrence]
                     [--maintenance-start]
                     [--maintenance-time-zone]
                     [--name]
                     [--no-wait]
                     [--resource-group]
                     [--use-k8s]
```

### az arcdata dc upgrade
```
az arcdata dc upgrade [--desired-version]
                      [--dry-run]
                      [--k8s-namespace]
                      [--name]
                      [--no-wait]
                      [--resource-group]
                      [--target]
                      [--use-k8s]
```

### az arcdata dc upload
```
az arcdata dc upload --path
```

## Azure Arc Data Controller Configuration

### az arcdata dc config add
```
az arcdata dc config add --config-file
                         --json-values
                         --path
```

### az arcdata dc config init
```
az arcdata dc config init [--force]
                          [--path]
                          [--source]
                          [--target]
```

### az arcdata dc config list
```
az arcdata dc config list [--config-profile]
```

### az arcdata dc config patch
```
az arcdata dc config patch --config-file
                           --patch-file
                           --path
```

### az arcdata dc config remove
```
az arcdata dc config remove --config-file
                            --json-path
                            --path
```

### az arcdata dc config replace
```
az arcdata dc config replace --config-file
                             --json-values
                             --path
```

### az arcdata dc config show
```
az arcdata dc config show [--k8s-namespace]
                          [--use-k8s]
```

## Azure Arc Data Controller Debug

### az arcdata dc debug copy-logs
```
az arcdata dc debug copy-logs --k8s-namespace
                              [--container]
                              [--exclude-dumps]
                              [--exclude-system-logs]
                              [--pod]
                              [--resource-kind]
                              [--resource-name]
                              [--skip-compress]
                              [--target-folder]
                              [--timeout]
                              [--use-k8s]
```

### az arcdata dc debug dump
```
az arcdata dc debug dump --k8s-namespace
                         [--container {controller}]
                         [--target-folder]
                         [--use-k8s]
```

## Azure Arc Data Controller Endpoint

### az arcdata dc endpoint list
```
az arcdata dc endpoint list --k8s-namespace
                            [--endpoint-name]
                            [--use-k8s]
```

## Azure Arc Data Controller Status

### az arcdata dc status show
```
az arcdata dc status show [--k8s-namespace]
                          [--name]
                          [--resource-group]
                          [--use-k8s]
```

## Azure Arc Data Resource Kind

### az arcdata resource-kind get
```
az arcdata resource-kind get --kind
                             [--dest]
```

### az arcdata resource-kind list
```
az arcdata resource-kind list
```

## Azure Arc Connected Machine

### az connectedmachine delete
```
az connectedmachine delete [--ids]
                           [--machine-name]
                           [--resource-group]
                           [--subscription]
                           [--yes]
```

### az connectedmachine list
```
az connectedmachine list [--resource-group]
```

### az connectedmachine show
```
az connectedmachine show [--ids]
                         [--machine-name]
                         [--resource-group]
                         [--subscription]
```

### az connectedmachine upgrade-extension
```
az connectedmachine upgrade-extension [--extension-targets]
                                      [--ids]
                                      [--machine-name]
                                      [--resource-group]
                                      [--subscription]
```

## Azure Arc Connected Machine Extension

### az connectedmachine extension create
```
az connectedmachine extension create --machine-name
                                     --name
                                     --resource-group
                                     [--auto-upgrade-minor {false, true}]
                                     [--enable-auto-upgrade {false, true}]
                                     [--force-update-tag]
                                     [--inst-handler-version]
                                     [--instance-view-type]
                                     [--location]
                                     [--no-wait]
                                     [--protected-settings]
                                     [--publisher]
                                     [--settings]
                                     [--status]
                                     [--tags]
                                     [--type]
                                     [--type-handler-version]
```

### az connectedmachine extension delete
```
az connectedmachine extension delete [--ids]
                                     [--machine-name]
                                     [--name]
                                     [--no-wait]
                                     [--resource-group]
                                     [--subscription]
                                     [--yes]
```

### az connectedmachine extension list
```
az connectedmachine extension list --machine-name
                                   --resource-group
                                   [--expand]
```

### az connectedmachine extension show
```
az connectedmachine extension show [--ids]
                                   [--machine-name]
                                   [--name]
                                   [--resource-group]
                                   [--subscription]
```

### az connectedmachine extension update
```
az connectedmachine extension update [--auto-upgrade-minor {false, true}]
                                     [--enable-auto-upgrade {false, true}]
                                     [--force-update-tag]
                                     [--ids]
                                     [--machine-name]
                                     [--name]
                                     [--no-wait]
                                     [--protected-settings]
                                     [--publisher]
                                     [--resource-group]
                                     [--settings]
                                     [--subscription]
                                     [--tags]
                                     [--type]
                                     [--type-handler-version]
```

### az connectedmachine extension wait
```
az connectedmachine extension wait [--created]
                                   [--custom]
                                   [--deleted]
                                   [--exists]
                                   [--ids]
                                   [--interval]
                                   [--machine-name]
                                   [--name]
                                   [--resource-group]
                                   [--subscription]
                                   [--timeout]
                                   [--updated]
```

## Azure Arc Connected Machine Private Endpoint Connection

### az connectedmachine private-endpoint-connection delete
```
az connectedmachine private-endpoint-connection delete [--ids]
                                                       [--name]
                                                       [--no-wait]
                                                       [--resource-group]
                                                       [--scope-name]
                                                       [--subscription]
                                                       [--yes]
```

### az connectedmachine private-endpoint-connection list
```
az connectedmachine private-endpoint-connection list --resource-group
                                                     --scope-name
```

### az connectedmachine private-endpoint-connection show
```
az connectedmachine private-endpoint-connection show [--ids]
                                                     [--name]
                                                     [--resource-group]
                                                     [--scope-name]
                                                     [--subscription]
```

### az connectedmachine private-endpoint-connection update
```
az connectedmachine private-endpoint-connection update [--connection-state]
                                                       [--id]
                                                       [--ids]
                                                       [--name]
                                                       [--no-wait]
                                                       [--resource-group]
                                                       [--scope-name]
                                                       [--subscription]
```

### az connectedmachine private-endpoint-connection wait
```
az connectedmachine private-endpoint-connection wait [--created]
                                                     [--custom]
                                                     [--deleted]
                                                     [--exists]
                                                     [--ids]
                                                     [--interval]
                                                     [--name]
                                                     [--resource-group]
                                                     [--scope-name]
                                                     [--subscription]
                                                     [--timeout]
                                                     [--updated]
```



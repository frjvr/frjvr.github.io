# Azure Healthcare APIs

## Azure Heakthcare APIs ACR

### az healthcareapis acr add
```
az healthcareapis acr add [--ids]
                          [--login-servers]
                          [--resource-group]
                          [--resource-name]
                          [--subscription]
```

### az healthcareapis acr list
```
az healthcareapis acr list --resource-group
                           --resource-name
```

### az healthcareapis acr remove
```
az healthcareapis acr remove [--ids]
                             [--login-servers]
                             [--resource-group]
                             [--resource-name]
                             [--subscription]
```

### az healthcareapis acr reset
```
az healthcareapis acr reset [--ids]
                            [--login-servers]
                            [--resource-group]
                            [--resource-name]
                            [--subscription]
```

## Azure Healthcare APIs Operation Result

### az healthcareapis operation-result show
```
az healthcareapis operation-result show [--ids]
                                        [--location-name]
                                        [--operation-result-id]
                                        [--subscription]
```

### Azure Healthcare APIs Private Endpoint Connection

### az healthcareapis private-endpoint-connection create
```
az healthcareapis private-endpoint-connection create --name
                                                     --resource-group
                                                     --resource-name
                                                     [--no-wait]
                                                     [--private-link-service-connection-state]
                                                     [--private-link-service-connection-state-actions-required]
                                                     [--private-link-service-connection-state-description]
                                                     [--private-link-service-connection-state-status {Approved, Pending, Rejected}]
```

### az healthcareapis private-endpoint-connection delete
```
az healthcareapis private-endpoint-connection delete [--ids]
                                                     [--name]
                                                     [--no-wait]
                                                     [--resource-group]
                                                     [--resource-name]
                                                     [--subscription]
                                                     [--yes]
```

### az healthcareapis private-endpoint-connection list
```
az healthcareapis private-endpoint-connection list --resource-group
                                                   --resource-name
```

### az healthcareapis private-endpoint-connection show
```
az healthcareapis private-endpoint-connection show [--ids]
                                                   [--name]
                                                   [--resource-group]
                                                   [--resource-name]
                                                   [--subscription]
```

### az healthcareapis private-endpoint-connection update
```
az healthcareapis private-endpoint-connection update [--ids]
                                                     [--name]
                                                     [--no-wait]
                                                     [--private-link-service-connection-state]
                                                     [--private-link-service-connection-state-actions-required]
                                                     [--private-link-service-connection-state-description]
                                                     [--private-link-service-connection-state-status {Approved, Pending, Rejected}]
                                                     [--resource-group]
                                                     [--resource-name]
                                                     [--subscription]
```

### az healthcareapis private-endpoint-connection wait
```
az healthcareapis private-endpoint-connection wait [--created]
                                                   [--custom]
                                                   [--deleted]
                                                   [--exists]
                                                   [--ids]
                                                   [--interval]
                                                   [--name]
                                                   [--resource-group]
                                                   [--resource-name]
                                                   [--subscription]
                                                   [--timeout]
                                                   [--updated]
```

## Azure Healthcare APIs Private Link Resource

### az healthcareapis private-link-resource list
```
az healthcareapis private-link-resource list --resource-group
                                             --resource-name
```

### az healthcareapis private-link-resource show
```
az healthcareapis private-link-resource show [--group-name]
                                             [--ids]
                                             [--resource-group]
                                             [--resource-name]
                                             [--subscription]
```

## Azure Healthcare APIs Service

### az healthcareapis service create
```
az healthcareapis service create --kind {fhir, fhir-R4, fhir-Stu3}
                                 --location
                                 --resource-group
                                 --resource-name
                                 [--access-policies]
                                 [--authentication-configuration]
                                 [--cors-configuration]
                                 [--cosmos-db-configuration]
                                 [--etag]
                                 [--export-configuration-storage-account-name]
                                 [--identity-type {None, SystemAssigned}]
                                 [--login-servers]
                                 [--no-wait]
                                 [--oci-artifacts]
                                 [--private-endpoint-connections]
                                 [--public-network-access {Disabled, Enabled}]
                                 [--tags]
```

### az healthcareapis service delete
```
az healthcareapis service delete [--ids]
                                 [--no-wait]
                                 [--resource-group]
                                 [--resource-name]
                                 [--subscription]
                                 [--yes]
```

### az healthcareapis service list
```
az healthcareapis service list [--resource-group]
```

### az healthcareapis service show
```
az healthcareapis service show [--ids]
                               [--resource-group]
                               [--resource-name]
                               [--subscription]
```

### az healthcareapis service update
```
az healthcareapis service update [--ids]
                                 [--no-wait]
                                 [--public-network-access {Disabled, Enabled}]
                                 [--resource-group]
                                 [--resource-name]
                                 [--subscription]
                                 [--tags]
```

### az healthcareapis service wait
```
az healthcareapis service wait [--created]
                               [--custom]
                               [--deleted]
                               [--exists]
                               [--ids]
                               [--interval]
                               [--resource-group]
                               [--resource-name]
                               [--subscription]
                               [--timeout]
                               [--updated]
```

## Azure Healthcare APIs Workspace

### az healthcareapis workspace create
```
az healthcareapis workspace create --name
                                   --resource-group
                                   [--etag]
                                   [--location]
                                   [--no-wait]
                                   [--public-network-access {Disabled, Enabled}]
                                   [--tags]
```

### az healthcareapis workspace delete
```
az healthcareapis workspace delete [--ids]
                                   [--name]
                                   [--no-wait]
                                   [--resource-group]
                                   [--subscription]
                                   [--yes]
```

### az healthcareapis workspace list
```
az healthcareapis workspace list [--resource-group]
```

### az healthcareapis workspace show
```
az healthcareapis workspace show [--ids]
                                 [--name]
                                 [--resource-group]
                                 [--subscription]
```

### az healthcareapis workspace update
```
az healthcareapis workspace update [--ids]
                                   [--name]
                                   [--no-wait]
                                   [--resource-group]
                                   [--subscription]
                                   [--tags]
```

### az healthcareapis workspace wait
```
az healthcareapis workspace wait [--created]
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

## Azure Healthcare APIs DICOM Service

### az healthcareapis workspace dicom-service create
```
az healthcareapis workspace dicom-service create --dicom-service-name
                                                 --resource-group
                                                 --workspace-name
                                                 [--etag]
                                                 [--identity-type {None, SystemAssigned, SystemAssigned,UserAssigned, UserAssigned}]
                                                 [--location]
                                                 [--no-wait]
                                                 [--public-network-access {Disabled, Enabled}]
                                                 [--tags]
                                                 [--user-assigned-identities]
```

### az healthcareapis workspace dicom-service delete
```
az healthcareapis workspace dicom-service delete [--dicom-service-name]
                                                 [--ids]
                                                 [--no-wait]
                                                 [--resource-group]
                                                 [--subscription]
                                                 [--workspace-name]
                                                 [--yes]
```

### az healthcareapis workspace dicom-service list
```
az healthcareapis workspace dicom-service list --resource-group
                                               --workspace-name
```

### az healthcareapis workspace dicom-service show
```
az healthcareapis workspace dicom-service show [--dicom-service-name]
                                               [--ids]
                                               [--resource-group]
                                               [--subscription]
                                               [--workspace-name]
```

### az healthcareapis workspace dicom-service update
```
az healthcareapis workspace dicom-service update [--dicom-service-name]
                                                 [--identity-type {None, SystemAssigned, SystemAssigned,UserAssigned, UserAssigned}]
                                                 [--ids]
                                                 [--no-wait]
                                                 [--resource-group]
                                                 [--subscription]
                                                 [--tags]
                                                 [--user-assigned-identities]
                                                 [--workspace-name]
```

### az healthcareapis workspace dicom-service wait
```
az healthcareapis workspace dicom-service wait [--created]
                                               [--custom]
                                               [--deleted]
                                               [--dicom-service-name]
                                               [--exists]
                                               [--ids]
                                               [--interval]
                                               [--resource-group]
                                               [--subscription]
                                               [--timeout]
                                               [--updated]
                                               [--workspace-name]
```

## Azure Healthcare APIs FHIR Service

### az healthcareapis workspace fhir-service create
```
az healthcareapis workspace fhir-service create --fhir-service-name
                                                --resource-group
                                                --workspace-name
                                                [--access-policies]
                                                [--authentication-configuration]
                                                [--cors-configuration]
                                                [--default {no-version, versioned, versioned-update}]
                                                [--etag]
                                                [--export-configuration-storage-account-name]
                                                [--identity-type {None, SystemAssigned, SystemAssigned,UserAssigned, UserAssigned}]
                                                [--kind {fhir-R4, fhir-Stu3}]
                                                [--location]
                                                [--login-servers]
                                                [--no-wait]
                                                [--oci-artifacts]
                                                [--public-network-access {Disabled, Enabled}]
                                                [--resource-type-overrides]
                                                [--tags]
                                                [--user-assigned-identities]
```

### az healthcareapis workspace fhir-service delete
```
az healthcareapis workspace fhir-service delete [--fhir-service-name]
                                                [--ids]
                                                [--no-wait]
                                                [--resource-group]
                                                [--subscription]
                                                [--workspace-name]
                                                [--yes]
```

### az healthcareapis workspace fhir-service list
```
az healthcareapis workspace fhir-service list --resource-group
                                              --workspace-name
```

### az healthcareapis workspace fhir-service show
```
az healthcareapis workspace fhir-service show [--fhir-service-name]
                                              [--ids]
                                              [--resource-group]
                                              [--subscription]
                                              [--workspace-name]
```

### az healthcareapis workspace fhir-service update
```
az healthcareapis workspace fhir-service update [--fhir-service-name]
                                                [--identity-type {None, SystemAssigned, SystemAssigned,UserAssigned, UserAssigned}]
                                                [--ids]
                                                [--no-wait]
                                                [--resource-group]
                                                [--subscription]
                                                [--tags]
                                                [--user-assigned-identities]
                                                [--workspace-name]
```

### az healthcareapis workspace fhir-service wait
```
az healthcareapis workspace fhir-service wait [--created]
                                              [--custom]
                                              [--deleted]
                                              [--exists]
                                              [--fhir-service-name]
                                              [--ids]
                                              [--interval]
                                              [--resource-group]
                                              [--subscription]
                                              [--timeout]
                                              [--updated]
                                              [--workspace-name]
```

## Azure Healthcare APIs IOT Connector

### az healthcareapis workspace iot-connector create
```
az healthcareapis workspace iot-connector create --iot-connector-name
                                                 --resource-group
                                                 --workspace-name
                                                 [--content]
                                                 [--etag]
                                                 [--identity-type {None, SystemAssigned, SystemAssigned,UserAssigned, UserAssigned}]
                                                 [--ingestion-endpoint-configuration]
                                                 [--location]
                                                 [--no-wait]
                                                 [--tags]
                                                 [--user-assigned-identities]
```

### az healthcareapis workspace iot-connector delete
```
az healthcareapis workspace iot-connector delete [--ids]
                                                 [--iot-connector-name]
                                                 [--no-wait]
                                                 [--resource-group]
                                                 [--subscription]
                                                 [--workspace-name]
                                                 [--yes]
```

### az healthcareapis workspace iot-connector list
```
az healthcareapis workspace iot-connector list --resource-group
                                               --workspace-name
```

### az healthcareapis workspace iot-connector show
```
az healthcareapis workspace iot-connector show [--ids]
                                               [--iot-connector-name]
                                               [--resource-group]
                                               [--subscription]
                                               [--workspace-name]
```

### az healthcareapis workspace iot-connector update
```
az healthcareapis workspace iot-connector update [--identity-type {None, SystemAssigned, SystemAssigned,UserAssigned, UserAssigned}]
                                                 [--ids]
                                                 [--iot-connector-name]
                                                 [--no-wait]
                                                 [--resource-group]
                                                 [--subscription]
                                                 [--tags]
                                                 [--user-assigned-identities]
                                                 [--workspace-name]
```

### az healthcareapis workspace iot-connector wait
```
az healthcareapis workspace iot-connector wait [--created]
                                               [--custom]
                                               [--deleted]
                                               [--exists]
                                               [--ids]
                                               [--interval]
                                               [--iot-connector-name]
                                               [--resource-group]
                                               [--subscription]
                                               [--timeout]
                                               [--updated]
                                               [--workspace-name]
```

## Azure Healthcare APIs IOT Connector FHIR Destination

### az healthcareapis workspace iot-connector fhir-destination create
```
az healthcareapis workspace iot-connector fhir-destination create --fhir-destination-name
                                                                  --fhir-service-resource-id
                                                                  --iot-connector-name
                                                                  --resource-group
                                                                  --resource-identity-resolution-type {Create, Lookup}
                                                                  --workspace-name
                                                                  [--content]
                                                                  [--etag]
                                                                  [--location]
                                                                  [--no-wait]
```

### az healthcareapis workspace iot-connector fhir-destination delete
```
az healthcareapis workspace iot-connector fhir-destination delete [--fhir-destination-name]
                                                                  [--ids]
                                                                  [--iot-connector-name]
                                                                  [--no-wait]
                                                                  [--resource-group]
                                                                  [--subscription]
                                                                  [--workspace-name]
                                                                  [--yes]
```

### az healthcareapis workspace iot-connector fhir-destination list
```
az healthcareapis workspace iot-connector fhir-destination list --iot-connector-name
                                                                --resource-group
                                                                --workspace-name
```

### az healthcareapis workspace iot-connector fhir-destination show
```
az healthcareapis workspace iot-connector fhir-destination show [--fhir-destination-name]
                                                                [--ids]
                                                                [--iot-connector-name]
                                                                [--resource-group]
                                                                [--subscription]
                                                                [--workspace-name]
```

### az healthcareapis workspace iot-connector fhir-destination update
```
az healthcareapis workspace iot-connector fhir-destination update --fhir-service-resource-id
                                                                  --resource-identity-resolution-type {Create, Lookup}
                                                                  [--add]
                                                                  [--content]
                                                                  [--etag]
                                                                  [--fhir-destination-name]
                                                                  [--force-string]
                                                                  [--ids]
                                                                  [--iot-connector-name]
                                                                  [--location]
                                                                  [--no-wait]
                                                                  [--remove]
                                                                  [--resource-group]
                                                                  [--set]
                                                                  [--subscription]
                                                                  [--workspace-name]
```

### az healthcareapis workspace iot-connector fhir-destination wait
```
az healthcareapis workspace iot-connector fhir-destination wait [--created]
                                                                [--custom]
                                                                [--deleted]
                                                                [--exists]
                                                                [--fhir-destination-name]
                                                                [--ids]
                                                                [--interval]
                                                                [--iot-connector-name]
                                                                [--resource-group]
                                                                [--subscription]
                                                                [--timeout]
                                                                [--updated]
                                                                [--workspace-name]
```

## Azure Healthcare APIs Workspace Private Endpoint Connection

### az healthcareapis workspace private-endpoint-connection create
```
az healthcareapis workspace private-endpoint-connection create --name
                                                               --resource-group
                                                               --workspace-name
                                                               [--no-wait]
                                                               [--private-link-service-connection-state]
```

### az healthcareapis workspace private-endpoint-connection delete
```
az healthcareapis workspace private-endpoint-connection delete [--ids]
                                                               [--name]
                                                               [--no-wait]
                                                               [--resource-group]
                                                               [--subscription]
                                                               [--workspace-name]
                                                               [--yes]
```

### az healthcareapis workspace private-endpoint-connection list
```
az healthcareapis workspace private-endpoint-connection list --resource-group
                                                             --workspace-name
```

### az healthcareapis workspace private-endpoint-connection show
```
az healthcareapis workspace private-endpoint-connection show [--ids]
                                                             [--name]
                                                             [--resource-group]
                                                             [--subscription]
                                                             [--workspace-name]
```

### az healthcareapis workspace private-endpoint-connection update
```
az healthcareapis workspace private-endpoint-connection update [--add]
                                                               [--force-string]
                                                               [--ids]
                                                               [--name]
                                                               [--no-wait]
                                                               [--private-link-service-connection-state]
                                                               [--remove]
                                                               [--resource-group]
                                                               [--set]
                                                               [--subscription]
                                                               [--workspace-name]
```

### az healthcareapis workspace private-endpoint-connection wait
```
az healthcareapis workspace private-endpoint-connection wait [--created]
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
                                                             [--workspace-name]
```

## Azure Healthcare APIs Workspace Private Link Resource

### az healthcareapis workspace private-link-resource list
```
az healthcareapis workspace private-link-resource list --resource-group
                                                       --workspace-name
```

### az healthcareapis workspace private-link-resource show
```
az healthcareapis workspace private-link-resource show [--group-name]
                                                       [--ids]
                                                       [--resource-group]
                                                       [--subscription]
                                                       [--workspace-name]
```

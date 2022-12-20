## Azure API Management

### az apim api create    
```
az apim api create --api-id
                   --display-name
                   --path
                   --resource-group
                   --service-name
                   [--api-type {graphql, http, soap, websocket}]
                   [--authorization-scope]
                   [--authorization-server-id]
                   [--bearer-token-sending-methods]
                   [--description]
                   [--no-wait]
                   [--open-id-provider-id]
                   [--protocols {http, https, ws, wss}]
                   [--service-url]
                   [--subscription-key-header-name]
                   [--subscription-key-query-param-name]
                   [--subscription-key-required]
                   [--subscription-required {false, true}]
```               
             
### az apim api delete
```
az apim api delete --api-id
                   --resource-group
                   --service-name
                   [--delete-revisions]
                   [--if-match]
                   [--no-wait]
                   [--yes]
```                   
                   
### az apim api import
```
az apim api import --path
                   --resource-group
                   --service-name
                   --specification-format {GraphQL, OpenApi, OpenApiJson, Swagger, Wadl, Wsdl}
                   [--api-id]
                   [--api-revision]
                   [--api-type {graphql, http, soap, websocket}]
                   [--api-version]
                   [--api-version-set-id]
                   [--description]
                   [--display-name]
                   [--no-wait]
                   [--protocols {http, https, ws, wss}]
                   [--service-url]
                   [--soap-api-type]
                   [--specification-path]
                   [--specification-url]
                   [--subscription-key-header-name]
                   [--subscription-key-query-param-name]
                   [--subscription-required {false, true}]
                   [--wsdl-endpoint-name]
                   [--wsdl-service-name]
```                
                   
### az apim api list
```
az apim api list --resource-group
                 --service-name
                 [--filter-display-name]
                 [--skip]
                 [--top]
```

### az apim api show
```
az apim api show --api-id
                 --resource-group
                 --service-name
```

### az apim api update
```
az apim api update --api-id
                   --resource-group
                   --service-name
                   [--add]
                   [--api-type {graphql, http, soap, websocket}]
                   [--description]
                   [--display-name]
                   [--force-string]
                   [--if-match]
                   [--no-wait]
                   [--path]
                   [--protocols {http, https, ws, wss}]
                   [--remove]
                   [--service-url]
                   [--set]
                   [--subscription-key-header-name]
                   [--subscription-key-query-param-name]
                   [--subscription-required {false, true}]
                   [--tags]
```

### az apim api wait
```
az apim api wait --api-id
                 --name
                 --resource-group
                 [--created]
                 [--custom]
                 [--deleted]
                 [--exists]
                 [--interval]
                 [--timeout]
                 [--updated]
```

## Azure API Management Operation

### az apim api operation create
```
az apim api operation create --api-id
                             --display-name
                             --method
                             --resource-group
                             --service-name
                             --url-template
                             [--description]
                             [--if-match]
                             [--operation-id]
                             [--params]
```

### az apim api operation delete
```
az apim api operation delete --api-id
                             --operation-id
                             --resource-group
                             --service-name
                             [--if-match]
```

### az apim api operation list
```
az apim api operation list --api-id
                           --resource-group
                           --service-name
```

### az apim api operation show
```
az apim api operation show --api-id
                           --operation-id
                           --resource-group
                           --service-name
```

### az apim api operation update
```
az apim api operation update --api-id
                             --operation-id
                             --resource-group
                             --service-name
                             [--add]
                             [--description]
                             [--display-name]
                             [--force-string]
                             [--if-match]
                             [--method]
                             [--remove]
                             [--set]
                             [--url-template]
```

## Azure API Management Release

### az apim api release create
```
az apim api release create --api-id
                           --api-revision
                           --resource-group
                           --service-name
                           [--if-match]
                           [--notes]
                           [--release-id]
```

### az apim api release delete
```
az apim api release delete --api-id
                           --release-id
                           --resource-group
                           --service-name
                           [--if-match]
```

### az apim api release list
```
az apim api release list --api-id
                         --resource-group
                         --service-name
```

### az apim api release show
```
az apim api release show --api-id
                         --release-id
                         --resource-group
                         --service-name
```

### az apim api release update
```
az apim api release update --api-id
                           --release-id
                           --resource-group
                           --service-name
                           [--add]
                           [--force-string]
                           [--if-match]
                           [--notes]
                           [--remove]
                           [--set]
```

## Azure API Management Revision

### az apim api revision create
```
az apim api revision create --api-id
                            --api-revision
                            --resource-group
                            --service-name
                            [--api-revision-description]
```

### az apim api revision list
```
az apim api revision list --api-id
                          --resource-group
                          --service-name
```

## Azure API Management Schema

### az apim api schema create
```
az apim api schema create --api-id
                          --resource-group
                          --schema-id
                          --schema-type
                          --service-name
                          [--no-wait]
                          [--resource-type]
                          [--schema-content]
                          [--schema-name]
                          [--schema-path]
```

### az apim api schema delete
```
az apim api schema delete --api-id
                          --resource-group
                          --schema-id
                          --service-name
                          [--if-match]
                          [--no-wait]
                          [--yes]
```

### az apim api schema get-etag
```
az apim api schema get-etag --api-id
                            --resource-group
                            --schema-id
                            --service-name
```

### az apim api schema list
```
az apim api schema list --api-id
                        --resource-group
                        --service-name
                        [--filter-display-name]
                        [--skip]
                        [--top]
```

### az apim api schema show
```
az apim api schema show --api-id
                        --resource-group
                        --schema-id
                        --service-name
```

### az apim api schema wait
```
az apim api schema wait --api-id
                        --name
                        --resource-group
                        --schema-id
                        [--created]
                        [--custom]
                        [--deleted]
                        [--exists]
                        [--interval]
                        [--timeout]
                        [--updated]
```

## Azure API Management Version Set

### az apim api versionset create
```
az apim api versionset create --display-name
                              --resource-group
                              --service-name
                              --versioning-scheme
                              [--description]
                              [--if-match]
                              [--version-header-name]
                              [--version-query-name]
                              [--version-set-id]
```

### az apim api versionset delete
```
az apim api versionset delete --resource-group
                              --service-name
                              --version-set-id
                              [--if-match]
```

### az apim api versionset list
```
az apim api versionset list --resource-group
                            --service-name
```

### az apim api versionset show
```
az apim api versionset show --resource-group
                            --service-name
                            --version-set-id
```

### az apim api versionset update
```
az apim api versionset update --resource-group
                              --service-name
                              --version-set-id
                              [--add]
                              [--description]
                              [--display-name]
                              [--force-string]
                              [--if-match]
                              [--remove]
                              [--set]
                              [--version-header-name]
                              [--version-query-name]
                              [--versioning-scheme]
```

## Azure API Management Deleted Services

### az apim deletedservice list
```
az apim deletedservice list
```

### az apim deletedservice purge
```
az apim deletedservice purge --location
                             --service-name
```

### az apim deletedservice show
```
az apim deletedservice show --location
                            --service-name
```

## Azure API Management Named Values

### az apim nv create
```
az apim nv create --display-name
                  --named-value-id
                  --resource-group
                  --service-name
                  [--if-match]
                  [--no-wait]
                  [--secret {false, true}]
                  [--tags]
                  [--value]
```

### az apim nv delete
```
az apim nv delete --named-value-id
                  --resource-group
                  --service-name
                  [--yes]
```

### az apim nv list
```
az apim nv list --resource-group
                --service-name
```

### az apim nv show
```
az apim nv show --named-value-id
                --resource-group
                --service-name
```

### az apim nv show-secret
```
az apim nv show-secret --named-value-id
                       --resource-group
                       --service-name
```

### az apim nv update
```
az apim nv update --named-value-id
                  --resource-group
                  --service-name
                  [--add]
                  [--force-string]
                  [--if-match]
                  [--remove]
                  [--secret {false, true}]
                  [--set]
                  [--tags]
                  [--value]
```

### az apim nv wait
```
az apim nv wait --named-value-id
                --resource-group
                --service-name
                [--created]
                [--custom]
                [--deleted]
                [--exists]
                [--interval]
                [--timeout]
                [--updated]
```

## Azure API Management Product

### az apim product create
```
az apim product create --product-name
                       --resource-group
                       --service-name
                       [--approval-required {false, true}]
                       [--description]
                       [--legal-terms]
                       [--no-wait]
                       [--product-id]
                       [--state {notPublished, published}]
                       [--subscription-required {false, true}]
                       [--subscriptions-limit]
```

### az apim product delete
```
az apim product delete --product-id
                       --resource-group
                       --service-name
                       [--delete-subscriptions]
                       [--if-match]
                       [--no-wait]
                       [--yes]
```

### az apim product list
```
az apim product list --resource-group
                     --service-name
```

### az apim product show
```
az apim product show --product-id
                     --resource-group
                     --service-name
```

### az apim product update
```
az apim product update --product-id
                       --resource-group
                       --service-name
                       [--add]
                       [--approval-required {false, true}]
                       [--description]
                       [--force-string]
                       [--if-match]
                       [--legal-terms]
                       [--no-wait]
                       [--product-name]
                       [--remove]
                       [--set]
                       [--state {notPublished, published}]
                       [--subscription-required {false, true}]
                       [--subscriptions-limit]
```

### az apim product wait
```
az apim product wait --product-id
                     --resource-group
                     --service-name
                     [--created]
                     [--custom]
                     [--deleted]
                     [--exists]
                     [--interval]
                     [--timeout]
                     [--updated]
```

### az apim product api add
```
az apim product api add --api-id
                        --product-id
                        --resource-group
                        --service-name
```

### az apim product api check
```
az apim product api check --api-id
                          --product-id
                          --resource-group
                          --service-name
```

### az apim product api delete
```
az apim product api delete --api-id
                           --product-id
                           --resource-group
                           --service-name
```

### az apim product api list
```
az apim product api list --product-id
                         --resource-group
                         --service-name
```


# Azure App Service Webapp

### az webapp browse
```
az webapp browse [--ids]
                 [--logs]
                 [--name]
                 [--resource-group]
                 [--slot]
                 [--subscription]
```

### az webapp create
```
az webapp create --name
                 --plan
                 --resource-group
                 [--assign-identity]
                 [--deployment-container-image-name]
                 [--deployment-local-git]
                 [--deployment-source-branch]
                 [--deployment-source-url]
                 [--docker-registry-server-password]
                 [--docker-registry-server-user]
                 [--https-only {false, true}]
                 [--multicontainer-config-file]
                 [--multicontainer-config-type {COMPOSE, KUBE}]
                 [--public-network-access {Disabled, Enabled}]
                 [--role]
                 [--runtime]
                 [--scope]
                 [--startup-file]
                 [--subnet]
                 [--tags]
                 [--vnet]
```

### az webapp create-remote-connection
```
az webapp create-remote-connection [--ids]
                                   [--instance]
                                   [--name]
                                   [--port]
                                   [--resource-group]
                                   [--slot]
                                   [--subscription]
                                   [--timeout]
```

### az webapp delete
```
az webapp delete [--ids]
                 [--keep-dns-registration]
                 [--keep-empty-plan]
                 [--keep-metrics]
                 [--name]
                 [--resource-group]
                 [--slot]
                 [--subscription]
```

### az webapp deploy
```
az webapp deploy [--async {false, true}]
                 [--clean {false, true}]
                 [--ids]
                 [--ignore-stack {false, true}]
                 [--name]
                 [--resource-group]
                 [--restart {false, true}]
                 [--slot]
                 [--src-path]
                 [--src-url]
                 [--subscription]
                 [--target-path]
                 [--timeout]
                 [--type {ear, jar, lib, startup, static, war, zip}]
```

### az webapp list
```
az webapp list [--resource-group]
```

### az webapp list-instances
```
az webapp list-instances --name
                         --resource-group
                         [--slot]
```

### az webapp list-runtimes
```
az webapp list-runtimes [--linux]
                        [--os {linux, windows}]
```

### az webapp restart
```
az webapp restart [--ids]
                  [--name]
                  [--resource-group]
                  [--slot]
                  [--subscription]
```

### az webapp scale
```
az webapp scale --instance-count
                [--ids]
                [--name]
                [--resource-group]
                [--slot]
                [--subscription]
```

### az webapp show
```
az webapp show [--ids]
               [--name]
               [--resource-group]
               [--slot]
               [--subscription]
```

### az webapp ssh
```
az webapp ssh [--ids]
              [--instance]
              [--name]
              [--port]
              [--resource-group]
              [--slot]
              [--subscription]
              [--timeout]
```

### az webapp start
```
az webapp start [--ids]
                [--name]
                [--resource-group]
                [--slot]
                [--subscription]
```

### az webapp stop
```
az webapp stop [--ids]
               [--name]
               [--resource-group]
               [--slot]
               [--subscription]
```

### az webapp up
```
az webapp up [--app-service-environment]
             [--dryrun]
             [--html]
             [--ids]
             [--launch-browser]
             [--location]
             [--logs]
             [--name]
             [--os-type {Linux, Windows}]
             [--plan]
             [--resource-group]
             [--runtime]
             [--sku {B1, B2, B3, D1, F1, FREE, I1, I1v2, I2, I2v2, I3, I3v2, I4v2, I5v2, I6v2, P1V2, P1V3, P2V2, P2V3, P3V2, P3V3, S1, S2, S3, SHARED, WS1, WS2, WS3}]
             [--subscription]
```

### az webapp update
```
az webapp update [--add]
                 [--client-affinity-enabled {false, true}]
                 [--force-dns-registration {false, true}]
                 [--force-string]
                 [--https-only {false, true}]
                 [--ids]
                 [--minimum-elastic-instance-count]
                 [--name]
                 [--prewarmed-instance-count]
                 [--remove]
                 [--resource-group]
                 [--set]
                 [--skip-custom-domain-verification {false, true}]
                 [--skip-dns-registration {false, true}]
                 [--slot]
                 [--subscription]
                 [--ttl-in-seconds {false, true}]
```

## Azure Webapp Auth

### az webapp auth set
```
az webapp auth set [--body]
                   [--ids]
                   [--name]
                   [--resource-group]
                   [--slot]
                   [--subscription]
```

### az webapp auth show
```
az webapp auth show [--ids]
                    [--name]
                    [--resource-group]
                    [--slot]
                    [--subscription]
```

### az webapp auth update
```
az webapp auth update [--aad-allowed-token-audiences]
                      [--aad-client-id]
                      [--aad-client-secret]
                      [--aad-client-secret-certificate-thumbprint]
                      [--aad-token-issuer-url]
                      [--action {AllowAnonymous, LoginWithAzureActiveDirectory, LoginWithFacebook, LoginWithGoogle, LoginWithMicrosoftAccount, LoginWithTwitter}]
                      [--allowed-external-redirect-urls]
                      [--enabled {false, true}]
                      [--facebook-app-id]
                      [--facebook-app-secret]
                      [--facebook-oauth-scopes]
                      [--google-client-id]
                      [--google-client-secret]
                      [--google-oauth-scopes]
                      [--ids]
                      [--microsoft-account-client-id]
                      [--microsoft-account-client-secret]
                      [--microsoft-account-oauth-scopes]
                      [--name]
                      [--resource-group]
                      [--runtime-version]
                      [--slot]
                      [--subscription]
                      [--token-refresh-extension-hours]
                      [--token-store {false, true}]
                      [--twitter-consumer-key]
                      [--twitter-consumer-secret]
```

## Azure Webapp Auth Apple

### az webapp auth apple show
```
az webapp auth apple show [--ids]
                          [--name]
                          [--resource-group]
                          [--slot]
                          [--subscription]
```

### az webapp auth apple update
```
az webapp auth apple update [--client-id]
                            [--client-secret]
                            [--client-secret-setting-name]
                            [--ids]
                            [--name]
                            [--resource-group]
                            [--scopes]
                            [--slot]
                            [--subscription]
                            [--yes]
```

## Azure Webapp Auth Configuration Version

### az webapp auth config-version revert
```
az webapp auth config-version revert [--ids]
                                     [--name]
                                     [--resource-group]
                                     [--slot]
                                     [--subscription]
```

### az webapp auth config-version show
```
az webapp auth config-version show [--ids]
                                   [--name]
                                   [--resource-group]
                                   [--slot]
                                   [--subscription]
```

### az webapp auth config-version upgrade
```
az webapp auth config-version upgrade [--ids]
                                      [--name]
                                      [--resource-group]
                                      [--slot]
                                      [--subscription]
```

## Azure Webapp Auth Facebook

### az webapp auth facebook show
```
az webapp auth facebook show [--ids]
                             [--name]
                             [--resource-group]
                             [--slot]
                             [--subscription]
```

### az webapp auth facebook update
```
az webapp auth facebook update [--app-id]
                               [--app-secret]
                               [--app-secret-setting-name]
                               [--graph-api-version]
                               [--ids]
                               [--name]
                               [--resource-group]
                               [--scopes]
                               [--slot]
                               [--subscription]
                               [--yes]
```

## Azure Webapp Auth Github

### az webapp auth github show
```
az webapp auth github show [--ids]
                           [--name]
                           [--resource-group]
                           [--slot]
                           [--subscription]
```

### az webapp auth github update
```
az webapp auth github update [--client-id]
                             [--client-secret]
                             [--client-secret-setting-name]
                             [--ids]
                             [--name]
                             [--resource-group]
                             [--scopes]
                             [--slot]
                             [--subscription]
                             [--yes]
```

## Azure Webapp Auth Google

### az webapp auth google show
```
az webapp auth google show [--ids]
                           [--name]
                           [--resource-group]
                           [--slot]
                           [--subscription]
```

### az webapp auth google update
```
az webapp auth google update [--allowed-audiences]
                             [--client-id]
                             [--client-secret]
                             [--client-secret-setting-name]
                             [--ids]
                             [--name]
                             [--resource-group]
                             [--scopes]
                             [--slot]
                             [--subscription]
                             [--yes]
```

## Azure Webapp Auth Microsoft

### az webapp auth microsoft show
```
az webapp auth microsoft show [--ids]
                              [--name]
                              [--resource-group]
                              [--slot]
                              [--subscription]
```

### az webapp auth microsoft update
```
az webapp auth microsoft update [--allowed-audiences]
                                [--client-id]
                                [--client-secret]
                                [--client-secret-setting-name]
                                [--ids]
                                [--issuer]
                                [--name]
                                [--resource-group]
                                [--slot]
                                [--subscription]
                                [--tenant-id]
                                [--yes]
```

## Azure Webapp Auth OpenID Connect

### az webapp auth openid-connect add
```
az webapp auth openid-connect add --provider-name
                                  [--client-id]
                                  [--client-secret]
                                  [--client-secret-setting-name]
                                  [--ids]
                                  [--name]
                                  [--openid-configuration]
                                  [--resource-group]
                                  [--scopes]
                                  [--slot]
                                  [--subscription]
                                  [--yes]
```

### az webapp auth openid-connect remove
```
az webapp auth openid-connect remove --provider-name
                                     [--ids]
                                     [--name]
                                     [--resource-group]
                                     [--slot]
                                     [--subscription]
```

### az webapp auth openid-connect show
```
az webapp auth openid-connect show --provider-name
                                   [--ids]
                                   [--name]
                                   [--resource-group]
                                   [--slot]
                                   [--subscription]
```

### az webapp auth openid-connect update
```
az webapp auth openid-connect update --provider-name
                                     [--client-id]
                                     [--client-secret]
                                     [--client-secret-setting-name]
                                     [--ids]
                                     [--name]
                                     [--openid-configuration]
                                     [--resource-group]
                                     [--scopes]
                                     [--slot]
                                     [--subscription]
                                     [--yes]
```

## Azure Webapp Auth Twitter

### az webapp auth twitter show
```
az webapp auth twitter show [--ids]
                            [--name]
                            [--resource-group]
                            [--slot]
                            [--subscription]
```

### az webapp auth twitter update
```
az webapp auth twitter update [--consumer-key]
                              [--consumer-secret]
                              [--consumer-secret-setting-name]
                              [--ids]
                              [--name]
                              [--resource-group]
                              [--slot]
                              [--subscription]
                              [--yes]
```

## Azure Webapp Classic Auth

### az webapp auth-classic show
```
az webapp auth-classic show [--ids]
                            [--name]
                            [--resource-group]
                            [--slot]
                            [--subscription]
```

### az webapp auth-classic update
```
az webapp auth-classic update [--aad-allowed-token-audiences]
                              [--aad-client-id]
                              [--aad-client-secret]
                              [--aad-client-secret-certificate-thumbprint]
                              [--aad-client-secret-setting-name]
                              [--aad-token-issuer-url]
                              [--action {AllowAnonymous, LoginWithAzureActiveDirectory, LoginWithFacebook, LoginWithGoogle, LoginWithMicrosoftAccount, LoginWithTwitter}]
                              [--allowed-redirect-urls]
                              [--enabled {false, true}]
                              [--facebook-app-id]
                              [--facebook-app-secret]
                              [--facebook-app-secret-setting-name]
                              [--facebook-oauth-scopes]
                              [--github-client-id]
                              [--github-client-secret]
                              [--github-client-secret-setting-name]
                              [--github-oauth-scopes]
                              [--google-client-id]
                              [--google-client-secret]
                              [--google-client-secret-setting-name]
                              [--google-oauth-scopes]
                              [--ids]
                              [--microsoft-account-client-id]
                              [--microsoft-account-client-secret]
                              [--microsoft-account-client-secret-setting-name]
                              [--microsoft-account-oauth-scopes]
                              [--name]
                              [--resource-group]
                              [--runtime-version]
                              [--slot]
                              [--subscription]
                              [--token-refresh-extension-hours]
                              [--token-store {false, true}]
                              [--twitter-consumer-key]
                              [--twitter-consumer-secret]
                              [--twitter-consumer-secret-setting-name]
```

## Azure Webapp Configuration

### az webapp config set
```
az webapp config set [--always-on {false, true}]
                     [--auto-heal-enabled {false, true}]
                     [--ftps-state {AllAllowed, Disabled, FtpsOnly}]
                     [--generic-configurations]
                     [--http20-enabled {false, true}]
                     [--ids]
                     [--java-container]
                     [--java-container-version]
                     [--java-version]
                     [--linux-fx-version]
                     [--min-tls-version]
                     [--name]
                     [--net-framework-version]
                     [--number-of-workers]
                     [--php-version]
                     [--prewarmed-instance-count]
                     [--python-version]
                     [--remote-debugging-enabled {false, true}]
                     [--resource-group]
                     [--slot]
                     [--startup-file]
                     [--subscription]
                     [--use-32bit-worker-process {false, true}]
                     [--vnet-route-all-enabled {false, true}]
                     [--web-sockets-enabled {false, true}]
                     [--windows-fx-version]
```

### az webapp config show
```
az webapp config show [--ids]
                      [--name]
                      [--resource-group]
                      [--slot]
                      [--subscription]
```

## Azure Webapp Access Restriction

### az webapp config access-restriction add
```
az webapp config access-restriction add --priority
                                        [--action {Allow, Deny}]
                                        [--description]
                                        [--http-headers]
                                        [--ids]
                                        [--ignore-missing-endpoint {false, true}]
                                        [--ip-address]
                                        [--name]
                                        [--resource-group]
                                        [--rule-name]
                                        [--scm-site {false, true}]
                                        [--service-tag]
                                        [--slot]
                                        [--subnet]
                                        [--subscription]
                                        [--vnet-name]
                                        [--vnet-resource-group]
```

### az webapp config access-restriction remove
```
az webapp config access-restriction remove [--action {Allow, Deny}]
                                           [--ids]
                                           [--ip-address]
                                           [--name]
                                           [--resource-group]
                                           [--rule-name]
                                           [--scm-site {false, true}]
                                           [--service-tag]
                                           [--slot]
                                           [--subnet]
                                           [--subscription]
                                           [--vnet-name]
```

### az webapp config access-restriction set
```
az webapp config access-restriction set --use-same-restrictions-for-scm-site {false, true}
                                        [--ids]
                                        [--name]
                                        [--resource-group]
                                        [--slot]
                                        [--subscription]
```

### az webapp config access-restriction show
```
az webapp config access-restriction show [--ids]
                                         [--name]
                                         [--resource-group]
                                         [--slot]
                                         [--subscription]
```

## Azure Webapp Settings

### az webapp config appsettings delete
```
az webapp config appsettings delete --setting-names
                                    [--ids]
                                    [--name]
                                    [--resource-group]
                                    [--slot]
                                    [--subscription]
```

### az webapp config appsettings list
```
az webapp config appsettings list --name
                                  --resource-group
                                  [--slot]
```

### az webapp config appsettings set
```
az webapp config appsettings set [--ids]
                                 [--name]
                                 [--resource-group]
                                 [--settings]
                                 [--slot]
                                 [--slot-settings]
                                 [--subscription]
```

## Azure Webapp Backup

### az webapp config backup create
```
az webapp config backup create --container-url
                               --resource-group
                               --webapp-name
                               [--backup-name]
                               [--db-connection-string]
                               [--db-name]
                               [--db-type {LocalMySql, MySql, PostgreSql, SqlAzure}]
                               [--slot]
```

### az webapp config backup list
```
az webapp config backup list --resource-group
                             --webapp-name
                             [--slot]
```

### az webapp config backup restore
```
az webapp config backup restore --backup-name
                                --container-url
                                --resource-group
                                --webapp-name
                                [--db-connection-string]
                                [--db-name]
                                [--db-type {LocalMySql, MySql, PostgreSql, SqlAzure}]
                                [--ignore-hostname-conflict]
                                [--overwrite]
                                [--slot]
                                [--target-name]
```

### az webapp config backup show
```
az webapp config backup show --resource-group
                             --webapp-name
                             [--slot]
```

### az webapp config backup update
```
az webapp config backup update --resource-group
                               --webapp-name
                               [--backup-name]
                               [--container-url]
                               [--db-connection-string]
                               [--db-name]
                               [--db-type {LocalMySql, MySql, PostgreSql, SqlAzure}]
                               [--frequency]
                               [--retain-one {false, true}]
                               [--retention]
                               [--slot]
```

## Azure Webapp Connection String

### az webapp config connection-string delete
```
az webapp config connection-string delete --setting-names
                                          [--ids]
                                          [--name]
                                          [--resource-group]
                                          [--slot]
                                          [--subscription]
```

### az webapp config connection-string list
```
az webapp config connection-string list --name
                                        --resource-group
                                        [--slot]
```

### az webapp config connection-string set
```
az webapp config connection-string set --connection-string-type {ApiHub, Custom, DocDb, EventHub, MySql, NotificationHub, PostgreSQL, RedisCache, SQLAzure, SQLServer, ServiceBus}
                                       [--ids]
                                       [--name]
                                       [--resource-group]
                                       [--settings]
                                       [--slot]
                                       [--slot-settings]
                                       [--subscription]
```

## Azure Webapp Container Settings

### az webapp config container delete
```
az webapp config container delete [--ids]
                                  [--name]
                                  [--resource-group]
                                  [--slot]
                                  [--subscription]
```

### az webapp config container set
```
az webapp config container set [--docker-custom-image-name]
                               [--docker-registry-server-password]
                               [--docker-registry-server-url]
                               [--docker-registry-server-user]
                               [--enable-app-service-storage {false, true}]
                               [--ids]
                               [--multicontainer-config-file]
                               [--multicontainer-config-type {COMPOSE, KUBE}]
                               [--name]
                               [--resource-group]
                               [--slot]
                               [--subscription]
```

### az webapp config container show
```
az webapp config container show [--ids]
                                [--name]
                                [--resource-group]
                                [--show-multicontainer-config]
                                [--slot]
                                [--subscription]
```

## Azure Webapp Hostname Configuration

### az webapp config hostname add
```
az webapp config hostname add [--hostname]
                              [--ids]
                              [--resource-group]
                              [--slot]
                              [--subscription]
                              [--webapp-name]
```

### az webapp config hostname delete
```
az webapp config hostname delete [--hostname]
                                 [--ids]
                                 [--resource-group]
                                 [--slot]
                                 [--subscription]
                                 [--webapp-name]
```

### az webapp config hostname get-external-ip
```
az webapp config hostname get-external-ip [--ids]
                                          [--resource-group]
                                          [--subscription]
                                          [--webapp-name]
```

### az webapp config hostname list
```
az webapp config hostname list --resource-group
                               --webapp-name
                               [--slot]
```

## Azure Webapp Snapshot

### az webapp config snapshot list
```
az webapp config snapshot list --name
                               --resource-group
                               [--slot]
```

### az webapp config snapshot restore
```
az webapp config snapshot restore --time
                                  [--ids]
                                  [--name]
                                  [--resource-group]
                                  [--restore-content-only]
                                  [--slot]
                                  [--source-name]
                                  [--source-resource-group]
                                  [--source-slot]
                                  [--subscription]
```

## Azure Webapp SSL Certificates

### az webapp config ssl bind
```
az webapp config ssl bind --certificate-thumbprint
                          --ssl-type {IP, SNI}
                          [--ids]
                          [--name]
                          [--resource-group]
                          [--slot]
                          [--subscription]
```

### az webapp config ssl create
```
az webapp config ssl create --hostname
                            --name
                            --resource-group
                            [--slot]
```

### az webapp config ssl delete
```
az webapp config ssl delete --certificate-thumbprint
                            --resource-group
```

### az webapp config ssl import
```
az webapp config ssl import --key-vault
                            --key-vault-certificate-name
                            [--ids]
                            [--name]
                            [--resource-group]
                            [--subscription]
```

### az webapp config ssl list
```
az webapp config ssl list --resource-group
```

### az webapp config ssl show
```
az webapp config ssl show --certificate-name
                          --resource-group
```

### az webapp config ssl unbind
```
az webapp config ssl unbind --certificate-thumbprint
                            [--ids]
                            [--name]
                            [--resource-group]
                            [--slot]
                            [--subscription]
```

### az webapp config ssl upload
```
az webapp config ssl upload --certificate-file
                            --certificate-password
                            [--ids]
                            [--name]
                            [--resource-group]
                            [--slot]
                            [--subscription]
```

## Azure Webapp Storage Account

### az webapp config storage-account add
```
az webapp config storage-account add --access-key
                                     --account-name
                                     --custom-id
                                     --share-name
                                     --storage-type {AzureBlob, AzureFiles}
                                     [--ids]
                                     [--mount-path]
                                     [--name]
                                     [--resource-group]
                                     [--slot]
                                     [--slot-setting]
                                     [--subscription]
```

### az webapp config storage-account delete
```
az webapp config storage-account delete --custom-id
                                        [--ids]
                                        [--name]
                                        [--resource-group]
                                        [--slot]
                                        [--subscription]
```

### az webapp config storage-account list
```
az webapp config storage-account list --name
                                      --resource-group
                                      [--slot]
```

### az webapp config storage-account update
```
az webapp config storage-account update --custom-id
                                        [--access-key]
                                        [--account-name]
                                        [--ids]
                                        [--mount-path]
                                        [--name]
                                        [--resource-group]
                                        [--share-name]
                                        [--slot]
                                        [--slot-setting]
                                        [--storage-type {AzureBlob, AzureFiles}]
                                        [--subscription]
```

## Azure Webapp Connection

### az webapp connection delete
```
az webapp connection delete [--connection]
                            [--id]
                            [--name]
                            [--no-wait]
                            [--resource-group]
                            [--yes]
```

### az webapp connection list
```
az webapp connection list [--name]
                          [--resource-group]
                          [--source-id]
```

### az webapp connection list-configuration
```
az webapp connection list-configuration [--connection]
                                        [--id]
                                        [--name]
                                        [--resource-group]
```

### az webapp connection list-support-types
```
az webapp connection list-support-types [--target-type {appconfig, confluent-cloud, cosmos-cassandra, cosmos-gremlin, cosmos-mongo, cosmos-sql, cosmos-table, eventhub, keyvault, mysql, mysql-flexible, postgres, postgres-flexible, redis, redis-enterprise, servicebus, signalr, sql, storage-blob, storage-file, storage-queue, storage-table, webpubsub}]
```

### az webapp connection show
```
az webapp connection show [--connection]
                          [--id]
                          [--name]
                          [--resource-group]
```

### az webapp connection validate
```
az webapp connection validate [--connection]
                              [--id]
                              [--name]
                              [--resource-group]
```

### az webapp connection wait
```
az webapp connection wait [--connection]
                          [--created]
                          [--custom]
                          [--deleted]
                          [--exists]
                          [--id]
                          [--interval]
                          [--name]
                          [--resource-group]
                          [--timeout]
                          [--updated]
```

## Azure Webapp Create Connection

### az webapp connection create appconfig
```
az webapp connection create appconfig [--app-config]
                                      [--client-type {dotnet, java, nodejs, none, python}]
                                      [--connection]
                                      [--name]
                                      [--no-wait]
                                      [--private-endpoint {false, true}]
                                      [--resource-group]
                                      [--secret]
                                      [--service-principal]
                                      [--source-id]
                                      [--system-identity]
                                      [--target-id]
                                      [--target-resource-group]
                                      [--user-identity]
                                      [--vault-id]
```

### az webapp connection create confluent-cloud
```
az webapp connection create confluent-cloud --bootstrap-server
                                            --kafka-key
                                            --kafka-secret
                                            --schema-key
                                            --schema-registry
                                            --schema-secret
                                            [--client-type {dotnet, go, java, none, python, springBoot}]
                                            [--connection]
                                            [--name]
                                            [--no-wait]
                                            [--resource-group]
                                            [--source-id]
                                            [--vault-id]
```

### az webapp connection create cosmos-cassandra
```
az webapp connection create cosmos-cassandra [--account]
                                             [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                             [--connection]
                                             [--key-space]
                                             [--name]
                                             [--no-wait]
                                             [--private-endpoint {false, true}]
                                             [--resource-group]
                                             [--secret]
                                             [--service-endpoint {false, true}]
                                             [--service-principal]
                                             [--source-id]
                                             [--system-identity]
                                             [--target-id]
                                             [--target-resource-group]
                                             [--user-identity]
                                             [--vault-id]
```

### az webapp connection create cosmos-gremlin
```
az webapp connection create cosmos-gremlin [--account]
                                           [--client-type {dotnet, java, nodejs, none, php, python}]
                                           [--connection]
                                           [--database]
                                           [--graph]
                                           [--name]
                                           [--no-wait]
                                           [--private-endpoint {false, true}]
                                           [--resource-group]
                                           [--secret]
                                           [--service-endpoint {false, true}]
                                           [--service-principal]
                                           [--source-id]
                                           [--system-identity]
                                           [--target-id]
                                           [--target-resource-group]
                                           [--user-identity]
                                           [--vault-id]
```

### az webapp connection create cosmos-mongo
```
az webapp connection create cosmos-mongo [--account]
                                         [--client-type {dotnet, go, java, nodejs, none, springBoot}]
                                         [--connection]
                                         [--database]
                                         [--name]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--service-principal]
                                         [--source-id]
                                         [--system-identity]
                                         [--target-id]
                                         [--target-resource-group]
                                         [--user-identity]
                                         [--vault-id]
```

### az webapp connection create cosmos-sql
```
az webapp connection create cosmos-sql [--account]
                                       [--client-type {dotnet, java, nodejs, none, python}]
                                       [--connection]
                                       [--database]
                                       [--name]
                                       [--no-wait]
                                       [--private-endpoint {false, true}]
                                       [--resource-group]
                                       [--secret]
                                       [--service-endpoint {false, true}]
                                       [--service-principal]
                                       [--source-id]
                                       [--system-identity]
                                       [--target-id]
                                       [--target-resource-group]
                                       [--user-identity]
                                       [--vault-id]
```

### az webapp connection create cosmos-table
```
az webapp connection create cosmos-table [--account]
                                         [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                         [--connection]
                                         [--name]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--service-principal]
                                         [--source-id]
                                         [--system-identity]
                                         [--table]
                                         [--target-id]
                                         [--target-resource-group]
                                         [--user-identity]
                                         [--vault-id]
```

### az webapp connection create eventhub
```
az webapp connection create eventhub [--client-type {dotnet, go, java, kafka-springBoot, nodejs, none, python, springBoot}]
                                     [--connection]
                                     [--name]
                                     [--namespace]
                                     [--no-wait]
                                     [--private-endpoint {false, true}]
                                     [--resource-group]
                                     [--secret]
                                     [--service-endpoint {false, true}]
                                     [--service-principal]
                                     [--source-id]
                                     [--system-identity]
                                     [--target-id]
                                     [--target-resource-group]
                                     [--user-identity]
                                     [--vault-id]
```

### az webapp connection create keyvault
```
az webapp connection create keyvault [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                     [--connection]
                                     [--name]
                                     [--new {false, true}]
                                     [--no-wait]
                                     [--private-endpoint {false, true}]
                                     [--resource-group]
                                     [--service-endpoint {false, true}]
                                     [--service-principal]
                                     [--source-id]
                                     [--system-identity]
                                     [--target-id]
                                     [--target-resource-group]
                                     [--user-identity]
                                     [--vault]
                                     [--vault-id]
```

### az webapp connection create mysql
```
az webapp connection create mysql [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                  [--config-connstr {false, true}]
                                  [--connection]
                                  [--database]
                                  [--name]
                                  [--no-wait]
                                  [--private-endpoint {false, true}]
                                  [--resource-group]
                                  [--secret]
                                  [--server]
                                  [--service-endpoint {false, true}]
                                  [--source-id]
                                  [--target-id]
                                  [--target-resource-group]
                                  [--vault-id]
```

### az webapp connection create mysql-flexible
```
az webapp connection create mysql-flexible [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                           [--config-connstr {false, true}]
                                           [--connection]
                                           [--database]
                                           [--name]
                                           [--no-wait]
                                           [--resource-group]
                                           [--secret]
                                           [--server]
                                           [--source-id]
                                           [--system-identity]
                                           [--target-id]
                                           [--target-resource-group]
                                           [--vault-id]
```

### az webapp connection create postgres
```
az webapp connection create postgres [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                     [--config-connstr {false, true}]
                                     [--connection]
                                     [--database]
                                     [--name]
                                     [--new {false, true}]
                                     [--no-wait]
                                     [--private-endpoint {false, true}]
                                     [--resource-group]
                                     [--secret]
                                     [--server]
                                     [--service-endpoint {false, true}]
                                     [--source-id]
                                     [--system-identity]
                                     [--target-id]
                                     [--target-resource-group]
                                     [--vault-id]
```

### az webapp connection create postgres-flexible
```
az webapp connection create postgres-flexible [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                              [--config-connstr {false, true}]
                                              [--connection]
                                              [--database]
                                              [--name]
                                              [--no-wait]
                                              [--resource-group]
                                              [--secret]
                                              [--server]
                                              [--source-id]
                                              [--system-identity]
                                              [--target-id]
                                              [--target-resource-group]
                                              [--vault-id]
```

### az webapp connection create redis
```
az webapp connection create redis [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                  [--connection]
                                  [--database]
                                  [--name]
                                  [--no-wait]
                                  [--private-endpoint {false, true}]
                                  [--resource-group]
                                  [--secret]
                                  [--server]
                                  [--source-id]
                                  [--target-id]
                                  [--target-resource-group]
                                  [--vault-id]
```

### az webapp connection create redis-enterprise
```
az webapp connection create redis-enterprise [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                             [--connection]
                                             [--database]
                                             [--name]
                                             [--no-wait]
                                             [--resource-group]
                                             [--secret]
                                             [--server]
                                             [--source-id]
                                             [--target-id]
                                             [--target-resource-group]
                                             [--vault-id]
```

### az webapp connection create servicebus
```
az webapp connection create servicebus [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                       [--connection]
                                       [--name]
                                       [--namespace]
                                       [--no-wait]
                                       [--private-endpoint {false, true}]
                                       [--resource-group]
                                       [--secret]
                                       [--service-endpoint {false, true}]
                                       [--service-principal]
                                       [--source-id]
                                       [--system-identity]
                                       [--target-id]
                                       [--target-resource-group]
                                       [--user-identity]
                                       [--vault-id]
```

### az webapp connection create signalr
```
az webapp connection create signalr [--client-type {dotnet, none}]
                                    [--connection]
                                    [--name]
                                    [--no-wait]
                                    [--private-endpoint {false, true}]
                                    [--resource-group]
                                    [--secret]
                                    [--service-principal]
                                    [--signalr]
                                    [--source-id]
                                    [--system-identity]
                                    [--target-id]
                                    [--target-resource-group]
                                    [--user-identity]
                                    [--vault-id]
```

### az webapp connection create sql
```
az webapp connection create sql [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                [--config-connstr {false, true}]
                                [--connection]
                                [--database]
                                [--name]
                                [--no-wait]
                                [--private-endpoint {false, true}]
                                [--resource-group]
                                [--secret]
                                [--server]
                                [--service-endpoint {false, true}]
                                [--source-id]
                                [--system-identity]
                                [--target-id]
                                [--target-resource-group]
                                [--vault-id]
```

### az webapp connection create storage-blob
```
az webapp connection create storage-blob [--account]
                                         [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                         [--connection]
                                         [--name]
                                         [--new {false, true}]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--service-principal]
                                         [--source-id]
                                         [--system-identity]
                                         [--target-id]
                                         [--target-resource-group]
                                         [--user-identity]
                                         [--vault-id]
```

### az webapp connection create storage-file
```
az webapp connection create storage-file [--account]
                                         [--client-type {dotnet, java, nodejs, none, php, python, ruby, springBoot}]
                                         [--connection]
                                         [--name]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--source-id]
                                         [--target-id]
                                         [--target-resource-group]
                                         [--vault-id]
```

### az webapp connection create storage-queue
```
az webapp connection create storage-queue [--account]
                                          [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                          [--connection]
                                          [--name]
                                          [--no-wait]
                                          [--private-endpoint {false, true}]
                                          [--resource-group]
                                          [--secret]
                                          [--service-endpoint {false, true}]
                                          [--service-principal]
                                          [--source-id]
                                          [--system-identity]
                                          [--target-id]
                                          [--target-resource-group]
                                          [--user-identity]
                                          [--vault-id]
```

### az webapp connection create storage-table
```
az webapp connection create storage-table [--account]
                                          [--client-type {dotnet, java, nodejs, none, python}]
                                          [--connection]
                                          [--name]
                                          [--no-wait]
                                          [--private-endpoint {false, true}]
                                          [--resource-group]
                                          [--secret]
                                          [--service-endpoint {false, true}]
                                          [--source-id]
                                          [--target-id]
                                          [--target-resource-group]
                                          [--vault-id]
```

### az webapp connection create webpubsub
```
az webapp connection create webpubsub [--client-type {dotnet, java, nodejs, none, python}]
                                      [--connection]
                                      [--name]
                                      [--no-wait]
                                      [--private-endpoint {false, true}]
                                      [--resource-group]
                                      [--secret]
                                      [--service-principal]
                                      [--source-id]
                                      [--system-identity]
                                      [--target-id]
                                      [--target-resource-group]
                                      [--user-identity]
                                      [--vault-id]
                                      [--webpubsub]
```

## Azure Webapp Connection Update

### az webapp connection update appconfig
```
az webapp connection update appconfig [--client-type {dotnet, java, nodejs, none, python}]
                                      [--connection]
                                      [--id]
                                      [--name]
                                      [--no-wait]
                                      [--private-endpoint {false, true}]
                                      [--resource-group]
                                      [--secret]
                                      [--service-principal]
                                      [--system-identity]
                                      [--user-identity]
                                      [--vault-id]
```

### az webapp connection update confluent-cloud
```
az webapp connection update confluent-cloud --connection
                                            [--bootstrap-server]
                                            [--client-type {dotnet, go, java, none, python, springBoot}]
                                            [--kafka-key]
                                            [--kafka-secret]
                                            [--name]
                                            [--no-wait]
                                            [--resource-group]
                                            [--schema-key]
                                            [--schema-registry]
                                            [--schema-secret]
                                            [--source-id]
                                            [--vault-id]
```

### az webapp connection update cosmos-cassandra
```
az webapp connection update cosmos-cassandra [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                             [--connection]
                                             [--id]
                                             [--name]
                                             [--no-wait]
                                             [--private-endpoint {false, true}]
                                             [--resource-group]
                                             [--secret]
                                             [--service-endpoint {false, true}]
                                             [--service-principal]
                                             [--system-identity]
                                             [--user-identity]
                                             [--vault-id]
```

### az webapp connection update cosmos-gremlin
```
az webapp connection update cosmos-gremlin [--client-type {dotnet, java, nodejs, none, php, python}]
                                           [--connection]
                                           [--id]
                                           [--name]
                                           [--no-wait]
                                           [--private-endpoint {false, true}]
                                           [--resource-group]
                                           [--secret]
                                           [--service-endpoint {false, true}]
                                           [--service-principal]
                                           [--system-identity]
                                           [--user-identity]
                                           [--vault-id]
```

### az webapp connection update cosmos-mongo
```
az webapp connection update cosmos-mongo [--client-type {dotnet, go, java, nodejs, none, springBoot}]
                                         [--connection]
                                         [--id]
                                         [--name]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--service-principal]
                                         [--system-identity]
                                         [--user-identity]
                                         [--vault-id]
```

### az webapp connection update cosmos-sql
```
az webapp connection update cosmos-sql [--client-type {dotnet, java, nodejs, none, python}]
                                       [--connection]
                                       [--id]
                                       [--name]
                                       [--no-wait]
                                       [--private-endpoint {false, true}]
                                       [--resource-group]
                                       [--secret]
                                       [--service-endpoint {false, true}]
                                       [--service-principal]
                                       [--system-identity]
                                       [--user-identity]
                                       [--vault-id]
```

### az webapp connection update cosmos-table
```
az webapp connection update cosmos-table [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                         [--connection]
                                         [--id]
                                         [--name]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--service-principal]
                                         [--system-identity]
                                         [--user-identity]
                                         [--vault-id]
```

### az webapp connection update eventhub
```
az webapp connection update eventhub [--client-type {dotnet, go, java, kafka-springBoot, nodejs, none, python, springBoot}]
                                     [--connection]
                                     [--id]
                                     [--name]
                                     [--no-wait]
                                     [--private-endpoint {false, true}]
                                     [--resource-group]
                                     [--secret]
                                     [--service-endpoint {false, true}]
                                     [--service-principal]
                                     [--system-identity]
                                     [--user-identity]
                                     [--vault-id]
```

### az webapp connection update keyvault
```
az webapp connection update keyvault [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                     [--connection]
                                     [--id]
                                     [--name]
                                     [--no-wait]
                                     [--private-endpoint {false, true}]
                                     [--resource-group]
                                     [--service-endpoint {false, true}]
                                     [--service-principal]
                                     [--system-identity]
                                     [--user-identity]
                                     [--vault-id]
```

### az webapp connection update mysql
```
az webapp connection update mysql [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                  [--config-connstr {false, true}]
                                  [--connection]
                                  [--id]
                                  [--name]
                                  [--no-wait]
                                  [--private-endpoint {false, true}]
                                  [--resource-group]
                                  [--secret]
                                  [--service-endpoint {false, true}]
                                  [--vault-id]
```

### az webapp connection update mysql-flexible
```
az webapp connection update mysql-flexible [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                           [--config-connstr {false, true}]
                                           [--connection]
                                           [--id]
                                           [--name]
                                           [--no-wait]
                                           [--resource-group]
                                           [--secret]
                                           [--system-identity]
                                           [--vault-id]
```

### az webapp connection update postgres
```
az webapp connection update postgres [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                     [--config-connstr {false, true}]
                                     [--connection]
                                     [--id]
                                     [--name]
                                     [--no-wait]
                                     [--private-endpoint {false, true}]
                                     [--resource-group]
                                     [--secret]
                                     [--service-endpoint {false, true}]
                                     [--system-identity]
                                     [--vault-id]
```

### az webapp connection update postgres-flexible
```
az webapp connection update postgres-flexible [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                              [--config-connstr {false, true}]
                                              [--connection]
                                              [--id]
                                              [--name]
                                              [--no-wait]
                                              [--resource-group]
                                              [--secret]
                                              [--system-identity]
                                              [--vault-id]
```

### az webapp connection update redis
```
az webapp connection update redis [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                  [--connection]
                                  [--id]
                                  [--name]
                                  [--no-wait]
                                  [--private-endpoint {false, true}]
                                  [--resource-group]
                                  [--secret]
                                  [--vault-id]
```

### az webapp connection update redis-enterprise
```
az webapp connection update redis-enterprise [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                             [--connection]
                                             [--id]
                                             [--name]
                                             [--no-wait]
                                             [--resource-group]
                                             [--secret]
                                             [--vault-id]
```

### az webapp connection update servicebus
```
az webapp connection update servicebus [--client-type {dotnet, go, java, nodejs, none, python, springBoot}]
                                       [--connection]
                                       [--id]
                                       [--name]
                                       [--no-wait]
                                       [--private-endpoint {false, true}]
                                       [--resource-group]
                                       [--secret]
                                       [--service-endpoint {false, true}]
                                       [--service-principal]
                                       [--system-identity]
                                       [--user-identity]
                                       [--vault-id]
```

### az webapp connection update signalr
```
az webapp connection update signalr [--client-type {dotnet, none}]
                                    [--connection]
                                    [--id]
                                    [--name]
                                    [--no-wait]
                                    [--private-endpoint {false, true}]
                                    [--resource-group]
                                    [--secret]
                                    [--service-principal]
                                    [--system-identity]
                                    [--user-identity]
                                    [--vault-id]
```

### az webapp connection update sql
```
az webapp connection update sql [--client-type {django, dotnet, go, java, nodejs, none, php, python, ruby, springBoot}]
                                [--config-connstr {false, true}]
                                [--connection]
                                [--id]
                                [--name]
                                [--no-wait]
                                [--private-endpoint {false, true}]
                                [--resource-group]
                                [--secret]
                                [--service-endpoint {false, true}]
                                [--system-identity]
                                [--vault-id]
```

### az webapp connection update storage-blob
```
az webapp connection update storage-blob [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                         [--connection]
                                         [--id]
                                         [--name]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--service-principal]
                                         [--system-identity]
                                         [--user-identity]
                                         [--vault-id]
```

### az webapp connection update storage-file
```
az webapp connection update storage-file [--client-type {dotnet, java, nodejs, none, php, python, ruby, springBoot}]
                                         [--connection]
                                         [--id]
                                         [--name]
                                         [--no-wait]
                                         [--private-endpoint {false, true}]
                                         [--resource-group]
                                         [--secret]
                                         [--service-endpoint {false, true}]
                                         [--vault-id]
```

### az webapp connection update storage-queue
```
az webapp connection update storage-queue [--client-type {dotnet, java, nodejs, none, python, springBoot}]
                                          [--connection]
                                          [--id]
                                          [--name]
                                          [--no-wait]
                                          [--private-endpoint {false, true}]
                                          [--resource-group]
                                          [--secret]
                                          [--service-endpoint {false, true}]
                                          [--service-principal]
                                          [--system-identity]
                                          [--user-identity]
                                          [--vault-id]
```

### az webapp connection update storage-table
```
az webapp connection update storage-table [--client-type {dotnet, java, nodejs, none, python}]
                                          [--connection]
                                          [--id]
                                          [--name]
                                          [--no-wait]
                                          [--private-endpoint {false, true}]
                                          [--resource-group]
                                          [--secret]
                                          [--service-endpoint {false, true}]
                                          [--vault-id]
```

### az webapp connection update webpubsub
```
az webapp connection update webpubsub [--client-type {dotnet, java, nodejs, none, python}]
                                      [--connection]
                                      [--id]
                                      [--name]
                                      [--no-wait]
                                      [--private-endpoint {false, true}]
                                      [--resource-group]
                                      [--secret]
                                      [--service-principal]
                                      [--system-identity]
                                      [--user-identity]
                                      [--vault-id]
```

## Azure Webapp Cross-Origin Resource Sharing

### az webapp cors add
```
az webapp cors add --allowed-origins
                   [--ids]
                   [--name]
                   [--resource-group]
                   [--slot]
                   [--subscription]
```

### az webapp cors remove
```
az webapp cors remove --allowed-origins
                      [--ids]
                      [--name]
                      [--resource-group]
                      [--slot]
                      [--subscription]
```

### az webapp cors show
```
az webapp cors show [--ids]
                    [--name]
                    [--resource-group]
                    [--slot]
                    [--subscription]
```

## Azure Webapp Deleted

### az webapp deleted list
```
az webapp deleted list [--name]
                       [--resource-group]
                       [--slot]
```

### az webapp deleted restore
```
az webapp deleted restore --deleted-id
                          [--ids]
                          [--name]
                          [--resource-group]
                          [--restore-content-only]
                          [--slot]
                          [--subscription]
```

## Azure Webapp Deployment

### az webapp deployment list-publishing-credentials
```
az webapp deployment list-publishing-credentials [--ids]
                                                 [--name]
                                                 [--resource-group]
                                                 [--slot]
                                                 [--subscription]
```

### az webapp deployment list-publishing-profiles
```
az webapp deployment list-publishing-profiles [--ids]
                                              [--name]
                                              [--resource-group]
                                              [--slot]
                                              [--subscription]
                                              [--xml]
```

## Azure Webapp Deployment Container

### az webapp deployment container config
```
az webapp deployment container config --enable-cd {false, true}
                                      [--ids]
                                      [--name]
                                      [--resource-group]
                                      [--slot]
                                      [--subscription]
```

### az webapp deployment container show-cd-url
```
az webapp deployment container show-cd-url [--ids]
                                           [--name]
                                           [--resource-group]
                                           [--slot]
                                           [--subscription]
```

## Azure Webapp Deployment Github Actions

### az webapp deployment github-actions add
```
az webapp deployment github-actions add --repo
                                        [--branch]
                                        [--force]
                                        [--ids]
                                        [--login-with-github]
                                        [--name]
                                        [--resource-group]
                                        [--runtime]
                                        [--slot]
                                        [--subscription]
                                        [--token]
```

### az webapp deployment github-actions remove
```
az webapp deployment github-actions remove --repo
                                           [--branch]
                                           [--ids]
                                           [--login-with-github]
                                           [--name]
                                           [--resource-group]
                                           [--slot]
                                           [--subscription]
                                           [--token]
```

## Azure Webapp Deployment Slot

### az webapp deployment slot auto-swap
```
az webapp deployment slot auto-swap --slot
                                    [--auto-swap-slot]
                                    [--disable]
                                    [--ids]
                                    [--name]
                                    [--resource-group]
                                    [--subscription]
```

### az webapp deployment slot create
```
az webapp deployment slot create --name
                                 --resource-group
                                 --slot
                                 [--configuration-source]
                                 [--deployment-container-image-name]
                                 [--docker-registry-server-password]
                                 [--docker-registry-server-user]
```

### az webapp deployment slot delete
```
az webapp deployment slot delete --slot
                                 [--ids]
                                 [--name]
                                 [--resource-group]
                                 [--subscription]
```

### az webapp deployment slot list
```
az webapp deployment slot list [--ids]
                               [--name]
                               [--resource-group]
                               [--subscription]
```

### az webapp deployment slot swap
```
az webapp deployment slot swap --slot
                               [--action {preview, reset, swap}]
                               [--ids]
                               [--name]
                               [--preserve-vnet {false, true}]
                               [--resource-group]
                               [--subscription]
                               [--target-slot]
```

## Azure Webapp Deployment Source Control

### az webapp deployment source config
```
az webapp deployment source config --repo-url
                                   [--branch]
                                   [--git-token]
                                   [--github-action]
                                   [--ids]
                                   [--manual-integration]
                                   [--name]
                                   [--repository-type {externalgit, git, github, localgit, mercurial}]
                                   [--resource-group]
                                   [--slot]
                                   [--subscription]
```

### az webapp deployment source config-local-git
```
az webapp deployment source config-local-git [--ids]
                                             [--name]
                                             [--resource-group]
                                             [--slot]
                                             [--subscription]
```

### az webapp deployment source config-zip
```
az webapp deployment source config-zip --src
                                       [--ids]
                                       [--name]
                                       [--resource-group]
                                       [--slot]
                                       [--subscription]
                                       [--timeout]
```

### az webapp deployment source delete
```
az webapp deployment source delete [--ids]
                                   [--name]
                                   [--resource-group]
                                   [--slot]
                                   [--subscription]
```

### az webapp deployment source show
```
az webapp deployment source show [--ids]
                                 [--name]
                                 [--resource-group]
                                 [--slot]
                                 [--subscription]
```

### az webapp deployment source sync
```
az webapp deployment source sync [--ids]
                                 [--name]
                                 [--resource-group]
                                 [--slot]
                                 [--subscription]
```

### az webapp deployment source update-token
```
az webapp deployment source update-token [--git-token]
```

## Azure Webapp Deployment User

### az webapp deployment user set
```
az webapp deployment user set --user-name
                              [--password]
```

### az webapp deployment user show
```
az webapp deployment user show
```

## Azure Webapp Hybrid Connection

### az webapp hybrid-connection add
```
az webapp hybrid-connection add --hybrid-connection
                                --name
                                --namespace
                                --resource-group
                                [--slot]
```

### az webapp hybrid-connection list
```
az webapp hybrid-connection list --name
                                 --resource-group
                                 [--slot]
```

### az webapp hybrid-connection remove
```
az webapp hybrid-connection remove --hybrid-connection
                                   --name
                                   --namespace
                                   --resource-group
                                   [--slot]
```

## Azure Webapp Identity

### az webapp identity assign
```
az webapp identity assign [--identities]
                          [--ids]
                          [--name]
                          [--resource-group]
                          [--role]
                          [--scope]
                          [--slot]
                          [--subscription]
```

### az webapp identity remove
```
az webapp identity remove [--identities]
                          [--ids]
                          [--name]
                          [--resource-group]
                          [--slot]
                          [--subscription]
```

### az webapp identity show
```
az webapp identity show [--ids]
                        [--name]
                        [--resource-group]
                        [--slot]
                        [--subscription]
```

## Azure Webapp Logs

### az webapp log config
```
az webapp log config [--application-logging {azureblobstorage, filesystem, off}]
                     [--detailed-error-messages {false, true}]
                     [--docker-container-logging {filesystem, off}]
                     [--failed-request-tracing {false, true}]
                     [--ids]
                     [--level {error, information, verbose, warning}]
                     [--name]
                     [--resource-group]
                     [--slot]
                     [--subscription]
                     [--web-server-logging {filesystem, off}]
```

### az webapp log download
```
az webapp log download [--ids]
                       [--log-file]
                       [--name]
                       [--resource-group]
                       [--slot]
                       [--subscription]
```

### az webapp log show
```
az webapp log show [--ids]
                   [--name]
                   [--resource-group]
                   [--slot]
                   [--subscription]
```

### az webapp log tail
```
az webapp log tail [--ids]
                   [--name]
                   [--provider]
                   [--resource-group]
                   [--slot]
                   [--subscription]
```

## Azure Webapp Deployment Logs

### az webapp log deployment list
```
az webapp log deployment list --name
                              --resource-group
                              [--slot]
```

### az webapp log deployment log show
```
az webapp log deployment show --name
                              --resource-group
                              [--deployment-id]
                              [--slot]
```

## Azure Webapp Scan

### az webapp scan list-result
```
az webapp scan list-result [--ids]
                           [--name]
                           [--resource-group]
                           [--slot]
                           [--subscription]
```

### az webapp scan show-result
```
az webapp scan show-result --scan-id
                           [--ids]
                           [--name]
                           [--resource-group]
                           [--slot]
                           [--subscription]
```

### az webapp scan start
```
az webapp scan start [--ids]
                     [--name]
                     [--resource-group]
                     [--slot]
                     [--subscription]
                     [--timeout]
```

### az webapp scan stop
```
az webapp scan stop [--ids]
                    [--name]
                    [--resource-group]
                    [--slot]
                    [--subscription]
```

### az webapp scan track
```
az webapp scan track --scan-id
                     [--ids]
                     [--name]
                     [--resource-group]
                     [--slot]
                     [--subscription]
```

## Azure Webapp Traffic Routing

### az webapp traffic-routing clear
```
az webapp traffic-routing clear [--ids]
                                [--name]
                                [--resource-group]
                                [--subscription]
```

### az webapp traffic-routing set
```
az webapp traffic-routing set --distribution
                              [--ids]
                              [--name]
                              [--resource-group]
                              [--subscription]
```

### az webapp traffic-routing show
```
az webapp traffic-routing show [--ids]
                               [--name]
                               [--resource-group]
                               [--subscription]
```

## Azure Webapp Virtual Network Integration

### az webapp vnet-integration add
```
az webapp vnet-integration add --name
                               --resource-group
                               --subnet
                               --vnet
                               [--skip-delegation-check {false, true}]
                               [--slot]
```

### az webapp vnet-integration list
```
az webapp vnet-integration list --name
                                --resource-group
                                [--slot]
```

### az webapp vnet-integration remove
```
az webapp vnet-integration remove --name
                                  --resource-group
                                  [--slot]
```

## Azure Webapp Continuous Webjob

### az webapp webjob continuous list
```
az webapp webjob continuous list --name
                                 --resource-group
                                 [--slot]
```

### az webapp webjob continuous remove
```
az webapp webjob continuous remove --webjob-name
                                   [--ids]
                                   [--name]
                                   [--resource-group]
                                   [--slot]
                                   [--subscription]
```

### az webapp webjob continuous start
```
az webapp webjob continuous start --webjob-name
                                  [--ids]
                                  [--name]
                                  [--resource-group]
                                  [--slot]
                                  [--subscription]
```

### az webapp webjob continuous stop
```
az webapp webjob continuous stop --webjob-name
                                 [--ids]
                                 [--name]
                                 [--resource-group]
                                 [--slot]
                                 [--subscription]
```

## Azure Webapp Triggered Webjob

### az webapp webjob triggered list
```
az webapp webjob triggered list --name
                                --resource-group
                                [--slot]
```

### az webapp webjob triggered log
```
az webapp webjob triggered log --webjob-name
                               [--ids]
                               [--name]
                               [--resource-group]
                               [--slot]
                               [--subscription]
```

### az webapp webjob triggered remove
```
az webapp webjob triggered remove --webjob-name
                                  [--ids]
                                  [--name]
                                  [--resource-group]
                                  [--slot]
                                  [--subscription]
```

### az webapp webjob triggered run
```
az webapp webjob triggered run --webjob-name
                               [--ids]
                               [--name]
                               [--resource-group]
                               [--slot]
                               [--subscription]
```







                                 




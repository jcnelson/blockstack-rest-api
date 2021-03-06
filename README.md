# Blockstack REST API

## Names

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get all names | GET /names | - | 
| Register name | POST /names | - | 
| Get name info | GET /names/{name} | - | 
| Get name history | GET /names/{name}/history | - | 
| Get historical zone file | GET /names/{name}/zoneFile/{zoneFileHash}  | - | 
| Delete user | DELETE /names/{name} | - | 
| Transfer name | PATCH /names/{name} | Payload: {"owner": OWNER } | 
| Set zone file | PATCH /names/{name} | Payload: {"zoneFile": ZONE_FILE } | 
| Set zone file hash | PATCH /names/{name} | Payload: {"zoneFileHash": ZONE_FILE_HASH } | 

## Namespaces

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get all namespaces | GET /namespaces | - | 
| Create namespace | POST /namespaces | - | 
| Launch namespace | PUT /namespaces/{tld} | - | 
| Get namespace names | GET /namespaces/{tld}/names | - | 
| Pre-register a name | POST /namespaces/{tld}/names | - | 
| Update pre-registered name | PUT /namespaces/{tld}/names/{name} | - | 

## Prices

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get namespace price | GET /prices/namespaces/{tld} | - | 
| Get name price | GET /prices/names/{name} | - | 

## Users

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get all users | GET /users | - | 
| Create user | POST /users | - | 
| Get user | GET /users/{userID} | - | 
| Delete user | DELETE /users/{userID} | - | 
| Update profile | PATCH /users/{userID} | Payload: {"profile": PROFILE } | 

## User Stores

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get all stores | GET /users/{userID}/stores | - | 
| Create store | POST /users/{userID}/stores | - | 
| Get store | GET /users/{userID}/stores/{storeID} | - | 
| Update store | PUT /users/{userID}/stores/{storeID} | - | 
| Delete store | DELETE /users/{userID}/stores/{storeID} | - | 
| - | - | - | 
| Get directory files (ls) | GET /users/{userID}/stores/{storeID}/directories?path={path} | - | 
| Get directory info (stat) | HEAD /users/{userID}/stores/{storeID}/directories?path={path} | - | 
| Create directory (mkdir) | POST /users/{userID}/stores/{storeID}/directories?path={path} | - | 
| Delete directory (rmdir) | DELETE /users/{userID}/stores/{storeID}/directories?path={path} | - | 
| - | - | - | 
| Get file data (open) | GET /users/{userID}/stores/{storeID}/files?path={path} | - | 
| Get file info (stat) | HEAD /users/{userID}/stores/{storeID}/files?path={path} | - | 
| Create file | POST /users/{userID}/stores/{storeID}/files?path={path} | - | 
| Delete file (rm) | DELETE /users/{userID}/stores/{storeID}/files?path={path} | - | 

## User Collections

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get all collections | GET /users/{userID}/collections | - | 
| Create collection | POST /users/{userID}/collections | - | 
| Get all collection items | GET /users/{userID}/collections/{collectionID} | - | 
| Create collection item | GET /users/{userID}/collections/{collectionID} | - | 
| Get collection item | GET /users/{userID}/collections/{collectionID}/{itemID} | - | 

## User Apps

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get all app accounts | GET /users/{userID}/apps | - | 
| Create app account | POST /users/{userID}/apps | - | 
| Get app account | GET /users/{userID}/apps/{appID} | - | 
| List app resources | GET /users/{userID}/apps/{appID}/resources | - | 
| Get app resource | GET /users/{userID}/apps/{appID}/resources/{resourceID} | - | 

## Blockchains

| Method  | API Call | Notes | 
| ------------- | ------------- | ------------- |
| Get block operations | GET /blockchains/{blockchainName}/block/{blockHeight} | - | 
| Get raw name history | GET /blockchains/{blockchainName}/names/{nameID}/history | - | 
| Get consensus hash | GET /blockchains/{blockchainName}/consensusHash | - | 

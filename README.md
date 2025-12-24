
│ Error: cannot destroy service without setting deletion_protection=false and running `terraform apply`
│ 
│ 
╵
╷
│ Error: Error creating service account: googleapi: Error 409: Service account sda-prod-cr-sa already exists within project projects/sky3-geo-sat-prd-u-sda-1.
│ Details:
│ [
│   {
│     "@type": "type.googleapis.com/google.rpc.ResourceInfo",
│     "resourceName": "projects/sky3-geo-sat-prd-u-sda-1/serviceAccounts/sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com"
│   }
│ ]
│ , alreadyExists
│ 
│   with google_service_account.service_accounts["cloud_run"],
│   on main.tf line 85, in resource "google_service_account" "service_accounts":
│   85: resource "google_service_account" "service_accounts" {
│ 
╵
╷
│ Error: Error creating notification config for bucket sda-prod-untrusted-bucket: googleapi: Error 403: Service account 'service-632210246751@gs-project-accounts.iam.gserviceaccount.com' denied permission to publish to topic '//pubsub.googleapis.com/projects/sky3-geo-sat-prd-d-sda-1/topics/sda-dmz-topic' because of error: 'Request is prohibited by organization's policy. vpcServiceControlsUniqueIdentifier: KRDUkZUCHb9iLsfnBUtnhDtEorMGRPqCaJ5CHQXKH8c569jX5xrdBb2y6LoApVoMVarDHanlrmEdJ_-R', forbidden
│ 
│   with google_storage_notification.data_notifications_temp,
│   on main.tf line 259, in resource "google_storage_notification" "data_notifications_temp":
│  259: resource "google_storage_notification" "data_notifications_temp" {
│ 
╵
╷
│ Error: Error waiting to create Job: Error waiting for Creating Job: Error code 9, message: spec.template.spec.containers[0].env[0].value_from.secret_key_ref.name: Secret Manager API has not been used in project 632210246751 before or it is disabled. Enable it by visiting https://console.developers.google.com/apis/api/secretmanager.googleapis.com/overview?project=632210246751 then retry. If you enabled this API recently, wait a few minutes for the action to propagate to our systems and retry.
│ spec.template.spec.containers[0].env[1].value_from.secret_key_ref.name: Secret Manager API has not been used in project 632210246751 before or it is disabled. Enable it by visiting https://console.developers.google.com/apis/api/secretmanager.googleapis.com/overview?project=632210246751 then retry. If you enabled this API recently, wait a few minutes for the action to propagate to our systems and retry.
│ 
│   with module.cloud_run_jobs["space_track"].google_cloud_run_v2_job.default,
│   on blueprints/cloud-run-jobs/main.tf line 17, in resource "google_cloud_run_v2_job" "default":
│   17: resource "google_cloud_run_v2_job" "default" {
│ 
╵
╷
│ Error: Error waiting to create Job: Error waiting for Creating Job: Error code 9, message: spec.template.spec.containers[0].env[1].value_from.secret_key_ref.name: Secret Manager API has not been used in project 632210246751 before or it is disabled. Enable it by visiting https://console.developers.google.com/apis/api/secretmanager.googleapis.com/overview?project=632210246751 then retry. If you enabled this API recently, wait a few minutes for the action to propagate to our systems and retry.
│ spec.template.spec.containers[0].env[2].value_from.secret_key_ref.name: Secret Manager API has not been used in project 632210246751 before or it is disabled. Enable it by visiting https://console.developers.google.com/apis/api/secretmanager.googleapis.com/overview?project=632210246751 then retry. If you enabled this API recently, wait a few minutes for the action to propagate to our systems and retry.
│ 
│   with module.cloud_run_jobs["n2yo"].google_cloud_run_v2_job.default,
│   on blueprints/cloud-run-jobs/main.tf line 17, in resource "google_cloud_run_v2_job" "default":
│   17: resource "google_cloud_run_v2_job" "def

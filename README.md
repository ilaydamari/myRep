
│ Error: cannot destroy service without setting deletion_protection=false and running `terraform apply`
│ 
│ 
╵
╷
│ Error: Error waiting to create Service: Error waiting for Creating Service: Error code 9, message: The user-provided container failed to start and listen on the port defined provided by the PORT=3000 environment variable within the allocated timeout. This can happen when the container port is misconfigured or if the timeout is too short. The health check timeout can be extended. Logs for this revision might contain more information.
│ 
│ Logs URL: https://console.cloud.google.com/logs/viewer?project=sky3-geo-sat-prd-u-sda-1&resource=cloud_run_revision/service_name/cibus-convertor/revision_name/cibus-convertor-00001-wwm&advancedFilter=resource.type%3D%22cloud_run_revision%22%0Aresource.labels.service_name%3D%22cibus-convertor%22%0Aresource.labels.revision_name%3D%22cibus-convertor-00001-wwm%22 
│ For more troubleshooting guidance, see https://cloud.google.com/run/docs/troubleshooting#container-failed-to-start
│ 
│   with google_cloud_run_v2_service.services["cibus_convertor"],
│   on main.tf line 162, in resource "google_cloud_run_v2_service" "services":
│  162: resource "google_cloud_run_v2_service" "services" {
│ 
╵
╷
│ Error: Error creating notification config for bucket sda-prod-untrusted-bucket: googleapi: Error 403: Service account 'service-632210246751@gs-project-accounts.iam.gserviceaccount.com' denied permission to publish to topic '//pubsub.googleapis.com/projects/sky3-geo-sat-prd-d-sda-1/topics/sda-dmz-topic' because of error: 'Request is prohibited by organization's policy. vpcServiceControlsUniqueIdentifier: UaiaFZPWQdd3bOvo7heQ9XWfwlRVCJ5Re64b46fWrqOe5SuRDpaR__HHK7Scn3sA7bHxsXQ8eQpAtqse', forbidden
│ 
│   with google_storage_notification.data_notifications_temp,
│   on main.tf line 259, in resource "google_storage_notification" "data_notifications_temp":
│  259: resource "google_storage_notification" "data_notifications_temp" {
│ 
╵
╷
│ Error: Error waiting to create Job: Error waiting for Creating Job: Error code 9, message: spec.template.spec.containers[0].env[1].value_from.secret_key_ref.name: Secret projects/632210246751/secrets/EMAIL-n2yo/versions/latest was not found
│ spec.template.spec.containers[0].env[2].value_from.secret_key_ref.name: Secret projects/632210246751/secrets/PASSWORD-n2yo/versions/latest was not found
│ 
│   with module.cloud_run_jobs["n2yo"].google_cloud_run_v2_job.default,
│   on blueprints/cloud-run-jobs/main.tf line 17, in resource "google_cloud_run_v2_job" "default":
│   17: resource "google_cloud_run_v2_job" "default" {
│ 
╵
╷
│ Error: Error waiting to create Job: Error waiting for Creating Job: Error code 9, message: spec.template.spec.containers[0].env[0].value_from.secret_key_ref.name: Secret projects/632210246751/secrets/EMAIL-space-track/versions/latest was not found
│ spec.template.spec.containers[0].env[1].value_from.secret_key_ref.name: Secret projects/632210246751/secrets/PASSWORD-space-track/versions/latest was not found
│ 
│   with module.cloud_run_jobs["space_track"].google_cloud_run_v2_job.default,
│   on blueprints/cloud-run-jobs/main.tf line 17, in resource "google_cloud_run_v2_job" "default":
│   17: resource "google_cloud_run_v2_job" "default" {

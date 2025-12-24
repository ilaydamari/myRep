
│ Error: cannot destroy service without setting deletion_protection=false and running `terraform apply`
│ 
│ 
╵
╷
│ Error: Error waiting to create Service: Error waiting for Creating Service: Error code 9, message: The user-provided container failed to start and listen on the port defined provided by the PORT=3000 environment variable within the allocated timeout. This can happen when the container port is misconfigured or if the timeout is too short. The health check timeout can be extended. Logs for this revision might contain more information.
│ 
│ Logs URL: https://console.cloud.google.com/logs/viewer?project=sky3-geo-sat-prd-u-sda-1&resource=cloud_run_revision/service_name/cibus-convertor/revision_name/cibus-convertor-00001-t9r&advancedFilter=resource.type%3D%22cloud_run_revision%22%0Aresource.labels.service_name%3D%22cibus-convertor%22%0Aresource.labels.revision_name%3D%22cibus-convertor-00001-t9r%22 
│ For more troubleshooting guidance, see https://cloud.google.com/run/docs/troubleshooting#container-failed-to-start
│ 
│   with google_cloud_run_v2_service.services["cibus_convertor"],
│   on main.tf line 162, in resource "google_cloud_run_v2_service" "services":
│  162: resource "google_cloud_run_v2_service" "services" {
│ 
╵
╷
│ Error: Error creating notification config for bucket sda-prod-untrusted-bucket: googleapi: Error 403: Service account 'service-632210246751@gs-project-accounts.iam.gserviceaccount.com' denied permission to publish to topic '//pubsub.googleapis.com/projects/sky3-geo-sat-prd-d-sda-1/topics/sda-dmz-topic' because of error: 'Request is prohibited by organization's policy. vpcServiceControlsUniqueIdentifier: PQzvwLtO7J7eRcFt4di_Q3F0bBS_Ar1TimcMxTZUB0DQsqAqS9TbR5fhO9frZB1wddro_tRVXwgKUzWL', forbidden
│ 
│   with google_storage_notification.data_notifications_temp,
│   on main.tf line 259, in resource "google_storage_notification" "data_notifications_temp":
│  259: resource "google_storage_notification" "data_notifications_temp" {
│ 
╵

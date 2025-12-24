
│ Error: Error creating notification config for bucket sda-prod-untrusted-bucket: googleapi: Error 403: Service account 'service-632210246751@gs-project-accounts.iam.gserviceaccount.com' denied permission to publish to topic '//pubsub.googleapis.com/projects/sky3-geo-sat-prd-d-sda-1/topics/sda-dmz-topic' because of error: 'Request is prohibited by organization's policy. vpcServiceControlsUniqueIdentifier: aKia8NxfB8d0Xth7FQXx-T9zsot-dmXMT_tjjDRI7Q7-Jyy7-FP24kTsx6k8LA_OgDWMx2D3LQzTAGet', forbidden
│ 
│   with google_storage_notification.data_notifications_temp,
│   on main.tf line 259, in resource "google_storage_notification" "data_notifications_temp":
│  259: resource "google_storage_notification" "data_notifications_temp" {

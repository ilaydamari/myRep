{
insertId: "694cdd5b00042b50550451cd"
labels: {1}
logName: "projects/sky3-geo-sat-prd-d-sda-1/logs/run.googleapis.com%2Fstdout"
payload: "textPayload"
receiveLocation: "me-west1"
receiveTimestamp: "2025-12-25T06:44:43.600285348Z"
resource: {2}
severity: "DEFAULT"
textPayload: "[2025-12-25T06:44:43.274Z] [INFO] Attempting to read JSON file from GCS: gs://sda-prod-untrusted-bucket/TLEs/spaceTrack"
timestamp: "2025-12-25T06:44:43.273232Z"
traceSampled: false
}



{
insertId: "694cdd5b00047628085ef919"
labels: {
instanceId: "0007e26d681839abba787c919824aa807381b250c7e8140d6039eb7c42498270c5684cdd0df115fdf245d8ed9a2a956474d4f7ea9d9a7998ed08a461db748ae7fabc17e3b3384ac2565ae4e9d8001418"
}
logName: "projects/sky3-geo-sat-prd-d-sda-1/logs/run.googleapis.com%2Fstderr"
payload: "textPayload"
receiveLocation: "me-west1"
receiveTimestamp: "2025-12-25T06:44:43.618345832Z"
resource: {
labels: {
configuration_name: "sda-dmz-cr"
location: "me-west1"
project_id: "sky3-geo-sat-prd-d-sda-1"
revision_name: "sda-dmz-cr-00001-rkw"
service_name: "sda-dmz-cr"
}
type: "cloud_run_revision"
}
severity: "DEFAULT"
textPayload: "[2025-12-25T06:44:43.293Z] [ERROR] Error processing file | Meta: {"message":"sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com does not have storage.objects.get access to the Google Cloud Storage object. Permission 'storage.objects.get' denied on resource (or it may not exist)."}"
timestamp: "2025-12-25T06:44:43.292392Z"
traceSampled: false
}

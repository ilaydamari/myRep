Already have image (with digest): hashicorp/terraform:latest
google_service_account.service_accounts["cibus_convertor"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/serviceAccounts/cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_service_account.service_accounts["cloud_run"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/serviceAccounts/sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_pubsub_topic.service_topics["cibus_convertor"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/topics/cibus-convertor-topic]
data.google_storage_bucket.existing_state_bucket[0]: Reading...
data.google_artifact_registry_repository.existing_registry[0]: Reading...
module.cloud_run_jobs["n2yo"].google_service_account.cloud_run_job_sa: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/serviceAccounts/n2yo-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["celestrack"].google_service_account.cloud_run_job_sa: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/serviceAccounts/celestrack-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["space_track"].google_service_account.cloud_run_job_sa: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/serviceAccounts/space-track-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_cloud_scheduler_job.scheduler_jobs["celestrack-scheduler"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/europe-west1/jobs/celestrack-scheduler]
google_cloud_scheduler_job.scheduler_jobs["n2yo-scheduler"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/europe-west1/jobs/n2yo-scheduler]
google_cloud_scheduler_job.scheduler_jobs["space-track-scheduler"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/europe-west1/jobs/space-track-scheduler]
module.sda-preprod-untrusted-bucket[0].module.gcs.google_storage_bucket.bucket: Refreshing state... [id=sda-prod-untrusted-bucket]
module.cloud_run.module.cloud_run.google_cloud_run_v2_service.service[0]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/sda-untrusted-cr]
module.sda-preprod-untrusted-bucket[0].module.gcs.google_storage_managed_folder.folder["TLEs/"]: Refreshing state... [id=sda-prod-untrusted-bucket/TLEs/]
module.sda-preprod-untrusted-bucket[0].module.gcs.google_storage_managed_folder.folder["Pics/"]: Refreshing state... [id=sda-prod-untrusted-bucket/Pics/]
data.google_artifact_registry_repository.existing_registry[0]: Read complete after 0s [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/repositories/sda]
data.google_storage_bucket.existing_state_bucket[0]: Read complete after 0s [id=sda-prod-untrusted-state]
google_project_iam_member.service_account_roles["cloud_run-roles/pubsub.subscriber"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/pubsub.subscriber/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/eventarc.eventReceiver"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/eventarc.eventReceiver/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/pubsub.publisher"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/pubsub.publisher/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/compute.networkAdmin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/compute.networkAdmin/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cibus_convertor-roles/run.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/run.admin/serviceAccount:cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/storage.objectCreator"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.objectCreator/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/storage.objectUser"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.objectUser/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cibus_convertor-roles/storage.objectCreator"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.objectCreator/serviceAccount:cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cibus_convertor-roles/run.invoker"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/run.invoker/serviceAccount:cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cibus_convertor-roles/run.jobsExecutor"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/run.jobsExecutor/serviceAccount:cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cibus_convertor-roles/storage.objectViewer"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.objectViewer/serviceAccount:cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/storage.objectViewer"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.objectViewer/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cibus_convertor-roles/logging.logWriter"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/logging.logWriter/serviceAccount:cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/pubsub.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/pubsub.admin/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/viewer"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/viewer/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cibus_convertor-roles/pubsub.subscriber"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/pubsub.subscriber/serviceAccount:cibus-convertor-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_project_iam_member.service_account_roles["cloud_run-roles/pubsub.viewer"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/pubsub.viewer/serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_cloud_run_v2_service.services["cibus_convertor"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/cibus-convertor]
module.cloud_run_jobs["space_track"].google_project_iam_member.sa_roles["roles/run.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/run.admin/serviceAccount:space-track-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["space_track"].google_project_iam_member.sa_roles["roles/cloudscheduler.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/cloudscheduler.admin/serviceAccount:space-track-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["space_track"].google_project_iam_member.sa_roles["roles/storage.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.admin/serviceAccount:space-track-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["space_track"].google_project_iam_member.sa_roles["roles/secretmanager.secretAccessor"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/secretmanager.secretAccessor/serviceAccount:space-track-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["celestrack"].google_project_iam_member.sa_roles["roles/cloudscheduler.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/cloudscheduler.admin/serviceAccount:celestrack-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["celestrack"].google_project_iam_member.sa_roles["roles/secretmanager.secretAccessor"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/secretmanager.secretAccessor/serviceAccount:celestrack-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["celestrack"].google_project_iam_member.sa_roles["roles/run.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/run.admin/serviceAccount:celestrack-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["celestrack"].google_project_iam_member.sa_roles["roles/storage.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.admin/serviceAccount:celestrack-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["n2yo"].google_project_iam_member.sa_roles["roles/secretmanager.secretAccessor"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/secretmanager.secretAccessor/serviceAccount:n2yo-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["n2yo"].google_project_iam_member.sa_roles["roles/run.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/run.admin/serviceAccount:n2yo-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["n2yo"].google_project_iam_member.sa_roles["roles/storage.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/storage.admin/serviceAccount:n2yo-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
module.cloud_run_jobs["n2yo"].google_project_iam_member.sa_roles["roles/cloudscheduler.admin"]: Refreshing state... [id=sky3-geo-sat-prd-u-sda-1/roles/cloudscheduler.admin/serviceAccount:n2yo-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com]
google_eventarc_trigger.service_triggers["cibus_convertor"]: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/triggers/cibus-convertor-trigger]
module.cloud_run_jobs["celestrack"].google_cloud_run_v2_job.default: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/jobs/celestrack]
module.cloud_run_jobs["n2yo"].google_cloud_run_v2_job.default: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/jobs/n2yo]
module.cloud_run_jobs["space_track"].google_cloud_run_v2_job.default: Refreshing state... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/jobs/space-track]
Terraform used the selected providers to generate the following execution
plan. Resource actions are indicated with the following symbols:
  + create
  ~ update in-place
  - destroy
Terraform will perform the following actions:
  # google_cloud_run_v2_service.services["cibus_convertor"] will be updated in-place
  ~ resource "google_cloud_run_v2_service" "services" {
        id                      = "projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/cibus-convertor"
        name                    = "cibus-convertor"
        # (33 unchanged attributes hidden)
      - scaling {
          - manual_instance_count = 0 -> null
          - min_instance_count    = 0 -> null
            # (1 unchanged attribute hidden)
        }
        # (2 unchanged blocks hidden)
    }
  # google_storage_notification.data_notifications_temp will be created
  + resource "google_storage_notification" "data_notifications_temp" {
      + bucket             = "sda-prod-untrusted-bucket"
      + event_types        = [
          + "OBJECT_FINALIZE",
        ]
      + id                 = (known after apply)
      + notification_id    = (known after apply)
      + object_name_prefix = "TLEs/"
      + payload_format     = "JSON_API_V1"
      + self_link          = (known after apply)
      + topic              = "projects/sky3-geo-sat-prd-d-sda-1/topics/sda-dmz-topic"
    }
  # module.cloud_run.module.cloud_run.google_cloud_run_v2_service.service[0] will be destroyed
  # (because google_cloud_run_v2_service.service is not in configuration)
  - resource "google_cloud_run_v2_service" "service" {
      - annotations             = {} -> null
      - conditions              = [
          - {
              - last_transition_time = "2025-11-12T09:43:02.879352Z"
              - state                = "CONDITION_SUCCEEDED"
              - type                 = "RoutesReady"
                # (5 unchanged attributes hidden)
            },
          - {
              - last_transition_time = "2025-11-12T09:41:39.792507Z"
              - state                = "CONDITION_SUCCEEDED"
              - type                 = "ConfigurationsReady"
                # (5 unchanged attributes hidden)
            },
        ] -> null
      - create_time             = "2025-11-12T09:41:36.286564Z" -> null
      - creator                 = "untrusted-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com" -> null
      - custom_audiences        = [] -> null
      - default_uri_disabled    = false -> null
      - deletion_protection     = true -> null
      - effective_annotations   = {} -> null
      - effective_labels        = {
          - "goog-terraform-provisioned" = "true"
        } -> null
      - etag                    = "\"CNCs0cgGEKC90ogB/cHJvamVjdHMvc2t5My1nZW8tc2F0LXByZC11LXNkYS0xL2xvY2F0aW9ucy9tZS13ZXN0MS9zZXJ2aWNlcy9zZGEtdW50cnVzdGVkLWNy\"" -> null
      - generation              = "1" -> null
      - iap_enabled             = false -> null
      - id                      = "projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/sda-untrusted-cr" -> null
      - ingress                 = "INGRESS_TRAFFIC_INTERNAL_ONLY" -> null
      - invoker_iam_disabled    = false -> null
      - labels                  = {} -> null
      - last_modifier           = "untrusted-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com" -> null
      - latest_created_revision = "projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/sda-untrusted-cr/revisions/sda-untrusted-cr-00001-vv6" -> null
      - latest_ready_revision   = "projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/sda-untrusted-cr/revisions/sda-untrusted-cr-00001-vv6" -> null
      - launch_stage            = "GA" -> null
      - location                = "me-west1" -> null
      - name                    = "sda-untrusted-cr" -> null
      - observed_generation     = "1" -> null
      - project                 = "sky3-geo-sat-prd-u-sda-1" -> null
      - reconciling             = false -> null
      - terminal_condition      = [
          - {
              - last_transition_time = "2025-11-12T09:43:02.909044Z"
              - state                = "CONDITION_SUCCEEDED"
              - type                 = "Ready"
                # (5 unchanged attributes hidden)
            },
        ] -> null
      - terraform_labels        = {
          - "goog-terraform-provisioned" = "true"
        } -> null
      - traffic_statuses        = [
          - {
              - percent  = 100
              - type     = "TRAFFIC_TARGET_ALLOCATION_TYPE_LATEST"
                # (3 unchanged attributes hidden)
            },
        ] -> null
      - uid                     = "0830addd-dd41-417a-a3f3-3f8111d246b9" -> null
      - update_time             = "2025-11-12T09:41:36.286564Z" -> null
      - uri                     = "https://sda-untrusted-cr-ptlac6mvkq-zf.a.run.app" -> null
      - urls                    = [
          - "https://sda-untrusted-cr-632210246751.me-west1.run.app",
          - "https://sda-untrusted-cr-ptlac6mvkq-zf.a.run.app",
        ] -> null
        # (5 unchanged attributes hidden)
      - template {
          - annotations                      = {} -> null
          - execution_environment            = "EXECUTION_ENVIRONMENT_GEN1" -> null
          - gpu_zonal_redundancy_disabled    = false -> null
          - labels                           = {} -> null
          - max_instance_request_concurrency = 80 -> null
          - service_account                  = "sda-prod-cr-sa@sky3-geo-sat-prd-u-sda-1.iam.gserviceaccount.com" -> null
          - session_affinity                 = false -> null
          - timeout                          = "300s" -> null
            # (2 unchanged attributes hidden)
          - containers {
              - args           = [] -> null
              - build_info     = [] -> null
              - command        = [] -> null
              - depends_on     = [] -> null
              - image          = "me-west1-docker.pkg.dev/sky3-geo-sat-prd-u-sda-1/sda/sda-untrusted:latest" -> null
              - name           = "default" -> null
                # (2 unchanged attributes hidden)
              - env {
                  - name  = "PROJECT_ID" -> null
                  - value = "sky3-geo-sat-prd-d-sda-1" -> null
                }
              - env {
                  - name  = "TOPIC_ID" -> null
                  - value = "sda-prod-topic" -> null
                }
              - env {
                  - name  = "URL_MAPPING" -> null
                    # (1 unchanged attribute hidden)
                }
              - ports {
                  - container_port = 8080 -> null
                  - name           = "http1" -> null
                }
              - resources {
                  - cpu_idle          = true -> null
                  - limits            = {
                      - "cpu"    = "1000m"
                      - "memory" = "512Mi"
                    } -> null
                  - startup_cpu_boost = false -> null
                }
              - startup_probe {
                  - failure_threshold     = 1 -> null
                  - initial_delay_seconds = 0 -> null
                  - period_seconds        = 240 -> null
                  - timeout_seconds       = 240 -> null
                  - tcp_socket {
                      - port = 8080 -> null
                    }
                }
            }
          - scaling {
              - max_instance_count = 10 -> null
              - min_instance_count = 0 -> null
            }
          - vpc_access {
              - egress    = "PRIVATE_RANGES_ONLY" -> null
                # (1 unchanged attribute hidden)
              - network_interfaces {
                  - subnetwork = "projects/sky3-geo-sat-prod-u-0/regions/me-west1/subnetworks/prod-untrusted-sda-1" -> null
                  - tags       = [] -> null
                    # (1 unchanged attribute hidden)
                }
            }
        }
      - traffic {
          - percent  = 100 -> null
          - type     = "TRAFFIC_TARGET_ALLOCATION_TYPE_LATEST" -> null
            # (2 unchanged attributes hidden)
        }
    }
Plan: 1 to add, 1 to change, 1 to destroy.
module.cloud_run.module.cloud_run.google_cloud_run_v2_service.service[0]: Destroying... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/sda-untrusted-cr]
google_storage_notification.data_notifications_temp: Creating...
google_cloud_run_v2_service.services["cibus_convertor"]: Modifying... [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/cibus-convertor]
google_cloud_run_v2_service.services["cibus_convertor"]: Modifications complete after 0s [id=projects/sky3-geo-sat-prd-u-sda-1/locations/me-west1/services/cibus-convertor]
google_storage_notification.data_notifications_temp: Creation complete after 1s [id=sda-prod-untrusted-bucket/notificationConfigs/1]
╷
│ Error: cannot destroy service without setting deletion_protection=false and running `terraform apply`
│ 

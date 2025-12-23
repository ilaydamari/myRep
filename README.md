# module.cloud_run.google_service_account.cloud_run_service_account[0] will be destroyed
  # (because google_service_account.cloud_run_service_account is not in configuration)
  - resource "google_service_account" "cloud_run_service_account" {
      - account_id   = "sda-prod-cr-sa" -> null
      - disabled     = false -> null
      - email        = "sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com" -> null
      - id           = "projects/sky3-geo-sat-prd-d-sda-1/serviceAccounts/sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com" -> null
      - member       = "serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com" -> null
      - name         = "projects/sky3-geo-sat-prd-d-sda-1/serviceAccounts/sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com" -> null
      - project      = "sky3-geo-sat-prd-d-sda-1" -> null
      - unique_id    = "101208253553989312142" -> null
        # (2 unchanged attributes hidden)
    }
  # module.cloud_run.module.cloud_run.google_cloud_run_v2_service.service[0] will be destroyed
  # (because google_cloud_run_v2_service.service is not in configuration)
  - resource "google_cloud_run_v2_service" "service" {
      - annotations             = {} -> null
      - conditions              = [
          - {
              - last_transition_time = "2025-11-12T14:57:01.336842Z"
              - state                = "CONDITION_SUCCEEDED"
              - type                 = "RoutesReady"
                # (5 unchanged attributes hidden)
            },
          - {
              - last_transition_time = "2025-11-12T14:55:28.837386Z"
              - state                = "CONDITION_SUCCEEDED"
              - type                 = "ConfigurationsReady"
                # (5 unchanged attributes hidden)
            },
        ] -> null
      - create_time             = "2025-11-12T14:55:25.582268Z" -> null
      - creator                 = "dmz-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com" -> null
      - custom_audiences        = [] -> null
      - default_uri_disabled    = false -> null
      - deletion_protection     = true -> null
      - effective_annotations   = {} -> null
      - effective_labels        = {
          - "goog-terraform-provisioned" = "true"
        } -> null
      - etag                    = "\"CN2_0sgGEODo0pUC/cHJvamVjdHMvc2t5My1nZW8tc2F0LXByZC1kLXNkYS0xL2xvY2F0aW9ucy9tZS13ZXN0MS9zZXJ2aWNlcy9zZGEtZG16LWNy\"" -> null
      - generation              = "1" -> null
      - iap_enabled             = false -> null
      - id                      = "projects/sky3-geo-sat-prd-d-sda-1/locations/me-west1/services/sda-dmz-cr" -> null
      - ingress                 = "INGRESS_TRAFFIC_INTERNAL_ONLY" -> null
      - invoker_iam_disabled    = false -> null
      - labels                  = {} -> null
      - last_modifier           = "dmz-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com" -> null
      - latest_created_revision = "projects/sky3-geo-sat-prd-d-sda-1/locations/me-west1/services/sda-dmz-cr/revisions/sda-dmz-cr-00001-9bn" -> null
      - latest_ready_revision   = "projects/sky3-geo-sat-prd-d-sda-1/locations/me-west1/services/sda-dmz-cr/revisions/sda-dmz-cr-00001-9bn" -> null
      - launch_stage            = "GA" -> null
      - location                = "me-west1" -> null
      - name                    = "sda-dmz-cr" -> null
      - observed_generation     = "1" -> null
      - project                 = "sky3-geo-sat-prd-d-sda-1" -> null
      - reconciling             = false -> null
      - terminal_condition      = [
          - {
              - last_transition_time = "2025-11-12T14:57:01.367020Z"
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
      - uid                     = "ff6ae9c2-8e62-4f94-a959-6bf13ded0761" -> null
      - update_time             = "2025-11-12T14:55:25.582268Z" -> null
      - uri                     = "https://sda-dmz-cr-oiibs6nkdq-zf.a.run.app" -> null
      - urls                    = [
          - "https://sda-dmz-cr-128853460417.me-west1.run.app",
          - "https://sda-dmz-cr-oiibs6nkdq-zf.a.run.app",
        ] -> null
        # (5 unchanged attributes hidden)
      - template {
          - annotations                      = {} -> null
          - execution_environment            = "EXECUTION_ENVIRONMENT_GEN1" -> null
          - gpu_zonal_redundancy_disabled    = false -> null
          - labels                           = {} -> null
          - max_instance_request_concurrency = 80 -> null
          - service_account                  = "sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com" -> null
          - session_affinity                 = false -> null
          - timeout                          = "300s" -> null
            # (2 unchanged attributes hidden)
          - containers {
              - args           = [] -> null
              - build_info     = [] -> null
              - command        = [] -> null
              - depends_on     = [] -> null
              - image          = "me-west1-docker.pkg.dev/sky3-geo-sat-prd-d-sda-1/sda/sda-dmz:latest" -> null
              - name           = "default" -> null
                # (2 unchanged attributes hidden)
              - env {
                  - name  = "PROJECT_ID" -> null
                  - value = "sky3-geo-sat-prd-t-sda-1" -> null
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
                  - subnetwork = "projects/sky3-geo-sat-prod-d-0/regions/me-west1/subnetworks/prod-dmz-sda-1" -> null
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
Plan: 21 to add, 0 to change, 2 to destroy.
─────────────────────────────────────────────────────────────────────────────
Note: You didn't use the -out option to save this plan, so Terraform can't
guarantee to take exactly these actions if you run "terraform apply" now.
Finished Step #2 - "tf plan"
Starting Step #3 - "tf apply"
Already have image (with digest): hashicorp/terraform:latest
╷
│ Error: Error acquiring the state lock
│ 
│ Error message: writing "gs://sda-prod-dmz-state/default.tflock" failed:
│ googleapi: Error 412: At least one of the pre-conditions you specified did
│ not hold., conditionNotMet
│ Lock Info:
│   ID:        1766496909713081
│   Path:      gs://sda-prod-dmz-state/default.tflock
│   Operation: OperationTypePlan
│   Who:       root@2a5d50132a31
│   Version:   1.14.3
│   Created:   2025-12-23 13:35:10.665898127 +0000 UTC
│   Info:      
│ 
│ 
│ Terraform acquires a state lock to protect the state from being written
│ by multiple users at the same time. Please resolve the issue above and try
│ again. For most commands, you can disable locking with the "-lock=false"
│ flag, but this is not recommended.
╵
Finished Step #3 - "tf apply"

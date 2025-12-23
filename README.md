{
  "version": 4,
  "terraform_version": "1.14.3",
  "serial": 4,
  "lineage": "a3a9058b-d78d-3e2c-ddbb-9d8c30a4def4",
  "outputs": {},
  "resources": [
    {
      "mode": "data",
      "type": "google_cloud_run_v2_service",
      "name": "existing_services",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.cloud_run",
      "mode": "managed",
      "type": "google_service_account",
      "name": "cloud_run_service_account",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "index_key": 0,
          "schema_version": 0,
          "attributes": {
            "account_id": "sda-prod-cr-sa",
            "create_ignore_already_exists": null,
            "description": "",
            "disabled": false,
            "display_name": "",
            "email": "sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com",
            "id": "projects/sky3-geo-sat-prd-d-sda-1/serviceAccounts/sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com",
            "name": "projects/sky3-geo-sat-prd-d-sda-1/serviceAccounts/sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-prd-d-sda-1",
            "timeouts": null,
            "unique_id": "101208253553989312142"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjozMDAwMDAwMDAwMDB9fQ=="
        }
      ]
    },
    {
      "module": "module.cloud_run.module.cloud_run",
      "mode": "managed",
      "type": "google_cloud_run_v2_service",
      "name": "service",
      "provider": "provider[\"registry.terraform.io/hashicorp/google-beta\"]",
      "instances": [
        {
          "index_key": 0,
          "schema_version": 0,
          "attributes": {
            "annotations": {},
            "binary_authorization": [],
            "build_config": [],
            "client": "",
            "client_version": "",
            "conditions": [
              {
                "execution_reason": "",
                "last_transition_time": "2025-11-12T14:57:01.336842Z",
                "message": "",
                "reason": "",
                "revision_reason": "",
                "severity": "",
                "state": "CONDITION_SUCCEEDED",
                "type": "RoutesReady"
              },
              {
                "execution_reason": "",
                "last_transition_time": "2025-11-12T14:55:28.837386Z",
                "message": "",
                "reason": "",
                "revision_reason": "",
                "severity": "",
                "state": "CONDITION_SUCCEEDED",
                "type": "ConfigurationsReady"
              }
            ],
            "create_time": "2025-11-12T14:55:25.582268Z",
            "creator": "dmz-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com",
            "custom_audiences": [],
            "default_uri_disabled": false,
            "delete_time": "",
            "deletion_protection": true,
            "description": "",
            "effective_annotations": {},
            "effective_labels": {
              "goog-terraform-provisioned": "true"
            },
            "etag": "\"CN2_0sgGEODo0pUC/cHJvamVjdHMvc2t5My1nZW8tc2F0LXByZC1kLXNkYS0xL2xvY2F0aW9ucy9tZS13ZXN0MS9zZXJ2aWNlcy9zZGEtZG16LWNy\"",
            "expire_time": "",
            "generation": "1",
            "iap_enabled": false,
            "id": "projects/sky3-geo-sat-prd-d-sda-1/locations/me-west1/services/sda-dmz-cr",
            "ingress": "INGRESS_TRAFFIC_INTERNAL_ONLY",
            "invoker_iam_disabled": false,
            "labels": {},
            "last_modifier": "dmz-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com",
            "latest_created_revision": "projects/sky3-geo-sat-prd-d-sda-1/locations/me-west1/services/sda-dmz-cr/revisions/sda-dmz-cr-00001-9bn",
            "latest_ready_revision": "projects/sky3-geo-sat-prd-d-sda-1/locations/me-west1/services/sda-dmz-cr/revisions/sda-dmz-cr-00001-9bn",
            "launch_stage": "GA",
            "location": "me-west1",
            "name": "sda-dmz-cr",
            "observed_generation": "1",
            "project": "sky3-geo-sat-prd-d-sda-1",
            "reconciling": false,
            "scaling": [],
            "template": [
              {
                "annotations": {},
                "containers": [
                  {
                    "args": [],
                    "base_image_uri": "",
                    "build_info": [],
                    "command": [],
                    "depends_on": [],
                    "env": [
                      {
                        "name": "PROJECT_ID",
                        "value": "sky3-geo-sat-prd-t-sda-1",
                        "value_source": []
                      },
                      {
                        "name": "TOPIC_ID",
                        "value": "sda-prod-topic",
                        "value_source": []
                      },
                      {
                        "name": "URL_MAPPING",
                        "value": "",
                        "value_source": []
                      }
                    ],
                    "image": "me-west1-docker.pkg.dev/sky3-geo-sat-prd-d-sda-1/sda/sda-dmz:latest",
                    "liveness_probe": [],
                    "name": "default",
                    "ports": [
                      {
                        "container_port": 8080,
                        "name": "http1"
                      }
                    ],
                    "resources": [
                      {
                        "cpu_idle": true,
                        "limits": {
                          "cpu": "1000m",
                          "memory": "512Mi"
                        },
                        "startup_cpu_boost": false
                      }
                    ],
                    "startup_probe": [
                      {
                        "failure_threshold": 1,
                        "grpc": [],
                        "http_get": [],
                        "initial_delay_seconds": 0,
                        "period_seconds": 240,
                        "tcp_socket": [
                          {
                            "port": 8080
                          }
                        ],
                        "timeout_seconds": 240
                      }
                    ],
                    "volume_mounts": [],
                    "working_dir": ""
                  }
                ],
                "encryption_key": "",
                "execution_environment": "EXECUTION_ENVIRONMENT_GEN1",
                "gpu_zonal_redundancy_disabled": false,
                "labels": {},
                "max_instance_request_concurrency": 80,
                "node_selector": [],
                "revision": "",
                "scaling": [
                  {
                    "max_instance_count": 10,
                    "min_instance_count": 0
                  }
                ],
                "service_account": "sda-prod-cr-sa@sky3-geo-sat-prd-d-sda-1.iam.gserviceaccount.com",
                "service_mesh": [],
                "session_affinity": false,
                "timeout": "300s",
                "volumes": [],
                "vpc_access": [
                  {
                    "connector": "",
                    "egress": "PRIVATE_RANGES_ONLY",
                    "network_interfaces": [
                      {
                        "network": "",
                        "subnetwork": "projects/sky3-geo-sat-prod-d-0/regions/me-west1/subnetworks/prod-dmz-sda-1",
                        "tags": []
                      }
                    ]
                  }
                ]
              }
            ],
            "terminal_condition": [
              {
                "execution_reason": "",
                "last_transition_time": "2025-11-12T14:57:01.367020Z",
                "message": "",
                "reason": "",
                "revision_reason": "",
                "severity": "",
                "state": "CONDITION_SUCCEEDED",
                "type": "Ready"
              }
            ],
            "terraform_labels": {
              "goog-terraform-provisioned": "true"
            },
            "timeouts": null,
            "traffic": [
              {
                "percent": 100,
                "revision": "",
                "tag": "",
                "type": "TRAFFIC_TARGET_ALLOCATION_TYPE_LATEST"
              }
            ],
            "traffic_statuses": [
              {
                "percent": 100,
                "revision": "",
                "tag": "",
                "type": "TRAFFIC_TARGET_ALLOCATION_TYPE_LATEST",
                "uri": ""
              }
            ],
            "uid": "ff6ae9c2-8e62-4f94-a959-6bf13ded0761",
            "update_time": "2025-11-12T14:55:25.582268Z",
            "uri": "https://sda-dmz-cr-oiibs6nkdq-zf.a.run.app",
            "urls": [
              "https://sda-dmz-cr-128853460417.me-west1.run.app",
              "https://sda-dmz-cr-oiibs6nkdq-zf.a.run.app"
            ]
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjoxMjAwMDAwMDAwMDAwLCJkZWxldGUiOjEyMDAwMDAwMDAwMDAsInVwZGF0ZSI6MTIwMDAwMDAwMDAwMH19",
          "dependencies": [
            "module.cloud_run.google_service_account.cloud_run_service_account",
            "module.cloud_run.module.cloud_run.google_service_account.service_account",
            "module.cloud_run.module.cloud_run.google_vpc_access_connector.connector"
          ]
        }
      ]
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_schema",
      "name": "default",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_subscription",
      "name": "default",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_subscription_iam_binding",
      "name": "authoritative",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_subscription_iam_binding",
      "name": "bindings",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_subscription_iam_member",
      "name": "members",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_topic",
      "name": "default",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "schema_version": 0,
          "attributes": {
            "effective_labels": {
              "goog-terraform-provisioned": "true"
            },
            "id": "projects/sky3-geo-sat-prd-d-sda-1/topics/sda-dmz-topic",
            "ingestion_data_source_settings": [],
            "kms_key_name": "",
            "labels": null,
            "message_retention_duration": "86400s",
            "message_storage_policy": [
              {
                "allowed_persistence_regions": [
                  "europe-west1",
                  "me-west1"
                ],
                "enforce_in_transit": false
              }
            ],
            "message_transforms": [],
            "name": "sda-dmz-topic",
            "project": "sky3-geo-sat-prd-d-sda-1",
            "schema_settings": [],
            "terraform_labels": {
              "goog-terraform-provisioned": "true"
            },
            "timeouts": null
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjoxMjAwMDAwMDAwMDAwLCJkZWxldGUiOjEyMDAwMDAwMDAwMDAsInVwZGF0ZSI6MTIwMDAwMDAwMDAwMH19",
          "dependencies": [
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_schema.default"
          ]
        }
      ]
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_topic_iam_binding",
      "name": "authoritative",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_topic_iam_binding",
      "name": "bindings",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    },
    {
      "module": "module.sda_dmz_pubsub[0].module.pubsub",
      "mode": "managed",
      "type": "google_pubsub_topic_iam_member",
      "name": "bindings",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": []
    }
  ],
  "check_results": null
}

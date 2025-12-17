

<header>

<!--
  <<< Author notes: Course header >>>
  Include a 1280×640 image, course title in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Add your open source license, GitHub uses MIT license.
-->

# Review pull requests

_Collaborate and work together on GitHub._

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Step 1: Open a pull request

_Welcome to "Review pull requests"! :wave:_

Let's get started by opening a pull request.

**What is a pull request?**: Collaboration happens on a pull request. The pull request shows the changes in your branch to other people. This pull request is going to keep the changes you just made on your branch and propose applying them to the `main` branch.

### :keyboard: Activity: Create a pull request

1. Click on the **Pull requests** tab in your repository.
2. Click **New pull request**.
3. In the **base:** dropdown, make sure **main** is selected.
4. Select the **compare:** dropdown, and click `update-game`.
5. Click **Create pull request**.
6. Enter a title for your pull request: `Update the game over message`.
7. Enter a description for your pull request: `Update the game over message so people know how to play again!`
8. Click **Create pull request**.
9. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---



{
  "version": 4,
  "terraform_version": "1.14.1",
  "serial": 23,
  "lineage": "93e0d785-a587-1312-0aea-87b4e2fe46cb",
  "outputs": {},
  "resources": [
    {
      "mode": "managed",
      "type": "google_cloud_run_service_iam_binding",
      "name": "eventarc_invoker",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "index_key": "sda-dmz-cr",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFgz5VyN0=",
            "id": "v1/projects/sky3-geo-sat-ppd-d-sda-1/locations/me-west1/services/sda-dmz-cr/roles/run.invoker",
            "location": "me-west1",
            "members": [
              "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com"
            ],
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/run.invoker",
            "service": "v1/projects/sky3-geo-sat-ppd-d-sda-1/locations/me-west1/services/sda-dmz-cr"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_cloud_run_v2_service.services",
            "google_service_account.service_accounts"
          ]
        }
      ]
    },
    {
      "mode": "managed",
      "type": "google_cloud_run_v2_service",
      "name": "services",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "index_key": "sda-dmz-cr",
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
                "last_transition_time": "2025-12-11T11:24:59.276449Z",
                "message": "",
                "reason": "",
                "revision_reason": "",
                "severity": "",
                "state": "CONDITION_SUCCEEDED",
                "type": "RoutesReady"
              },
              {
                "execution_reason": "",
                "last_transition_time": "2025-12-11T11:24:52.110342Z",
                "message": "",
                "reason": "",
                "revision_reason": "",
                "severity": "",
                "state": "CONDITION_SUCCEEDED",
                "type": "ConfigurationsReady"
              }
            ],
            "create_time": "2025-12-09T11:19:01.155278Z",
            "creator": "dmz-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com",
            "custom_audiences": [],
            "delete_time": "",
            "deletion_protection": false,
            "description": "",
            "effective_annotations": {},
            "effective_labels": {
              "goog-terraform-provisioned": "true"
            },
            "etag": "\"CILU6skGELjdjrAD/cHJvamVjdHMvc2t5My1nZW8tc2F0LXBwZC1kLXNkYS0xL2xvY2F0aW9ucy9tZS13ZXN0MS9zZXJ2aWNlcy9zZGEtZG16LWNy\"",
            "expire_time": "",
            "generation": "4",
            "id": "projects/sky3-geo-sat-ppd-d-sda-1/locations/me-west1/services/sda-dmz-cr",
            "ingress": "INGRESS_TRAFFIC_INTERNAL_ONLY",
            "invoker_iam_disabled": false,
            "labels": {},
            "last_modifier": "dmz-sat-iac-sa@sky3-geo-cicd.iam.gserviceaccount.com",
            "latest_created_revision": "projects/sky3-geo-sat-ppd-d-sda-1/locations/me-west1/services/sda-dmz-cr/revisions/sda-dmz-cr-00004-fh5",
            "latest_ready_revision": "projects/sky3-geo-sat-ppd-d-sda-1/locations/me-west1/services/sda-dmz-cr/revisions/sda-dmz-cr-00004-fh5",
            "launch_stage": "GA",
            "location": "me-west1",
            "name": "sda-dmz-cr",
            "observed_generation": "4",
            "project": "sky3-geo-sat-ppd-d-sda-1",
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
                        "name": "MATZOV_BUCKET",
                        "value": "sat-sky-shar-sha-preprod-t-junction-2",
                        "value_source": []
                      },
                      {
                        "name": "SDA_FOLDER",
                        "value": "9900/SDA/idfcts",
                        "value_source": []
                      },
                      {
                        "name": "SOURCE_BUCKET",
                        "value": "sda-preprod-untrusted-bucket",
                        "value_source": []
                      },
                      {
                        "name": "TARGET_BUCKET",
                        "value": "sda-preprod-trusted-bucket",
                        "value_source": []
                      },
                      {
                        "name": "TRUSTED_PROJECT_ID",
                        "value": "sky3-geo-sat-ppd-t-sda-1",
                        "value_source": []
                      }
                    ],
                    "image": "me-west1-docker.pkg.dev/sky3-geo-sat-ppd-d-sda-1/sda/untrustedtotrusted:latest",
                    "liveness_probe": [],
                    "name": "",
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
                          "cpu": "1",
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
                "execution_environment": "",
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
                "service_account": "sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
                "session_affinity": false,
                "timeout": "300s",
                "volumes": [],
                "vpc_access": [
                  {
                    "connector": "",
                    "egress": "PRIVATE_RANGES_ONLY",
                    "network_interfaces": [
                      {
                        "network": "projects/sky3-geo-sat-preprod-d-0/global/networks/preprod-dmz-sat",
                        "subnetwork": "projects/sky3-geo-sat-preprod-d-0/regions/me-west1/subnetworks/preprod-dmz-sda-1",
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
                "last_transition_time": "2025-12-11T11:24:59.308876Z",
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
            "uid": "4599eca6-a134-4272-bc84-36471234fc7c",
            "update_time": "2025-12-11T11:24:50.906211Z",
            "uri": "https://sda-dmz-cr-f6nmanuzba-zf.a.run.app",
            "urls": [
              "https://sda-dmz-cr-877183981220.me-west1.run.app",
              "https://sda-dmz-cr-f6nmanuzba-zf.a.run.app"
            ]
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjoxMjAwMDAwMDAwMDAwLCJkZWxldGUiOjEyMDAwMDAwMDAwMDAsInVwZGF0ZSI6MTIwMDAwMDAwMDAwMH19",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        }
      ]
    },
    {
      "mode": "managed",
      "type": "google_eventarc_trigger",
      "name": "sda_dmz_trigger",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "index_key": 0,
          "schema_version": 0,
          "attributes": {
            "channel": "",
            "conditions": {},
            "create_time": "2025-12-09T13:44:13.613969558Z",
            "destination": [
              {
                "cloud_function": "",
                "cloud_run_service": [
                  {
                    "path": "/process",
                    "region": "me-west1",
                    "service": "sda-dmz-cr"
                  }
                ],
                "gke": [],
                "http_endpoint": [],
                "network_config": [],
                "workflow": ""
              }
            ],
            "effective_labels": {
              "component": "sda-dmz",
              "environment": "preprod",
              "goog-terraform-provisioned": "true"
            },
            "etag": "",
            "event_data_content_type": "",
            "id": "projects/sky3-geo-sat-ppd-d-sda-1/locations/me-west1/triggers/sda-dmz-trigger",
            "labels": {
              "component": "sda-dmz",
              "environment": "preprod"
            },
            "location": "me-west1",
            "matching_criteria": [
              {
                "attribute": "type",
                "operator": "",
                "value": "google.cloud.pubsub.topic.v1.messagePublished"
              }
            ],
            "name": "projects/sky3-geo-sat-ppd-d-sda-1/locations/me-west1/triggers/sda-dmz-trigger",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "service_account": "sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "terraform_labels": {
              "component": "sda-dmz",
              "environment": "preprod",
              "goog-terraform-provisioned": "true"
            },
            "timeouts": null,
            "transport": [
              {
                "pubsub": [
                  {
                    "subscription": "projects/sky3-geo-sat-ppd-d-sda-1/subscriptions/eventarc-me-west1-sda-dmz-trigger-sub-522",
                    "topic": "projects/sky3-geo-sat-ppd-d-sda-1/topics/sda-dmz-topic"
                  }
                ]
              }
            ],
            "uid": "3e6b1ae3-4a75-4ffd-8f40-5b5b9b91fa82",
            "update_time": "2025-12-09T13:44:22.600715408Z"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjoxMjAwMDAwMDAwMDAwLCJkZWxldGUiOjEyMDAwMDAwMDAwMDAsInVwZGF0ZSI6MTIwMDAwMDAwMDAwMH19",
          "dependencies": [
            "data.google_cloud_run_v2_service.existing_services",
            "google_cloud_run_v2_service.services",
            "google_service_account.service_accounts",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_schema.default",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription.default",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription_iam_binding.authoritative",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription_iam_binding.bindings",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription_iam_member.members",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic.default",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic_iam_binding.authoritative",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic_iam_binding.bindings",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic_iam_member.bindings"
          ]
        }
      ]
    },
    {
      "mode": "managed",
      "type": "google_project_iam_member",
      "name": "service_account_roles",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "index_key": "cloud_run-roles/artifactregistry.writer",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/artifactregistry.writer/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/artifactregistry.writer"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/compute.networkAdmin",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/compute.networkAdmin/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/compute.networkAdmin"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/compute.viewer",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/compute.viewer/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/compute.viewer"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/dataflow.worker",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/dataflow.worker/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/dataflow.worker"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/eventarc.eventReceiver",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/eventarc.eventReceiver/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/eventarc.eventReceiver"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/iam.serviceAccountTokenCreator",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/iam.serviceAccountTokenCreator/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/iam.serviceAccountTokenCreator"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/logging.logWriter",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/logging.logWriter/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/logging.logWriter"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/pubsub.admin",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/pubsub.admin/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/pubsub.admin"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/pubsub.publisher",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/pubsub.publisher/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/pubsub.publisher"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/pubsub.subscriber",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/pubsub.subscriber/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/pubsub.subscriber"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/pubsub.viewer",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/pubsub.viewer/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/pubsub.viewer"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/run.admin",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/run.admin/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/run.admin"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/run.developer",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/run.developer/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/run.developer"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/run.invoker",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/run.invoker/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/run.invoker"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/storage.admin",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/storage.admin/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/storage.admin"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        },
        {
          "index_key": "cloud_run-roles/storage.objectAdmin",
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFg0FAQDQ=",
            "id": "sky3-geo-sat-ppd-d-sda-1/roles/storage.objectAdmin/serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/storage.objectAdmin"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "google_service_account.service_accounts"
          ]
        }
      ]
    },
    {
      "mode": "managed",
      "type": "google_pubsub_topic_iam_member",
      "name": "untrusted_gcs_publisher",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "index_key": 0,
          "schema_version": 0,
          "attributes": {
            "condition": [],
            "etag": "BwZFhRt1PIY=",
            "id": "projects/sky3-geo-sat-ppd-d-sda-1/topics/sda-dmz-topic/roles/pubsub.publisher/serviceAccount:service-656810250574@gs-project-accounts.iam.gserviceaccount.com",
            "member": "serviceAccount:service-656810250574@gs-project-accounts.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "role": "roles/pubsub.publisher",
            "topic": "projects/sky3-geo-sat-ppd-d-sda-1/topics/sda-dmz-topic"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "bnVsbA==",
          "dependencies": [
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_schema.default",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription.default",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription_iam_binding.authoritative",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription_iam_binding.bindings",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_subscription_iam_member.members",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic.default",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic_iam_binding.authoritative",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic_iam_binding.bindings",
            "module.sda_dmz_pubsub.module.pubsub.google_pubsub_topic_iam_member.bindings"
          ]
        }
      ]
    },
    {
      "mode": "managed",
      "type": "google_service_account",
      "name": "service_accounts",
      "provider": "provider[\"registry.terraform.io/hashicorp/google\"]",
      "instances": [
        {
          "index_key": "cloud_run",
          "schema_version": 0,
          "attributes": {
            "account_id": "sda-preprod-cr-sa",
            "create_ignore_already_exists": null,
            "description": "",
            "disabled": false,
            "display_name": "Cloud Run Service Account",
            "email": "sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "id": "projects/sky3-geo-sat-ppd-d-sda-1/serviceAccounts/sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "member": "serviceAccount:sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "name": "projects/sky3-geo-sat-ppd-d-sda-1/serviceAccounts/sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com",
            "project": "sky3-geo-sat-ppd-d-sda-1",
            "timeouts": null,
            "unique_id": "102459489771664995189"
          },
          "sensitive_attributes": [],
          "identity_schema_version": 0,
          "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjozMDAwMDAwMDAwMDB9fQ=="
        }
      ]
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
            "id": "projects/sky3-geo-sat-ppd-d-sda-1/topics/sda-dmz-topic",
            "ingestion_data_source_settings": [],
            "kms_key_name": "",
            "labels": {},
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
            "project": "sky3-geo-sat-ppd-d-sda-1",
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
    }
  ],
  "check_results": null
}


Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/review-pull-requests) &bull; [Review the GitHub status page](https://www.githubstatus.com/)


&copy; 2023 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>

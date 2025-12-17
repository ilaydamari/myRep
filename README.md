

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

##############################################################













{
  "textPayload": "[2025-12-17T13:13:59.314Z] [ERROR] Error writing file: gs://sda-preprod-trusted-bucket/TLEs/celestrack | Meta: {\"message\":\"{\\n  \\\"error\\\": {\\n    \\\"code\\\": 403,\\n    \\\"message\\\": \\\"sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com does not have storage.objects.create access to the Google Cloud Storage object. Permission 'storage.objects.create' denied on resource (or it may not exist).\\\",\\n    \\\"errors\\\": [\\n      {\\n        \\\"message\\\": \\\"sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com does not have storage.objects.create access to the Google Cloud Storage object. Permission 'storage.objects.create' denied on resource (or it may not exist).\\\",\\n        \\\"domain\\\": \\\"global\\\",\\n        \\\"reason\\\": \\\"forbidden\\\"\\n      }\\n    ]\\n  }\\n}\\n\"}",
  "insertId": "6942ac970004c70fef7c9da2",
  "resource": {
    "type": "cloud_run_revision",
    "labels": {
      "revision_name": "sda-dmz-cr-00005-d5d",
      "service_name": "sda-dmz-cr",
      "configuration_name": "sda-dmz-cr",
      "location": "me-west1",
      "project_id": "sky3-geo-sat-ppd-d-sda-1"
    }
  },
  "timestamp": "2025-12-17T13:13:59.313103Z",
  "labels": {
    "instanceId": "0007e26d6826bb8da8415d26a9633fae2f9093e1d25640beea63c3018d02fe15887479d05daec77f109dcd54fa39df8b19d718bbce0a8fd99e6ecb7de2418813c183e0b63d34dcf9a17ed3f8174a2b"
  },
  "logName": "projects/sky3-geo-sat-ppd-d-sda-1/logs/run.googleapis.com%2Fstderr",
  "receiveTimestamp": "2025-12-17T13:13:59.344060567Z"
}







{
  "textPayload": "[2025-12-17T13:13:59.601Z] [ERROR] Error writing file to Matzov: gs://sda-preprod-trusted-bucket/TLEs/celestrack | Meta: {\"message\":\"{\\n  \\\"error\\\": {\\n    \\\"code\\\": 403,\\n    \\\"message\\\": \\\"sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com does not have storage.objects.create access to the Google Cloud Storage object. Permission 'storage.objects.create' denied on resource (or it may not exist).\\\",\\n    \\\"errors\\\": [\\n      {\\n        \\\"message\\\": \\\"sda-preprod-cr-sa@sky3-geo-sat-ppd-d-sda-1.iam.gserviceaccount.com does not have storage.objects.create access to the Google Cloud Storage object. Permission 'storage.objects.create' denied on resource (or it may not exist).\\\",\\n        \\\"domain\\\": \\\"global\\\",\\n        \\\"reason\\\": \\\"forbidden\\\"\\n      }\\n    ]\\n  }\\n}\\n\"}",
  "insertId": "6942ac97000927eb866be671",
  "resource": {
    "type": "cloud_run_revision",
    "labels": {
      "project_id": "sky3-geo-sat-ppd-d-sda-1",
      "revision_name": "sda-dmz-cr-00005-d5d",
      "service_name": "sda-dmz-cr",
      "configuration_name": "sda-dmz-cr",
      "location": "me-west1"
    }
  },
  "timestamp": "2025-12-17T13:13:59.600043Z",
  "labels": {
    "instanceId": "0007e26d6826bb8da8415d26a9633fae2f9093e1d25640beea63c3018d02fe15887479d05daec77f109dcd54fa39df8b19d718bbce0a8fd99e6ecb7de2418813c183e0b63d34dcf9a17ed3f8174a2b"
  },
  "logName": "projects/sky3-geo-sat-ppd-d-sda-1/logs/run.googleapis.com%2Fstderr",
  "receiveTimestamp": "2025-12-17T13:13:59.677710387Z"
}

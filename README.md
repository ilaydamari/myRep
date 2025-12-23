terraform state mv `
  module.cloud_run.google_service_account.cloud_run_service_account[0] `
  google_service_account.service_accounts["cloud_run"]

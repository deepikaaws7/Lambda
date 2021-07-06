# Lambda
module "_s3_bucket" {
  for_each             = { for k in local.s3_bucket_list : k.bucket_name_key => k }
  

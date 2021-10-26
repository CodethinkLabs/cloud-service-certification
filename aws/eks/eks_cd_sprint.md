# Sprint outcomes from codethink's github actions sprint wk41/42 2021

We achieved most of our sprint goals, not all of the work completed can be landed
currently until the process discussions we opened have been concluded.

* Ushered in PR to establish initial GitHub Action workflow for format checking
  of terraform files:
  - https://github.com/finos/cloud-service-certification/pull/144
* Pull request to modify terraform fmt workflow to only run when necessary:
  - https://github.com/finos/cloud-service-certification/pull/148
* Raised the issue of the IAM permissions being out of date on slack.
    * This was subsequently fixed by Abdullah Garcia:
      https://github.com/finos/cloud-service-certification/pull/145
    * Discussion in github on the approaches to take to ensure users
      don't hit the same issue in the future:
      https://github.com/finos/cloud-service-certification/discussions/157
* Testing of current EKS terraform files
    * Pull request to update the terraform version required by the eks terraform
      definitions: https://github.com/finos/cloud-service-certification/pull/147
* Initial implementation for a pipeline that verifies the AWS EKS terraform
  through automated deployment via GitHub actions:
  - Pull request: https://github.com/finos/cloud-service-certification/pull/150
  - Pipeline can be seen working @
    https://github.com/CodethinkLabs/cloud-service-certification/runs/3952797845
  - Discussion on enabling the use of secrets/credentials for forked
    repositories:
    https://github.com/finos/cloud-service-certification/discussions/152

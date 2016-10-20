# minio-release

## Features
Basic deployment for a minio server with an attached persistent disk for storage.

## Deploying

You can deploy minio-release to BOSH-lite for local testing, or a real BOSH install.  Instructions for setting up BOSH-lite are at https://github.com/cloudfoundry/bosh-lite.

Check out the "templates" directory for a BOSH v1 and v2 (cloud config) manifest for deployment.  Your settings will vary based on your IaaS setup, but particularly pay attention to the "properties" section for the job to set your own Access Key and Secret Key for the server.

You can adjust the size of the persistent disk attached to the job in the manifest to change the storage capacity of the server.

Also, you will need to adjust the name of the stemcell in the deployment manifest to match what ever stemcell is appropriate for your IaaS.

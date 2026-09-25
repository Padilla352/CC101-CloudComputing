# MinIO Deployment

## Overview

MinIO was deployed as an object storage server using Docker. The deployment was performed in an Ubuntu 24.04 environment using KillerCoda.

## Docker Image

The original laboratory instructions referenced the `minio/minio` image. In my environment, pulling that image returned an access/authorization error. After troubleshooting, the `elestio/minio` image was successfully pulled and used for the deployment.

## Pull the MinIO Image

```bash
docker pull elestio/minio

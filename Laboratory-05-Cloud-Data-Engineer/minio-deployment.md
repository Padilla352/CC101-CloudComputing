# MinIO Deployment

## Overview

For this laboratory, I deployed an S3-compatible MinIO object storage
server using Docker on a KillerCoda Ubuntu 24.04 environment.

The original laboratory command used the `minio/minio` image. Because that
image could not be pulled in my environment, I used the available
`elestio/minio` image instead.

## Docker Command

The command I successfully used was:

```bash

docker run -d \
  -p 9000:9000 \
  -p 9001:9001 \
  --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  elestio/minio \
  server /data --console-address ":9001"

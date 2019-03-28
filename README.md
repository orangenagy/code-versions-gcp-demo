# Code repository

## Overview
Under ROOT we have the code repository, a tree structure similar to what we have in NFS. We can sync this to a GCS bucket if we want to avoid mounting buckets in GCP.

## Steps
1. rsync the bucket
```cd ROOT
gsutil -d -r . gs://<code_bucket>/```

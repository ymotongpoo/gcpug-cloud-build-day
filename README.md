# GCPUG Cloud Build Day demo

This repository is created to demonstrate the following features of [Google Cloud Build](https://cloud.google.com/cloud-build/) for [GCPUG Cloud Build Day](https://gcpug-tokyo.connpass.com/event/143453/)

* Native [Cloud Builder](https://cloud.google.com/cloud-build/docs/cloud-builders) support for Go
* Concurrent build using [build step order configuration](https://cloud.google.com/cloud-build/docs/configuring-builds/configure-build-step-order)
* Allowing [Docker's QEMU support](https://hub.docker.com/r/multiarch/qemu-user-static/) on Google Cloud Build
* Artifacts & images deployment

## How to try

1. Create Google Cloud Stroage bucket with the name `$PROJECT_ID-hello`.
2. Run Google Cloud Build

```
$ gcloud builds submit --config cloudbuild.yaml .
```
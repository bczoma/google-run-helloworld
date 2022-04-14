# Cloud Run Hello World with Logging

## Deploy

```sh
# Set an environment variable with your GCP Project ID
export GOOGLE_CLOUD_PROJECT=<PROJECT_ID>

# Submit a build using Google Cloud Build
gcloud builds submit --tag gcr.io/${GOOGLE_CLOUD_PROJECT}/helloworld-with-logging

# Deploy to Cloud Run
gcloud run deploy helloworld-with-logging \
--image gcr.io/${GOOGLE_CLOUD_PROJECT}/helloworld-with-logging
```


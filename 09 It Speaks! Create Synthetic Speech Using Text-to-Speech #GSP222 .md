# GSP222
## Run in cloudshell
```cmd
export PROJECT_ID=$(gcloud config get-value project)
gcloud services enable texttospeech.googleapis.com
gcloud iam service-accounts create tts-qwiklab
gcloud iam service-accounts keys create tts-qwiklab.json --iam-account tts-qwiklab@$PROJECT_ID.iam.gserviceaccount.com
export GOOGLE_APPLICATION_CREDENTIALS=tts-qwiklab.json
```

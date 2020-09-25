# Google Cloud Functions course

## Creating a Project
To create a new project in Google Cloud, go to [Firebase Console](https://console.firebase.google.com) or create a new project from [Google Cloud Platform](https://console.cloud.google.com)  also.

## Create python virtual environment
Install python venv with the following command:
Windows
```
python -m venv "name_of_virtual_env"
```
Linux
```
sudo apt install python3-venv
python3 -m venv venv
source venv/bin/activate
```
To add packages to virtual environment we use "requirements.txt" and execute it as:
```
pip install -r requirements.txt
```
### Deploying the function to google cloud
First we have to set the project id with following command
```
gcloud config set project [YOUR PROJECT ID]
```
Then we deploy our function with this command:
```
.\google-cloud-sdk\bin\gcloud functions deploy [FUNCTION NAME] --runtime python37 --trigger-http

```
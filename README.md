# Encrypted-G-Drive
Project to encrypt files stored in Google Drive

## Getting Set-up
1. Create Virtru account and note the App ID
2. Create "O Auth Client ID" from google developer console 
3. Download and copy the ID created to the file location of api code to authorize the user
4. Add the virtru email and app id to credentials file (see illustration below)
5. Select file you want to upload to drive (We choose the file location to be same as the api code path) (see cli command run instruction below)
6. Run the encrypt command
7. File is encrypted and uploaded (this can be decrypted only with the user private credentials generated)
8. Run the command to decrypt
9. At the api code path you will find the decrypted file

## Running node app
Run node app using command below:

```
node secure-file-gdrive.js [encrypt|decrypt] <file_to_encrypt_or_decrypt>
```

## Setting up Virtru credentials

Once `credentials.json` file has been created by google drive api, update it as below with virtru app id and email obtained from Virtru dashboard:

```
{
    "installed": {...},
    "virtru": {
        "app_id": "app_id_from_virtru_dashboard",
        "email": "login_email_to_virtru_dashboard"
    }
}
```
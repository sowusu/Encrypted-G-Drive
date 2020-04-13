# Encrypted-G-Drive
Project to encrypt files stored in Google Drive


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
# SAP Build Project: Purchase Order Creation

## Version History
- **v1.0.0**: Fixed pricing element validation errors and added NetPriceQuantity.

## Prerequisites for Deployment
To run this project after importing, ensure the following BTP Destinations are configured:
1. **Destination Name**: `S4_ZARANTECH`
   - **URL**: http://mtsapserver6.btp.com:8000
   - **Proxy Type**: OnPremise
   - **Authentication**: BasicAuthentication (user - ZJULCAPM00)
2. **Destination Name**: `CAP_SERVICE`
   - **URL**: https://73a2caddtrial-dev-training-poc-srv.cfapps.us10-001.hana.ondemand.com/odata/v4/catalog
   - **Proxy Type**: OnPremise
   - **Authentication**: BasicAuthentication (OAuth2ClientCredentials (client id, secret, token url - <url>/oauth/token))


steps to impor this project into build lobby

1. Pull the Repository: Run git pull origin main to fetch the latest files to your machine.
2. Import to Lobby: Go to your SAP Build Lobby, click Import, and select the .mtar file from your local repository folder.
3. Map the Destination: Open the imported project, navigate to the Actions step, and link it back to your active BTP target destination (using the notes you left in your README.md).
4. Deploy: Click the Deploy button to make the workflow live.
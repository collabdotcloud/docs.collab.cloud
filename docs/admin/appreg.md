# Connections Application Register (AppReg)

If you are using API's for Connections SmartCloud you need to check these list

- The URL needs to be adjusted to your new company url. <https://apps.[DC].collabserv.com> needs to be changed to <https://companyname.collab.cloud>

- You're OAuth integration needs a new Client ID and Client Secret

- all the Connections content related API's should work.

- Not supported at the moment are the BSS API's.

## Oidc Endpoints

There are 2 sets of url's depending on your datacenter location.

### Europe

Authentication endpoint <https://logineu.collab.cloud/auth/realms/connections-mt/protocol/openid-connect/auth>

Token endpoint <https://logineu.collab.cloud/auth/realms/connections-mt/protocol/openid-connect/token>

### North America

Authentication endpoint <https://loginna.collab.cloud/auth/realms/connections-mt/protocol/openid-connect/auth>

Token endpoint <https://loginna.collab.cloud/auth/realms/connections-mt/protocol/openid-connect/token>

## API and Authentication

Depending on the API endpoints the way for authentication is slightly different. See [HCL API documentation](https://ds-infolib.hcltechsw.com/ldd/lcwiki.nsf) for more details.
Any endpoint which contains the authentication method oauth can be used directly. [Example files feed](https://ds-infolib.hcltechsw.com/ldd/appdevwiki.nsf/xpAPIViewer.xsp?lookupName=API+Reference#action=openDocument&res_title=Getting_a_feed_of_your_pinned_files_ic50&content=apicontent).
For this endpoint you have 2 options basic and oauth.

### OAuth endpoints

These endpoints can be called directly after the OAUTH/OIDC authentication flow has finished.
Example endpoint is ```/files/oauth/api/nonce```

### Basic and Form endpoints

These endpoints need some more care.
In order to use the basic endpoints you need to call an oauth endpoint first to get the LTPAToken2 cookie.
One way to get the LTPAToken2 is to call the files nonce endpoint at ```/files/oauth/api/nonce```

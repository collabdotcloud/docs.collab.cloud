# Known Issues

Below are the current known platform issues within the ThreeThirds collaboration platform. Please email [support@collab.cloud](mailto:support@collab.cloud) to report defects within the platform.

Keep in mind that we are starting with a fresh empty environment where we import thousands of users and a massive amount of data into, very fast. This can during the migration period temporarily cause slowness and other minor hickups on the platform, before all users and all data is migrated.

We kindly ask for your patience as we are working as fast as we can to get all customers migrated before the hard deadline.

Thank you for your understanding!

---

## Spelling service is unavailable

We discovered a potential performance problem due to a bug in the spelling service of the richtext editor. The spelling service will be unavailable from July 22. The vendor is currently working on a fix. We expect to get the fix during August.

## Internet Explorer 11

Internet Explorer 11 is not supported on our environment. While we realize it is supported on HCL Connections 6.5 on premise, it is not on HCL Connections 6.5 Multi Tenant. We have filed a request to support this in future versions with HCL.

## Slowness on the platform

We see a slowness on the platform, this is expected. We are transferring many customers and terabytes of data on the same disks Connections is using. At the same time search is indexing all new content we bulk add.

## Slowness on Viewing Documents

Servers are in good shape and adequately sized. We see 2 issues, thumbnails are constantly being generated for the millions of files we are importing. We also think there is a bug or configuration issue on one of the servers. We are giving this topic our highest priority right now.

## Search

The Search index is not up to date. It is being rebuilt as soon as possible. This is due to constant importing of data into the databases and file system, it is impossible to keep up until migrations are finished. New content is being indexed, migrated content will be indexed with a delay

## Sametime

### Sametime Login

The "Remember me" function in login page is not working and will result in a indefinite reload on starting the app on next day. This issue will appear on embedded Sametime within Notes client as well as in Sametime standalone client.
Please do not use this function until this issue is solved.

### Sametime Connections Plugin

The Sametime Connections plugin (upper right corner) is not working as expected. Login is successful but no chat will be received if someone is ping you.
Please use the webchat (webchatna.collab.cloud / webchateu.collab.cloud) instead until this issue is resolved

## Open Cases with HCL

### Newsletter

Wrong links in newsletters for example the invitation to communities duplicates the hostname.

### Wiki

Wrong links in Apps menu and API calls to oauth endpoints in wikis return wrong links

### Files search results

The searchresults for community files show an inaccessible link for communities.

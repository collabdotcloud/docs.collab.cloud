# Known Issues

Below are the current known platform issues within the ThreeThirds collaboration platform. Please email [support@collab.cloud](mailto:support@collab.cloud) to report defects within the platform.

Keep in mind that we are starting with a fresh empty environment where we import thousands of users and a massive amount of data into, very fast. This can during the migration period temporarily cause slowness and other minor hickups on the platform, before all users and all data is migrated.

We kindly ask for your patience as we are working as fast as we can to get all customers migrated before the hard deadline.

Thank you for your understanding!

---

## Slowness on the platform
We see a slowness on the platform, this is expected. We are transferring many customers and terabytes of data on the same disks Connections is using. At the same time search is indexing all new content we bulk add.

##Slowness on Viewing Documents
Servers are in good shape and adequately sized. We see 2 issues, thumbnails are constantly being generated for the millions of files we are importing. We also think there is a bug or configuration issue on one of the servers. We are giving this topic our highest priority right now.

##Bad Gateway
Some of you might occasionally see a bad gateway message. We have been working hard on these and have already seen a massive decrease in the amount of times this happens after some actions on our side. We keep investigating, please hit the refresh button if it happens

##Sametime 9 and 10 client
There is currently an issue we have raised with HCL were it is not possible to logon to Sametime using the rich client prior to version 11. We have an open case with HCL, in the meanwhile please use the webchat or upgrade your client. You can download the most recent version on downladseu.collab.cloud or downloadsna.collab.cloud

##Internet Explorer 11
Internet Explorer 11 is not supported on our environment. While we realize it is supported on HCL Connections 6.5 on premise, it is not on HCL Connections 6.5 Multi Tenant. We have filed a request to support this in future versions with HCL

# Hybrid Customers
If you are a "Hybrid" customer (you have both an on-premise Domino environment and Mail in _collab.cloud_) you need to register new users in your on-premise Domino Directory.

The following is for Administrators to consider:

* You will need to register your new user in the Domino Directory, and set a password for the Notes ID if your user is to use Notes client.
* Notes ID/Internet passwords are not used to authenticate to Connections/Verse mail via browser and/or apps, plugins or other.
* If you are registering an on-premise Mail or Apps user - this user is completely independent of the _collab.cloud_ environment and this procedure does not apply.

---

## Register user in Domino Directory

Register the user as per your normal process, ensure that your nominated _collab.cloud_ mail servers have been specified, and that the correct Policy is applied. </br></br>
    ![domreg-basics](/assets/images/screen-shots/admin/domreg-basics.png)</br>
    ![domreg-mailserver](/assets/images/screen-shots/admin/domreg-mailserver.png)

---

## Directory Sync

Your Mail cluster is configured to synchronize your Domino Directory with the _collab.cloud_ identity management system and the Admin App approximately every <strong>4 hours</strong>\** </br></br>
    ![domreg-sync](/assets/images/screen-shots/admin/domreg-sync.png)

The Directory Sync process will detect changes in the Domino Directory and perform the following:

* Add any new users registered in the Domino Directory to _collab.cloud_ and will be visible in the Admin App
* Assign a _Clustered Mail Cloud_ license to any new users who are registered against your nominated _collab.cloud_ Mail Servers and mailboxes created
* Assign a _Clustered Mail Cloud_ license to any existing users who have been moved/updated to _collab.cloud_ Mail Servers and mailboxes transferred via Domino (adminP) process
* Assign a _Clustered Mail Cloud_ license to any existing Connections users in _collab.cloud_ who have been registered in the Domino Directory for mail
* Remove all licenses from any users who have been deleted from the Domino Directory and set the user status to Inactive

> ** The 4-hour sync process is temporary while migrations from IBM Connections Cloud are being completed and the User management processes are being finalised.

</br>
After the sync process has created/updated the user in the Admin App - you can then set a password and (if required) assign a Connections license. </br></br>
    ![domreg-adminapp](/assets/images/screen-shots/admin/domreg-adminapp.png)

You may also notice that the _Shortname/UserID_ field in the Person Document is updated with a unique number or univeral ID value.

* For users migrated from IBM Cloud it may be a value like `200112345`
* For new users it may be a value like `60474dad-d943-404c-8e1a-fb096bc54716`

</br>
    ![domreg-persondoc](/assets/images/screen-shots/admin/domreg-persondoc.png)

This is the assigned UID from the _collab.cloud_ identity system and is critical for Connections/Mail/IM integration and authentication. </br>
Please do not remove this value (as it will just reappear next sync and break functionality in the meantime).

---

## Set/Reset user password

Clicking the reset password button gives you 2 options as follows

  ![password reset](/assets/images/screen-shots/admin/reset.png)

  Clicking "Send reset email" sends a link to the user at their specified email address that they can click on to set their password.

  Clicking "Set password" allows you to set a temporary password for the user. They will need to change this as soon as they login.

> NOTE: For new Mail users - using the "Set password" function is required as the user will not be able to retrieve the password email if they have never logged in.

---

## Updating user info

Name changes performed via the Domino (adminP) process will be synchronized with the _collab.cloud_ Admin App - however <strong>email addresses are not changed automatically</strong>.</br></br>
Please send a request to [support@collab.cloud](mailto:support@collab.cloud) for email address changes for _Clustered Mail Cloud_ users.

---

## Deleting Users from Domino Directory

When a user is deleted from the Domino directory. The _Clustered Mail Cloud_ license is removed from the user in the Admin App via the sync process. The user remains Active until your administrator logs into the Admin App and performs further actions such as:

* Add/Remove other licenses for the user if required
* Set the user to `Inactive` if the user is intended to be deleted

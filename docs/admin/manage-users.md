# Manage your Users
How you manage your Users depends on your Organization Account Type. Follow the steps below to create a new User in your Organization account. If you are a Hybrid customer (you have both an on-premise Domino environment and Mail in _collab.cloud_) you will need to follow the steps for [Hybrid Customers](https://docs.collab.cloud/admin/manage-users-hybrid/)

---

## Adding a new user

1. From the "My Users" page, click the add button (bottom right)

    ![fab](/assets/images/screen-shots/admin/fab.png)

1. Provide all required information for the new user. The email must be unique. Note that you may use this form to create a guest / external user, if you do so that user will be provisioned as a connections guest and will not be able to be changed.

**Note!** External users cannot be invited directly in the Community. External users needs to be created in the dialog below.

    ![new user](/assets/images/screen-shots/admin/new-user.png)

---

## Adding a subscription

Locate the new user in your Users list and click them. If you have available subscriptions you will be presented with an option to assign a subscription to the user, click the menu and choose the appropriate subscription then click add.

### Connections

Connections subscriptions that are assigned to your Organization will be presented in the menu. Usually these options will be either: _Connections Engagement Suite_, _Connections Social_ or _Connections Docs_. Assigning a Connections license to a new User will create a new Profile in Connections. </br></br>
    ![add subscription](/assets/images/screen-shots/admin/add-sub.png)

### Mail
<strong>NOTE</strong>: Clustered Mail Cloud subscriptions can not yet be added via the _collab.cloud_ Admin App. For Clustered Mail Cloud subscriptions to be added to your User, please send a request to [support@collab.cloud](mailto:support@collab.cloud). </br>
For Hybrid customers - please follow the steps in the [Hybrid Customers](https://docs.collab.cloud/admin/manage-users-hybrid/) doc.

---

## Set/Reset user password

Clicking the reset password button gives you 2 options as follows

  ![password reset](/assets/images/screen-shots/admin/reset.png)

  Clicking "Send reset email" sends a link to the user at their specified email address that they can click on to set their password.

  Clicking "Set password" allows you to set a temporary password for the user. They will need to change this as soon as they login.

> NOTE: For new Mail users - using the "Set password" function is required as the user will not be able to retrieve the password email if they have never logged in.

---

## Updating user info

You can change a users name or email address by clicking the "EDIT" button from a user's record.

  ![edit user](/assets/images/screen-shots/admin/edit-user.png)

## Changing user role

When editing a user you may make them an organisation admin by changing their role from user to admin. You cannot change the role of a guest (visitor) user.

  ![user role](/assets/images/screen-shots/admin/user-role.png)

## Controlling user access

To disable access to all _collab.cloud_ services you may make a user Inactive when editing their details, this will _immediately_ remove them from all relevant groups and block access to logging in, it does not however remove any subscriptions from the user, if you wish to recover and reuse any connections subscriptions, you may also remove those by clicking the `x` on each subscription.

You may also update an "Inactive" user by setting them to "Active", this will reinstate any relevant groups and access as required.

  ![user status](/assets/images/screen-shots/admin/user-status.png)

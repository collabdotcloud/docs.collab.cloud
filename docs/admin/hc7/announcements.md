# Orient Me Announcements

Organisation Admins are now able to show announcements in our Connections environment. 

That's how it looks like:

![Header](/assets/images/admin/announcement/header.png)

It will open a dialog, when you click on *More*

![dialog](/assets/images/admin/announcement/dialog.png)

These announcements can be created in the [appregistry](/admin/appreg.md).

## Example

```json
{
    "name": "com.ibm.orientme.defaults",
    "title": "com.ibm.orientme.defaults",
    "description": "Global Defaults for OrientMe Service",
    "services": [
        "OrientMe"
    ],
    "state": "enabled",
    "extensions": [
        {
            "name": "Announcements override",
            "type": "com.ibm.announcements",
            "payload": {
                "cache-headers": {
                    "cache-control": "max-age=0"
                },
                "announcements": [
                    {
                        "title": "Collab Cloud Connections 7 Update",
                        "message": "We have updated our Collab.cloud to HCL Connections 7",
                        "link": "https://docs.collab.cloud/admin/hc7/whats-new/",
                        "linkTitle": "HCL Connections 7"
                    }
                ]
            },
            "path": "orientme"
        }
    ]
}
```

***Restrictions:*** There can only be one app active in the appregistry. If you have multiple messages just add it in the payload

```json
"payload": {
                "announcements": [
                    {
                        "title": "Collab Cloud Connections 7 Update",
                        "message": "We have updated our Collab.cloud to HCL Connections 7",
                        "link": "https://docs.collab.cloud/admin/hc7/whats-new/",
                        "linkTitle": "HCL Connections 7"
                    },
                    {
                        "title": "New CEO",
                        "message": "We are proud to announce a new CEO",
                        "link": "https://docs.collab.cloud/admin/hc7/whats-new/",
                        "linkTitle": "HCL Connections 7"
                    }
                ]
            }
```
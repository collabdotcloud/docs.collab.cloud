# What is Meeting integration

The meeting integration allows you to add a link to your personal meeting room in the HCL Connections header bar for easy access.

There are 2 options:
![Named Meeting Integration](/assets/images/admin/meeting/meeting.png)

and

![Meeting Integration](/assets/images/admin/meeting/meeting-header.png)

## Option 1: Named meeting integration

see [WebEx integration](/admin/extension-webex.md)

## Option 2: General Icon

### Enable integration

Similar to the WebEx integration the OrgAdmin needs to add the following appregistry extension

```js
{
    "name": "My WebMeeting",
    "title": "My WebMeeting",
    "description": "Allows each user to quickly access their own Web Meeting",
    "services": [
        "Customizer"
    ],
    "state": "enabled",
    "extensions": [
        {
            "name": "webMeeting",
            "type": "com.ibm.customizer.ui",
            "payload": {
                "include-files": [
                    "extensions/meeting/commonTools.js",
                    "extensions/meeting/webMeeting.js"
                ],
                "cache-headers": {
                    "cache-control": "max-age=43200"
                }
            },
            "path": "global",
            "state": "enabled"
        }
    ]
}
```

### Using the meeting link

Each user needs to put their meeting link in their Profile.
see [WebEx Link](/users/using-webex-extension.md).

The link name needs to be set to **Meeting** (case sensitive).

If everything is configured correctly, the meeting icon will appear.

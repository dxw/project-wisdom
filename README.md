# Project Wisdom

A Zendesk App that fetches contextual information about a ticket from its custom
project field.

## Prerequisites

To run the app locally, you'll need to have [Zendesk Apps Tools](https://develop.zendesk.com/hc/en-us/articles/360001075048-Installing-and-using-the-Zendesk-apps-tools) installed.

## Getting started

### Clone the repo

```bash
git clone git@github.com:dxw/project_wisdom.git
```

### Run the server locally

```bash
cd project_wisdom
zat server
```

You'll need the Airtable API Key and Base Key (available from the dxw 1Password).

### Access a ticket

Go to a ticket in Zendesk and append `?zat=true` to the url. eg:

```
https://dxw.zendesk.com/agent/tickets/123345?zat=true
```

Click on the `Apps` button on the ticket view to see the app in action!

## Building a new version

Run `zat validate`, review any errors/warnings, and then run `zat package`.

Upload the resulting Zip file to Zendeks following the [instructions on the Zendesk website](https://support.zendesk.com/hc/en-us/articles/203662486-Managing-your-installed-apps#topic_x3y_r22_r5).

# React My Teams

## Summary

This sample uses Microsoft Graph to list the Teams the current user is a member of. When the user clicks on one of the teams, the web part retrieves information about the default channel (General) and opens it.
The web part can be configured to open the team on the web browser or client app.

![Demo](./assets/Preview.png)

## Used SharePoint Framework Version

![drop](https://img.shields.io/badge/drop-1.7.1-green.svg)

## Applies to

- [SharePoint Framework](https:/dev.office.com/sharepoint)

## Prerequisites

- Office 365 subscription with SharePoint Online licence
- SharePoint Framework [development environment](https://dev.office.com/sharepoint/docs/spfx/set-up-your-development-environment) already set up.

## Solution

| Solution       | Author(s)      |
| -------------- | -------------- |
| react-my-teams | Joel Rodrigues |

## Version history

| Version | Date              | Comments        |
| ------- | ----------------- | --------------- |
| 1.0     | February 26, 2019 | Initial release |

## Disclaimer

**THIS CODE IS PROVIDED _AS IS_ WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

---

## Minimal Path to Awesome

- Clone this repository
- in the command line run:
  - `npm install`
  - `gulp serve --nobrowser`
- navigate to the hosted version of SharePoint workbench, eg. https://contoso.sharepoint.com/_layouts/15/workbench.aspx

### Grant the service principal permission to the MicroSoft Graph API

o365 spo login https://contoso-admin.sharepoint.com
o365 spo serviceprincipal grant add --resource 'Microsoft Graph' --scope 'User.Read.All'
o365 spo serviceprincipal grant add --resource 'Microsoft Graph' --scope 'User.ReadWrite.All'
o365 spo serviceprincipal grant add --resource 'Microsoft Graph' --scope 'Group.Read.All'
o365 spo serviceprincipal grant add --resource 'Microsoft Graph' --scope 'Group.ReadWrite.All'

## Features

This Web Part lists all the teams the current user is a member of.

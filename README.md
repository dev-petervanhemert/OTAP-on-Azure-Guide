# OTAP-on-Azure-Guide

- Create or config Azure Active Directory.
- Create new Users.
    - tfsServices user
    - tfsBuild user
    - tfsReport user
    - tfsDeveloper users
    - Add goup AAD DC Administrators.
- Change pssword new users. 
- Add Users to Group. 
          
- Create Virtual Network (Classic).
- Create AAD Domain Services.
- Add DNS server from Domain Service to the classic Network.
- Create Virtual Network (Resource Management).
    - Add DNS server (ip from AAD Domain Services)
- Peer the vNets.

- Prerequisites for VM.
    - Create NSG.
    - Create Storage Account.
    - Create Availebility Set.
- Create VM for Team Foundation Services 2017.
    - Connect to domain AD
    - Install TFS 2017 on VM.
- Create VM for SonarQube.
    - Connect to domain AD
    - Install SonarQUbe.
- Create VM for Development.
        -Install Visual Studio 2017.


## Create an Azure Active Directory tenant.

1. Navigate to https://manage.windowsazure.com and log in with the account that has an Azure subscription.
2. Click ACTIVE DIRECTORY management icon in the left pane.
3. Click NEW button at the bottom of the page.
4. Choose APP SERVICES > ACTIVE DIRECTORY > DIRECTORY > CUSTOM CREATE.
> <img src="/Images/01-CreateAD/02-CreateAD.PNG" width="600"/> 
5. In the Add directory page, enter a name and domain name. For country or region choose United States or the country were Data Catalog is available.
> <img src="/Images/01-CreateAD/03-CreateAD.PNG" width="600"/> 
6. Choose OK icon. An Azure Active Directory is created.

## Add a user to your Azure Active Directory tenant

You need a user from your Azure AD to register an Azure AD app. Here's how to add a user to your Azure Active Directory tenant:
1. In your Azure Active Directory, click USERS.
> <img src="/Images/02-Add Users/01-AddUser.png" width="600"/> 
2. At the bottom of the page, click ADD USER. A user account is used to register a Data Catalog app.

# API Key Management

To allow even larger organisations to handle API keys, we invested into a sound API key management. Users with the role **Account Admin**, **Compliance Manager** or **Project Manager** will find the API Key Management under ***> ADMINSITRATION > Scanners & API Keys**. you will hav the choice between  **API Keys** and **Public Release Keys**. 

At TrustSource we distinguish:

1. **API Keys**
   These are the standard keys, used to grant access to a specific set of actions.  

2. **Public Release Keys** ([read more](releasekeys.md))

   These keys are designed to be associated with a particular release of a software product / project or module. The scope of this key type will be limited to retrieve information of a particular module version, that has been approved for release. Upon creation you associate the key with the released product of choice and this binding can't be removed anymore. The idea behind this sort of key is to allow you to publish the key together with your software, especially for devices without display, e.g. in form of a QR code, which then can be linked to display the information you want, e.g /VEX, /notice or /SBOM.

Please choose **API Keys** for now and you will see a screen like show in the follwoing screenshot.

![ApiKeyMgmt](/Users/janthielscher/dev/api-docs/docs/assets/ApiKeyMgmt.jpg)

If you do not see a list, you might be the first entering this section. Then you will have to add your first key. In this screen you will have all functionality to craete, manage  and delete API keys. 



## Create an API Key

To create an API Key just push the "Create New" button at the bottom of the list. The service will open a modal and request a name and the scope.

> [!NOTE]
>
> Users with the role of a **Compliance Manager** have visibility of all keys, but will only be able to create ***Public Release Keys***. To create an API Key, you must be assigned either the *Manager* or the *Account Manager* role.  

### Assign a Key Name

Especially when using more than a handful of keys it makes sense to add meaningful names to keys. You may indicate the user, the department or a cost center in the name. The name will be used throughout the application for reference in all reportings, so you will have an immediate understanding of who is causing what sort of events.

### Assign a Scope to the Key

Maybe you do not want every key to read and write everything. Especially in larger organisations keys might get known by a larger audience. To limit the risk of loosing senstive information, we offer the option to limit capabilities of keys by assigning them roles. You may pick the roles from the list by typing a role name. It is possible to assign several roles. 

> [!NOTE]
>
> Modification of roles will only be possible while the key is unpublished/inactive! 

See roles and right section for  a detailed understanding of which role covers which action.

We have been discussing to limit the scope of keys to particular projects but did not yet get there. On the one hand it seems interesting to allow a key only to change/query information of a single project, on the other hand this would increase the complexity of key management, especially for centralised CI/CD approaches. Each project would have to bring its own API Key. Feel free to leave us a comment on the discussions to this topic.  

## Publish / Unpublish an API Key

To change the scope of a key or to temprarily pause a key from being actionable, you unpublish the key. This is comparable to deactivate the key temporarily. While a key is upublished, requests using that key will be rejected with a 403. 

It is always possible to publish the key again after having it unpublished. You may repeat this step as often as with a light switch.

## Delete an API Key

To finally delete a key, you must unpublish/deactivate it first. Deactivated keys may be deleted by clicking on the corresponding Delete button in the same line. You may be required to confirm the deletion by re-entering the key name before the request is accepted. After successful deletion the key will disappear. However, the taces and logs remain valid.




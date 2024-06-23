# API Key Management

To allow even larger organisations to handle API keys, we invested into a sound API key management. Users with the role **Account Admin**, **Compliance Manager** or **Project Manager** will find the API Key Management under **> ADMINSITRATION > Scanners & API Keys**.

<img src="/Users/janthielscher/dev/api-docs/docs/assets/APIKey_Screen.jpg" alt="Screen to manage API Keys" style="zoom:80%;" />

Here you will have all functionality to craete, manage  and delete API keys. We distinguish the following types of keys:

1. API Keys
   These are the standard keys, used to grant access to a specific set of actions.  

2. Public Release Keys

   These keys are designed to be associated with a particular release of a software product / project or module. The scope of this key type will be limited to retrieve information of a particular module version, that has been approved for release. Upon creation you associate the key with the released product of choice and this binding can't be removed anymore. RThe idea behind this sprt of key os to allow you to publish the key with your software, especially for devices without display, e.g. in forma QR code, which then can be linked to display the information yopu want, e.g /VEX, /notice or /SBOM.

3. Public BOM-Keys **- DEPRECATED**

   This form of key is available for backward compatibility only. Before allowing the association of a key with a release it has been possible to assign a specific SBOM to a key. We do not support this linking anymore, but since there are already keys in the field, we still offer to manage existing keys here.

4. Public Notice-Keys **- DEPRECATED**

   The same information applies here but for Notice Files. Please use ***Public Release Keys*** instead.



## Create an API Key

To create an API Key just push the "Create New" button at the bottom of the list. Users with the role of a **Compliance Manager** have visibility of all keys, but will only be able to create ***Public Release Keys***. 

### Assign a Key Name

Especially when using more than a handful of keys it makes a lot of sense to add meaningful names to keys. You may indicate a user, the department or a cost center in the name. The name will be used throughout the application, so you will have an immediate understanding of who is causing what sort of events.

### Assign a Scope to the Key

Maybe you do not want every key to read and write everything. Especially in larger organisations keys might get knwon by a lrger audience. To limit the risk of loosing senstive information, we offer the option to limit capabilities of keys by assigning them roles. You may pick the roles from the list by typing a role name. It is possible to assign several roles. 

> [!NOTE]
>
> Modification of roles will only be possible while the key is unpublished! 

We have been discussing to limit the scope of keys to particular projects but did not yet get there. On the one hand it seems interesting to allow a key only to change/query information of a single project, on the other hand this would increase the complexity of key management, especially for centralised CI/CD approaches a lot. Each project would have to bring its own API Key. Feel free to leave us a comment on the discussions to this topic.  

## Publish / Unpublish an API Key

To change the scope of a key or to temprarily pause a key from being actionable, you may unpublish a key. This is comparable to deactive the key temporarily. While a key is upublished requests using that key will be rejected with a 403. 

## Scoping an API Key

dcdd

## Delete an API Key






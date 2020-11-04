# Manage Tokens

HERE Data Hub APIs use project tokens that are tied to your Account or HERE Accounts SSO identity. Make sure to keep your credentials safe and don't include them directly in any web pages as they are the key to generate new access tokens.

Usually, you use two tokens:

* **token for working** - this has read&write permissions on your spaces. Keep this information private
* **token for sharing** - this should be generated with read-only permissions and can be included in web pages for publishing your data

## Token Administration

Log into the **Data Hub Token Generator** site with your `Email address` and `Password` or `HERE Accounts SSO identity`:

[`https://xyz.api.here.com/token-ui/`](https://xyz.api.here.com/token-ui/)

[![Login Screen](images/start-token-login.png)](https://xyz.api.here.com/token-ui/)

## Assign Access Rights

Once logged in, you see the list of spaces that are available to your account and the permissions that are available to be encoded in the token.

Available permissions for the token are:

* ReadFeatures
* CreateFeatures
* UpdateFeatures
* DeleteFeatures
* ManageSpaces

From the list, select the spaces the token should have access to. Note that some spaces can only be read and not written to.
It's good practice to keep the number, rights and layers to a minimum needed for your project.

![Assign Rights](images/generate-tokens.png)

## Generate Token

Next, click on **Generate Token** to see your token:

![List of Generated Tokens](images/token-list.png)

> #### Note
>
> You can revoke the token at any time by just deleting it on the **Manage Token** tab.

## Mandrill to Mailjet

This is a comand line tool to transfer your Mandrill data to your newly created Mailjet account.

You will need to have:
 - [Node JS installed with NPM](https://nodejs.org/en/)
 - a [Mailjet account](https://mailjet.com)
 - your [Mailjet API Keys](https://app.mailjet.com/account/api_keys)
 - and one last time, your [Mandrill API Key](https://mandrillapp.com/settings)

At the moment, the tool is migrating:
 - your sender addresses
 - your templates
 - your subaccounts

### Notes

When a newly added sender is registered to the mailjet API, it [needs to be validated](http://dev.mailjet.com/guides/#validate-sender-and-domain) in order to be used to send transactional and marketing emails

If you encounter any issue regarding this tool, please post an issue in the <issue link>
If your issue is related to the migration itself, please contact our support at `api@mailjet.com`

### Differences with Mandrill

Subaccounts are represented as API Key with Mailjet. They do not share senders, contacts, templates (templates can however be defined as `global`)

With Mailjet, your sender addresses are not global and not share through all your subaccounts.
Each subaccount can have its own senders. In order to migrate your Mandrill account, this tool create your sender list for each subaccount you have.

## Usage

```

$ git clone <repo> mandrill-to-mailjet && cd $_

$ npm install

$ npm run migration

```

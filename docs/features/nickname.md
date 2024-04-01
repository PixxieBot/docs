# Nickname Command

The `/nickname` command can be used to make PixxieBot rename a member of your server with a funny or nasty random nickname.

In order to determine who can rename who, we follow the permissions you have granted your members as per Discord's permissions system, as set out by the roles you have assigned them. Therefore, PixxieBot will respect whatever nickname management permissions you have set up in your server and cannot be used to circumvent your permissions setup.

Basically, if a server member can't open another member's Discord profile and rename them manually, they will not be able to use PixxieBot to get around that missing permission.

This means that there are some limitations as to who can rename who as outlined below as per Discord's permissions system.

Server members cannot rename other members:

- If the member running the command doesn't have the "Manage Nicknames" permissions on any of their server roles.
- If their highest role is the same or higher than the server member they're trying to rename.
- If the person they're trying to rename is the server owner (nobody can rename a server owner as per Discord's permissions system).
- They cannot rename themselves if they don't have the "Change Nickname" permissions on any of their server roles or if PixxieBot's role isn't higher than theirs.

{% hint style="info" %}
Want to allow your members to rename each other? One way is to set up a nickname role you place above the highest server member role and then make that role self-assignable, either in Discord's [Channels & Roles tab of your server](https://support.discord.com/hc/en-us/articles/10394859532823-Community-Onboarding-Examples) or using a thrid-party role assignment bot like [Yagpdb](https://yagpdb.xyz).
{% endhint %}

PixxieBot also cannot rename:

- Server members whose highest role is higher than PixxieBot's role.
- Server owners (Discord's permissions system defines the server owner as the highest roled server member).

Server owners cannot be renamed by anyone but themselves as per Discord's permissions system, therefore:

- They cannot use PixxieBot to rename themselves, but PixxieBot will post a nickname suggestion in a message instead so they can set it manually.
- Nobody can use PixxieBot to rename the server owner since Discord considers no role higher than server ownership.

{% hint style="info" %}
Not everyone likes being renamed, so to ensure PixxieBot cannot be used by your server members to tease or bully others, you can set up a role which you can place just above the highest regular member role and assign to users who don't want to be renamed. Since they will now have a higher role than regular members, as per Discord's permissions system, they cannot be renamed by anyone with a role lower than them.
{% endhint %}

# Configuring the Bot: Permissions
***

You can configure the Bot's permissions in two ways.

If you give the bot **Administrator** permissions it will just "work" and won't need much permission configuration.
If you don't want to give the Bot Administrator access to your server then you will need to do a bunch of Permission configurations.

This section will guide you through configuring the Bot's Permissions when using **Administrator** Permissions and without using **Administrator** permissions.


## Using Administrator permissions: **[Recommended]**

You will only need to setup a few Permissions for your Users to be able to open tickets when using [Thread mode](../dashboard/settings/thread-mode.md). You will need to give your Users the `Send messages in Threads` Permission in your Panel channel so that they can write in Tickets.

Now you can go ahead with the next step of the Bot Configuration:  [Bot Configuration](./configuration.md)


## Using seperate Permissions: [Complicated]


Not using Administrator permissions makes the Setup more complicated. You will need to manually give the Bot it's permissions on the `Role`, `The Panel Channel(s)`, `The Transcipts channel`, `Ticket category(s)` and `Ticket Notification Channel (when using Threads)`.

You will need to set each of these Permissions to `True` in each of the above named sections so that the bot can work:

* `View Channels`
* `Manage Channels`
* `manage roles`
* `Manage Webhooks`
* `Send Messages`
* `Send Messages in Threads`
* `Create Public Threads`
* `Create Private Threads`
* `Embed Links`
* `Attach Files`
* `Add Reactions`
* `Use External Emojis`
* `Mention @everyone`
* `Manage Threads`
* `Read Message History`
* `Use Application Commands`


When using [Thread mode](../dashboard/settings/thread-mode.md) you will also need to give your Users the `Send messages in Threads` Permission in your Panel channel so that they can write in Tickets.

You can now also run the `/checkpermissions` command that will tell you which Permissions are missing and where. If you're not the owner of the server, now would be a good time to get the owner to designate you as an admin of Tickets so that you can use this command. You can do this by asking the owner to run the command `/addadmin @YourUsername` in a channel the bot can see. If successful, Tickets will show you a ✅.
If you ran the `/checkpermissions` command and none are missing then you have succesfully completed this section of the setup.

Now we can start configuring the rest of the Bot: [Bot Configuration](./configuration.md)

> **Note:** You can find an explanation of each permission and it's uses in: [Permission Explained](../miscellaneous/permissions-explained.md)
# Draupnir
Draupnir ist ein Moderations und Abuse Protection Bot, welcher sehr verbreitet ist in der Matrix Welt. Wir nutzen eine Instance, die von [asgard.chat](https://asgard.chat) gehosted wird. 

## Protections Module
**Aktiv haben wir folgende Protections Module von Draupnir:**
* **BanPropagationProtection** - When you ban a user in any protected room with a client, this protection will turn the room level ban into a policy for a policy list of your choice. This will then allow the bot to ban the user from all of your rooms.
* **BasicFloodingProtection** - If a user posts more than 10 messages in 60s they'll be banned for spam. This does not publish the ban to any of your ban lists. This is a legacy protection from Mjolnir and contains bugs.
* **InvalidEventProtection** - Protect the room against malicious events or evasion of other protections.
* **JoinRoomsOnInviteProtection** - Automatically joins rooms when invited by members of the management room and offers to protect them
* **MemberBanSynchronisationProtection** - Synchronises `m.ban` events from watch policy lists with room level bans.
* **PolicyChangeNotification** - Provides notification of policy changes from watched lists.
* **RedactionSynchronisationProtection** - Redacts messages when a new ban policy has been issued that matches config.automaticallyRedactForReasons. Work in progress.
* **RoomsSetBehaviour** - Unprotects parted rooms and update the list of protected rooms.
* **ServerBanSynchronisationProtection** - Synchronise server bans from watched policy lists across the protected rooms set by producing ServerACL events

## Policy Lists
**Wir folgen diesen Public Policy Lists:**
* [#community-moderation-effort-bl:neko.dev](https://matrix.to/#/#community-moderation-effort-bl:neko.dev)
* [#cs-auto-open_reg:codestorm.net](https://matrix.to/#/#cs-auto-open_reg:codestorm.net)
* [#huginn-muninn-active-threats:feline.support](https://matrix.to/#/#huginn-muninn-active-threats:feline.support)
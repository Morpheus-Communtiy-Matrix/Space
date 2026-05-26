# Morpheus Link Bot
Der [Morpheus Link Bot](https://github.com/M2tecDev/morpheus-link-bot) ist ein Link Moderations Bot. Dieser hat eine Whitelist und eine Blacklist von Links.  Genauere Infos zu dem Bot gibts in dem Repo [Link-Moderation-Bot](https://github.com/Morpheus-Communtiy-Matrix/Link-Moderation-Bot)


## Funktionsweise
Wird in einer Nachricht ein Link, der auf der Blacklist ist, gesendet wird die betreffende Nachricht gelöscht und der User verwarnt. Bei mehrfachen senden eines Blacklisted Links wird der User für 5 Minuten muted und kann in allen Räumen des Spaces nicht mehr schreiben.

Wird in einer Nachricht ein Link, der auf der Whitelist ist, gesendet bleibt die betreffende Nachricht stehen und der Bot antwortet mit einer Link Preview, sofern er eine Gennerieren kann und der Link nicht auf der Ignorelist steht.

Wird in einer Nachricht ein Link, der weder auf White– noch auf Blacklist steht, gesendet wird die betreffende Nachricht vorsorglich gelöscht und der Link wird zur Überpfüfung in den Link Moderation Raum gesendet. Dort entscheiden Mods darüber, ob ein Link Freigegeben wird. Wenn ein Mod über den Link entschieden hat wird der User in dem Raum der Ursprungsnachricht über das Ergebnis benachrichtigt.

Wenn du einen Link Anfragen möchtest sende am besten eine Nachricht mit nur dem Link in [#link-bot-commands](https://matrix.to/#/!DzRpAroBgyJ2JzMptj9aNEdfCqNkzpPwzaSz_c7U0LE?via=mikaff.de&via=matrix.org&via=nope.chat).

## Commands
Die folgenden User Commands können in [#link-bot-commands](https://matrix.to/#/!DzRpAroBgyJ2JzMptj9aNEdfCqNkzpPwzaSz_c7U0LE?via=mikaff.de&via=matrix.org&via=nope.chat) genutzt werden. Mod Commands können nur von Mods in dem Link Moderation Raum genutzt werden.
### User Commands
* `!urlstatus <link>`: Abfrage, ob ein Link White– oder Blacklisted ist.
* `!pending`: Abfrage, welche Links noch nicht von den Mods bearbeitet wurden
* `!stats`: Abfrage wie viele Domains auf White– und Blacklist sind.
* `!status`: Status des Bots abfragen

### Mod Commands
* `!sendpending`: Sendet erneut die Nachricht, von Links, deren Überprüfung noch aussteht.
* `!allow <link>`: Link auf Whitelist setzen (Liste von Links mit Leerzeichen getrennt möglich)
* `!unallow <link>`: Link von Whitelist nehmen (Liste von Links mit Leerzeichen getrennt möglich)
* `!block <link>`: Link auf Blacklist (Liste von Links mit Leerzeichen getrennt möglich)
* `!unblock <link>`: Link von der Blacklist nehmen (Liste von Links mit Leerzeichen getrennt möglich)
* `!ignore <link>`: Link auf Ignlorelist setzen (Liste von Links mit Leerzeichen getrennt möglich)
* `!unignore <link>`: Link von Ignorelist nehmen (Liste von Links mit Leerzeichen getrennt möglich)
* `!reloadlists`: custom Blacklists neuladen
* `!mute <@nutzer:server> [-t Minuten]`: User stummschalten
* `!unmute <@nutzer:server>`: User entstummschalten

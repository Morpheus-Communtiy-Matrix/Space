# Youtube Bot
Der Peertube Bot (@peertube.rss:mikaff.de) sendet eine Nachricht in [#Morpheus Content](), wenn eine neues Video eines Kanals von [TheMorpheus](https://the-morpheus.de) auf [Morpheus Peertube Instanz](https://tube.the-morpheus.de) erscheint.  
Dazu verwenden wir den [Maubot-RSS](https://github.com/maubot/rss), welcher die RSS Feeds der Peertube Kanäle von [TheMorpheus](https://the-morpheus.de) parsed.  

**Nachrichten Template**: `Neues Video von <Kanal Name>: [$title]($link)`

**Folgende RSS Feeds parsed der Bot:**
* [The Morpheus](https://tube.the-morpheus.de/feeds/videos.xml?videoChannelId=3) `ID: 1`
* [The Morpheus Tutorials](https://tube.the-morpheus.de/feeds/videos.xml?videoChannelId=4) `ID: 2`
# Youtube Bot
Der Youtube Bot (@youtube.rss:mikaff.de) sendet eine Nachricht in [#Morpheus Content](), wenn eine neues Video eines Kanals von [TheMorpheus](https://the-morpheus.de) erscheint.  
Dazu verwenden wir den [Maubot-RSS](https://github.com/maubot/rss), welcher die RSS Feeds der Youtube Kanäle von [TheMorpheus](https://the-morpheus.de) parsed.  
Einzelne RSS-Feeds werden nicht geparsed, da Youtube die Feeds erst erstellt, wenn Content im Jeweiligen Format auf dem Kanal erschienen ist.

Das Template der Nachrichten wird für jedes Format angepasst.
* **Videos**: `Neues Video von <Kanal Name>: [$title]($link)`
* **Shorts**: `Neues Short von <Kanal Name>: [$title]($link)`
* **Livestreams**: `<Kanal Name> ist jetzt Live: [$title]($link)`

**Folgende RSS Feeds parsed der Bot:**
* [The Morpheus](https://www.youtube.com/feeds/videos.xml?channel_id=UCkZ3fSYruC0IXv6p34BHciQ)
  * [Videos](https://www.youtube.com/feeds/videos.xml?playlist_id=UULFkZ3fSYruC0IXv6p34BHciQ) `ID: 6`
  * [Shorts](https://www.youtube.com/feeds/videos.xml?playlist_id=UUSHkZ3fSYruC0IXv6p34BHciQ) `ID: 7`
  * [Livestreams](https://www.youtube.com/feeds/videos.xml?playlist_id=UULVkZ3fSYruC0IXv6p34BHciQ) `ID: 8`
* [The Morpheus Tutorials](https://www.youtube.com/feeds/videos.xml?channel_id=UCLGY6_j7kZfA1dmmjR1J_7w)
  * [Videos](https://www.youtube.com/feeds/videos.xml?playlist_id=UULFLGY6_j7kZfA1dmmjR1J_7w) `ID: 9`
  * [Shorts](https://www.youtube.com/feeds/videos.xml?playlist_id=UUSHLGY6_j7kZfA1dmmjR1J_7w) `ID: 10`
  * [Livestreams](https://www.youtube.com/feeds/videos.xml?playlist_id=UULVLGY6_j7kZfA1dmmjR1J_7w) `ID: 11`
* [The Morpheus Talks](https://www.youtube.com/feeds/videos.xml?channel_id=UCRnhQIE4fc5mEn6SVqYfsCQ)
  * [Videos](https://www.youtube.com/feeds/videos.xml?playlist_id=UULFRnhQIE4fc5mEn6SVqYfsCQ) `ID: 12`
  * [Shorts](https://www.youtube.com/feeds/videos.xml?playlist_id=UUSHRnhQIE4fc5mEn6SVqYfsCQ) `ID: none (Not created cause no shorts on this chanel)`
  * [Livestreams](https://www.youtube.com/feeds/videos.xml?playlist_id=UULVRnhQIE4fc5mEn6SVqYfsCQ) `ID: 13`
* [The Morpheus Reacts](https://www.youtube.com/feeds/videos.xml?channel_id=UC229fht5PxqEFSZb-Z8MzIw)
  * [Videos](https://www.youtube.com/feeds/videos.xml?playlist_id=UULF229fht5PxqEFSZb-Z8MzIw) `ID: 14`
  * [Shorts](https://www.youtube.com/feeds/videos.xml?playlist_id=UUSH229fht5PxqEFSZb-Z8MzIw) `ID: none (Not created cause no shorts on this chanel)`
  * [Livestreams](https://www.youtube.com/feeds/videos.xml?playlist_id=UULV229fht5PxqEFSZb-Z8MzIw) `ID: none (Not created cause no live streams on this chanel)`
* [MetaMorpheus](https://www.youtube.com/feeds/videos.xml?channel_id=UC9kUHlWDqm8D7WdXN7syFSA)
  * [Videos](https://www.youtube.com/feeds/videos.xml?playlist_id=UULF9kUHlWDqm8D7WdXN7syFSA) `ID: 15`
  * [Shorts](https://www.youtube.com/feeds/videos.xml?playlist_id=UUSH9kUHlWDqm8D7WdXN7syFSA) `ID: 16`
  * [Livestreams](https://www.youtube.com/feeds/videos.xml?playlist_id=UULV9kUHlWDqm8D7WdXN7syFSA) `ID: none (Not created cause no live streams on this chanel)`
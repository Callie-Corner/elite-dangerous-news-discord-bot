## From the API at: `https://cms.elitedangerous.com/api/news`

A single article will appear in such a format:
```json
{
    "title": "Odyssey Alpha Update 1.0",
    "body": "<p>Greetings Commanders,</p> <p>We're excited for you to take your first steps in Elite Dangerous: Odyssey. Read below to ensure the best possible experience during the Alpha.</p> <p>To gain access to the Alpha you must pre-order the <a href="https://store.steampowered.com/app/1336350/Elite_Dangerous_Odyssey/">Deluxe Alpha version</a> of Odyssey.</p> <p><strong>Alpha Phase 1 Focus: Core Systems and Networking</strong></p> <p><strong>Start Time: 13:00 UTC/14:00 BST</strong></p> <p><strong>Features:</strong></p> <ul><li>New commander creation; starting from scratch</li> <li>On-foot in 1 system: Adityan (Rest of galaxy is permit locked)</li> <li>Travel via Apex Interstellar – new to Elite Dangerous</li> <li>Variety of local missions available from NPC's and mission boards</li> </ul><p>New content will be rolled out in further <a href="https://forums.frontier.co.uk/threads/alpha-rollout-plan.568118/">Alpha phases</a>.</p> <p><strong>Specifications*</strong></p> <p><strong>Recommended Specs (High Settings at 1080p)</strong></p> <ul><li>Intel Core i5-8600K / AMD Ryzen 5 1600 (above 4 GHz recommended)</li> <li>12GB RAM</li> <li>NVIDIA GeForce GTX 1060 6GB / AMD Radeon RX 5500</li> <li>60GB available space</li> </ul><p><strong>Minimum Specs (Low Settings at 720p)</strong></p> <ul><li>Intel Core i5-4590 / AMD FX-4350</li> <li>8GB RAM</li> <li>NVIDIA GeForce GTX 770 / AMD Radeon R9 280X</li> <li>60GB available space</li> <li>Please note, the VR implementations are not currently optimised and not ready for testing at this time.</li> </ul><p><em>*These specifications are subject to change as we move toward release.</em></p> <p><strong>IMPORTANT: Advice for the Alpha</strong></p> <ul><li>Phase 1 does not feature a tutorial, please reference the control page for help.</li> <li>Planetary Tech, including geometry, will not be final until release. However, players may see colouration changes throughout the Alpha phases.</li> <li>All players will start with only a flight suit and pistol. It is not recommended that you start combat missions until you have at least purchased the Maverick suit as AI will be very challenging.</li> </ul><p>If you encounter any issues during your Alpha experience please report them as soon as possible via the Odyssey section on the <a href="https://issues.frontierstore.net/"><strong>Issue Tracker</strong></a> where our development team will be actively investigating reports.</p> <p>Good luck and o7 Commanders!</p>",
    "image": "/sites/default/files/2021-03/odyssey_keyart_final_1920x1080.jpg",
    "nid": 2656,
    "slug": "odyssey-alpha-update-10",
    "forumLink": "https://forums.frontier.co.uk/forums/elite-dangerous-odyssey-alpha.416/",
    "date": "2021-03-29T13:54:23+0100"
}
```

To access the direct website link to the article, just replace `[slug]` with the slug from the article, like so:
```
https://www.elitedangerous.com/news/article/[slug]
```
To access one of the comma delimited images, you can use this link, replacing `[image]`, for one of the image values:
```
https://cms.elitedangerous.com[image]
```
In a bunch of older articles, they sometimes start with the comma delimiter, meaning the images have since then been deleted.

## From the node gathered by the API

To remedy the issue of same title/slug posts, we can use the node id to get the json information, by replaceing `[nid]` with the post node id in the following url:
```
https://cms.elitedangerous.com/node/[nid]?_format=json
```

And the data format of those show up as follows:
```json
{
    "nid": [ { "value": 2656 } ],
    "uuid": [ { "value": "0f62e4b1-e46a-416c-bf4d-57d20e3a7840" } ],
    "vid": [ { "value": 3590 } ],
    "langcode": [ { "value": "en" } ],
    "type": [ { "target_id": "news_article",
                "target_type": "node_type",
                "target_uuid": "2c11893a-3fb8-4b48-8358-b94db68f3407"
            } ],
    "revision_timestamp": [ { "value": "2021-03-29T12:56:52+00:00",
                              "format": "Y-m-d\TH:i:sP"
                          } ],
    "revision_uid": [ { "target_id": 1,
                        "target_type": "user",
                        "target_uuid": "2d5b9c4b-35f1-4cb1-b4b1-740c83b51a2a",
                        "url": "user/1"
                    } ],
    "revision_log": [ ],
    "status": [ { "value": true } ],
    "uid": [ { "target_id": 1,
               "target_type": "user",
               "target_uuid": "2d5b9c4b-35f1-4cb1-b4b1-740c83b51a2a",
               "url": "/user/1"
           } ],
    "title": [ { "value": "Odyssey Alpha Update 1.0" } ],
    "created": [ { "value": "2021-03-29T12:54:23+00:00",
                   "format": "Y-m-d\TH:i:sP"
               } ],
    "changed": [ { "value": "2021-03-29T13:00:03+00:00",
                   "format": "Y-m-d\TH:i:sP"
               } ],
    "promote": [ { "value": true } ],
    "sticky": [ { "value": false } ],
    "default_langcode": [ { "value": true } ],
    "revision_translation_affected": [ { "value": true } ],
    "path": [ { "alias": "/odyssey-alpha-update-10",
              "pid": 44,
              "langcode": "en"
            } ],
    "field_forum_link": [ { "value": "https://forums.frontier.co.uk/forums/elite-dangerous-odyssey-alpha.416/" } ],
    "field_image": [ { "target_id": 781,
                       "alt": "Elite Dangerous: Odyssey",
                       "title": "Elite Dangerous: Odyssey",
                       "width": 1920,
                       "height": 1080,
                       "target_type": "file",
                       "target_uuid": "3c42f864-272f-4b50-9d24-42e169773e45",
                       "url": "http://cms.elitedangerous.com/sites/default/files/2021-03/odyssey_keyart_final_1920x1080.jpg"
                   } ],
    "field_slug": [ { "value": "odyssey-alpha-update-10" } ],
    "body": [ { "value": "<p>Greetings Commanders,</p> <p>We're excited for you to take your first steps in Elite Dangerous: Odyssey. Read below to ensure the best possible experience during the Alpha.</p> <p>To gain access to the Alpha you must pre-order the <a href="https://store.steampowered.com/app/1336350/Elite_Dangerous_Odyssey/">Deluxe Alpha version</a> of Odyssey.</p> <p><strong>Alpha Phase 1 Focus: Core Systems and Networking</strong></p> <p><strong>Start Time: 13:00 UTC/14:00 BST</strong></p> <p><strong>Features:</strong></p> <ul> <li>New commander creation; starting from scratch</li> <li>On-foot in 1 system: Adityan (Rest of galaxy is permit locked)</li> <li>Travel via Apex Interstellar – new to Elite Dangerous</li> <li>Variety of local missions available from NPC's and mission boards</li> </ul> <p>New content will be rolled out in further <a href="https://forums.frontier.co.uk/threads/alpha-rollout-plan.568118/">Alpha phases</a>.</p> <p><strong>Specifications*</strong></p> <p><strong>Recommended Specs (High Settings at 1080p)</strong></p> <ul> <li>Intel Core i5-8600K / AMD Ryzen 5 1600 (above 4 GHz recommended)</li> <li>12GB RAM</li> <li>NVIDIA GeForce GTX 1060 6GB / AMD Radeon RX 5500</li> <li>60GB available space</li> </ul> <p><strong>Minimum Specs (Low Settings at 720p)</strong></p> <ul> <li>Intel Core i5-4590 / AMD FX-4350</li> <li>8GB RAM</li> <li>NVIDIA GeForce GTX 770 / AMD Radeon R9 280X</li> <li>60GB available space</li> <li>Please note, the VR implementations are not currently optimised and not ready for testing at this time.</li> </ul> <p><em>*These specifications are subject to change as we move toward release.</em></p> <p><strong>IMPORTANT: Advice for the Alpha</strong></p> <ul> <li>Phase 1 does not feature a tutorial, please reference the control page for help.</li> <li>Planetary Tech, including geometry, will not be final until release. However, players may see colouration changes throughout the Alpha phases.</li> <li>All players will start with only a flight suit and pistol. It is not recommended that you start combat missions until you have at least purchased the Maverick suit as AI will be very challenging.</li> </ul> <p>If you encounter any issues during your Alpha experience please report them as soon as possible via the Odyssey section on the <a href="https://issues.frontierstore.net/"><strong>Issue Tracker</strong></a> where our development team will be actively investigating reports.</p> <p>Good luck and o7 Commanders!</p> ",
                "format": "basic_html",
                "processed": "<p>Greetings Commanders,</p> <p>We're excited for you to take your first steps in Elite Dangerous: Odyssey. Read below to ensure the best possible experience during the Alpha.</p> <p>To gain access to the Alpha you must pre-order the <a href="https://store.steampowered.com/app/1336350/Elite_Dangerous_Odyssey/">Deluxe Alpha version</a> of Odyssey.</p> <p><strong>Alpha Phase 1 Focus: Core Systems and Networking</strong></p> <p><strong>Start Time: 13:00 UTC/14:00 BST</strong></p> <p><strong>Features:</strong></p> <ul><li>New commander creation; starting from scratch</li> <li>On-foot in 1 system: Adityan (Rest of galaxy is permit locked)</li> <li>Travel via Apex Interstellar – new to Elite Dangerous</li> <li>Variety of local missions available from NPC's and mission boards</li> </ul><p>New content will be rolled out in further <a href="https://forums.frontier.co.uk/threads/alpha-rollout-plan.568118/">Alpha phases</a>.</p> <p><strong>Specifications*</strong></p> <p><strong>Recommended Specs (High Settings at 1080p)</strong></p> <ul><li>Intel Core i5-8600K / AMD Ryzen 5 1600 (above 4 GHz recommended)</li> <li>12GB RAM</li> <li>NVIDIA GeForce GTX 1060 6GB / AMD Radeon RX 5500</li> <li>60GB available space</li> </ul><p><strong>Minimum Specs (Low Settings at 720p)</strong></p> <ul><li>Intel Core i5-4590 / AMD FX-4350</li> <li>8GB RAM</li> <li>NVIDIA GeForce GTX 770 / AMD Radeon R9 280X</li> <li>60GB available space</li> <li>Please note, the VR implementations are not currently optimised and not ready for testing at this time.</li> </ul><p><em>*These specifications are subject to change as we move toward release.</em></p> <p><strong>IMPORTANT: Advice for the Alpha</strong></p> <ul><li>Phase 1 does not feature a tutorial, please reference the control page for help.</li> <li>Planetary Tech, including geometry, will not be final until release. However, players may see colouration changes throughout the Alpha phases.</li> <li>All players will start with only a flight suit and pistol. It is not recommended that you start combat missions until you have at least purchased the Maverick suit as AI will be very challenging.</li> </ul><p>If you encounter any issues during your Alpha experience please report them as soon as possible via the Odyssey section on the <a href="https://issues.frontierstore.net/"><strong>Issue Tracker</strong></a> where our development team will be actively investigating reports.</p> <p>Good luck and o7 Commanders!</p>",
                "summary": ""
            } ]
}
```

Most of this data is useless to us, but there are parities that you can obviously deduce. Using the `field_forum_link`, however, we can craft a link to where the forum article will be or already is at.

# NFT TON Events
NFT TON Events is a collection of unique events on The Open Network. Each NFT is a gift from the organizer for the participant, which confirms the information about attending the event. Each time you participate in an event, TON Events send a unique NFT, which is verified by a cryptographic record. These NFT are Non-Fungible Tokens and contain all information about the event.

## Usage
```
title                    // Title to display
image                    // 
description              // 
native_name              // 
native_name_lang         // 
english_name             // 
time                     // 
timezone                 // 
duration                 // duration|h=x|m=x|s=x or time interval|date1|date2|options
date                     // start date|YYY/|MM/DD or start and end dates|YYYY/MM/DD-YYYY/MM/DD
venue                    // 
location                 // 
coordinates              // coord|LAT|LON|region:XXXX_type:event|display=inline,title
type                     // 
theme                    // 
cause                    // 
motive                   // 
target                   // 
patron                   // or patrons
organisers               // or organizers
participants             // 
outcome                  // 
awards                   // 
url                      // 
blank_label              // or |blank_data
blank1_label             // or |blank1_data
blank2_label             // or |blank2_data
website                  // URL|example.com
notes                    // 
```
## Parameters
Template parameters

|Parameter| |Description |Type |Status |
|-|-|-|-|-|
|Title |`title` `event` `name` `Event_Name` |Name of the event, if omitted, the page name will be used |Line |optional |
|Image |`image` `image_name` `Image_Name` |Name of the image of the event |File |suggested |
|Image size |`image_size` `Imagesize` |Image size in pixels |Unknown |deprecated |
|Part of |`partof` |no description |Unknown |optional |
|Logo |`logo` |Logo filename |File |optional |
|Logo size |`logo_size` |no description |Unknown |optional |
|Description |`description` |Description to event. |Line |optional |
|date |`date` |start date YYYY/MM/DD for the date of a single-day event or start and end dates YYYY/MM/DD-YYYY/MM/DD for multi-day events |Unknown |optional |
|time |`time` |no description |Unknown |optional |
|timezone |`timezone` |no description |Unknown |optional |
|duration |`duration` |no description |Unknown |optional |
|Venue |`venue` |name of the particular venue (alternative to location) |Unknown |optional |
|place |`place` |no description |Unknown |optional |
|Location |`Location` `location` |The location of the event |Line |optional |
|Coordinates |`coordinates` |Use, with display=inline,title (ex: \|LAT\|LON\|region:XXXX_type:event\|display=inline,title) |Unknown |optional |
|type |`type` |no description |Unknown |optional |
|theme |`theme` |no description |Unknown |optional |
|cause |`cause` |no description |Unknown |optional |
|motive |`motive` |no description |Unknown |optional |
|target |`target` |no description |Unknown |optional |
|Patrons |`patron` `patrons` | | |optional |
|Organizers |`organizers` `organisers` |no description |Unknown |optional |
|Participants |`participants` |The typical number of participants |Line |optional |
|Outcome |`outcome` `result` |no description |Line |optional |
|awards |`awards` |no description |Unknown |optional |
|url |`url` |no description |Unknown |optional |
|blank_label |`blank_label` |no description |Unknown |optional |
|blank_data |`blank_data` |no description |Unknown |optional |
|blank1_label |`blank_label` |no description |Unknown |optional |
|blank1_data |`blank_data` |no description |Unknown |optional |
|blank2_label |`blank_label` |no description |Unknown |optional |
|blank2_data |`blank_data` |no description |Unknown |optional |
|Website |`website` `URL` |Use URL (ex: URL\|example.com) |Unknown |optional |
|Notes |`notes` |Free-form notes for NFT |Unknown |optional |

## Example
[TON NFT EXPLORER](https://explorer.tonnft.tools/collection/EQC3xU7M2blJMsJLgE5WRKeomCXwtlSXU_wHIL7q57MkcLy5)
```json
{
    "name": "TON NFT Moscow Club",
    "description": "NFT TON Events is a collection of unique events on The Open Network. Each NFT is a gift from the organizer for the participant, which confirms the information about attending the event. Each time you participate in an event, TON Events send a unique NFT, which is verified by a cryptographic record. These NFT are Non-Fungible Tokens and contain all information about the event.",
    "image": "ipfs://CID/logo.png",
    "attributes": [
        {
            "trait_type": "date",
            "value": "2022/05/29"
        },
        {
            "trait_type": "time",
            "value": "12:00"
        },
        {
            "trait_type": "timezone",
            "value": "GMT+3"
        },
        {
            "trait_type": "place",
            "value": "Boiling Point"
        },
        {
            "trait_type": "coordinates",
            "value": "55.758330032651834, 37.579751297813836"
        },
        {
            "trait_type": "type",
            "value": "talk"
        },
        {
            "trait_type": "website",
            "value": "https://leader-id.ru/events/301817"
        }
    ]
}
```
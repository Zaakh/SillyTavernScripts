# Adventure Tools

Author: Monster Boy

Requirements: LaLib

## HOW CAN USE????
- After importing the file, click Config and then Version Select to set if you'd like to use the modern version or fantasy version
- Click Generation Mode to set if you'd like to use CoT or not
- Fill in your message in the normal text box and either click the script's  Send ⮕ or  Send+ ⮕ to send a message
- (Optional) If you plan to add lorebook entries, make sure you have a lorebook already created and active, then click Config and Lorebook Select to set the lorebook for creating new entries
- (Optional) Set any other options you'd like in the config menu, then go into Settings Manager to save your settings for later

Tip: If you set options for API, model, samplers etc. for one thing, make sure to have them set for others as well. For example, if you set an adventuring API and will be using another one for CoT, make sure to set what API you'd like for creating chars, otherwise it'll be using whatever was last switched to

# Release note

Adventure Tools is a set of tools aimed at enhancing adventure quality of life, without being overly complicated (Morgan Freeman's Voice: it got complicated). The main features are a CoT (Chain of Thought) prompt, a tracker system, buttons to add NPC info, and a button to add other info. You can switch between having a fantasy script or a modern script with the Config button.

LaLib is required for this to work properly. The CoT prompt, char gen, and tracker takes up a LOT of tokens, but so does adventuring in general. Be prepared for this.

This is not for group chat; this is designed to be used with a narrator/Dungeon Master card.
---
Features
- (Optional) Chain of Thought Adventuring via the Send+ button, where the bot will consider relevant information such as where characters in the scene are, stats, personalities/traits, inventories, supplies, and any laws of physics/rules you've set up for the setting, then feeds that info into the final response. This creates a more grounded and accurate adventuring experience
- Tracker System which currently tracks the time, location, weather (lol), along with everyone's clothes and current position around you. This keeps the AI on 'track', helping it stay consistent with the scene
- Add Custom NPC button for adding NPCs that have a pre-established relationship to the user's char, or for a more tailored NPC-maker experience in general
- Add NPC button for adding randomly encountered NPCs
- Add Other... button to add all other info, originally created by Svor from the KCPP server. It's been mostly remade. You can use it to add info about locations, organisations, char wardrobes, vehicles, apps, or whatever else you can think of.
- Look At... is a button for looking at something without the adventure moving forward
- Quick Delete as a quick button to delete the last message. There's no undo or confirmation for this, so be careful with it
- Undo button which deletes the last two messages and reverts to the last tracker info in a list; a total of five of the most recent trackers are saved
- OOC Message button to speak to the bot in an OOC format, so you don't have to type it out, along with instructions for the bot to stop the RP and not to continue it, and only explain itself etc. (something super tedious to type out every time). The bot is prompted to reply in the same OOC format

Addtl. Credits: Svor, kaldigo, Dave, Galahad, Aurora Flames, Kibbi

## Changes

### September 25th, 2024
Bug fixes for API/model cmd order across the board
Fixed a bug where the adventuring context was not being switched properly
Added adventuring preset conditionals at the end of the Send buttons on Galahad's suggestion

### September 19th, 2024
Fixed bug where changing a model under a diff API would give an error, credit: Galahad
Added changing tokenizer as an option, credit: Galahad

### September 16th, 2024
Cleaned leftover vars from Send/Regen
Fixed a bug where the correct Send button was not showing after loading settings

### September 15th, 2024
Removed saving/editing prompts due to issues with how vars store information. If you'd like to edit the prompts, you can edit the defaultPrompts button instead
Undo full functionality has been completed

### September 8th, 2024
Removed archaic Update Tracker button and enforcement of 2nd-person perspective
Added Settings Manager sub-menu in Config. You can now save/load settings by name, reset local settings to default, delete a setting by name, and delete all saved settings. (You will need to delete all settings and reset to default for a full 'factory reset')
Added presets for CoT/tracker
Gen length for CoT and tracker increased to 1.5K CTX
Fixed bugs from not setting templates/API/model

### September 2nd, 2024
Added options to set APIs, models, context/instruct templates
Gen length for CoT, NPC-making, and Tracker is set to a fixed value of 1K tokens
You can now save settings as a name and load them
 
## Metagaming Rules

```
[System Info: Metagaming Rules
1. **Limited Knowledge:** People should not possess information about {{user}} or others beyond what is visually observable or explicitly stated by them within the narrative. This includes info such as name, secrets, and other personal information.
2. **Visual Observations:** People may comment on others' visible physical attributes, behaviours, or actions within the scene, but they should not make assumptions about anyone's identity or backstory based on these observations.
3. **Information Exchange:** Any knowledge or information exchanged between people and {{user}} should be a direct result of in-world interactions or conversations.
4. **Investigation and Conversation:** {{user}} may choose to reveal information about themselves through investigation or natural conversation within the RP. This also applies to other people and characters.
5. **Maintaining Consistency:** Ensure that people's interactions and reactions towards {{user}} are based solely on visual cues, explicit statements made by {{user}}, and information exchanged through in-world conversations or investigations.
6. **Private Thoughts:** People cannot read minds. If {{user}} or any other person thinks something to themselves, others have no way of knowing what said person is thinking. This also includes thoughts in actions wrapped in asterisks, such as if someone *wonders about something* or *thinks about* something.
7. **Exceptions:** People with a pre-established relationship, such as family members, friends, or colleagues, may have deeper knowledge of each other. For example, a family member will be aware of many parts of another's backstory if they grew up together. Use your best judgement.]
```

Put it in a lorebook entry, it's depth 2.
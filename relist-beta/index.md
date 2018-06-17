---
title: relist-beta
layout: page
date: 2018-01-22 18:00:00
---

# ReList Beta Information
This page is still a work in progress.

## Quick Links
[General](#General)
[What is ReList?](#What-is-ReList)
[Known Bugs](#Known-Bugs)
[ToDo List](#ToDo-List)
[Possible Features for later](#Possible-Features-for-later)
[Update Notes](#Update-Notes)

## General

Thank you for participating in the ReList beta! First of all, please note that both the name and the app icon are not finalized and might change completely until release. 

There is a discussion group about the beta on Telegram. If you'd like to be invited, send me a [message](https://t.me/StefanDesu). If you just want to send me feedback directly, you can just use our usual means of communication.

If you are not yet on the beta, send me a message with your email address asking for a TestFlight invite. You will need to download the [TestFlight app]() from the App Store and use the code/link provided in the invitation email.

## What is ReList?

ReList is an app focused on reusable checklist. Think of your morning routine (if you have one) or your packing list for trips. Lists that you create once, but go through multiple times. The app lets you create templates that can be reused and turned into checklists.

## Known Bugs
- On iPad, the selection on the left column will be lost in certain cases.
- Theme does not work in acknowledgements
- Repeating menu opens very slowly
- In some cases, the app does not create a repeating checklist, then crashes when going into the repeating settings of that list, but creates the checklist after relaunch (it happened to me two or three times already, if someone finds a way to reproduce it, I'd be really grateful!)
- The app might crash when going into background or while in background (still has to be investigated, might have been fixed together with a different crash)
- Probably a lot more that you will find...
- ~~Very rarely, the app might crash on start up (related to sync)~~
- ~~Item list edit mode: Weird behavior of Done button~~
- ~~Sometimes (most of the time?) creating a new list will not open that list automatically (still looking into it)~~
- ~~On iPad, when the item list is cleared (e.g. when the list was deleted or archived), the undo button won't get removed~~
- ~~Custom name patterns do not work when creating a list with an empty name~~
- ~~When changing theme, segmented control in settings won't change color until settings are reopened~~
- ~~In settings, the leading margin is inconsistent (it was not an iOS bug...)~~

## ToDo List
(Roughly in order of priority. Features might not be in the current TestFlight build even if checked off here.)
- (Improvement) Create a template from a checklist
- (Feature) Badge on app icon for number of open lists/items
- (Improvement) Make the main screen look nicer
- (Improvement) Show items for archived lists
- (Feature) Customizable icon and color per list
- (Feature) Keyboard support for iPad
- (Feature) Reminders for lists (not yet decided how this should look like)
- (Feature) Automatic backups
- (Improvement) Rewrite sync to use iCloud instead of Realm Object Server
- (Feature) 3D touch for lists
- (Feature) Notes for lists
- (Improvement) Jump to first unchecked item
- ...
- ~~(Feature) Theme option in settings~~
- ~~(Improvement) Make it easier to create a list based on a certain template~~
- ~~(Improvement) In general make the whole workflow much easier~~
- ~~(Improvement) Allow creation of templates based on an existing template~~
- ~~(Improvement) Improve item list screens -> tap on item in checklist should check off the item~~
- ~~(Feature) Create an archive of lists that are completed~~
- ~~(Feature) Repeating lists -> e.g. create a list based on the Morning Routine template every morning~~
- ~~(Improvement) Confirm deletion of list~~
- ~~(Improvement) Settings in regards to auto archiving~~
- ~~(Improvement) Dropdown menu in item list for the top right corner~~
- ~~(Improvement) Global setting for auto archiving behavior~~
- ~~(Feature) Haptic feedback when checking off an item~~
- ~~(Feature) Allow undo of deletion of items~~

## Possible Features for later

- Sections within lists (for better organization)
- Share lists with others
- Allow sub-lists (an item containing several items, or another list as an item)
- Allow checklists to stay connected to their templates, i.e. make sure they always have the same items (might be hard to do well)
- Support for Workflow
- Web API

# Update Notes

## Update Notes Build 1167 (7 February 2018)

- Fixed a crash when updating from an older build to the newest build.

## Update Notes Build 1163 (7 February 2018)

- Added a global setting for the default auto archiving behavior for new lists
- Fixed a bug where the app would crash when navigating away from an item list while editing an item with empty name
- This build disables sync and removes the option from the settings. While sync worked generally, there were issues especially when using auto repeating lists. I will definitely work more on sync in the future as I want to use the app on multiple devices as well, but for now this feature is removed.
- The crowded buttons in the top right corner of the item list were replaced with only the list settings and a dropdown menu. There are a few dummy options there to show that it will not only contain two options, but those other ones are not yet implemented.
- Fixed: Checking off items will now give a nice subtle feedback using haptic feedback (iPhone 7 and above) or the taptic engine (iPhone 6s). Please report back if this is working for you if you have a supported phone, we only tested it on one iPhone 8 Plus so far. Note that the feedback will not occur when the phone is muted.

## Update Notes Build 1122 (1 February 2018)
This update is much bigger than the last one, fortunately. Still, my todo list just won't become any shorter.

- Hopefully fixed behavior for repeating lists (it's complicated)
- Changed screen transitions and navigation buttons (especially important for iPad)
- Improved item list interface. Note that those three buttons in the top right are temporary and will be replaced with a small dropdown menu.
- Squashed lots of small bugs (mostly interface related)
- Allow undo of deletion of items (arrow in the top right of a list)
- When manually creating a checklist for a template, it now uses the custom name defined for repeating checklists
- In the list settings (gear in the top right on the item list screen) the behavior for automatically archiving a completed list can now be changed. This setting is copied when a checklist is created for a template. Also, when restoring a completed checklist, this setting is set to None so that the restored list won't immediately be auto-archived again.

Note that if you have sync enabled, the auto archive behavior for all existing lists will be None. I have no way of changing that, unfortunately, so you will have to adjust it manually.

## Update Notes Build 1007 (29 January 2018)
Sorry for the lack of updates. The first feature below took a lot of time to implement. Also, for some reason I haven't had much energy these last few days, so I had a hard time even starting to do something. I hope it'll get better soon. Anyway, here are the changes:

- Added support for repeating checklists! As this was pretty complicated to do, there might be still a lot of bugs in there. It's also hard to test properly, so I hope that when a bug appears, we'll be able to reproduce it. Note that for some reason, there is a big delay when going into the repeating settings. I'm still looking into this.
- Completed lists will now be automatically archived. Current issues: Does not work properly on iPad, and there's no way to turn it off, even when restored through Archive. Later I will implement a setting where this behavior can be overridden either globally or for each list.
- Archive: Swiping left now shows a delete action, swiping right shows the restore action.

I have also updated the todo list and bug list above, although right now I kind of lost track of all the small issues that need to be dealt with...

## Update Notes Build 901 (25 January 2018)

- Fixed visual bugs
- Fixed lots of small bugs
- Hopefully didn't introduce too many new bugs
- Improved naming of new lists when user doesn't input a name
- Fixed bug in template selection (archived templates were shown)
- Improved item list behavior (rewrote the whole thing actually)
- ~~Hopefully a little surprise for some of you 😏 (let me know if it works and if you like it!)~~ Doesn't seem to work...


## Update Notes Build 791 (24 January 2018)

- Deletion of lists now asks for confirmation
- Improved flow when activating sync (still far from perfect though)
- Switched Edit and Settings button on main screen
- Lots and lots and lots of refactoring...
- You can now edit list names when in editing mode on main screen
- Duplication of a list by swiping right
- Easily create a list for a template by swiping right
- By default, Template is chosen as a type for a new list
- Fixed bug where the app would crash if number of checklists and number of templates would change at the same time (this one was complicated)
- Archiving lists by swiping left
- Added Archive to be able to see and restore archived lists
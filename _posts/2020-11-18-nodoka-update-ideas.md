---
layout: post
title: Ideas for a Nodoka Update
date: 2020-11-18 15:30:00
author: Stefan
---

If you didn't know, I have an app on the iOS App Store called "Nodoka Meditation Timer" ([App Store](https://itunes.apple.com/de/app/nodoka-meditation-timer/id1320621736?l=en&mt=8), [more info](/nodoka/)). I made it at the end of 2017 because I wanted to learn how to make iPhone apps. However, as you might see in the update log, I haven't updated the app in a long time. With the start of my job, making apps fell completely under the rug and I haven't really touched it since.

But I'm not going to give up! I still use my own app, and I have some ideas on how to make it better. Mostly, these are just ideas that I want to have in the app myself. Since I haven't touched the app in over two years, and there is a new technology called SwiftUI for making user interfaces with Swift, I'm planning on rebuilding my app using SwiftUI.

The first part will be to recreate my existing app mostly like it is now, but with SwiftUI and a cleaner code structure. The next step would be to start implementing new features. Here are some ideas I have had that I would like to have in Nodoka:

- iCloud sync of the history
- Statistics and charts
- Longer meditation times (the max is current 45 minutes)
- Random interval sound[^1]
- Custom sounds for start, end, and interval sound
- Adding audio files for custom guided meditations[^2]
- Meditation in the background (currently, the app has to be in the foreground and running for it to work)
- Better integration with iOS features (Shortcuts support, Siri support, Widgets, etc.)
- Apple Watch app
- Mac app[^3]
- Reminder notifications
- App icon selection

That is A LOT. I think that having all of this in the app, it could be the best meditation timer on the App Store. I also want to implement these features without cluttering the user interface. I haven't really thought about how to implement some of the more complex features when it comes to the UI, but it should be possible that the main interface (basically the start screen where you start your meditation) stays as simple as it is now.

What do you think? If you have an iPhone, feel free to try out [the app](https://itunes.apple.com/de/app/nodoka-meditation-timer/id1320621736?l=en&mt=8) and let me know what you would improve!

---
[^1]: The idea is that sometimes you just get lost in thoughts for very long periods of time, and having a subtle sound at random intervals could help remind you that you are currently meditating.
[^2]: I could imagine getting some guided meditations from YouTube and loading them into the app. Of course, I wouldn't build a YouTube downloader into the app, but getting an audio file from a YouTube video is easy.
[^3]: Not sure if a Mac app makes sense, but it should be fairly trivial if the app is made with SwiftUI.

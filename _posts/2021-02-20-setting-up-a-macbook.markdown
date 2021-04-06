---
layout: single
title:  "Setting Up a New Mac"
date:   2021-04-06 15:15:00 -0800
# classes: wide
toc: true
categories: tutorial
---

I generally only pay for apps that I think truly deserve my money, so for the most part everything here is free and open source. I have all of these linked on my [macos-workflow](https://github.com/raviriley/macos-workflow) GitHub repo but some people have asked me for a more thorough explanation. This post is a work in progress, more info coming soon. 

## [Alfred](https://www.alfredapp.com/)
Used to do everything from the keyboard. The free version is powerful but the paid version is life-changing. On average I use Alfred 30 times a day, so the $35 "Powerpack" has paid for itself in time saved. Saving a few seconds per task here and there may seem trivial but if you're working from the computer all day like I am those extra seconds really add up in a meaningful way. (This goes hand in hand with having a fast typing speed so you can execute commands faster - mine is about 100 WPM.)

### Features I use a lot:

File search - much faster and more powerful than Spotlight

Navigation - lets you fly around your computer from the keyboard and launch applications and scripts with ease

Snippet expansion - useful for shortening what you have to type for frequently used snippets or simplifying hard to type sequences. For example, I have `!sid` mapped to my 10-digit student ID and `:lenny` mapped to ( ͡° ͜ʖ ͡°). 

<!-- insert image here of typing on a form vs using snippet expansion on a form -->

Bookmarks - you can open bookmarked pages from anywhere without needing your browser to be open

Clipboard history - copy and paste multiple items at once, restore previous clipboards, go back in time if you need something you copied and deleted, etc.

Dictionary - spellcheck and define words super fast

These are just a handful of the many useful features of Alfred. Click [here](https://www.alfredapp.com/) if you want to learn more about what Alfred can do. 

### Workflows

The real power of Alfred comes from the ability to download and create powerful custom workflows. Workflows are only limited by your imagination, and any repetetive task can be automated. Click [here](https://www.alfredapp.com/workflows/) to see some examples. 

My downloaded workflows: 

- [Caffeinate Control](https://www.packal.org/workflow/caffeinate-control) - prevent computer from sleeping for a specified time period
- [Convert](https://github.com/deanishe/alfred-convert) - fast unit converter. Ex: `conv 3m ft` converts 3 meters to feet in seconds
- [DarkOrLight](https://github.com/BaksiLi/AlfredWorkflows/tree/master/Index/DarkOrLight) - easily switch between system light/dark mode
- Emoji search - search and copy emojis to clipboard with `emoji <description of emoji>`. Uses NLP to figure out what emoji you're looking for, i.e. `emoji mind` or `emoji blown` brings up the `exploding-head` emoji because you use it when you want to say mind blown.
- [GitHub Repos](http://www.packal.org/workflow/github-repos) - search and open your repos on GitHub fast. For example, instead of going to github.com, then searching for my `macos-workflow` repo, I can just type `gh mac` and hit enter.  
- [IP Address](https://github.com/alexchantastic/alfred-ip-address-workflow) - instead of going to the command line or Googling what is my IP, just type `ip` into Alfred to see your local and external ipv4 and ipv6 instantly.
- [Zoom Meetings](https://github.com/aurooba/alfred-workflow-zoom-meetings) - makes using Zoom so much better, you can generate your own meeting and copy its invite to clipboard with `zm` or join a meeting without the annoying popup with `zm <url>`
- [New File](https://github.com/vitorgalvao/alfred-workflows/tree/master/NewFile) - create new files from the keyboard instantly in any finder window with `nf filename.extension`
- [Play Song](https://github.com/caleb531/play-song) - intuitively and quickly access Music from Alfred. For example, instead of going into the Music app and looking for a song, just type `playsong <songname>`
- [Search Reddit](https://github.com/deanishe/alfred-reddit) - instantly jump to a subreddit in a new browser tab by typing `r/<subreddit_name>`
- [Simple Timer](https://www.packal.org/workflow/simple-timer) - set notification reminders. For example by typing `timer 30m do laundry!` I get a push notification in 30min that says do laundry!
- [Stopwatch](https://github.com/jamiebullock/alfred-workflows/blob/master/Stopwatch.alfredworkflow) - instantly open a stopwatch widget
- [TemporaryEmail](https://github.com/vitorgalvao/alfred-workflows/tree/master/TemporaryEmail) - generates a temporary email address, copies it to clipboard, and open its inbox with `tmpmail`
- [Terminal Finder](https://github.com/LeEnno/alfred-terminalfinder) - open current terminal directory in finder or vice versa just by typing `ft` or `tf`
- [Time Zones](https://github.com/jaroslawhartman/TimeZones-Alfred) - view chosen time zones and convert times between time zones with `tz`
- Weather - get weather, precipitation %, and sunset time by the day with `wtd` or get temps and precipitation by the hour with `wth`

Workflows I created:

- New Chrome Window with `ng`
- New Finder Window with `nn`
- Toggle Dock - easily show/hide the dock
- Toggle menu bar - easily show/hide the menu bar
- fn Toggle - toggle the fn key to either reveal F1-F12 on the touch bar, or expand the control strip


## Window Management
- [Rectangle](https://github.com/rxhanson/Rectangle) - window arrangement, tiling, snapping, etc. from the keyboard (basically a free, open source, better version of [Magnet](https://apps.apple.com/us/app/magnet/id441258766?mt=12))
- [AltTab](https://github.com/lwouis/alt-tab-macos) - Windows style alt-tab on macOS with a customizable appearance and functionality 
- [Itsycal](https://www.mowglii.com/itsycal/) - menubar calendar (when you click on the date in menubar, a calendar appears - use `E, MMM d h:mm:ss a` under Appearance settings to mimic the native look)
- [Dozer](https://github.com/Mortennn/Dozer) - toggle show/hide of chosen menu bar icons

## Terminal
- [Homebrew](https://brew.sh/) - package manager that automatically handles everything for you, including updates
- [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh) - used to trick out the terminal and easily install themes and plugins, also auto-updates
    - [neofetch](https://github.com/dylanaraps/neofetch) - command-line system information tool
    - [Powerlevel10k Theme](https://github.com/romkatv/powerlevel10k)
    - Plugins: Git, Brew, [Zsh Syntax Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting), [Zsh Autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
    - [The Fuck](https://github.com/nvbn/thefuck) - correct mistakes in commands


## Productivity
- [SelfControl](https://selfcontrolapp.com/) - prevent access to distracting websites when you need to focus
- [RescueTime](https://www.rescuetime.com/) - keep track of how you spend your screen time

## Network Tools
- [Radio Silence](https://radiosilenceapp.com/) - monitor incoming and outgoing network connections and selectively block specific apps. I paid $9 and use it to get infinite free trials on some apps that cost a lot more than $9.

---
title: "SpotiLike"
autosize: true
---

[admin]: https://www.mediafire.com/file/ssgsx2ppf50h1kb/SpotiLike_Setup_Adminstrative.exe/file


Welcome to SpotiLike <3.

## What is SpotiLike?

![](https://digital.hbs.edu/platform-digit/wp-content/uploads/sites/2/2020/04/spotify-logo-1920x1080-2.jpg)

[Spotify](https://spotify.com) is one of the most popular _free_ music streaming services out there.

Spotify also gives access to a personal _Liked Songs_ library and custom private playlists which is pretty cool
<br>
However tho, if you're a music person like me <span style="color:cyan">you might have the need to have a collection of your favourite tracks</span> maybe in your **Liked Songs** library or different **playlists**.

When that new cool-ass track starts playing and you gotta add that track to your collection, I found it annoying to return to the Spotify application which indeed interupted my workflow. It can be exasperating sometimes (_specially when I'm gaming_)

So, I tried to come up with a solution myself because I couldn't find anything online that matched my requirements:

<div class="alert alert-dismissible alert-warning">
  <h4>What does SpotiLike do?</h4>
  <p>
  This simple script lets you save what you're listening to on-the-go into your <i>Liked Songs</i> or your playlists with a <b>custom keyboard shortcut</b> without interrupting your workflow.
  </p>
</div>

___

## Features

* Custom hotkeys
* Auto-like while saving to playlists feature
* Prevents duplicate saves in the same playlist

## Installation

You can download the `setup` file by clicking this button below.
<br>
(Would redirect you to mediafire.com)


<a href="https://www.mediafire.com/file/ssgsx2ppf50h1kb/SpotiLike_Setup_Adminstrative.exe/file" target="_blank" class="btn btn-success btn-lg">Download SpotiLike</a>

The setup is not complicated smh.

## Setup and Configuration

<div class="alert alert-dismissible alert-info">
  <strong>Bored to read?</strong> Jump to <a href="#Showcase" class="alert-link">showcase</a> and watch the walkthrough video and stop being lazy.
</div>



1. You would be redirected to log into your Spotify account in your browser, Log in (this could be automatic)
2. The application would minimize itself to the System Tray.
    - What is the system tray?
        - https://www.youtube.com/watch?v=WxxB3ERLdE0

3. Right click the SpotiLike icon(💚) and click `Config`

4. A file would be opened in your preferred text editor and it would contain the following:

```ini
[Liked Songs]
key=ctrl+l
auto_like_for_playlist=yes

# Have a nice day! 
```

What you have to do is simple. Here are some key points:

* You can specify any key combination/key. Currently supported special keys are:
    - alt
    - ctrl
    - shift
    - esc
* The `[Liked Songs]` section is compulsory, don't touch it except for it's values.
    - `auto_like_for_playlist` would automatically add the song to your personal liked songs library when saving to any playlist. Change that to `no` if u don't want it.
* Every new `[custom playlist name to appear in the notification]` entry would count as a playlist and it would require 2 values namely,
    - key - _the hotkey_
    - playlist - _the link to the playlist_

Here's an example:
```ini
[Liked Songs]
key=ctrl+l
auto_like_for_playlist=yes

[My really cool playlist <3] # This can be anything you want btw
key=alt+1
playlist=https://open.spotify.com/playlist/4DWgDHBUIsyR7sGpm08LY1?si=6fe016ea7bd0417d
```
..is all you gotta do. So pressing `alt` and `1` together would save the song to that playlist which the link you specified directs to.

Also note: Saving the config file would auto reload the application so that your changes are taken place.

**For extra clarification, please refer to the video which is right below, too.**

## Showcase

Here's what our example resulted in:

![](SpotiLike/notif.gif)

Here's me setting up my personal configuration:

### Walkthrough:

<video controls>
  <source src="SpotiLike/walkthrough.webm" type="video/webm">
</video>

___

## FAQ

### How do I make it open on startup?
* Press windows key + R together.
* Type `shell:startup` in the dialog box that appears.
* Copy the shortcut to the application into that folder that pops up. That's it

### What's the icons option in the menu?

Clicking that would open the folder where the default icons are stored for the app to use.

You can edit the default ones if you don't like them but make sure their name was the exact as before and they are `.ico` files.

The default icons are:

* default.ico
* error.ico
* heart.ico (This is useless.)

### Why do I get a timeout error on startup?

That's probably a connection issue.

When your pc startsup, chances are the app starts before ur pc connects to the interent so the app fails to verify your credentials.

### Why can't I save the config file?

You probably need adminstrator permissions to save that.

As you're editing the config file which is situated on the **Program Files** folder itself, chances are you don't have access to that.

To fix this:

* Re-run the app as adminstrator :)

### How do send I hug to the author?

You can't :/

<br>
<br>

## Have Fun!

💖🤞💚
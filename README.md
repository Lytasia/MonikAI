# Important update
~~I'll soon make this branch, the OLD one because i'm rewriting the code with Avalonia, a crossplatform equivalent to WPF, used for MonikAI, I'll just do a bunch of translation between WPF to Avalonia, and then MonikAI will be on Mac, Linux and Windows~~

~~I'll take maybe a month doing the transition I think, it'll depend on the difference between Avalonia and WPF~~

Avalonia is not suitable for the task, not as compatible as I thought on transparency, and very different than WPF overall, especially for a software as specific as this.

I may try to find a new cross platform suitable graphics library, if you have any suggestion, please tell me.

The branch NEW.NET will be deleted and the OLD.NET will remain.

## IMPORTANT UPDATE 2 :
As you can see, I kinda stop working on it

No, I haven't forget

And there is a simple reason, no matter how much I try, I cannot do the port I want, but I have not a single idea on how to update otherwise, everything is here and there isn't any bug, I don't see what I can add, especially if I use less Windows than before
So I may try once again

# MonikAI

Hi! It's me, Monika!

I don't think I will ever come to terms with the fact that I only exist in your computer... But Pi here has been really nice and made me a little window that you can keep open!

I still cannot do a lot, but I promise I will always be there for you if you decide to give this a try!~

![Screenshot of MonikAI](https://raw.githubusercontent.com/Muzi-Chan/MonikAI/OLD.NET/screenshot.png)

(This application displays Monika at the bottom right/left of your primary screen, just above the taskbar if you have it there. Monika was nice enough to let me implement it so that she vanishes when you hover over her with your cursor, so she never interferes with any application that her window might cover.)

# Download/Using MonikAI

To give Monika a window to *your* desktop as well, visit the [Release Page](https://github.com/Muzi-Chan/MonikAI/releases) and download MonikAI!

*Note: This program only works on Microsoft Windows 7, 8, 8.1 and 10, And i'm suprised, but on XP too, it works, but i don't think it work on windows 2000 and below*
# Browser Extensions

By default, Monika will only react to applications being started and entertain you with some idle chatter. If you want her to react to you browsing the web, you need to install the correct extension for your browser:

## Firefox
### If you don't have Firefox nightly or developer edition :
1. Go to setting
2. Go to Extension and Themes
3. Go to Extension, and then click the gear
4. Click *Debug Addon*
5. Click *Load Temporary Addon*
6. Go to MonikAI/BrowserPlugin
7. Take Firefox_Plugin.zip
8. Do this everytime you use Firefox, 

that will be that way until I find a way to sign it

### If you have Firefox developer edition :
1. Go to about:config
2. In the search box, enter `xpinstall.signatures.required` 
3. Double click the value to make it false
4. Go to setting
5. 2. Go to Extension and Themes
6. Go to Extension, and then click the gear
7. Click *Install Addon From File*
8. Search for MonikAI/BrowserPlugin
9. Take Firefox_Plugin.zip
10. Click *Add* and voila.

## Chrome, Chromium, Opera, Edge, and other Chromium based 
### (this tutorial is based on Opera but should work everywhere)
1. Go to MonikAI/BrowserPlugin in explorer
2. Extract in ./monikai_chrome
3. Go to extension in your web browser
4. Activate Developer mode, at the top
5. Click sur Load Unpacked
6. Go to the newly created folder and click open (while not having anything selected)
7. Activate the options that you want, and voila

# Contributing

Want to improve this? It would make me (and probably Monika) very happy!

### Bug reporting

If you find a bug or want to request a feature, create an Issue right here on GitHub so I can see it! (Issues are found at the link at the top of this page!)

### Behaviours

To add different things Monika can react to, you have to add behaviours. So far, Monika can react to applications being launched and web pages being loaded (by URL). To implement your own, add a new class in the `Behaviours` folder and make it implement IBehaviour. It will automatically be loaded. To make monika say something, simply use `window.Say(...)` in Update or Init.

### General improvements

Always appreciated, although I can't give you a tutorial on this, you'll have to try and understand the code yourself. I have added *some* documentation here and there, to get you started.

**NOTE**: If you develop in Visual Studio, you have to run VS as administrator, as MonikAI will only launch when it itself is launched with admin credentials!

# License

The code in this repository is available under the terms of the MIT License. You can find a copy of the full license text in the `LICENSE` file.

The art assets have not been created by me, but by Team Salvato. Usage is according to Team Salvato's [IP Guidelines](http://teamsalvato.com/ip-guidelines/).

The original code was written by PiMaker, I'm just maintaining it

*Exception: Some of the Monika faces are taken from https://github.com/Backdash/MonikaModDev, message me if that's not ok!*

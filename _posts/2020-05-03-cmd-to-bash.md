# Quickly switching from Command Prompt / Powershell to Bash with Windows Subsystem Linux

Although I was born and raised using Windows machines for as long as I can remember, the majority of my software development has been done MacOs and Linux. As such for a while now I've been searching for ways to maximize all my Unix command line muscle memory, but within a Windows environment. I've tried a few things over the years. Git Bash was one of the first tools I found that allowed the use of Bash commands within Windows, granted with a few quirks and problems of its own. The introduction of Windows Subsystem Linux however put an end to my need for Git Bash, now that I can access a (mostly) full fledged Linux OS right there inside my Windows machine.

Up until very recently though I had been using the WSL side of my computer either by running the Ubuntu launcher as a separate terminal window (which landed me in the root of the WSL machine, and I then needed to furiously `cd` my way into whatever directory I needed to work in), or switching shells within Visual Studio Code which automatically took care of the switching. But what if I wanted to work outside of VScode?

I recently discovered a small command that has made my life even easier for any work I need to do, anywhere in the machine. Within any Command Prompt or Powershell window you can simply run the command

```cmd
bash
```

and the Linux subsystem you have installed is activated and switched too, right there in whatever directory you are sitting in.

Sitting in the users root of my Windows machine in the VScode terminal running CMD:

![cmd](/assets/images/cmd-to-bash/cmd.png)

Running

```cmd
bash
```

![bash](/assets/images/cmd-to-bash/bash.png)

And VOILA! I'm now running Ubuntu bash in the same directory. I have not yet found a way to switch _back_ to powershell or cmd but will update this post if I do.

Happy bashing on Windows!

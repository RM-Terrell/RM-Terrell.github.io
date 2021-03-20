---
layout: post
title: "Custom snippets in VS Code"
author: "RM Terrell"
photo_credit: "RM Terrell"
categories: journal
tags: [vscode, javascript]
image: skin_track.jpg
---
A few snippet extensions I've installed have inspired me to venture into creating my own custom ones. Turns out VSCode has a great system for doing this and can be a huge time saver for boilerplate code.

### The Initial Annoyance
A snippet I've gotten a lot of use out of is `testa` which comes from the Jest Snippets extension (I think, I have a lot of extensions and its hard to tell at this point). This snippet scaffolds out an async
jest test like this

![testa](/assets/img/custom-snippets-vscode/before_snippet.png)

This is very useful but each time I do it I need to go back, add a semi colon, and make the test description a template literal instead of single quotes. This comes from the ESLINT rules I'm using (the semi colon) and personal preference for easy, long, indented test names (the template literal). Sure would be nice if I didn't have to make that edit every time right?

### Creating the snippet

With <kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+<kbd>P</kbd> (assuming Windows, use CMND instead if on Mac) open up the command pallet and search for "Configure User snippets"

![1](/assets/img/custom-snippets-vscode/snippet_setting_1.png)

Click that option at the top then click the javascript option

![2](/assets/img/custom-snippets-vscode/snippet_setting.png)

Once you're in there you have a whole file to create your own custom snippets. I created the slightly modified version of the `testa` snippet like so

![final](/assets/img/custom-snippets-vscode/final_snippet.png)

The one tricky bit here was those `\n` characters. Those are to create new lines in the resulting snippet automatically. Now when I type `testa` I get a second option (mine with my custom description) that scaffolds out an async test as per the standards in the repo I'm working in.

![result](/assets/img/custom-snippets-vscode/final_result.png)

### Syncing

The other great thing about this solution, is that the file for custom snippets is tracked as part of VSCodes setting sync feature. So when you create custom snippets on one machine, you will have these on any other.

Happy snipping.

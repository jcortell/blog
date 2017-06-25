---
id: 8308
title: Cool online presentations with free software
date: 2017-05-26T08:45:38+00:00
author: Jorge Cortell
categories:
  - Copyfight
  - Free Software
  - Geek Fun
  - General
  - Hacking
  - "Life's pleasures"
  - Personal
  - Technology
  - Technolust
  - Why not? Utopia?
---
It has been a while since I wrote a tutorial to _Share The Wealth_, so it’s about time I shared some practical (if basic) knowledge beyond reposting a link.

For years I have had a pet project in the backburner: I wanted to create presentations without the need of dedicated software, commercial (like PowerPoint or Keynote), or free (like LibreOffice or OpenOffice). That way I could avoid bringing my computer to a lecture, and not worry about what computer system would be available in the auditorium. As long as there is internet connectivity or a USB port, I can bring a URL and a USB as a backup, and it will work.

I also wanted some minimum functionality like:

  * Being able to print the presentation or export it into PDF
  * Keyboard controls (including overview)
  * Accesible from any device
  * Progress bar
  * Transitions and effects
  * Reproducible in any browser without the need of any plug-in or additional software
  * Presenter window with next slide, notes and countdown
  * All in a file format that is easy to use, like HTML or Markdown

Of course, your wishes shall be granted by the gods of Free Software. Behold the no-dependencies JavaScript [Reveal.js](https://github.com/hakimel/reveal.js).

But to make the presentation truly awesome, there were a few more things I needed to do, like incorporating it into my Git workflow (for branches, versions, and all those Git goodies) and hosting it.

Let me walk you through the process, so you can also be up and running with Presentation Awesomeness in no time:

First, create a new repository on GitHub or GitLab (if you don’t know what that is, you need to read other tutorials first). For this tutorial, I’ll use GitHub, although in the office we use Gitlab.

Give your presentation a name, like “MyPresentation”.

Clone it to your local machine. You can use the GUI application (I like the new Electron-based beta), or use the CLI (“Terminal” for Apple OSX users):

`git clone git@github.com:yourusername/MyPresentation.git`
  
[Obvious note: substitute “yourusername” for your user name]

Clone reveal.js onto your local machine. This time:
  
`git clone git@github.com:hakimel/reveal.js.git`

Go to the File System (“Finder” in OSX), locate your Git working directory (“Folder” in OSX), and move (or copy) the content of the directory “reveal.js” to the “MyPresentation” folder.

Modify the index.html file. This is where your presentation content and format goes. Take a look at the [detailed tutorial here](https://github.com/hakimel/reveal.js).

Once done, “push” the project to your Git. If using the CLI:
  
`git push`

Feel free to use Grunt for local dynamic serving. Some people even use generator-reveal, a Yeoman generator, to have each slide as an individual HTML or Markdown file.

If you are using GitHub, now, “automagically”, your slides are published at yourusername.github.io/MyPresentation

One more detail: if you want to access the slides themselves (for a hosted presentation) instead of the “repo” (repository of all the files you just “pushed”), you need to go to GitHub and enable “GitHub pages” in this particular repository. Just go to the repository index.html page in GitHub, and select the down-arrow menu icon on the upper right (nexto to &#8220;insights&#8221;) “settings>pages” and activate GitHub pages for that repo.

Additionally, there are many plugins you can use with reveal.js, like [kreator](https://github.com/hakimel/reveal.js/wiki/Plugins,-Tools-and-Hardware). Enjoy!
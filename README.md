# Vim Workshop

> Changing cold feet to a warm bath

* * *

1. [Intro](/README.md/#intro)
  1. [Audience](/README.md/#audience)
  2. [Structure](/README.md/#structure)
  3. [Requirements](/README.md/#requirements)
2. [This Repo](/README.md/#this-repo)
  1. [Presentation](/README.md/#presentation)
    1. [Preparation](/README.md/#preparation)
    2. [Why Vim](/README.md/#why-vim)
    3. [Learning is difficult](/README.md/#learning-is-difficult)
    4. [History](/README.md/#history)
    5. [Vim GUI and don't panic](/README.md/#vim-gui-and-dont-panic)
    6. [Modes](/README.md/#modes)
    7. [Undo/Redo/Repeat](/README.md/#undoredorepeat)
    8. [Motions](/README.md/#motions)
    9. [Exercise 1: Getting familiar with some commands and the gui](/README.md/#exercise-1-getting-familiar-with-some-commands-and-the-gui)
    10. [More motions](/README.md/#more-motions)
    11. [Operators](/README.md/#operators)
    12. [Operator + Motion 1](/README.md/#operator--motion-1)
    13. [Exercise 2: Get used to motions and operators](/README.md/#exercise-2-get-used-to-motions-and-operators)
    14. [Even more motions](/README.md/#even-more-motions)
    15. [Operator + Motion 2](/README.md/#operator--motion-2)
    16. [Exercise 3: Not so efficient editing](/README.md/#exercise-3-not-so-efficient-editing)
    17. [Searching](/README.md/#searching)
    18. [Operator + search](/README.md/#operator--search)
    19. [Exercise 4: Slightly more efficient editing](/README.md/#exercise-4-slightly-more-efficient-editing)
    20. [Cut/Copy/Paste & Visual mode](/README.md/#cutcopypaste--visual-mode)
      1. [Cut/Copy/Paste](/README.md/#cutcopypaste)
      2. [Visual mode](/README.md/#visual-mode)
      3. [Visual mode + motions](/README.md/#visual-mode--motions)
      4. [Visual mode + operators](/README.md/#visual-mode--operators)
    21. [Exercise 5: Use visual mode to create a CSV file](/README.md/#exercise-5-use-visual-mode-to-create-a-csv-file)
    22. [Search/Replace](/README.md/#searchreplace)
    23. [Exercise 6: Use Search/Replace to create a CSV file](/README.md/#exercise-6-use-searchreplace-to-create-a-csv-file)
    24. [Text objects](/README.md/#text-objects)
    25. [More text objects](/README.md/#more-text-objects)
    26. [Operator + text objects](/README.md/#operator--text-objects)
    27. [If there's time left...](/README.md/#if-theres-time-left...)
      1. [vimrc](/README.md/#vimrc)
      2. [buffers](/README.md/#buffers)
      3. [windows](/README.md/#windows)
      4. [plugins](/README.md/#plugins)
    28. [Vim in other software](/README.md/#vim-in-other-software)
    29. [Credits and links](/README.md/#credits-and-links)
    30. [Images](/README.md/#Images)
  2. [files](/README.md/#files)
    1. [1-lorem.txt](/README.md/#1-loremtxt)
    2. [2-lorem-wrapped.txt](/README.md/#2-lorem-wrappedtxt)
    3. [3-sinatra.rb](/README.md/#3-sinatrarb)
    4. [4-boilerplate.html](/README.md/#4-boilerplatehtml)
    5. [5-string_calculator_spec.rb](/README.md/#5-string_calculator_specrb)
    6. [6-digits.txt](/README.md/#6-digitstxt)
    7. [7-markdown.txt](/README.md/#7-markdowntxt)
  3. [startvim](/README.md/#startvim)
  4. [vim-config](/README.md/#vim-config)
3. [Request for feedback](/README.md/#request-for-feedback)
4. [Links] (/README.md/#links)
  1. [Vim tips] (/README.md/#vim-tips)
  2. [Fun] (/README.md/#fun)
5. [TODO] (/README.md/#todo)
6. [License](/README.md/#license)

## Intro

We (that is Alexander Swen and [Joël Stemmer][Joel]) created this workshop to help our coding colleagues at [Nedap][nedap] to become more productive using Vim. This repo contains my continuated version of the original work we did at Nedap. It's a fork of [Nedap's Vim workshop repo][nedap_vim_workshop].
It is my experience that it takes about three hours to give this workshop and I have good experiences with about 12 people in a classroom setting.
You need every participant to have a workstation that has vim installed and a clone of this repo.
I bought a PDF version of the [Vim Cheat-sheet][cheat] by Max Cantor. I recommend all participants to buy one. Max kindly gave me permission to give away prints of this sheet. So, if you're reading this because you consider to give this workshop, consider to buy that cheatsheet and distribute them as well.

### Audience

This workshop is originaly developped for our colleagues at Nedap. They're programmers and sysadmins. Some of them never touched Vim, others use it occasionaly and some are experienced Vim users. Afterwards some of them started using Vim instead of their other editor, others improved their skills and work more efficient now.
This workshop is now intended for people who want to use Vim but fear the learning curve and for people who do simple things in Vim but want to benefit more from the powerful features Vim has to offer. However, everytime I gave this workshop there was some bloke that I would classify as "highly experienced". And even that kind of guys learned something new they said afterwards.
The workshop gives a structured overview of modes, motions and operators in such a way that the audience has an understanding of the mass of commands they see when they open vim for the 1st time. (or actually they only see that once they found the help command ;-).

### Structure

The idea is that you explain people how they can work superfast with Vim. To do this you should use the presentation "vim.odp" and let people try what you explained in the "exercises". These are very important as I believe practicing what you just learned improves the persistancy of the knowledge.
I also believe that people who just listen to a story for a while will remember far less than when they immediately get proof and see it's not that hard.
That's why the practicefiles are included. At the moment not all of them are used. They can be used off course.

### Requirements

To succesfully train people using Vim you need the following:
- A deep understanding of all commands explained in the presentation.
- A classroom style presentation room, with:
  + Enough tables and seats for the participants
  + Beamer
- A computer (preferably a laptop) to run the Libreoffice Impress presentation on.
- I like to use a [Presenter][presenter] to switch slides. This allows me to walk arround the classroom.

## This Repo

Is created to easily distribute the example files and handouts of this workshop to the participants. Now it holds everything related.

### Presentation

File called presentation/vim.odp.
The presentation is here to support the explanations about Vim. It is created in Libreoffice Impress and has two different background colours: Blue for things the presenter has to tell and explain, green for exercises the participants need to do themselves.
Exercises contain a few tasks and a reference of what I explained before.

#### Preparation

This slide informs users where to find this repo and (a bit) how to install Vim on their computer. It promises an USB stick to be available when no interwebs is there. (I never solely rely on working interwebs on public events).
I recommend to start showing this sheet well in advance of the actual training if you have the chance to avoid very long delays when you want to start.
This slide is followed by a splash slide that you can bring to front to draw attention and make clear you wish to start.

#### Why Vim

To give participants an idea of what they're going to learn and why Vim is still a cool editor after 35 years of development you let them count in their heads how much keystrokes it would take them in another editor (I allways use Notepad or, if the users really hate Windows Gedit for example) to make "This is another header" a header in this [simple markdown example](/README.md/#7-markdowntxt).

#### Learning is difficult

The picture of the learning curves of editors is a joke, but not without good background. Learning Vim can be a hurdle to take. However, once you know a litle bit you can already be working very fast, at least as fast as you did in your previous edittor before. A good read about this is [A blog post by Yehuda Katz about his "learning Vim" experience][yehuda].

#### History

A good read on the history is [Peteris Krumins' article about the hjkl keys in Vim][catonmat]. I allways explain how the hjkl thing came into Vim.
Tell a brief history of Vim. I always mention the following milestones:
- 1976 Vi created as improvement over ex. (vi is short for Visual).
- 1988 Bram Molenaar created 1st clone of Elvis on Amiga.
- 1991 Vim released in the wild by Bram Molenaar. (Vim meant either "Vi Improved" or "Vi Imitated").
- 1998 Syntax highlighting was added.
- 2006 7.0 released
- 2013-08-10: 7.4 released

#### Vim GUI and don't panic

Let's show the real stuff: the GUI. I took a screenshot once and pasted that and then lost it. That's why it's not listed in [The images list](/README.md/#images). However this to show a bit what's where etc. I tell the people that there is a gvimrc option to get rid of the toolbar.
Then the "don't panic" slide is here to show the commands I mention and first glimpse of the logic in commands. Emphasize on the detail that "q" and "wq" are abbreviations of complete commands. Tell that remembering a command is far more easy when you remember the word for it. "h" for help! is fairly obvious right?

#### Modes

Then we start talking about modes. Vim is the only editor I'm aware of that's defaulting to insert mode, moreover: I don't know any editor that has any other mode than "insertmode".
The most of our work is not keying in text, it's more about "changing text". And that should be done using the whole bunch of nifty commands Vim has to offer.
The first sheet explains the functions of the several modes and the second tells some ways of switching between them.

#### Undo/Redo/Repeat

Explain undo and redo commands. And that Vim keeps buffers of actions until you close the file. So the undo-/redobuffers are still available after you saved the file.
Learn people immediately to stay as short as they can in Insert mode. A good reason is because each insert action should result in a undo/redo event. Another reason is that you don't make silly mistakes like having ":w" in your tekst, or "i" in a script.
People love to hear about the dot command.
And the slide "repeat action _n_ times is great too" is here to explain another form of repeation.

#### Motions

They were already mentioned. But it is good to explain hjkl again. And I explain that ([reminding the blog post of Yehuda][yehuda]) people should definitely not try to use solely hjkl motions but rather stay one arrow keys as long as the feel more comfortable there. However, point out that not having to leave the homerow is a big timesaver.

#### Exercise 1: Getting familiar with some commands and the gui

People are now listening to you for quite some time so it's time for their first steps. Let's summarize what we've learned so far. Let's see who knows the result of the commands on this slide.
Then, of course a coffee break would be nice to have.

#### More motions

three slides with more motions. I walk through most of them. The first one has a nice revelation for those who know about regex: some motions are similar to regular expressions. (at least 0 ^ $ are)

#### Operators

Show some operators. Explain that most of these (exept for deletions) put you into insert mode.

#### Operator + Motion 1

This is the most important part of the whole workshop: the power of combining operators and motions. Essentially the rest is more of this. All participants have to understand this before you continue.

#### Exercise 2: Get used to motions and operators

File: [1-lorem.txt](/README.md/#1-loremtxt)
Let's immediately try this. If they do exactly what's on the exercise slide participants run into a situation where they change not a real word but a comma. Results are not important here: just the feeling of 3j, c4w etc.

#### Even more motions

Then we continue with even more motions.

#### Operator + Motion 2

And those can be combined with operators too.

#### Exercise 3: Not so efficient editing

File: [4-boilerplate.html](README.md/#4-boilerplatehtml)
This is the first time to edit this file. People have to really dw and then retype (they don't know copy/paste yet).

#### Searching

Explain how to search. People like to know that regexes are supported here.

#### Operator + search

And how search can be combined with operators as well.

#### Exercise 4: Slightly more efficient editing

File: [4-boilerplate.html](README.md/#4-boilerplatehtml)
This is the second time to edit this file. People should be able to move arround quicker now.

#### Cut/Copy/Paste & Visual mode

At this point people should be begging for copy/paste commands. They retyped "navigation" a million times now.

##### Cut/Copy/Paste

Immediately tell yw to show that also yank can be combined with a motion. And tell the rest. pay some atention to yy. They all should note the similarity with cc/dd now. Then tell them that with this knowledge the previous two exercises would have been way easier.

##### Visual mode

Time for visual mode now. The visual block mode is quite unique. Only [Sublime text][sublime] has that function too (afaik).
A nice example to show "select all": ggVG

##### Visual mode + motions

Visual mode can't realy exist without motions.

##### Visual mode + operators

After you've selected something you can also operate on it! great!

#### Exercise 5: use visual mode to create a CSV file

File: [6-digits.txt](README.md/#6-digitstxt)
This file will be used twice as well: this time participants may only use visual mode to achieve the goal: create a CSV file.
They should all ask if this can't be done using search and replace

#### Search/Replace

Search/replace is a real powertool. Simple things can be done very quick. Especially repetitive work is often a good candidate to be done using search/replace. Or rather "substitute" like it's called in awk/sed/perl and other tools.

#### Exercise 6: Use Search/Replace to create a CSV file

File: [6-digits.txt](README.md/#6-digitstxt)
Let the participants use search/replace to change the file [6-digits.txt](/README.md/#6-digitstxt) to a CSV file (they may choose their own separator). The following three commands (after removing lines 1,3 and last) should be sufficient:
``` vim
:%s/^| //
:%s/ | /,/
:%s/   |//
```
Then, just for fun, show the power of search and replace by using:
``` vim
:%s?\D\+\(\d\+\)\D\+\(\d\+\)\D\+?\1,\2?
```


#### Text objects

Shows some basic text objects. Tell something about inner and arround.

#### More text objects

Shows some more text objects.

#### Operator + text objects

Explains the power of combining operators and text objects. Some examples are shown on the slides and one can choose to add an exercise: use [3-sinatra.rb](/README.md/#3-sinatrarb) for example to let users change stuff between quotes or [4-boilerplate.html](/README.md/#4-boilerplatehtml) to let them try "cit".

#### If there's time left

4 bonus subjects. Only to be discussed when the clock and the audience's attention allow for it (the participants are learning stuff for quite a while at this point and I can imagine they loose interest and attention).

##### vimrc

An explanation of the vimrc config file and how one can try his modifications while editting. In the (yet to be created) advanced workshop the use of the command :options will help.

##### buffers

A little explanation on vim buffers is usefull. This subject is covered more deeply in the (yet to be created) advanced workshop.

##### windows

A little explanation on vim splits is usefull. This subject is covered more deeply in the (yet to be created) advanced workshop.

##### plugins

A little explanation on vim plugins is usefull. This subject is covered more deeply in the (yet to be created) advanced workshop.

#### Vim in other software

A short list of some other programs that support features from vim. The list is not exhaustive, just to give an impression. Recently "vifm" was added.

#### Credits and links

This sheet shows a bunch of usefull links.

#### Images

All images used in the Impress presentation are located in this folder. Below a list of them and where I found them:
<table>
  <tr><td>Jimi-Hendrix.jpg</td><td><a href="http://images2.fanpop.com/images/photos/5000000/Jimi-Hendrix-jimi-hendrix-5029449-1024-768.jpg">fanpop.com</a></td></tr>
  <tr><td>achtergrond blauw.jpg</td><td><a href="http://templates.libreoffice.org/template-center/typography">Typoography template </a>and kindly recreated by my colleague <a href="https://github.com/dreagle">Ronald van Zon</a></td></tr>
  <tr><td>achtergrond blauw.png</td><td><a href="http://templates.libreoffice.org/template-center/typography">Typoography template </a>and kindly recreated by my colleague <a href="https://github.com/dreagle">Ronald van Zon</a></td></tr>
  <tr><td>achtergrond groen.jpg</td><td><a href="http://templates.libreoffice.org/template-center/typography">Typography template</a></td></tr>
  <tr><td>adm-3a-hjkl-keyboard.jpg</td><td><a href="http://www.catonmat.net/blog/why-vim-uses-hjkl-as-arrow-keys/">Catonmat.net</a></td></tr>
  <tr><td>demo1.avi</td><td><a href="https://github.com/aswen">Alexander Swen</a></td></tr>
  <tr><td>learning_curve-text-editors.jpg</td><td><a href="https://www.google.com/search?site=&tbm=isch&source=hp&biw=1148&bih=957&q=%22classical+learning+curves+for+some+common+editors%22&oq=%22classical+learning+curves+for+some+common+editors%22">Can't find origin</a></td></tr>
  <tr><td>Lear Siegler ADM-3A computer terminal.jpg</td><td><a href="http://www.catonmat.net/blog/why-vim-uses-hjkl-as-arrow-keys/">Catonmat.net</a></td></tr>
  <tr><td>repetitive tasks.png</td><td><a href="https://plus.google.com/+BrunoOliveira/posts/MGxauXypb1Y">Bruno Oliveira</a></td></tr>
  <tr><td>vim3d_the_editor.png</td><td><a href="http://www.ivankristianto.com/vi-and-vim-editor-cheat-sheet-pdf/">Ivan Kristianto</a></td></tr>
  <tr><td>vim-bottom.jpg</td><td>Screenshot created by <a href="https://github.com/aswen">Alexander Swen</a></td></tr>
</table>

### Files

The repo contains a bunch of examplefiles to let the participants play with during exercises. Most of them are found on internet and some are intentionally damaged.

#### 1-lorem.txt

Used in [Exercise 2](/README.md/#exercise-2-get-used-to-motions-and-operators) to let participants change random text.
This file was found on [nl.lipsum.com][lipsum].

#### 2-lorem-wrapped.txt

File currently not used. Was added to show effect of word wrapping.
This file was found on [nl.lipsum.com][lipsum].

#### 3-sinatra.rb

File currently not used. Might be usefull in future.
This file was found on [Sinatrarb.com][sinatra_origin].

#### 4-boilerplate.html

Used in [Exercise 3](/README.md/#exercise-3-not-so-efficient-editing) and [Exercise 4](/README.md/#exercise-4-slightly-more-efficient-editing) to let participants experience how they can work more efficient using copy/paste.
This file was found on [Imakewebthings' deck.js Github repo][boiler_origin].

#### 5-string_calculator_spec.rb

This file was originally used to demonstrate ci" and similar functions.
This file was found on [Katacasts' string_calculator Github repo][string_calc_origin].

#### 6-digits.txt

File used in [Exercise 5](/README.md/#exercise-5-use-visual-mode-to-create-a-csv-file) and [Exercise 6](/README.md/#exercise-6-use-searchreplace-to-create-a-csv-file) to demonstrate how easy you can change a lot of lines at ones using visual mode and how to be even more efficient using [Search/Replace](/README.md/#searchreplace).

#### 7-markdown.txt

File that's used in [Why Vim?](/README.md/#why-vim) demo.

### startvim

This script is created to make it easy for Linux and Mac users to start vim with the specific config for this workshop.
It tries to either start mvim or gvim. For Windows users there's no help...
This script can be improved to work better on macs as on some of them there has to be a symlink to the vim executable from the homedir before it's found by "which".

### vim-config

We created a config that has some usefull default settings. This is to make sure that everyone participating in the workshop has the same settings and to avoid strange behaviour because of peoples own settings. I strongly recommend to encourage the use of this config during the workshop, even for experienced users.

## Request for feedback

I would highly appreciate feedback on this workshop. Especially if you attended one of my workshops I like to improve both this workshop and my training skillz. You can contact me via [Mail][mailme].

## Links

The last sheet contains some links to interesting websites. Here's that list.

### Vim tips
- [Vim.org][vimorg]
- [Drew Neils vimcasts][vimcast]
- [Vimcheatsheet][cheat]
- [Tim Popes plugins][tpope]
- [ZZappers Vim tips][zzapper]

### Fun
- [Vimgolf][vimgolf]
- [Vim Adventures][vimadventures]

## Todo

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Vim workshop</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/aswen/vim-workshop" property="cc:attributionName" rel="cc:attributionURL">Alexander Swen</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/nedap/vim-workshop" rel="dct:source">https://github.com/nedap/vim-workshop</a>. It was created by Alexander Swen & Joël Stemmer for Nedap N.V..

[Joel]: https://github.com/jstemmer "Joël Stemmer"
[nedap]: http://www.nedap.com/ "Nedap"
[nedap_vim_workshop]: https://github.com/nedap/vim-workshop "Nedap's Vim workshop repo"
[cheat]: http://vimcheatsheet.com "Vim cheat-sheet"
[presenter]: http://www.logitech.com/nl-nl/mice-pointers/presenter "Logitech Presenter"
[yehuda]: http://yehudakatz.com/2010/07/29/everyone-who-tried-to-convince-me-to-use-vim-was-wrong/ "Everyone Who Tried to Convince Me to use Vim was Wrong"
[catonmat]: http://www.catonmat.net/blog/why-vim-uses-hjkl-as-arrow-keys "Here is why vim uses the hjkl keys as arrow keys"
[sublime]: http://www.sublimetext.com "Sublime text"
[lipsum]: http://nl.lipsum.com/intro "Lipsum.com"
[sinatra_origin]: http://www.sinatrarb.com/intro "Sinatrarb"
[boiler_origin]: https://github.com/imakewebthings/deck.js/blob/master/boilerplate.html "Imakewebthings deck.js"
[string_calc_origin]: https://github.com/katacasts/string_calculator/blob/master/spec/string_calculator_spec.rb "Katacasts string calculator"
[mailme]: mailto:vim@swen.nu "my mailaddress"

[vimorg]: http://www.vim.org "Vim.org"
[vimcast]: http://www.vimcasts.org "Vimcasts.org"
[cheat]: http://vimcheatsheet.com "Vim Cheatsheet"
[vimgolf]: http://vimgolf.com "Vim Golf"
[vimadventures]: http://vim-adventures.com "Vim adventures"
[tpope]: http://github.com/tpope
[zzapper]: http://zzapper.co.uk/vimtips.html "Vim tips from zzapper"

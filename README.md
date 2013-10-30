# Vim Workshop

> Changing cold feet to a warm bath

* * *

1. [Intro](/README.md/#intro)
  1. [Audience](/README.md/#audience)
2. [This Repo](/README.md/#this-Repo)
  1. [Presentation](/README.md/#presentation)
    1. [Preparation](/README.md/#preparation)
    2. [Why Vim](/README.md/#why-vim)
    3. [Learning is difficult](/README.md/#learning-is-difficult)
    4. [History](/README.md/#history)
    5. [Modes](/README.md/#modes)
    6. [Undo/Redo/Repeat](/README.md/#undoredorepeat)
    7. [Motions](/README.md/#motions)
    8. [Exercise 1: Getting familiar with some commands and the gui](/README.md/#exercise-1-getting-familiar-with-some-commands-and-the-gui)
    9. [More motions](/README.md/#more-motions)
    10. [Operators](/README.md/#operators)
    11. [Operator + Motion 1](/README.md/#operator--motion-1)
    12. [Exercise 2: Get used to motions and operators](/README.md/#exercise-2-get-used-to-motions-and-operators)
    13. [Even more motions](/README.md/#even-more-motions)
    14. [Operator + Motion 2](/README.md/#operator--motion-2)
    15. [Exercise 3: Not so efficient editing](/README.md/#exercise-3-not-so-efficient-editing)
    16. [Searching](/README.md/#searching)
    17. [Operator + search](/README.md/#operator--search)
    18. [Exercise 4: Slightly more efficient editing](/README.md/#exercise-4-slightly-more-efficient-editing)
    19. [Cut/Copy/Paste & Visual mode](/README.md/#cutcopypaste--visual-mode)
      1. [Cut/Copy/Paste](/README.md/#cutcopypaste)
      2. [Visual mode](/README.md/#visual-mode)
      3. [Visual mode + motions](/README.md/#visual-mode--motions)
      4. [Visual mode + operators](/README.md/#visual-mode--operators)
    20. [Exercise 5: Use visual mode to create a CSV file](/README.md/#exercise-5-use-visual-mode-to-create-a-csv-file)
    21. [Search/Replace](/README.md/#searchreplace)
    22. [Exercise 6: Use Search/Replace to create a CSV file](/README.md/#exercise-6-use-searchreplace-to-create-a-csv-file)
    23. [Text objects](/README.md/#text-objects)
    24. [More text objects](/README.md/#more-text-objects)
    25. [Operator + text objects](/README.md/#operator--text-objects)
    26. [If there's time left...](/README.md/#if-theres-time-left...)
      1. [vimrc](/README.md/#vimrc)
      2. [buffers](/README.md/#buffers)
      3. [windows](/README.md/#windows)
      4. [plugins](/README.md/#plugins)
    27. [Vim in other software](/README.md/#vim-in-other-software)
    28. [Credits and links](/README.md/#credits-and-links)
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
4. [License](/README.md/#license)

## Intro

We (that is Alexander Swen and [Joël Stemmer][Joel]) created this workshop to help our coding colleagues at [Nedap][nedap] to become more productive using Vim. This repo contains my continuated version of the original work we did at Nedap. It's a fork of [Nedap's Vim workshop repo][nedap_vim_workshop].
It is my experience that it takes about three hours to give this workshop and I have good experiences with about 12 people in a classroom setting.
You need every participant to have a workstation that has vim installed and a clone of this repo.

[Joel]: https://github.com/jstemmer "Joël Stemmer"
[nedap]: http://www.nedap.com/ "Nedap"
[nedap_vim_workshop]: https://github.com/nedap/vim-workshop "Nedap's Vim workshop repo"

### Audience

This workshop is originaly developped for our colleagues at Nedap. They're programmers and sysadmins. Some of them never touched Vim, others use it occasionaly and some are experienced Vim users. Afterwards some of them started using Vim instead of their other editor, others improved their skills and work more efficient now.
This workshop is now intended for people who want to use Vim but fear the learning curve and for people who do simple things in Vim but want to benefit more from the powerful features Vim has to offer. However, everytime I gave this workshop there was some bloke that I would classify as "highly experienced". And even that kind of guys learned something new they said afterwards.

The workshop gives a structured overview of modes, motions and operators in such a way that the audience has an understanding of the mass of commands they see when they open vim for the 1st time. (or actually they only see that once they found the help command ;-).

## This Repo

Is created to easily distribute the example files and handouts of this workshop to the participants.

### Presentation

The presentation is here to support the explanations about Vim. It is created in Libreoffice Impress and has two different background colours: Blue for things the presenter has to tell and explain, green for exercises the participants need to do themselves.

#### Preparation

#### Why Vim

#### Learning is difficult

#### History

#### Modes

#### Undo/Redo/Repeat

#### Motions

#### Exercise 1: Getting familiar with some commands and the gui

#### More motions

#### Operators

#### Operator + Motion 1

#### Exercise 2: Get used to motions and operators

#### Even more motions

#### Operator + Motion 2

#### Exercise 3: Not so efficient editing

#### Searching

#### Operator + search

#### Exercise 4: Slightly more efficient editing

#### Cut/Copy/Paste & Visual mode

##### Cut/Copy/Paste

##### Visual mode

##### Visual mode + motions

##### Visual mode + operators

#### Exercise 5: use visual mode to create a CSV file

#### Search/Replace

#### Exercise 6: Use Search/Replace to create a CSV file

Let the participants use search/replace to change the file [6-digits.txt](/README.md/#6-digitstxt) to a CSV file (they may choose their own separator). The following three commands (after removing lines 1,3 and last) should be sufficient:
``` vim
:%s/^| //
:%s/ | /,/
:%s/   |//
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

### files

The repo contains a bunch of examplefiles to let the participants play with during exercises. Most of them are found on internet and some are intentionally damaged.

#### 1-lorem.txt

Used in [Exercise 2](/README.md/#exercise-2-get-used-to-motions-and-operators) to let participants change random text.
This file was found on [nl.lipsum.com][lipsum].

[lipsum]: http://nl.lipsum.com/intro "Lipsum.com"

#### 2-lorem-wrapped.txt

File currently not used. Was added to show effect of word wrapping.
This file was found on [nl.lipsum.com][lipsum].

[lipsum]: http://nl.lipsum.com/intro "Lipsum.com"

#### 3-sinatra.rb

File currently not used. Might be usefull in future.
This file was found on [Sinatrarb.com][sinatra_origin].

[sinatra_origin]: http://www.sinatrarb.com/intro "Sinatrarb"

#### 4-boilerplate.html

Used in [Exercise 3](/README.md/#exercise-3-not-so-efficient-editing) and [Exercise 4](/README.md/#exercise-4-slightly-more-efficient-editing) to let participants experience how they can work more efficient using copy/paste.
This file was found on [Imakewebthings' deck.js Github repo][boiler_origin].

[boiler_origin]: https://github.com/imakewebthings/deck.js/blob/master/boilerplate.html "Imakewebthings deck.js"

#### 5-string_calculator_spec.rb

This file was originally used to demonstrate ci" and similar functions.
This file was found on [Katacasts' string_calculator Github repo][string_calc_origin].

[string_calc_origin]: https://github.com/katacasts/string_calculator/blob/master/spec/string_calculator_spec.rb "Katacasts string calculator"

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

[mailme]: mailto:vim@swen.nu "my mailaddress"

### License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Vim workshop</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/aswen/vim-workshop" property="cc:attributionName" rel="cc:attributionURL">Alexander Swen</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/nedap/vim-workshop" rel="dct:source">https://github.com/nedap/vim-workshop</a>. It was created by Alexander Swen & Joël Stemmer for Nedap N.V..

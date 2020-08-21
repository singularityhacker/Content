# Writing on GitHub II

![Writing in GutHub 2](https://i.imgur.com/7q9dp9A.png)

In a [previous post](https://medium.com/@justiceconder/writing-on-github-c35ddd12bfd8), I spoke about moving to GitHub as a technical writing platform. In this post, I will address some of the challenges I faced, methods of resolution, and future goals as I continue down this journey. If you want to know the exact reasons I have made this change, review the previous post.

**Editors**

When I first started down this path, I wasn't accustomed to writing in markdown so the first thing I did is clone some repositories to my local machine and look for a good markdown editor. This is where things got strange. It seems that writing in markdown has become something of a rising trend to the degree that there are several paid editors on the market with some even requiring a subscription. Thankfully I didn't capitulate to these scams and decided to just go all in and use VS Code as my editor. I had to brush up on the interface, staging and committing changes, and package installation. The exercise proved beneficial but one aspect of the workflow I still didn't like was the subpar Grammarly integration. 

By accident, I discovered that editing files directly from within the browser on the GitHub website itself proved sufficient for most things I was doing. After adding a Chrome extension that made editing markdown files even more friendly and realizing that the Grammarly chrome extension worked as well when this extension was enabled, I started to really fall into a daily groove. What's cool is that all my content is still available locally if needed (meaning I can interact with it with any application on my machine) but still conveniently available to be edited within a browser window. It's really the best of both worlds. 

**Organization**

A word on organization. Github projects. 

**Image Management**

Imgur and the upload app

**Presentation**

Hack.md

Awesome slides

A good way to make private content public content.

**The trivium of technical writing**

...

---

**Organization and Collaborative Discussion**

GitHub projects and issues to the rescue. See the issue that tracked my thoughts and notes for this very post here: https://github.com/singularityhacker/Content/issues/2

**A Full Local Setup**

If writing in git is largely about getting to the source of things then it makes sense to get to the source of things in tooling as well. This has been a rocky patch since taking on this experiment. A few things to take into mind:

*   I thought I needed a markdown app to conveniently edit MD files in such a way that the rendered MD would appear next to my typed text. I even almost paid for this as a service.
*   After trying several MD MacOS apps, I was disappointed that Grammarly did not work while using them so I looking at MD editor web solution because Grammarly works in the browser context. This proved to be not ideal because I had to grant the web app access to my GitHub account and atomic commits were weird as the web apps I tried were not clear in when they would since to my repo.

So I've settled into using VS Code for my writing tool.

*   No third-party access to my repo.
*   Unambiguous git interaction.
*   MD extension that permits side by side rendering of MD content.
*   A Grammarly extension.
*   Proximity to the source _and experience_ of things. This includes an ide interface, extension ecosystem, and two birds with one stone in learning a single way to write content and code.
*   Building a second brain with [Foam](https://foambubble.github.io/foam/)

But using VS Code meant brushing up on the following

*   watched basic tutorials on VSCode
*   Learned how to install extensions
*   Learned how to push to github
*   And who to edit/preview MD (cmd+k V)
*   Grammarly removed from the market place. Use the package directly: [https://github.com/znck/grammarly/releases/tag/v0.12.2](https://github.com/znck/grammarly/releases/tag/v0.12.2)

A Minimal Setup in the Browser

**The trivium of technical writing**

Code/Content/Diagrams

See the triangle: diagram/content/code

Not suggesting a curry-Howard correspondence but a meaningful continuum.

We are made for image recognition. The memory master leverage cognitive cathedrals to retain large amounts of information. Even some programming languages are introducing this correspondence: [https://ballerina.io/](https://ballerina.io/)

Content as "wet code" and code as "dry code": [http://unenumerated.blogspot.com/2006/11/wet-code-and-dry.html](http://unenumerated.blogspot.com/2006/11/wet-code-and-dry.html)

Content/code is a continuum, not binary. The code should be self-documenting and content should be precise enough to be formally modeled to some extent.

On the idea that code/content as a continuum:

*   [https://meta.wikimedia.org/wiki/Abstract_Wikipedia/July_2020_announcement](https://meta.wikimedia.org/wiki/Abstract_Wikipedia/July_2020_announcement)
*   [https://www.inklestudios.com/ink/](https://www.inklestudios.com/ink/)
*   [https://en.wikipedia.org/wiki/AI_Dungeon_2](https://en.wikipedia.org/wiki/AI_Dungeon_2)
*   https://beta.openai.com/

On the importance of written communication

*   [Written communication is remote work super power](https://snir.dev/blog/remote-async-communication/)
*   [Why writing matters in remote work](http://www.timcasasola.com/blog/writing)
*   :point\_up\_2: The above post got amplified right on up to [Chris Coyier](https://css-tricks.com/why-does-writing-matter-in-remote-work/)

Notes to touch on:

Some notes on recent pattern changes and advances:

*   Images: imgur image uploader
*   Less is more: Writing through the browser isn't bad
*   Volume: link to word count plugin
*   Top-level project board
*   Private journaling
*   Github actions (entry point of executable content)
*   Github as social network: [https://i.imgur.com/X7mhZ1E.jpg](https://i.imgur.com/X7mhZ1E.jpg)
*   Easier MD writing with [chrome extension](https://github.com/ckeditor/github-writer)
*   The github writer extension above makes Grammarly work!! Woooohooooo!
*   A review of the vision: natural language to format language is a spectrum, not binary.
*   Version control as the single resource of truth. GitOps
*   From don't break the chain to quantified daily contribution with Github actions
*   Don't break the chain on my watch: [https://apps.apple.com/us/app/contributions-for-github/id1153432612](https://apps.apple.com/us/app/contributions-for-github/id1153432612)
*   A big circle from larger complexity to the simplest setup. (In browser editing with the markdown plugin + Grammarly)
*   HackMD.io as a presentation and sharing mechanism
*   How I'm handling images (Imgur + [https://github.com/mileswd/mac2imgur](https://github.com/mileswd/mac2imgur))

Questions I said I would address in my previous post:

*   The details of my new writing setup (The circle)
*   Steps to migrate existing Google docs projects to GitHub ([https://www.buymeacoffee.com/docstomarkdown](https://www.buymeacoffee.com/docstomarkdown))
*   A status report on how things are going (Felt advantages: visibility. Facts confront feelings.)

Tips:

*   Use issues for quick notes and prolonged ideation
*   Migrate issue to document when you're ready to start on the document
*   Use a project board with milestones to maintain a cadence
*   Create your projects at the topmost level of your GitHub so you can use a single cross-cutting kanban board and link issues to any of your repositories.

# Writing on GitHub II

![Writing in GutHub 2](https://i.imgur.com/7q9dp9A.png)

In a [previous post](https://medium.com/@justiceconder/writing-on-github-c35ddd12bfd8), I spoke about moving to GitHub as a technical writing platform. In this post, I will address some of the challenges I faced, methods of resolution, and future goals as I continue down this journey. If you want to know the exact reasons I have made this change, review my [previous post](https://medium.com/@justiceconder/writing-on-github-c35ddd12bfd8).

**Writing Mode**

When I first started down this path, I wasn't accustomed to writing in markdown so the first thing I did is clone some repositories to my local machine and look for a good markdown editor. This is where things got strange. It seems that writing in markdown has become something of a rising trend to the degree that there are several paid editors on the market with some even requiring a subscription. That kind of blew my mind. A subscription text editor? Thankfully, I didn't capitulate and decided to just use [Visual Studio Code](https://code.visualstudio.com/) as my editor. I had to brush up on the IDE interface, staging and committing changes, and package installation. I few things I liked about this setup were

*   No third-party access to my repository
*   Unambiguous git interactions
*   Side-by-side rendering of markdown content
*   A Grammarly extension (removed from the market place but still available [here](https://github.com/znck/grammarly/releases/tag/v0.12.2))
*   Options to use "second/external brain" approaches with things like [Foam](https://foambubble.github.io/foam/)

The exercise proved beneficial but one aspect of the workflow I still really didn't like was the Grammarly integration. By accident, I discovered that editing files directly from within the browser on the GitHub website itself proved sufficient for most things I wanted to do. Talk about going full circle. After adding [GitHub Writer](https://github.com/ckeditor/github-writer), a browser extension that made editing markdown files even more friendly and realizing that the [Grammarly browser extension](https://support.grammarly.com/hc/en-us/articles/115000091552-Install-the-Grammarly-browser-extension) worked as well when this extension was enabled, I started to really fall into a groove. What's cool is that all my content is still available locally if needed (meaning I can interact with it with any application on my machine) but still conveniently available to be edited within a browser window. It's really the best of both worlds.

**Image Management**

Image paths in GitHub repositories can be tricky. While GitHub does offer an [image hosting CDN](https://gist.github.com/vinkla/dca76249ba6b73c5dd66a4e986df4c8d) mechanism, there is no mechanism to view-all-uploaded or [delete images](https://stackoverflow.com/questions/33215211/github-how-do-i-delete-an-attachment-in-github-issues) once uploaded. I didn't want to use dropbox as that entire domain can be blocked on some corporate networks so landed on a slick [Imgur](https://imgur.com/) workflow that handles my local screenshot needs as well. With this [mac app](https://github.com/mileswd/mac2imgur) and an imgur account, you can drag and drop images to be uploaded or just take any screenshot and it will be uploaded to your account and the link copied to your clipboard. 

**Content Presentation**

I'm most frequently working in private repositories but have a need to present content to people who don't have access. This is where [HackMD](https://hackmd.io/) comes in. It allows me to pull in content from a private repo and present it in a slide show way. Any updates to that file in git can be pulled into the HackMD version and it also allows pushing the other direction as well. 

**Workflow and Organization**

*   Use issues for quick notes and prolonged ideation
*   Migrate issue to document when you're ready to start on the document
*   Use a project board with milestones to maintain a cadence
*   Create your projects at the topmost level of your GitHub so you can use a single cross-cutting kanban board and link issues to any of your repositories.

...

---

**Organization and Collaborative Discussion**

GitHub projects and issues to the rescue. See the issue that tracked my thoughts and notes for this very post here: https://github.com/singularityhacker/Content/issues/2

**A Full Local Setup**

If writing in git is largely about getting to the source of things then it makes sense to get to the source of things in tooling as well. This has been a rocky patch since taking on this experiment. 

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
*   A review of the vision: natural language to format language is a spectrum, not binary.
*   Version control as the single resource of truth. GitOps
*   From don't break the chain to quantified daily contribution with Github actions

Questions I said I would address in my previous post:

*   The details of my new writing setup (The circle)

*   Steps to migrate existing Google docs projects to GitHub ([https://www.buymeacoffee.com/docstomarkdown](https://www.buymeacoffee.com/docstomarkdown))
*   Don't break the chain on my watch: [https://apps.apple.com/us/app/contributions-for-github/id1153432612](https://apps.apple.com/us/app/contributions-for-github/id1153432612)

*   A status report on how things are going (Felt advantages: visibility. Facts confront feelings.)

---
date: '2025-02-15T18:42:25+11:00'
draft: false
title: 'Ollama set up and my use cases'
disableShare: true
tags: ["macbook pro", "ollama", "llm"]
---
After I successfully installed Ventura to my old mac (see previous post) I went straight to installing Ollama and trying models.
I have used following youtube tutorial: https://www.youtube.com/watch?v=GWB9ApTPTv4 and I can say it is really good. And Ollama documentation is great as well: https://github.com/ollama/ollama/blob/main/README.md.

So far I tried running llama 3.2 7b and codegemma 7b. After getting used to chat gpt this seems like crazy slow. But, given that I have specific usecases in mind that might still fit me well.



## My use cases

### 1. Bookmarks
A while ago I created a soft that served me as a bookmark manager. 
It had two parts - telegram bot and a web interface. The way how it worked was you send a web url and python would scrape the website for the title and assign tags based on some rules. 
For example if domain name is youtube it assigned "video", if title had words like "python" it assigned "programming" and "python". It used to run on Heroku until it had free tier. And telegram bot used to run on my raspberry pi at home. The database however is cloud monge, so it is the only thing that is alive now. What I would like to do next is create a new version of the bookmarks, and the way how I plan to use LLM is to summarise the content of the page and auto-assign tags. We'll see how it would work. I'll dedicate a separate set of posts under the tag "bookmarx"

### 2. Document retriever
I have quiet a lot of different documents and sometimes I simply forgot were are they and how to find them. Moreover, I sometimes may need only part of the info from that document. For example, I need to run descaling for my coffee machine time to time. And I do not store that info in my head as I know that there is a manual or this info can be googled. But I find google becomes worse nowadays, and sometimes it takes like 10 minutes to find what you want. Or, another example will be my personal documents like visas or emails or flight info. That stuff is buried in the gmail and, unfortunately, my gmail has a lot in it so search finds everything - both the stuff I need and the stuff I don't

### 3. Expenses and budget planner
I've created my own budget planner app and it was quiet good in terms of ability to create different scenarious and so on. The main issue that I found is that without actual expenses it is tough to make any judjements about how you are doing. The reason why I haven't used any solution on the market is lack of trust. Plus I do use multiple banks for different reasons, so having all info in the one place would be neat. So what I tried to do is created a custom CV model that would read the PDFs that my bank exports and put it as a list of transactions. Unfortunately, even within single bank the output of the PDF is not consistent and some adjustments required. I was thinknig on reying a multi-modal llm to try to combat this issue and to have at least all thransactions in a table format for a start.


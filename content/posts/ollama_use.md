---
date: '2025-02-15T18:42:25+11:00'
draft: false
title: 'Ollama set up and my use cases'
disableShare: true
tags: ["macbook pro", "ollama", "llm"]
---
After successfully installing Ventura on my old Mac (see previous post), I went straight to installing Llama and trying out models. I used the following YouTube tutorial: https://www.youtube.com/watch?v=GWB9ApTPTv4, which I found to be really good. The Llama documentation is also great: https://github.com/ollama/ollama/blob/main/README.md.

So far, I have tried running Llama 3.2 7B and CodeGemma 7B. After getting used to Chat GPT, this seems like a significant slowdown. However, given that I have specific use cases in mind, it might still be suitable for me.

## My use cases

### 1. Bookmarks
A while ago, I created software that served as a bookmark manager. It had two parts - a Telegram bot and a web interface. The way it worked was that you would send a web URL, and Python would scrape the website for the title and assign tags based on some rules. For example, if the domain name was YouTube, it assigned "video", or if the title contained words like "Python", it assigned "programming" and "Python". It used to run on Heroku until they discontinued their free tier. The Telegram bot used to run on my Raspberry Pi at home. However, the database is still hosted on Cloud MongoDB, so that's the only part that remains active now. What I would like to do next is create a new version of the bookmarks manager, and I plan to use LLM to summarize the content of each page and auto-assign tags. I'll dedicate a separate series of posts under the tag "bookmarx" to this project.

### 2. Document retriever
I have a large number of different documents, and sometimes I simply forget where they are or how to find them. Moreover, I often only need a specific part of the information from that document. For example, I need to descale my coffee machine periodically, but I don't store that information in my head because I know it's available in the manual or can be found online. However, I've noticed that Google has become less effective lately, and sometimes it takes around 10 minutes to find what I'm looking for. Another example is my personal documents, such as visas, emails, or flight information, which are buried in my Gmail inbox. Unfortunately, my Gmail account contains a lot of unnecessary information, so the search results often include both relevant and irrelevant data.

### 3. Expenses and budget planner
I've created my own budget planner app, which was quite good at allowing me to create different scenarios. However, I found that without actual expense data, it's difficult to make accurate judgments about my financial situation. The reason I haven't used any existing solutions on the market is that I lack trust in them. Additionally, I use multiple banks for different purposes, so having all my information in one place would be convenient. To address this issue, I tried creating a custom CV model that could read the PDFs exported by my bank and convert them into a list of transactions. Unfortunately, even within a single bank, the output of the PDF is not consistent, requiring adjustments to be made. I was thinking of trying a multi-modal LLM to combat this issue and at least get all my transactions in a table format for starters.


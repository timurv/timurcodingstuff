---
date: '2025-03-23T21:22:33+11:00'
draft: false
title: 'Vibe Coding'
disableShare: true
---
A few words about such new trend called "vibe coding". 
On one hand, I am amazed that you can create apps with zero knowledge of programming. 
However, I started programming at the age of 12, so it does look weird to say the least to see people who do not understand what is going on can create something that looks yes, generic but not too bad.
On the other hand, I could not miss the trend and it would be unfair to judge without trying. 
So here are my 2 cents about main tools that started the trend and some alternatives that I've tried and would like to try later.

## Cursor  https://www.cursor.com/
To say that I was impressed is to say nothing. Just chatting to the codebase in plain english is amazing. Like it is your real personal assistant that does what you want and does it instant and good enough. 
On the dowside I found following:
 - it does not know best practices and sometimes can write a bunch of code that is waay worse than it could be. Results are heavy application, incosotent behaviour and so on. My personal example was that I tried to have a little bit more responsive on the client side and t started to suggest adding SWR and ReactQuery to my relatively simple Next JS task manager. In particular, the issue was I had a component that created task and then another component that renders tasks. And I already had actions set up. Simple soltion that I ultimately used is just replacing client component with server component and then simply do reouter.refresh(). If I didn't know it I would have ended up in bloated codebase.
  - another significant thing that I found out was it suddenly became stupid. Like the code that it wrote initially it then re-wrote multiple times, created bugs, tried to fix the bugs and changed more code, added bugs to another code and so on. I would say it became unusable. When I tried to understand what happened, I realised that the issue was it swithced from Claude3.7 to GPT-4o-mini. And yes, I had a trial pro. After that I decided that I do not want to have a pro subscription, at least now.

## Github co-pilot
Chatting is good, but limited to the ChatGPT models. And I did found out that O3-mini, unfortunately significanly worse than Claude. At least it is twice as cheeper. However, I wanted to experience that power of vibe-coding again that Cursor showed me so I switched to alternative instead.

## Alternative
### Cline
So I discoverd that there is an extension to the VS code that is similar to Cursor chat, however it allows to use any model of your choice, including local ones. The extension called Cline https://app.cline.bot/. So I started testing it. Tested local models - nothing good, too slow and inefficient. Moved on to OpenAI 03-mini - it's way better but same as co-pilot. And then I connected Claude 3.7. And oh, boy, the vibe is back. It simply delivers. I don't know what to add. Ah, wait, I know. Prices. 3.7 is expensive. So need to be very mindful about it. And also I would like to add that I really like plan and act modes. So if you have feature you simple plan and discuss implementation and then just click "Act" and boom - the feature is implemented. Amazing. I would say that for me that works even better. It shows the pricing on top, so you know how much you really spend on developing the feature as well. Highly recommend.


### Way forward
At the moment combination of Cline and free tier of co-pilot work for me. However, it would be interesting to test Deepseek models as well. Also, there is another tool called Continue https://www.continue.dev/ which might be a good alternative to Cline. And another interesting project called Aider https://github.com/Aider-AI/aider, however it is designed for terminal. As for autocompletions there is a project called Supermaven https://supermaven.com/ which I might consider as well later.




---
date: '2025-03-17T17:23:04+11:00'
draft: true
title: 'Task managers'
disableShare: true
tags: ["development", "projects", "learning", "task manager"]
---
I like to set up tasks for the week/month/year and it does really help to offload the thoughts and be more productive.
Unfortunatly I am not always consitent about it. And I wish for the system that would help with it. That led me to trying multiple different apps and now I have a long love-hate relationships with task managers.

## What an ideal task manager look like for me?
1. Progress - a lot of task managers once the task is done it just dissapears! Does not bring any joy, really.
2. Multiple buckets for different stuff
3. Analytics! I do love numbers and I would like to see my capacity
4. Multi-platform - has mobile app or at least adjusted for mobile screen, but has a full functionality on desktop
5. Not too complicated, should be easy to add tasks
6. Goals - group tasks for certain goals.
7. *Telegram support - I can just message to add a task

I ended up using Microsoft OneNote as it is multi-platform and allows to add stuff quickly.
I like that I can see the tasks and when I plan for the next week I can just copy-past previous one. And because it is free-format it allows to fine-tune it as you want.
However, it does not have any analytics, and when I did set up a system for a week I have to double check to see how my weekly tasks align with monthly or yearly goals.
Also, at the begining of the week I might have one plan, but sometimes week require adjustments and I ended up with more tasks added later the week. It is alright, but the problem with it that my original tasks are still there and create a sense of stagnation. Therefore, I do not understand, should I plan better, how much should I reserve for additional tasks and, eventually - what is even achiavable?

Another problems that I noticed when planning include following:
 - I want to have a backlog, but too big of a backlog is hard to go through and feels like a burden
 - If the task manager focuses on accomplishement it feels like you need to go 100% which, to be honest, is hard to achieve without cheating. And in my opinion, should not even be the case. Initial plan might not be great and therefore, completion to 100% is dumb. On the other hand, low completion is terrible as well. 

Also some apps might just flush you and your data, but that is a different story...

But hey! I am a developer! I can do stuff! On my own! So lets build the one that I would love! And learn! What can go wrong? :)

## Development
So the first thing as a developer is fugure out the stack. 
I cannot develop natively to the apple or android yet, but I surely can create a web app. 
Ok, if it is a web app, what should I use? Frontend - React possibly? It is the most valued by the market in demand. Backend can be python.
But then - where to deploy, how to authentificate? So I started thinking about the ideal stack. 

### Ideal stack
After watching bunch of youtube videos I found the way to prototype quickly - https://v0.dev/. Brough by vercel, allows to quickly come up with the interface.
And it uses Next JS and Tailwind. Now, I know CSS, learned a bit of Tailwind, but not too proficient. And here where the powers of AI came to rescue me - installed Cursor editor and just went straight into. Deployed to Vercel, added Clark for easy auth, added database, done! 

## Final result
Just couple of days and my first prototype is up and running at https://www.seikou.work/
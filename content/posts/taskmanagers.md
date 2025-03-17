---
date: '2025-03-17T17:23:04+11:00'
draft: false
title: 'Task managers'
disableShare: true
tags: ["development", "projects", "learning", "task manager"]
---
I like to set up tasks for the week, month, or year, and it really helps to offload thoughts and be more productive. Unfortunately, I am not always consistent about it. And I wish for a system that would help with it. This led me to try multiple different apps, and now I have a long love-hate relationship with task managers.

## What an ideal task manager look like for me?
1. Progress - many task managers make the task disappear once it's done! It doesn't bring any joy.
2. Multiple buckets for different tasks
3. Analytics! I do love numbers and would like to see my capacity.
4. Multi-platform - has a mobile app or is at least adjusted for mobile screens, but has full functionality on desktop
5. Not too complicated; it should be easy to add tasks
6. Goals - group tasks for certain goals
7. *Telegram support - I can just message to add a task

I ended up using Microsoft OneNote as it's multi-platform and allows me to add stuff quickly. I like that I can see the tasks, and when I plan for the next week, I can just copy-paste from the previous one. And because it's free-format, it allows fine-tuning as needed. However, it doesn't have any analytics, and when I set up a system for a week, I have to double-check to see how my weekly tasks align with monthly or yearly goals. Also, at the beginning of the week, I might have one plan, but sometimes the week requires adjustments, and I end up adding more tasks later in the week. It's alright, but the problem is that my original tasks are still there and create a sense of stagnation. Therefore, I don't understand - should I plan better? How much should I reserve for additional tasks? And what's even achievable?

Another problem I noticed when planning includes:
- I want to have a backlog, but too big of a backlog is hard to go through and feels like a burden
- If the task manager focuses on accomplishment, it feels like you need to achieve 100%, which is hard without cheating. In my opinion, this shouldn't even be the case. The initial plan might not be great, so completion to 100% seems unnecessary. On the other hand, low completion is terrible as well.

Also, some apps might just flush your data, but that's a different story...

But hey! I'm a developer! I can do stuff on my own! So let's build one that I would love and learn from. What could go wrong? :)

## Development
So the first thing as a developer is to figure out the stack. I cannot develop natively for Apple or Android yet, but I can create a web app. If it's a web app, what should I use? Frontend - possibly React? It's in high demand. Backend could be Python. But then - where to deploy and how to authenticate? So I started thinking about the ideal stack.

### Ideal stack
After watching a bunch of YouTube videos, I found a way to prototype quickly using https://v0.dev/, brought by Vercel, which allows for quick interface creation. It uses Next JS and Tailwind. Now, I know CSS and have learned a bit of Tailwind, but I'm not too proficient. Here's where the power of AI came to rescue me - I installed the Cursor editor and went straight into it. Deployed to Vercel, added Clark for easy auth, added a database, done!

## Final result
Just a couple of days in, and my first prototype is up and running at https://www.seikou.work/
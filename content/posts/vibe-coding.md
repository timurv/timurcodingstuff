---
date: '2025-03-23T21:22:33+11:00'
draft: false
title: 'Vibe Coding'
disableShare: true
---
A few words about the new trend called "vibe coding". 
On one hand, I'm amazed that you can create apps with zero knowledge of programming. 
However, having started programming at the age of 12, it seems weird to see people who don't understand what's going on creating something that looks generic but not too bad.
On the other hand, I couldn't miss out on this trend and it would be unfair to judge without trying. 
So here are my thoughts on the main tools that started the trend and some alternatives that I've tried or plan to try later.

## Cursor  https://www.cursor.com/
To say that I was impressed is an understatement. Simply chatting with the codebase in plain English is amazing, like having a real personal assistant that does what you want instantly and well enough. 
However, I found some downsides:
 - it lacks knowledge of best practices and sometimes writes suboptimal code, resulting in heavy applications and inconsistent behavior. My personal example was trying to make a client-side task manager more responsive; Cursor suggested adding SWR and ReactQuery, which would have bloated the codebase. A simpler solution was to replace the client component with a server component and use `router.refresh()`. If I hadn't known this, I would have ended up with unnecessary complexity.
 - another significant issue I encountered was that it suddenly became unreliable. The code it initially wrote was rewritten multiple times, introducing bugs and attempting to fix them, which added more bugs to other parts of the code. I realized that the problem occurred when it switched from Claude 3.7 to GPT-4o-mini. Since I had a trial pro subscription at the time, I decided not to continue with a paid subscription.

## Github Co-Pilot
While chatting is useful, it's limited to ChatGPT models. Unfortunately, O3-mini is significantly worse than Claude, although it's twice as cheap. However, I wanted to experience the power of vibe-coding again that Cursor showed me, so I switched to an alternative instead.

## Alternative
### Cline
I discovered a VS Code extension called Cline (https://app.cline.bot/), which allows using any model of your choice, including local ones. I started testing it with local models, but they were too slow and inefficient. Moving on to OpenAI 03-mini was an improvement, but it's similar to Co-Pilot. When I connected Claude 3.7, the vibe was back - it simply delivers. One thing to note is that 3.7 is expensive, so you need to be mindful of costs. I also appreciate the plan and act modes; if you have a feature in mind, you can plan and discuss implementation, then click "Act" and see it implemented. This works even better for me, as it shows pricing estimates on top.

### Way Forward
Currently, combining Cline with the free tier of Co-Pilot works for me. However, I'm interested in testing Deepseek models as well. Another tool called Continue (https://www.continue.dev/) might be a good alternative to Cline. There's also an interesting project called Aider (https://github.com/Aider-AI/aider), although it's designed for terminal use. For autocompletions, I might consider Supermaven (https://supermaven.com/) later.




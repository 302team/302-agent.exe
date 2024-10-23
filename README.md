Presenting **Agent.exe**: the easiest way to let Claude's new [computer use](https://www.anthropic.com/news/3-5-models-and-computer-use) capabilities take over your computer!

<img width="374" alt="agent-exe" src="https://github.com/user-attachments/assets/26410465-bd70-4c02-89e5-26766de73f68">

https://github.com/user-attachments/assets/c544f7a5-7575-400f-891c-27279c4a2f96

### Motivation

I wanted to see how good Claude's new [computer use](https://www.anthropic.com/news/3-5-models-and-computer-use) APIs were, and the default project they provided felt too heavyweight. This is a simple Electron app that lets Claude 3.5 Sonnet control your local computer directly. I was planning on adding a "semi-auto" mode where the user has to confirm each action before it executes, but each step is so slow I found that wasn't necessary and if the model is getting confused you can easily just hit the "stop" button to end the run.

### Getting started

1.  `git clone https://github.com/corbt/agent.exe`
2.  `cd agent.exe`
3.  `npm install`
4.  `ANTHROPIC_API_KEY="<your-anthropic-api-key>" npm start`
5.  Prompt the model to do something interesting on your computer!

### Supported systems

- MacOS
- Theoretically Windows and Linux since all the deps are cross-platform

### Known limitations

- Only works on the primary display
- Lets an AI completely take over your computer
- Oh jeez, probably lots of other stuff too

### Tips

- Claude _really_ likes Firefox. It will use other browsers if it absolutely has to, but will behave so much better if you just install Firefox and let it go to its happy place.

### Roadmap

- I literally wrote this in 6 hours, probably isn't going anywhere. But I will review PRs and merge them if they seem cool.

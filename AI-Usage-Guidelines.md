# AI Usage Guidelines

## Research & Learn

**AI tools I use**
Claude Code and Cursor.

**Benefits and risks**
- Benefits: AI speeds up work, and it's great for ideas: where to look and how to approach something.
- Risk: AI can give a wrong answer and present it as correct. It sounds confident either way, which makes it easy to trust by mistake.

**What should never go into AI tools**
- API keys, passwords, tokens and other secrets.
- Confidential company information and user data.
- Private data from services like Supabase (database contents, service keys).

The best protection is to keep secrets out of the AI's reach in the first place: keep them in `.env` files that are not committed, and configure the tools so the AI can't read those files at all (for example by excluding them in the tool's settings).

**How to fact-check AI output**
- Read and test any code the AI writes before using it.
- Compare the answer with official documentation.
- Look for a second source, for example expert videos on YouTube, which often include more context and real opinions.

## Reflection

**When do I use AI, and when do I rely on my own skills?**
I use AI to explain how to do something and when I need inspiration. I do the thinking myself for architecture and for anything sensitive, such as how to handle data for an API (OpenRouter), Supabase and edge functions.

**How do I avoid over-reliance on AI?**
I always check the code that AI writes and I think critically about what it says. Autonomy is nice, but verification is mandatory.

**What steps will I take to protect data privacy?**
Keep keys and passwords out of anything the AI can read, and make sure secrets never end up in prompts or in the repository.

## Task

**A task I improved with AI**
Searching for information and doing quick everyday tasks became faster for me. For my project AutoCore I use AI for inspiration on where to take the design next, so I don't make mistakes and can build something really good.

**Did the output need editing or fact-checking?**
Yes, always. Even when the AI works autonomously, the result needs to be checked.

## Best practices I will follow at Focus Bear

1. **Verify everything.** Check all AI output, no exceptions. This is a habit, and it doesn't go away when the model gets better at reasoning.
2. **Cross-check with experts.** Ask on YouTube too, because videos usually have more valuable information and expert opinions.

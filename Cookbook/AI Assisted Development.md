# AI Assisted Development

*Источник: https://docs.rpg-architect.com/03-cookbook/03-ai-assisted-development/*

---

# AI Assisted Development

## **AI Assisted Development**[¶](#ai-assisted-development "Permanent link")

RPG Architect supports working alongside AI coding assistants to help you understand and write scripts more comfortably. This page explains what's available, how to set it up, and — just as importantly — what these tools are and aren't meant for.

## **What This Is — and Isn't**[¶](#what-this-is-and-isnt "Permanent link")

RPG Architect is built around scripting, and scripting can have a learning curve. The goal of AI-assisted development support is to lower that curve — to help you understand what commands exist, how they fit together, and how to express what you're trying to build. It is **not** here to write your game for you, and it's not a replacement for understanding what your scripts actually do.

This is aimed at the artistically-inclined developer who knows what they want their game to feel like but doesn't want to spend a week reading reference docs to figure out how to gate a door behind a switch. Think of it as a knowledgeable assistant sitting next to you while you work — one that can answer questions about RPG Architect's scripting system, suggest commands, and help you debug a script that isn't behaving.

**It is 100% optional.** Nothing in RPG Architect requires you to use AI tools. If you'd rather learn the scripting system the traditional way — through the documentation, examples, and trial and error — that path is fully supported and always will be.

## **What's Provided**[¶](#whats-provided "Permanent link")

We maintain a small collection of **Skills** — bundles of project-specific knowledge that teach an AI assistant how RPG Architect's scripting system works. The current skills cover areas such as scripting reference, command lookup, and writing/reviewing scripts. They are designed to give the assistant accurate, up-to-date context about the engine so its suggestions stay grounded in how RPG Architect actually behaves rather than in guesswork.

Skills are distributed as a single zip file you can download and install into a compatible AI assistant.

[Download user-skills.zip](user-skills.zip)

## **Compatible AI Assistants**[¶](#compatible-ai-assistants "Permanent link")

Skills are a feature of [Claude Code](https://docs.claude.com/en/docs/claude-code/overview) and the Claude Agent SDK from Anthropic. They work out of the box with Claude Code with no additional setup beyond installing the skills themselves.

Other AI coding assistants — such as Cursor, GitHub Copilot, and similar tools — use their own context formats and are not directly compatible with the skill bundle. The underlying _idea_ (giving an AI project-specific knowledge about RPG Architect) is portable, but you'd need to adapt the contents of the skills into whatever format your tool of choice supports. We don't currently maintain bundles for those tools.

## **Setting Up Claude Code**[¶](#setting-up-claude-code "Permanent link")

If you don't already have Claude Code installed:

1.  Visit the [Claude Code documentation](https://docs.claude.com/en/docs/claude-code/overview) and follow the installation instructions for your operating system.
2.  Sign in with your Anthropic account when prompted.
3.  Verify it works by opening a terminal in any directory and running `claude`.

## **Installing the Skills**[¶](#installing-the-skills "Permanent link")

1.  Download [user-skills.zip](user-skills.zip) using the link above.
2.  Extract the contents into your Claude Code skills directory:
    *   **Windows**: `%USERPROFILE%\.claude\skills\`
    *   **macOS / Linux**: `~/.claude/skills/`
3.  Restart Claude Code if it's already running.
4.  The skills will be available the next time you start a session in your RPG Architect project directory.

## **Using the Skills**[¶](#using-the-skills "Permanent link")

Once installed, you can simply ask the assistant questions about RPG Architect scripting in plain language — for example, _"how do I make an NPC only appear after the player has talked to the king?"_ or _"what's the difference between a global switch and a local switch?"_. The assistant will draw on the installed skills to give grounded, RPG Architect-specific answers.

You can also ask it to write or review scripts, explain what an existing script does, or help you debug behavior that isn't working as expected. As always, **you should review anything the assistant writes before using it in your project** — it's an aid, not an authority.

## **Updating Skills**[¶](#updating-skills "Permanent link")

The skills bundle on this page is updated periodically as RPG Architect's scripting system grows. To update, simply download the latest `user-skills.zip`, extract it over your existing skills directory, and restart Claude Code.
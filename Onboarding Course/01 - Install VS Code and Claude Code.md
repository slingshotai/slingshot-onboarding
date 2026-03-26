# Module 1: Install VS Code & Claude Code

## What We're Doing

VS Code is your workspace — a free code editor from Microsoft that works on every platform. Claude Code is Anthropic's AI assistant that runs inside it. Together, they're the engine that powers every SlingshotAI skill.

You don't need to know how to code. VS Code is just the container that Claude Code lives in.

## Watch the Video

> **Video:** [Setting up VS Code & Claude Code] *(link to walkthrough video)*
>
> Matt walks through the full setup on a clean machine — every click, every step. **Watch this first**, then follow the steps below. The video covers exactly what you'll see on screen.

## Step-by-Step Setup

This is the one module where you need to follow manual steps — because Claude can't help you until it's installed. After this, Claude does the heavy lifting for everything else.

### 1. Install VS Code

1. Go to **code.visualstudio.com**
2. Click the download button (it detects your operating system automatically)
3. **Mac:** Open the downloaded zip, drag Visual Studio Code into your Applications folder
4. **Windows:** Run the installer and follow the prompts
5. Launch VS Code

### 2. Install the Claude Code Extension

1. In VS Code, press **Cmd+Shift+X** (Mac) or **Ctrl+Shift+X** (Windows) to open Extensions
2. Type **"Claude Code"** in the search box
3. Find the one by **Anthropic** (it has millions of installs)
4. Click **Install**
5. If nothing seems to change, press **Cmd+Shift+P**, type "reload window", and hit Enter

### 3. Sign Up for Anthropic (If You Haven't Already)

Claude Code needs a paid Anthropic subscription. You need one of:
- **Claude Pro** ($20/month) — this is what most people start with
- **Claude Max** ($100/month) — more usage if you're running skills all day

To sign up:
1. Go to **claude.ai**
2. Create an account (email or Google sign-in)
3. Go to Settings and upgrade to Pro (or Max)

### 4. Install the CLI (Your First Terminal Moment)

Two quick definitions:

- **CLI** (Command Line Interface) — a way of talking to your computer by typing commands instead of clicking buttons. You know how you click an icon to open an app? The CLI lets you do the same thing by typing a command instead.
- **Terminal** — the place where you type those commands. It's built right into VS Code.

This step is optional but recommended. The extension works on its own, but the CLI is useful for some skills and gives you a reason to meet the terminal.

1. In VS Code, open the terminal: **Ctrl+`** (backtick) or **View → Terminal**
2. Copy and paste this command, then press Enter:

```
curl -fsSL https://claude.ai/install.sh | bash
```

3. Wait for it to finish — you'll see some text scroll by, then a success message
4. While you're in the terminal, type `claude` and press Enter — this triggers a login flow in your browser (same as the extension login). Sign in and click Allow.

**Why log in twice?** The VS Code extension and the CLI are like two doors into the same room — they share your conversation history and settings, but each needs its own login. This is a one-time setup.

That's it. You've just installed software and authenticated it using the terminal. When you see instructions that say "run this command" in later modules, this is where you do it — the terminal panel at the bottom of VS Code.

### 5. Connect Claude Code to Your Account

1. In VS Code, open any file (or create a new one — doesn't matter what)
2. Look for the **spark icon** (a small star/sparkle) in the **top-right corner** of the editor
3. Click it — Claude Code opens in a panel
4. First time: it opens your browser to sign in. Log in to your Anthropic account and click Allow
5. Return to VS Code — you should see the Claude Code chat panel

**Alternative:** Click **"Spark Claude Code"** in the bottom-right status bar, or press **Cmd+Shift+P** and type "Claude Code"

## What You Should See When It's Working

- VS Code is open
- The Claude Code panel is visible (a chat interface on the right or bottom)
- There's a text input at the bottom where you can type messages

## Test It

Type this into the Claude Code chat panel:

```
What's 2 + 2? And while you're at it, what day is it today?
```

If Claude answers both questions — congratulations. You've got Claude Code running. From this point on, Claude can help you with everything else.

## Common Issues

| Problem | What to do |
|---|---|
| "VS Code won't install" | Check you have enough disk space and the right version for your OS |
| "I can't find the Claude Code extension" | Search for "Claude" in the Extensions panel (Cmd+Shift+X). Make sure you're on VS Code 1.98 or higher. |
| "The spark icon isn't visible" | You need to have a file open. Try creating a new file first (Cmd+N). |
| "It's asking me to sign in" | You need an Anthropic account with a Pro or Max subscription at claude.ai |
| "Nothing happens when I type" | Make sure you're typing in the Claude Code chat panel, not the regular VS Code editor |
| "I got an error" | Try pressing Cmd+Shift+P → "reload window". If that doesn't work, close and reopen VS Code. |

## Done?

You've got your workspace set up. VS Code + Claude Code is the foundation for everything in SlingshotAI.

From this point on, you can ask Claude for help with anything. Stuck on a step in a future module? Just type your question in the Claude Code panel.

---

[[00 - Welcome|← Welcome]] | [[02 - Install and Set Up Obsidian|Next → Install & Set Up Obsidian]]

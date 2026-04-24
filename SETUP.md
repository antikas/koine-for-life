# Setting up Koine for Life

Ten minutes, no code, no terminal.

## What you need

- A computer running Windows or macOS.
- A Claude account. A paid plan is recommended (Pro or above). The free tier will work for casual use but you will hit limits quickly.
- This pack folder, unzipped somewhere you can find again. A good home is `Documents/koine-for-life/` on Windows, or `~/Documents/koine-for-life/` on Mac.

Decide where the pack lives before you start. Moving it later means redoing this step.

## Pick your interface

Three options. The first is the recommended default.

### Option 1. Claude Desktop (recommended)

Claude Desktop is a free app from Anthropic. It can read and write files on your computer, which is how the pack remembers things between conversations. This is the whole point.

Follow the Claude Desktop setup below.

### Option 2. Claude.ai in a web browser

Works without installing anything. The trade-off is that Claude cannot read or write files on your computer directly. You will need to paste state files into conversations and paste updates back out. Fine for trying the pack, awkward for daily use.

If you pick this, skip to "Using the pack without Desktop" at the end.

### Option 3. Claude Code

If you are a developer and already using Claude Code, point it at the pack folder and use it as your working directory. No other setup required.

## Claude Desktop setup

### Step 1. Install Claude Desktop

Download from [claude.ai/download](https://claude.ai/download). Install, sign in with your Claude account, open it once.

### Step 2. Enable the Filesystem extension

Open Settings. On Windows, click your name in the bottom-left, then Settings. On macOS, use the menu bar: Claude → Settings (or Cmd+,).

In Settings, go to **Extensions** (under "Desktop app" in the left sidebar), then click **Filesystem**.

Make sure it is **Enabled** (toggle on). If it is not installed, install it first (one click).

### Step 3. Add the pack folder

Still on the Filesystem extension screen, look for **Allowed Directories**. Click **Add directory** and select the folder where you unzipped this pack (for example `Documents/koine-for-life/`).

Click **Save**.

That is the whole setup.

### Step 4. Test it

Open a new conversation in Claude Desktop and type:

> Read the file GETTING-STARTED.md from my koine-for-life pack and tell me what it says.

If Claude reads the file and answers, you are set. If Claude says it cannot access the folder, go back to Step 3 and make sure you added the exact folder and saved.

### Step 5. Start the pack

Once the test works, type:

> Run me first.

That triggers the opening interview. Set aside twenty minutes. One conversation, you and the pack, getting to know each other.

After that, everything else opens with natural language. Check `README.md` for the list of phrases.

## Using the pack without Desktop

If you are on the web version of Claude.ai, or using something else that cannot read files directly, you can still use the pack, with one extra step each time.

When you want to use a skill:

1. Open the relevant skill file in your pack folder (for example, `pack/domains/finances/skills/check-in.md`).
2. Copy its contents and paste into Claude, saying: *"Use this skill with me. My relevant state is pasted below."*
3. Also paste the relevant state file (e.g. `pack/domains/finances/state.md`).
4. Work through the conversation.
5. At the end, Claude will tell you what to update in the state file. Copy it back in manually.

Clunky. Mostly for trying the pack before committing to Desktop.

## If you get stuck

Read `PRIVACY.md` if you are unsure what the pack sends where.

Read `GETTING-STARTED.md` for a plain-English overview of how the pack works.

The commonest cause of trouble is the wrong folder path in Step 3. Double-check the path and save again.

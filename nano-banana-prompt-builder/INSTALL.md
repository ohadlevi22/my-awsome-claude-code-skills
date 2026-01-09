# Installing the Nano Banana Prompt Builder Skill

This skill helps you build professional image generation prompts for Nano Banana through an interactive Q&A process. No API key needed - it outputs copy-paste ready prompts.

---

## Option 1: Claude Code (CLI)

### Method A: Local Installation (Recommended)

1. **Create the skills directory** (if it doesn't exist):
   ```bash
   mkdir -p ~/.claude/skills
   ```

2. **Copy the skill folder**:
   ```bash
   cp -r "nano-banana-prompt-builder" ~/.claude/skills/
   ```

3. **Verify installation**:
   ```bash
   ls ~/.claude/skills/nano-banana-prompt-builder/
   # Should show: SKILL.md
   ```

4. **Use in Claude Code**:
   ```
   /skill nano-banana-prompt-builder
   ```
   Or just describe what you want and Claude will find the skill automatically.

### Method B: Project-Specific Installation

If you want the skill only for a specific project:

1. **Create `.claude/skills` in your project**:
   ```bash
   mkdir -p .claude/skills
   ```

2. **Copy the skill**:
   ```bash
   cp -r "nano-banana-prompt-builder" .claude/skills/
   ```

3. **The skill is now available** when working in that project directory.

---

## Option 2: Claude Desktop App

### Step-by-Step Installation

1. **Open Claude Desktop** (claude.ai desktop app)

2. **Go to Settings**:
   - Click the menu icon (top left or ⌘+,)
   - Select "Settings" or "Preferences"

3. **Navigate to Skills**:
   - Find the "Skills" or "Agent Skills" section
   - Click "Add Skill" or "Upload Skill"

4. **Upload the skill**:
   - Click "Upload" or "Import"
   - Navigate to the `nano-banana-prompt-builder` folder
   - Select `SKILL.md`
   - Click "Open" or "Import"

5. **Confirm installation**:
   - The skill should now appear in your skills list
   - You can enable/disable it per conversation

### Alternative: Project-Based Skills

If you use Claude Projects:

1. **Open or create a Project**
2. **Go to Project Settings**
3. **Add to "Project Knowledge"** or "Skills"
4. **Upload SKILL.md**
5. **The skill is now available** in that project

---

## Option 3: Claude.ai (Web)

For Claude.ai web interface (Pro/Team/Enterprise users):

1. **Go to** [claude.ai](https://claude.ai)

2. **Create or open a Project** (left sidebar)

3. **Click "Add Content"** in project settings

4. **Upload SKILL.md** as project knowledge

5. **Start a conversation** in that project - the skill is now active

---

## Verifying It Works

After installation, test the skill:

1. **Start a new conversation**

2. **Say something like**:
   > "I have a photo of my kids and want to create an image of them as superheroes"

3. **Claude should**:
   - Recognize this as an image prompt building task
   - Start asking you questions about scene, lighting, style, etc.
   - Build a professional prompt step by step
   - Output a copy-paste ready prompt for Nano Banana

---

## File Locations Summary

| Platform | Location |
|----------|----------|
| **Claude Code (global)** | `~/.claude/skills/nano-banana-prompt-builder/SKILL.md` |
| **Claude Code (project)** | `./.claude/skills/nano-banana-prompt-builder/SKILL.md` |
| **Claude Desktop** | Uploaded via Settings → Skills |
| **Claude.ai Web** | Project → Add Content → Upload |

---

## Troubleshooting

### Skill not being detected

- Ensure the file is named exactly `SKILL.md`
- Check the folder structure is correct
- Restart Claude Code or refresh Claude Desktop

### Skill not triggering automatically

Say explicitly:
> "Use the nano-banana-prompt-builder skill to help me create an image prompt"

Or in Claude Code:
```
/skill nano-banana-prompt-builder
```

### Permission errors (Claude Code)

```bash
chmod -R 755 ~/.claude/skills/nano-banana-prompt-builder
```

---

## Usage Tips

1. **Have your reference photo ready** - Upload it to Google AI Studio / Nano Banana before starting

2. **Be open to suggestions** - The skill will offer options for lighting, composition, etc.

3. **Iterate freely** - After getting the prompt, paste the result into Nano Banana. If you want changes, come back and refine

4. **Copy the code block** - The final prompt is always in a code block for easy copying

---

## Updating the Skill

To update to a newer version:

1. **Claude Code**: Replace the files in `~/.claude/skills/nano-banana-prompt-builder/`
2. **Claude Desktop**: Delete and re-upload
3. **Claude.ai Web**: Remove from project knowledge and re-add

---

*Skill created: January 2026*

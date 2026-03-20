# Homestead Planner — Session Process

## How to start a new Claude session

Paste this as your opening message in a new Claude chat:

---

Here is the master context document for the Homestead Planner:
https://raw.githubusercontent.com/anthonypfeifer1/homestead-planner/main/homestead_planner.txt

Please read it and confirm you have the full context. This is the master spec document. Let's continue from the Session 14 start target.

---

Claude will fetch the document, confirm it has read it, and pick up from where the last session left off. The Session start target is always recorded at the bottom of Section 21 in the document.

---

## After each Claude session — update the document

**Step 1 — Download the new .docx from Claude**
- At the end of each session Claude presents a final .docx file
- Download it

**Step 2 — Convert .docx to .txt via Google Docs**
- Go to drive.google.com
- Click + New → File upload → select the new .docx
- Right-click the uploaded file → Open with → Google Docs
- File → Download → Plain Text (.txt)
- Save as `homestead_planner.txt`
- Drop it into `C:\Users\antho\OneDrive\Desktop\homestead-planner` replacing the old file

**Step 3 — Push to GitHub**
Open Git Bash and type these three commands manually (do not paste — causes errors):

```
cd ~/OneDrive/Desktop/homestead-planner
git add .
git commit -m "Session 14 updates"
git push origin main
```

Replace "Session 14" with the current session number.

**Step 4 — Verify**
Check that the file updated at:
https://github.com/anthonypfeifer1/homestead-planner

---

## Important notes

- Always type Git Bash commands manually — do not copy/paste (causes bracket paste errors)
- The raw URL never changes — Claude always fetches the latest version
- Keep the homestead-planner folder on your local C: drive / OneDrive, not an external drive
- Your GitHub username: anthonypfeifer1
- Repository: https://github.com/anthonypfeifer1/homestead-planner
- Raw file URL: https://raw.githubusercontent.com/anthonypfeifer1/homestead-planner/main/homestead_planner.txt

---

## Git Bash location

Git Bash is installed on your Windows machine. Search for "Git Bash" in the Start menu.

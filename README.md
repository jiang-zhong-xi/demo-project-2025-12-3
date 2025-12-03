# 🚀 Continue Hub Demo Repo

Welcome to the **Continue Hub Sample Repo** 👋  
Fork this repo, connect Continue to GitHub, and run your first agent in under 5 minutes.  

👉 [Learn about agents](https://docs.continue.dev/hub/agents/intro)  
👉 [Go to the Hub](https://hub.continue.dev/agents)

---

## 🧪 What You’ll Do

- Fix a bug automatically
- Clean up a messy codebase
- Run a security check
- Generate tests
- Document functions
- (Optional) Add a small feature

Each of these is powered by a **Continue Agent** — no setup required. Just fork, connect, and run a prompt.

---

## 🪄 How to Get Started

1. **Fork** this repo to your GitHub account   
2. **Open Mission Control in the Continue Hub:** [hub.continue.dev](https://hub.continue.dev/agents)   
3. **[Connect GitHub](https://hub.continue.dev/settings/integrations)**   
4. Run any of the prompts from [`agents.md`](./agents.md)

👉 In under 60 seconds, you’ll have a PR with code changes.

## Installation

To install the project, run the following command:

```bash
npm install
```

To install the CLI tool, run the following command:

```bash
npm install -g demo-project-2025-12-3
```

## Usage Examples

### Basic Command

```bash
demo-project-2025-12-3 --help
```

Output:

```
Usage: demo-project-2025-12-3 [options]

Options:
  -v, --version  output the version number
  -h, --help     display help for command
```

### Run a Specific Agent

```bash
demo-project-2025-12-3 run-agent --name bug-fix
```

Output:

```
Running bug-fix agent...
Agent completed successfully
```

### Check Agent Status

```bash
demo-project-2025-12-3 status
```

Output:

```
Agent Status:
- bug-fix: completed
- code-cleanup: pending
- security-check: pending
```

## API Reference

### Commands

| Command | Description | Options |
|---------|-------------|---------|
| `run-agent` | Run a specific agent | `--name <agent-name>` |
| `status` | Check agent status | None |
| `list-agents` | List all available agents | None |

### Configuration

To configure the CLI tool, create a `.demo-project-2025-12-3rc` file in your project root with the following options:

```json
{
  "defaultAgent": "bug-fix",
  "autoUpdate": true,
  "logLevel": "info"
}
```

Available configuration options:

- `defaultAgent`: Set the default agent to run
- `autoUpdate`: Enable automatic updates (true/false)
- `logLevel`: Set logging level (info, debug, error)

### Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `CONTINUE_API_KEY` | API key for Continue Hub | None |
| `GITHUB_TOKEN` | Token for GitHub integration | None |
| `DEBUG_MODE` | Enable debug logging | false |

### Troubleshooting

Common issues and solutions:

1. **Agent not running**:
   - Check if the agent name is correct
   - Verify your API key is valid
   - Ensure you have proper GitHub permissions

2. **Configuration not loading**:
   - Verify the `.demo-project-2025-12-3rc` file is in your project root
   - Check for JSON syntax errors
   - Ensure file permissions are correct

3. **Dependency issues**:
   - Run `npm install` to ensure all dependencies are installed
   - Check for version compatibility

### Version Compatibility

| CLI Version | Compatible Node.js Version | Notes |
|-------------|--------------------------|-------|
| 1.0.x | 14.x - 18.x | LTS recommended |
| 1.1.x | 16.x - 20.x | Latest features |

For the most up-to-date information, check the [GitHub releases page](https://github.com/continuedev/continue/releases).

---

## 🧰 Recommended agents

| # | Task                    | Prompt Example                                                                                   | Expected Outcome                                     |
|---|--------------------------|---------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| 1 | Fix a bug                | `Fix the TypeError in api/users.ts`                                                               | A PR fixing the bug and passing tests               |
| 2 | Clean up code            | `Clean up the repo according to ESLint and Prettier rules`                                       | Consistent code formatting, unused imports removed  |
| 3 | Run security check      | `Find and fix vulnerabilities in dependencies`                                                   | Dependency updated and lockfile regenerated         |
| 4 | Write tests              | `Write unit tests for src/utils/math.ts`                                                          | PR with Jest tests                                 |
| 5 | Add docstrings           | `Add JSDoc comments to all functions in src/helpers/`                                            | Code updated with clear docstrings                 |
| 6 | (Optional) Add feature   | `Add a new feature: Mark all todos as completed` (requires editing TodoApp example)              | PR with working feature, tests, and docs           |

---

## 🧠 Tips

- Keep the repo as-is. Let the workflow do the work.
- Check the PR tab after running a workflow.
- Try combining prompts: e.g., “Fix the bug and add a unit test.”

---

## 🏆 Bonus Challenge (Optional)

After you’ve tested the basics:
- Add a new file with a small bug.
- Write your own custom rule in Continue Hub.
- Automate fixing it with your own workflow.

---

## 💬 Feedback

We’d love to hear what worked for you (and what didn’t).  
Open a [discussion](https://github.com/continuedev/continue/discussions).

---

Made with ❤️ by the Continue Team

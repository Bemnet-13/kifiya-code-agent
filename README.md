# Kifiya Code Agent CLI

The **Kifiya Code Agent CLI** is a command-line AI workflow tool that connects to your tools, understands your code, and accelerates your development workflows.

With the Kifiya Code Agent CLI you can:

- Query and edit large codebases, even beyond a 1M token context window.
- Generate new apps from PDFs or sketches using advanced multimodal capabilities.
- Automate operational tasks such as querying pull requests or handling complex rebases.
- Connect new capabilities via tools and MCP servers, including [media generation with Imagen, Veo, or Lyria](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/tree/main/experiments/mcp-genmedia).
- Ground your queries with the integrated [Google Search](https://ai.google.dev/gemini-api/docs/grounding) tool.

---

## 🚀 Quickstart

1. **Prerequisites:**  
   Ensure you have [Node.js version 18](https://nodejs.org/en/download) or higher installed.

2. **Run the CLI:**  
   Use one of the following methods in your terminal:

   **Using npx:**

   **Or, install globally:**
   ```bash
   npm install -g kifiya-code-agent
   code-agent
   ```

3. **Pick a color theme** when prompted.

4. **Authenticate:**  
   Sign in with your personal Google account when prompted. This provides up to 60 model requests per minute and 1,000 per day.

You're now ready to use the Kifiya Code Agent CLI!

---

### 🔑 For advanced use or higher request limits

If you need to use a specific model or require more requests, use an API key:

1. Generate a key from [Google AI Studio](https://aistudio.google.com/apikey).
2. Set it as an environment variable (replace `YOUR_API_KEY`):

   ```bash
   export GEMINI_API_KEY="YOUR_API_KEY"
   ```

For additional authentication options (including Google Workspace), see the [authentication guide](./docs/cli/authentication.md).

---

## 💡 Examples

Once the CLI is running, interact with the Kifiya Code Agent right from your shell.

**Start a project in a new directory:**
```sh
cd new-project/
kifiya-code
> Write me a Discord bot that answers questions using a FAQ.md file I will provide
```

**Work with an existing project:**
```sh
git clone https://github.com/your-org/kifiya-code-agent
cd kifiya-code-agent
kifiya-code
> Give me a summary of all the changes from yesterday
```

---

## 📚 Next Steps

- Learn how to [contribute or build from source](./CONTRIBUTING.md).
- Explore available **[CLI Commands](./docs/cli/commands.md)**.
- For troubleshooting, see the **[Troubleshooting guide](./docs/troubleshooting.md)**.
- For comprehensive documentation, see the [full documentation](./docs/index.md).
- Check out some [popular tasks](#popular-tasks) for inspiration.

---

## 🛠 Troubleshooting

If you encounter issues, consult the [troubleshooting guide](docs/troubleshooting.md).

---

## ⭐ Popular Tasks

### Explore a new codebase

Navigate to your repository directory and run the CLI:

```sh
cd my-repo/
kifiya-code
> Describe the main pieces of this system's architecture.
> What security mechanisms are in place?
```

### Work with your existing code

```text
> Implement a first draft for GitHub issue #123.
> Help me migrate this codebase to the latest version of Java. Start with a plan.
```

### Automate your workflows

Integrate system tools and collaboration suites via MCP servers:

```text
> Make me a slide deck showing the git history from the last 7 days, grouped by feature and team member.
> Make a full-screen web app for a wall display to show our most interacted-with GitHub issues.
```

### Interact with your system

```text
> Convert all the images in this directory to png, and rename them to use dates from the EXIF data.
> Organize my PDF invoices by month of expenditure.
```

---

## 📄 Terms of Service and Privacy Notice

See the [Terms of Service and Privacy Notice](./docs/tos-privacy.md) for details on using Kifiya Code Agent CLI.

# Privacy Policy for CLI Share

CLI Share ("we," "us," or "our") is an open-source tool. This Privacy Policy explains how we handle data.

## 1. Local-first design
CLI Share is a local-first tool. We **do not collect, store, or transmit** your terminal logs, GitHub tokens, or conversation content to our own servers.

## 2. GitHub Authentication
To use the sharing feature, you must provide a GitHub Personal Access Token.
- **Local Storage**: This token is stored exclusively on your local machine in `~/.cli-share/config.json`.
- **Encryption/Protection**: The file is protected with `600` permissions (restricted to the current user).
- **Direct Communication**: The tool communicates directly with the GitHub API. Your token is never shared with us or any third party.

## 3. Terminal Logs
Terminal logs are captured locally into a temporary file (`/tmp/cli-session.log`). These logs are only uploaded to GitHub Gists when you explicitly trigger the `/share` or `cli-share` command.

## 4. Install analytics (Scarf)
When you install `@saurav-singh/cli-share` via npm, anonymous installation statistics may be reported with [Scarf](https://scarf.sh) (`@scarf/scarf`). No API keys are embedded in this project. Details: [Scarf package analytics](https://docs.scarf.sh/package-analytics/).

To opt out:

```bash
export SCARF_ANALYTICS=false
```

## 5. Third-Party Services
- **GitHub Gist API** — hosts shared conversations (when you choose to share). Subject to [GitHub's Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-privacy-statement).
- **Scarf** — install analytics as described above. Subject to [Scarf's privacy policy](https://about.scarf.sh/privacy-policy).

## 6. Contact
For any questions regarding privacy, please open an issue on our [GitHub Repository](https://github.com/saurav-shakya/cli-share).

# Local Commander for Gemini CLI

A Gemini CLI extension for [Local Commander](https://localcmd.app). It connects Gemini CLI to the hosted server `https://localcmd.app/mcp`, so your AI can inspect approved project files and Git state, run the checks and commands you authorize, and diagnose approved localhost services on Windows 11 computers you own. Your workspace at localcmd.app shows which computer ran each request and how it ended.

This repository holds configuration only. The service runs at localcmd.app.

## Requirements

- A Local Commander account at [localcmd.app](https://localcmd.app).
- A Windows 11 x64 computer with Node.js 20 or later and the paired agent: run `npx local-commander-agent@latest` on it, then choose full access or selected folders.
- The computer must be online for work and for reading results.

Once you approve a computer and connect your AI, it can do what your Windows account can do, just like you at the keyboard. You can limit it to certain folders, block commands, stop running work, or switch a computer off from the site at any time. Every run shows which computer did it. Whatever the AI asks for goes back to the AI.

## Install

```sh
gemini extensions install https://github.com/netbka/local-commander-gemini
```

Start `gemini` and run `/mcp auth local-commander`. Gemini CLI opens localcmd.app in your browser to sign in and approve access (OAuth 2.0); Gemini CLI never sees your password. Then ask it to list your computers and work on an approved project.

Remove with `gemini extensions uninstall local-commander`.

Using Antigravity CLI instead? Use the Antigravity plugin in [netbka/local-commander-plugins](https://github.com/netbka/local-commander-plugins).

## Links

Privacy: https://localcmd.app/privacy. Terms: https://localcmd.app/terms. Support: peter.mamrukov@localcmd.app (https://localcmd.app/support).

## License

MIT, for the files in this repository.

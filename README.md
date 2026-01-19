[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/hackteck/myop-setup/tree/master)

# The Pic-Time builders’ Myop env setup

# Prerequisites

Get a Claude Code account from Yasmin

# Setup

| Action | Details |
| :---- | :---- |
| Open account in Myop | [https://myop.dev](https://myop.dev) open an account and send to [hadar@myop.dev](mailto:hadar@myop.dev) a request to add you to the Pic-Time organization. It must be on your Pic-Time’s email |
| VSCode install | [https://code.visualstudio.com/download](https://code.visualstudio.com/download) Click next in the welcome wizard.  |
| node.js | Open a new PowerShell or Command Prompt as Administrator and run: winget install OpenJS.NodeJS.LTS On windows: click Start \> type PowerShell \> Right click Windows PowerShell \> Select run as administrator |
| Enable scripts execution | In PowerShell, change the execution policy to allow scripts to run:  Set-ExecutionPolicy \-ExecutionPolicy RemoteSigned \-Scope CurrentUser |
| Claude Code for VS Code (extension) | [https://code.claude.com/docs/en/vs-code](https://code.claude.com/docs/en/vs-code) Look for ‘install VSCode’ Connect it to Claude account provided by Yasmin: Open the Claude Code extension and click the Claude Code orange icon at the top right to open Claude Code. Choose ‘[calude.ai](http://calude.ai) Subscription’. In the popup, select Open. Use the Claude Code account from Yasmin. |
| Enable Git | Download git from [https://git-scm.com/downloads/win](https://git-scm.com/downloads/win) and install it |
| Enabling Claude to run in terminal | Open the VSCode and open the Claude prompt. Write “I cannot run claude from terminal, fix it” Follow the process and approve the requests by the agent: choose “Yes, don’t ask again” throughout the process |
| Install Myop MCP | Open the terminal window in VSCode (in the top bar menu) *“claude mcp add myop https://mcp.myop.dev/mcp \--transport http \--scope user”* Follow the process and the requests Ref: [https://docs.myop.dev/docs/mcp-setup/](https://docs.myop.dev/docs/mcp-setup/)  |
| Authorize Myop MCP | In the VSCode Claude prompt,  *“/mcp”* and select the Manage MCP servers Continue to authorize the Myop MCP. It will require you multiple Enters and approve the Claude and Myop connections Follow the defaults |
| Install Myop CLI | Open the terminal window (topbar terminal) and type *“npm install \-g @myop/cli”* |
| Install Myop Extension | Follow the introductions on [https://docs.myop.dev/docs/dev-extension/](https://docs.myop.dev/docs/dev-extension/) To install the chrome extension |
| 🙂 | We should be good |
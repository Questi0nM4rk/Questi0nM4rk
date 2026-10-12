<div align="center">

# Hey, I'm Jakub 👋

<a href="https://github.com/Questi0nM4rk"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=900&color=58A6FF&center=true&vCenter=true&width=620&lines=Backend+engineer+(.NET)+by+day;Agent+tooling+for+Claude+Code+by+night;Measure%2C+don't+claim." alt="Backend engineer (.NET) by day. Agent tooling for Claude Code by night. Measure, don't claim."></a>

<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
<img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun">
<img src="https://img.shields.io/badge/C%23%20%2F%20.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="C# / .NET">
<img src="https://img.shields.io/badge/Shell-4EAA25?style=flat-square&logo=gnubash&logoColor=white" alt="Shell">
<img src="https://img.shields.io/badge/Go%20%E2%86%92%20WASM-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go to WASM">
<img src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code">
<img src="https://img.shields.io/badge/Arch%20%2B%20Hyprland-1793D1?style=flat-square&logo=archlinux&logoColor=white" alt="Arch Linux with Hyprland">

</div>

---

## 🧭 How I build

| | |
| --- | --- |
| ✂️ **The best code is the code not written.** | Every file, flag and test has to say what is missing without it. |
| 📏 **Measure, don't claim.** | Every number in my READMEs comes with the command that produced it. |
| 💥 **Fail loud.** | One path, no silent fallback. A dead program tells no lies. |
| 🎯 **Intent first.** | I write down what the work is for before I write the work. |
| 🔁 **Prove it on the real path.** | An end-to-end run beats a test that restates the code. |
| 🛡️ **Agents need rules they cannot remove.** | Guardrails live outside the agent: in hooks, commits and CI. |

## 🛠️ What I build

A small stack for letting a coding agent check its own work. Each layer is its own repo and its own npm package.

```mermaid
flowchart LR
  A["🌳 shell-ast<br/>parse shell before it runs"] --> B["🪝 hook-kit<br/>agent hooks as one binary"]
  B --> C["🛡️ ai-guardrails<br/>rules agents can't weaken"]
  A --> C
  D["🥒 feats<br/>BDD tests for Bun"] -. tests .-> B
  D -. tests .-> C
  B --> E["🧰 qsm-marketplace<br/>27 Claude Code plugins"]
  F["🤖 cc-review<br/>Claude reviews my PRs"] -. reviews .-> C
```

<table>
<tr>
<td width="50%" valign="top">

### 🧰 [qsm-marketplace](https://github.com/Questi0nM4rk/qsm-marketplace)
My daily Claude Code setup as a marketplace of 27 small plugins: skills, agents, hooks and CLI tools that help an agent see, verify and evaluate its own work.

![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square) ![license](https://img.shields.io/github/license/Questi0nM4rk/qsm-marketplace?style=flat-square&color=555)

</td>
<td width="50%" valign="top">

### 🤖 [cc-review](https://github.com/Questi0nM4rk/cc-review)
A pull request reviewer that runs Claude Code in GitHub Actions and posts inline comments as its own GitHub App.

![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logoColor=black) ![license](https://img.shields.io/github/license/Questi0nM4rk/cc-review?style=flat-square&color=555)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛡️ [ai-guardrails](https://github.com/Questi0nM4rk/ai-guardrails)
Hooks, a commit gate and a CI check that flag when a coding agent weakens a project's own lint and hook rules.

![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square) ![license](https://img.shields.io/github/license/Questi0nM4rk/ai-guardrails?style=flat-square&color=555)

</td>
<td width="50%" valign="top">

### 🪝 [hook-kit](https://github.com/Questi0nM4rk/hook-kit)
Builds coding-agent hooks into one compiled binary that decides through stdout, stderr and the exit code.

![npm](https://img.shields.io/npm/v/@questi0nm4rk/hook-kit?style=flat-square&color=cb3837&label=npm) ![license](https://img.shields.io/github/license/Questi0nM4rk/hook-kit?style=flat-square&color=555)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🌳 [shell-ast](https://github.com/Questi0nM4rk/shell-ast)
A typed AST for bash, POSIX sh and mksh, so a tool can read a command before it runs.

![npm](https://img.shields.io/npm/v/@questi0nm4rk/shell-ast?style=flat-square&color=cb3837&label=npm) ![license](https://img.shields.io/github/license/Questi0nM4rk/shell-ast?style=flat-square&color=555)

</td>
<td width="50%" valign="top">

### 🥒 [feats](https://github.com/Questi0nM4rk/feats)
A BDD runner that turns Gherkin feature files into typed `bun:test` suites.

![npm](https://img.shields.io/npm/v/@questi0nm4rk/feats?style=flat-square&color=cb3837&label=npm) ![license](https://img.shields.io/github/license/Questi0nM4rk/feats?style=flat-square&color=555)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧠 [tagen](https://github.com/Questi0nM4rk/tagen)
Resolves a query against a catalog of skill cards and returns the matching set as a manifest.

![license](https://img.shields.io/github/license/Questi0nM4rk/tagen?style=flat-square&color=555)

</td>
<td width="50%" valign="top">

### 🗂️ [vori](https://github.com/Questi0nM4rk/vori)
Queries Obsidian-style markdown vaults from the terminal: tags, wikilinks, full text.

![license](https://img.shields.io/github/license/Questi0nM4rk/vori?style=flat-square&color=555)

</td>
</tr>
</table>

> 🧪 **Experiment:** [codebase-mcp](https://github.com/Questi0nM4rk/codebase-mcp) was my first try at code retrieval for agents. It taught me where over-engineering starts, and its README says so.

## 🎴 Away from the terminal

<img align="right" width="300" alt="My split Dactyl keyboard, left half" src="https://raw.githubusercontent.com/Questi0nM4rk/zmk-config-lozor/master/photo_left.jpg">

- 🃏 I do cardistry and card tricks.
- 🌀 I obsess over a random new thing for a month, then forget what I did a week later.
- 🔧 I like owning my tools, so I build them. Even my desktop is my own: [qsm-desktop](https://github.com/Questi0nM4rk/qsm-desktop) is a Quickshell shell for Hyprland, built on the [qsm-shell](https://github.com/Questi0nM4rk/qsm-shell) component library and previewed in [qsm-workbench](https://github.com/Questi0nM4rk/qsm-workbench).
- ⌨️ I type on a split Dactyl I built myself, running ZMK on nice!nano v2 boards: [zmk-config-lozor](https://github.com/Questi0nM4rk/zmk-config-lozor).

<br clear="right">

# 👻 Astral — Your Arch System Pilot

[![Rust](https://img.shields.io/badge/Built_with-Rust-orange?style=flat-square\&logo=rust)](https://www.rust-lang.org)
[![GPU Accelerated](https://img.shields.io/badge/NVIDIA-Optimized-blue?style=flat-square\&logo=nvidia)](https://developer.nvidia.com/)
[![Powered by Ollama + LiteLLM](https://img.shields.io/badge/LLM-LiteLLM%20%2B%20Ollama-informational?style=flat-square\&logo=openai)](https://github.com/BerriAI/litellm)
[![Privacy First](https://img.shields.io/badge/Privacy-Zero%20Cloud-critical?style=flat-square\&logo=gnuprivacyguard)](#)
[![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue?style=flat-square)](LICENSE)

**Astral** is a ghost-themed, next-gen system pilot for Arch Linux. It's like Jarvis — but private, local, and built for power users who want a true AI copilot on their own terms. Astral interfaces with your system tools, LLMs (LiteLLM, Ollama), Snapper, Nix, and more — all over secure local APIs.

---

## 🌌 Why Astral?

* 🧠 Operates like a Linux-native copilot for Arch
* ✨ Accepts screenshots, text, CLI, and clipboard prompts
* 📦 Integrates with Snapper, systemd, pacman, and btrfs
* 🔐 Built-in privacy: **runs 100% on your hardware**
* 🧬 Taps into Ollama, LiteLLM, and eventually local vision models

---

## 🚀 Features

| Feature                       | Status        |
| ----------------------------- | ------------- |
| Local Ollama + LiteLLM proxy  | ✅ Done        |
| Screenshot/image input        | ✅ In Progress |
| Shell + Nvim hook integration | 🛠️ Planned   |
| Snapper config + restore API  | 🛠️ Planned   |
| ENS/Unstoppable domain input  | 🧪 Prototype  |
| `ghostctl` + TUI mode support | ✅ Designed    |

---

## 🔧 Tech Stack

* **Rust** — Fast, safe, async-ready backend
* **Axum** — API + routing layer
* **Ollama / LiteLLM** — Local LLM execution engine
* **serde / reqwest** — Data handling & HTTP bridging
* **Zig** (optional sidecar for system watchers)

---

## 🔐 Privacy & Sovereignty

* ✅ No cloud inference ever
* ✅ No telemetry
* ✅ DNS-over-TLS and DNSSEC preferred
* ✅ Optional Tailscale/Headscale LAN-only access

---

## 🛠 Usage (dev preview)

```bash
cargo build --release
./astral --ask "What packages are bloating my system?"
```

Or pipe it prompts:

```bash
astral --upload ~/Screenshots/boot-error.png --ask "Why won't this boot?"
```

---

## 🌠 Future Vision

* Plug into `ghostctl monitor`, `ghostview`, or `ghostmesh`
* Add `astral-nvim` integration for inline code/chat/devops
* GPU heatmap awareness & sensor linking
* Model fallback switching (e.g., Mistral → Phi → GPT4All)

---

## 🧙 Contribute

* Join the `ghostkellz` dev community
* Add modules: NixOS, Snapper, Pipewire, D-Bus...
* Test new vision + multimodal LLM integrations

---

© 2025 CK Technology LLC / GhostKellz — Licensed under GNU GPLv3

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:0b3d91,100:1f6feb&height=220&section=header&text=Shub%20Saini&fontSize=64&fontColor=ffffff&fontAlignY=38&desc=Cryptography%20Engineer%20%C2%B7%20High-Performance%20Computing%20%C2%B7%20Blockchain%20Tooling&descSize=17&descAlignY=60" alt="Shub Saini header" width="100%" />

<a href="https://github.com/Shubsaini08">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&pause=1600&color=58A6FF&center=true&vCenter=true&width=720&lines=Elliptic-curve+cryptography+%E2%80%A2+secp256k1;Multi-threaded+C%2B%2B+%E2%80%A2+CUDA+%E2%80%A2+OpenCL;Async+blockchain+infrastructure+%E2%80%A2+Python;Turning+applied+math+into+fast%2C+resumable+software" alt="Typing animation" />
</a>

<br/>

[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/Shainshub)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:keyfoundhunt4ever@gmail.com)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Shubsaini08)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/m4ryWABM)

![Profile views](https://komarev.com/ghpvc/?username=Shubsaini08&label=Profile%20views&color=1f6feb&style=flat-square)
![Followers](https://img.shields.io/github/followers/Shubsaini08?style=flat-square&color=1f6feb&label=Followers)
![Repos](https://img.shields.io/badge/Public%20Repos-5%20featured-1f6feb?style=flat-square)

</div>

---

## 👤 About

```python
class ShubSaini:
    role      = "Cryptography student & engineer"
    focus     = ["secp256k1 / ECDLP", "iterative hashing", "GPU acceleration", "blockchain tooling"]
    languages = ["C++", "Python", "C", "C#", "TypeScript", "Java"]
    approach  = "Fast, resumable, well-instrumented software"
    open_to   = ["research collaborations", "performance engineering", "consulting & training"]
```

I work on the practical side of elliptic-curve cryptography and high-throughput computation: taking an idea from a math paper to a measured, checkpointed, multi-threaded implementation. I care about correctness first, then throughput, then observability.

<table>
<tr>
<td width="50%" valign="top">

### 🔬 Research Focus
- ECDLP: Baby-Step Giant-Step, small-difference analysis
- Iterative SHA-256 / SHA-512 chaining
- Key-derivation and address-generation analysis
- Range-based search strategies

</td>
<td width="50%" valign="top">

### ⚙️ Engineering Focus
- Multi-threaded C++ with OpenSSL and libsecp256k1
- CUDA / OpenCL acceleration
- Async Python services and RPC clients
- Checkpointing, logging and auto-resume

</td>
</tr>
</table>

---

## 🚀 Featured Projects

<div align="center">

[![shathecurev2](https://github-readme-stats.vercel.app/api/pin/?username=Shubsaini08&repo=shathecurev2&theme=github_dark&hide_border=true&bg_color=0d1117)](https://github.com/Shubsaini08/shathecurev2)
[![ETHPARSER](https://github-readme-stats.vercel.app/api/pin/?username=Shubsaini08&repo=ETHPARSER&theme=github_dark&hide_border=true&bg_color=0d1117)](https://github.com/Shubsaini08/ETHPARSER)

[![KEYFOUND](https://github-readme-stats.vercel.app/api/pin/?username=Shubsaini08&repo=KEYFOUND&theme=github_dark&hide_border=true&bg_color=0d1117)](https://github.com/Shubsaini08/KEYFOUND)
[![telecontrol](https://github-readme-stats.vercel.app/api/pin/?username=Shubsaini08&repo=telecontrol&theme=github_dark&hide_border=true&bg_color=0d1117)](https://github.com/Shubsaini08/telecontrol)

[![Pubkey](https://github-readme-stats.vercel.app/api/pin/?username=Shubsaini08&repo=Pubkey&theme=github_dark&hide_border=true&bg_color=0d1117)](https://github.com/Shubsaini08/Pubkey)

</div>

### 🔹 [shathecurev2](https://github.com/Shubsaini08/shathecurev2): CPU iterative hashing engine

A multi-threaded C++ engine that repeatedly applies SHA-256 (or SHA-512 → SHA-256) to input strings, treats each digest as a secp256k1 private key, and derives P2PKH / P2SH addresses.

- **~2.4M hashes/s** benchmarked on an Intel i9-13900K
- Full checkpointing, structured logging and automatic resume after interruption
- Entropy mutation for input variation
- Built on OpenSSL and libsecp256k1

```mermaid
flowchart LR
    A[Input string] --> B[Iterative SHA-256 / SHA-512]
    B --> C[Digest as secp256k1 private key]
    C --> D[Public key]
    D --> E[P2PKH / P2SH address]
    E --> F[(Checkpoint + log)]
    F -.auto-resume.-> B
```

![C++](https://img.shields.io/badge/C++-77%25-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-23%25-3776AB?style=flat-square&logo=python&logoColor=white)
![OpenSSL](https://img.shields.io/badge/OpenSSL-721412?style=flat-square&logo=openssl&logoColor=white)
![libsecp256k1](https://img.shields.io/badge/libsecp256k1-444?style=flat-square)

### 🔹 [ETHPARSER](https://github.com/Shubsaini08/ETHPARSER): real-time Ethereum block scanner

An asynchronous bot that follows the chain head, extracts addresses from every new block, and reports balances, transaction counts and large holders.

- Async RPC polling with **fallback endpoints** and rate-limit handling
- Automatic flagging of addresses holding **more than 10 ETH**
- Telegram broadcast via aiogram

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![asyncio](https://img.shields.io/badge/asyncio-444?style=flat-square)
![aiohttp](https://img.shields.io/badge/aiohttp-2C5BB4?style=flat-square&logo=aiohttp&logoColor=white)
![aiogram](https://img.shields.io/badge/aiogram-2CA5E0?style=flat-square&logo=telegram&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum%20JSON--RPC-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)

### 🔹 [KEYFOUND](https://github.com/Shubsaini08/KEYFOUND): Telegram crypto utility bot

A modular bot for everyday crypto tasks, with an async backend and command-based interface (`/bal`, `/derive`, `/list`).

- Live BTC balance checks and batch address processing
- Hash and public-key derivation
- Background news alerts, AI query mode and text-to-voice

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![python-telegram-bot](https://img.shields.io/badge/python--telegram--bot-2CA5E0?style=flat-square&logo=telegram&logoColor=white)
![aiohttp](https://img.shields.io/badge/aiohttp-2C5BB4?style=flat-square&logo=aiohttp&logoColor=white)
![pycryptodome](https://img.shields.io/badge/pycryptodome-444?style=flat-square)

### 🔹 [telecontrol](https://github.com/Shubsaini08/telecontrol): Telegram remote administration

Lets authorized administrators operate a machine from Telegram: shell commands, directory navigation, git clone, and file read/write.

- Strict **ID allow-listing** for access control
- Multi-device support with background keep-alive
- Python 3.8+, `subprocess` and `os`

> ⚠️ Intended only for machines you own, with the allow-list configured.

### 🔹 [Pubkey](https://github.com/Shubsaini08/Pubkey): Bitcoin public-key dataset

More than **100,000 Bitcoin public keys** extracted block by block from the blockchain, stored as plain-text files per block. It contains **no private keys** and is intended for researchers, forensic tooling and ECDLP studies. Continuously updated.

---

## 🧰 Tech Stack

<div align="center">

| | |
|:--|:--|
| **Languages** | ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black) ![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) |
| **HPC & GPU** | ![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white) ![OpenCL](https://img.shields.io/badge/OpenCL-ED1C24?style=flat-square&logo=khronosgroup&logoColor=white) ![Multithreading](https://img.shields.io/badge/Multi--threading-444?style=flat-square) ![Ray](https://img.shields.io/badge/Ray-028CF0?style=flat-square&logo=ray&logoColor=white) |
| **Cryptography** | ![secp256k1](https://img.shields.io/badge/secp256k1-F7931A?style=flat-square&logo=bitcoin&logoColor=white) ![OpenSSL](https://img.shields.io/badge/OpenSSL-721412?style=flat-square&logo=openssl&logoColor=white) ![ECDLP](https://img.shields.io/badge/ECDLP%20%2F%20BSGS-444?style=flat-square) ![SHA-2](https://img.shields.io/badge/SHA--256%20%2F%20512-444?style=flat-square) |
| **AI & Data** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![Joblib](https://img.shields.io/badge/Joblib-444?style=flat-square) |
| **DevOps & Tools** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white) |

</div>

---

## 🗺️ Roadmap

- [x] Multi-threaded CPU iterative hashing engine with checkpointing (`shathecurev2`)
- [x] Async Ethereum scanning and alerting (`ETHPARSER`)
- [x] Public Bitcoin public-key dataset (`Pubkey`)
- [ ] CUDA / OpenCL port of the hashing and key-derivation pipeline
- [ ] Baby-Step Giant-Step implementation with benchmarks
- [ ] Documentation, tests and reproducible benchmark suite for each repository

---

## 🤝 Work With Me

| Service | What you get |
|---|---|
| **Performance engineering** | Profiling, vectorization, threading and GPU offload for compute-heavy code |
| **Cryptographic tooling** | Custom utilities for key derivation, address generation and keyspace analysis |
| **Research prototypes** | Proof-of-concept implementations for ECC and hash-chain analysis |
| **Training & workshops** | ECC fundamentals, iterative hashing and GPU acceleration |
| **Authorized recovery** | Helping owners regain access to their *own* wallets from partial information |

Send a short spec or idea via [Telegram](https://t.me/Shainshub) or [email](mailto:keyfoundhunt4ever@gmail.com).

---

## 📊 GitHub Analytics

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=Shubsaini08&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&count_private=true&include_all_commits=true" alt="GitHub stats" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Shubsaini08&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117" alt="Top languages" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Shubsaini08&theme=github-dark-blue&hide_border=true&background=0d1117" alt="Streak" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Shubsaini08&theme=github-compact&hide_border=true&bg_color=0d1117&area=true" alt="Contribution graph" width="100%" />

</div>

---

## 🛡️ Responsible Use

My tools are published for research, education, and authorized recovery or testing of keys and systems that you own or have explicit permission to access. Do not use them against wallets, accounts or machines that are not yours.

---

## ☕ Support

If my work is useful to you, contributions are appreciated.

**BTC:** `bc1qwc24wqwu08x2cdnfzc40ezma4q5zsn37jxkkmt`

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1f6feb,50:0b3d91,100:0d1117&height=110&section=footer" alt="footer" width="100%" />

</div>

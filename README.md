# 🧩 Game Loader & Client Update Repository

This repository is intentionally minimal and serves a specific purpose:  
It is used **exclusively** for distributing update packages and version metadata for a game loader and client.

> 📦 **No source code is hosted here by design.** This is not a development repository.

---

## 🔧 Purpose

This repository acts as a lightweight update backend for a secure external loader. It includes:

- `.zip` packages uploaded under the [Releases](https://github.com/gc-cff/cff-updates/releases) tab
- A `version.json` file in the root, which contains metadata about the latest version

---

## 🚀 Update Flow

1. The external loader checks `version.json` at startup
2. If a newer version is available, it downloads the `.zip` from the provided `url`
3. The archive is extracted and the updated client is launched

---

## 🔐 Security Notes

* Executables in the archives are protected with **Themida (C++)** and **Babel (C#)** for anti-reverse engineering and integrity
* All files are designed to be used **only through the official loader**
* No source files, development assets, or intellectual property are stored here

---

## 📬 Contact

This repository is not meant for public issue tracking.
For questions or technical support, please reach out via the official loader or designated support channels (e.g. Discord or Telegram).

---

## ⚠️ Why This Repo Has No Code

This repository is not abandoned or incomplete.
It is intentionally structured this way to serve as a **secure update endpoint only**, with no need for source code or issue tracking.

Please do not open issues or reports regarding missing content.
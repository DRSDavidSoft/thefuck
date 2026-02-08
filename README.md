# The Fuck (Python 3.12 compatible fork)

This is a **maintained fork of [thefuck](https://github.com/nvbn/thefuck)** with fixes for **Python 3.12+**.

The original project is no longer compatible with Python 3.12 due to the removal of legacy standard library modules such as `imp` and `distutils`.
This fork updates the codebase to work correctly on modern Python versions while preserving original behavior.

---

## ✨ What’s fixed in this fork

-   ✅ Removed usage of `imp` (removed in Python 3.12)
-   ✅ Replaced `distutils.spawn.find_executable` with `shutil.which`
-   ✅ Fixed standard library shadowing issues (`types.py`)
-   ✅ Fully compatible with **Python 3.12+**
-   ✅ Works correctly on **Ubuntu 24.04 (Noble)**

No behavior changes. Only compatibility fixes.

---

## 🚀 Installation (recommended)

### Install with pipx (global, isolated)

pipx is the recommended way to install CLI Python tools.

```bash
sudo apt install pipx
pipx ensurepath
exec zsh
```

Install from this repository:

```bash
pipx install git+https://github.com/vo0ov/thefuck
```

Or from a local clone:

```bash
pipx install .
```

---

## 🧪 Verify installation

```bash
thefuck --version
```

Example output:

```text
The Fuck 3.32 using Python 3.12.3 and ZSH 5.9
```

---

## 🐚 Usage example:

```bash
apt updte
fuck
```

---

## 🐍 Python compatibility

| Python version | Status        |
| -------------- | ------------- |
| 3.8 – 3.11     | ✅            |
| 3.12+          | ✅            |
| < 3.8          | ❌ not tested |

---

## 📌 Original project

This repository is a fork of the original project:

https://github.com/nvbn/thefuck

For original documentation, rule descriptions, and examples, please refer to the upstream README.

---

## 📄 License

Same license as the original project.

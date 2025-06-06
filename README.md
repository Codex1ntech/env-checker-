# 🧰 env-checker-cli

> Portable CLI script to validate required tools, environment variables, and system configs — because "it works on my machine" is not a QA strategy.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Unix-lightgrey.svg)
![Shell](https://img.shields.io/badge/shell-Bash-green.svg)

---

## 📦 Features

- ✅ Validate system tools (e.g., git, curl, docker)
- 🔍 Check for missing environment variables
- 🧪 Configurable validation list
- 💡 Human-friendly output with emojis

---

## ⚙️ Installation

```bash
git clone https://github.com/Codex1ntech/env-checker-cli.git
cd env-checker-cli
chmod +x scripts/env-check.sh
./scripts/env-check.sh -c config.env
```

---

## 🧪 Configuration

You can create a custom `.env` file to define which variables must exist:

```env
API_KEY=your-api-key
USER=naz
```

Save it as `config.env` or pass a custom one using `-c yourfile.env`.

---

## 📸 Example Output

```bash
🔍 Checking tools...

✅ git found  
✅ curl found  
❌ docker missing  

🔍 Checking variables...

❌ ENV "API_KEY" is not set  
✅ ENV "USER" is set  

✅ Done
```

---

## 📁 Project Structure

```text
env-checker-cli/
├── README.md
├── LICENSE
├── config.env.example
├── scripts/
│   └── env-check.sh
├── examples/
│   └── sample-output.txt
```

---

## 🚀 Usage

```bash
./scripts/env-check.sh
./scripts/env-check.sh -c my-config.env
```

---

## 📄 License

MIT License © [Codex1ntech](https://github.com/Codex1ntech)

# 💻 VSCode IDE setup
My VSCode setup for C, Python and SQLite development, extending Harvard CS50's workflow.

[**PT-BR**](./docs/README.pt-br.md)

<img width="1267" height="757" alt="image" src="https://github.com/user-attachments/assets/ff35e077-69da-4b4d-8fbb-49d2b84a1ce2" />

## 📦 Dependencies
- [VSCode](https://code.visualstudio.com/download)
- [MinGW](https://www.mingw-w64.org/downloads/)
- [Python](https://www.python.org/downloads/)

## 🚀 Getting Started
<details>
  <summary>⚙️ MinGW Setup for C</summary>
  
  - Add `C:\mingw64\bin` to the PATH system environment variable;
  - Place header files (`.h`) in `C:\mingw64\include`;
  - Place source files (`.c`) or library files (`.a`,`.lib`) in `C:\mingw64\lib`;
  - Install the **VSCode C/C++ Extension Pack**;
  - Configure `launch.json`, `settings.json`, and `tasks.json` in the `.vscode` workspace (reference the [**.vscode folder**](./.vscode/)).

</details>

<details>
  <summary>🐍 Python Setup</summary>
  
  - Install latest stable **Python** version and ensure it's added to the System PATH;
  - Install the **Python Extension** for VSCode.

</details>

<details>
  <summary>🗄️ SQLite Setup</summary>

  - Install the [SQLite](https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite) VS Code extension by alexcvzz;
  - SQLite comes bundled with Python — confirm it is working by running:
```bash
    python -c "import sqlite3; print(sqlite3.sqlite_version)"
```

</details>

## 🔧 Troubleshooting
Common issues and their solutions.

[Full Troubleshooting Guide](./docs/TROUBLESHOOTING.md)

### Visual Studio Code C/C++ debug error (System.Security.SecurityException: Falha na validação de nome forte)
- **Problem:** Unable to start debugging. Unable to establish a connection to GDB. Debug output may contain more information.
- **Solution:** In the VSCode extensions tab, click "Switch to release version" and restart VSCode.

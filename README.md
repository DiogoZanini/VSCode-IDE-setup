# VSCode-IDE-setup
My VSCode IDE configuration

[**PT-BR**](./docs/README.pt-br.md)

## Dependencies
- [VSCode Installation](https://code.visualstudio.com/download)
- [MinGW Installation for C](https://www.mingw-w64.org/downloads/)

## Getting Started
<details>
  <summary>MinGW Setup for C</summary>
  
  - Add `C:\mingw64\bin` to the PATH system environment variable;
  - Place header files (`.h`) in `C:\mingw64\include`;
  - Place source files (`.c`) or library files (`.a`,`.lib`) in `C:\mingw64\lib`;
  - Install the **VSCode C/C++ Extension Pack**
  - Configure `launch.json`, `settings.json`, and `tasks.json` in the `.vscode` workspace (reference the [**.vscode folder**](./.vscode/))

</details>

## Troubleshooting
Common issues and their solutions.

[Full Troubleshooting Guide](./docs/TROUBLESHOOTING.md)

### Visual Studio Code C/C++ debug error (System.Security.SecurityException: Falha na validação de nome forte)
- **Problem:** Unable to start debugging. Unable to establish a connection to GDB. Debug output may contain more information.
- **Solution:** In the VSCode extensions tab, click "Switch to release version" and restart VSCode.

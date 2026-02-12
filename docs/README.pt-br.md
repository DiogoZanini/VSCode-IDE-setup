# Configuração do VSCode-IDE
Minha configuração do VSCode IDE

[**EN-US**](../README.md)

## Dependências
- [VSCode](https://code.visualstudio.com/download)
- [MinGW](https://www.mingw-w64.org/downloads/)
- [Python](https://www.python.org/downloads/)

## Primeiros Passos
<details>
  <summary>Configuração do MinGW para C</summary>

  - Adicione `C:\mingw64\bin` à variável de ambiente do sistema PATH.
  - Coloque os arquivos de cabeçalho (`.h`) em `C:\mingw64\include`.
  - Coloque os arquivos de código-fonte (`.c`) ou arquivos de biblioteca (`.a`, `.lib`) em `C:\mingw64\lib`.
  - Instale o **VSCode C/C++ Extension Pack**.
  - Configure os arquivos `launch.json`, `settings.json` e `tasks.json` no workspace `.vscode` (use a [**pasta .vscode**](./.vscode/) como referência).

</details>

<details>
  <summary>Configuração do Python</summary>

  - Instale a versão estável mais recente do **Python** e certifique-se de adicioná-lo ao PATH do sistema.
  - Instale a **extensão Python** para o VSCode.
  
</details>

<details>
  <summary>Configuração do SQLite</summary>

  - Instale a extensão [SQLite](https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite) para VS Code desenvolvida por alexcvzz;
  - O SQLite já vem incluído no Python — confirme que está funcionando executando:
```bash
    python -c "import sqlite3; print(sqlite3.sqlite_version)"
```

</details>

## Solução de problemas
Problemas comuns e suas soluções.

[Guia completo de solução de problemas](./docs/TROUBLESHOOTING.md)

### Erro de depuração de C/C++ no Visual Studio Code (System.Security.SecurityException: Falha na validação de nome forte)
- **Problema:** Não foi possível iniciar a depuração. Não foi possível estabelecer uma conexão com o GDB. A saída de depuração pode conter mais informações.
- **Solução:** Na guia de extensões do VSCode, clique em "Alternar para a versão de lançamento" e reinicie o VSCode.

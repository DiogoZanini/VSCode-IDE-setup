# Troubleshooting
Problems encountered and their solutions

## Visual Studio Code C/C++ debug error (System.Security.SecurityException: Falha na validação de nome forte)
- **Problem:** Unable to start debugging. Unable to establish a connection to GDB. Debug output may contain more information.
- **Cause:** Error in the C/C++ extension; it was operating on a pre-release version.
- **Solution:** In the VSCode extensions tab, click "Switch to release version" and restart VSCode.

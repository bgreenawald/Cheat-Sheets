# Python Virtual Environments

### Regular old virtual environments

Create a new virtual environment in the local project folder (Windows)
```bash
py -m virtualenv env
```

Create a new virtual environment in the local project folder (Linux)
```bash
python3 -m virtualenv env
```

Activate new environment in Powershell
```bash
.\\env\\Scripts\\activate.ps1
```
Note that this may or may not work based on file permissions. You definitely will need to check on your script execution policy.
```bash
Get-ExecutionPolicy
```
You're going to want it to be RemoteSigned at the very least, though less restrictive policies should work.
```bash
Set-ExecutionPolicy RemoteSigned
```
 While I have not tested this successfully, the simpler and safer option would like be to just unblock the file.
```bash
Unblock-File \\env\\Scripts\\activate.ps1
```
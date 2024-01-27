# Golang-Note

**Go exntesion**
```https://github.com/golang/vscode-go/releases/tag/v0.33.0```

**print log:**
```
// var participants // json stringify
jsonStr, _ := json.Marshal(participants)
fmt.Println(string(jsonStr))
```

```
// var participants // json stringify with beautify
jsonStr, _ := json.MarshalIndent(participants, "", "    ")
fmt.Println(string(jsonStr))
```
### Git SSH Key generate

check git available or not
```
git
```

if git not available, install git from https://git-scm.com/downloads

open cmd with C:\Users\{your_username}

```ssh-keygen```
or
```ssh-keygen -t rsa -b 4096```
or
```ssh-keygen -t ed25519 -C "your@email.address"```

type this command and press enter key
next step 2-3 press enter key
note: after successful generate rsa key.

**C:\Users\{your_username}\.ssh**

 

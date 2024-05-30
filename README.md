# Golang-Note

**Go exntesion**
```https://github.com/golang/vscode-go/releases/tag/v0.33.0```

**print log:**
```
// var participants // json stringify
jsonStr, _ := json.Marshal(participants)
fmt.Println(string(jsonStr))
```

**Go Crud Ref**
- [https://www.honeybadger.io/blog/how-to-create-crud-application-with-golang-and-mysql/](https://www.honeybadger.io/blog/how-to-create-crud-application-with-golang-and-mysql/)
- [https://techwasti.com/go-language-mysql-rest-api-crud-example](https://techwasti.com/go-language-mysql-rest-api-crud-example)
- [https://www.golangprograms.com/example-of-golang-crud-using-mysql-from-scratch.html](https://www.golangprograms.com/example-of-golang-crud-using-mysql-from-scratch.html)
- [https://medium.com/swlh/create-an-crud-rest-api-using-mysql-golang-part-1-65e74bbae283](https://medium.com/swlh/create-an-crud-rest-api-using-mysql-golang-part-1-65e74bbae283)
- [https://medium.com/@rasoky.maulana/create-a-crud-rest-api-using-mysql-golang-part-2-5af4942abdd2](https://medium.com/@rasoky.maulana/create-a-crud-rest-api-using-mysql-golang-part-2-5af4942abdd2)

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

### Git Basic Commands List

git global config: Reference Link
https://www.geeksforgeeks.org/how-to-set-git-username-and-password-in-gitbash/
https://linuxhint.com/configuration-user-and-password-with-git-bash/

specific branch clone:
```
git clone -b dev https://github.com/jatinchavda/Golang-Note.git
```

specific branch clone and without root folder:
```
git clone -b dev https://github.com/jatinchavda/Golang-Note.git .
```

change branch:
```
git checkout dev
```

files upload:
```
git add .
git commit -m "Theme & Plugin Starter Features"
git push
```

files download:
```
git pull
```

**git init with specific branch & connect remote branch**
```
git init -b master
git remote add origin https://github.com/jatinchavda/Golang-Note.git
```

Migration from OLD server to NEW server
```
git clone https://your.old.git.url
git checkout your_branch_name
git remote set-url origin https://you.new.git.url
git add .
git commit -m "Commit Text"
git push origin your_branch_name
```

Change local default branch Name:
```
git config --global init.defaultBranch main
```

unset username and email - global
```
git config --global --unset user.name
git config --global --unset user.email
```

unset username and email - project base
```
git config --unset user.name
git config --unset user.email
```

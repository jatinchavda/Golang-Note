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

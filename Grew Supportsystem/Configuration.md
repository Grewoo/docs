# Wiki - Grew Supportsystem
## Configuration
### Config.Locale
Change the language of the script.<br>
The specific language-file should be available in the local-folder.<br>
**Example**<br>
`Config.Locale = 'en'` for the Language in english

### Config.CheckVersion
Set on/off whether a version check should be carried out on server start / script restart.<br>
Default: "true"<br>
`Config.CheckVersion = true`

### Config.CreateWaitingMessage
Set on/off the Waitingmessage after execute the command.<br>
With this message you have no standstill of the game.<br>
Default: "true"<br>
`Config.CreateWaitingMessage = true`

### Config.CreateWaitingTime
Set the time in Secounds, how long you wait to open the meun.<br>
min/default: 3 secounds<br>
`Config.CreateWaitingTime = 3`

### Config.WriteOwnReports
Set on/off weather do you want to exclude the self-written reports<br>
Default: "true"<br>
`Config.WriteOwnReports = true`

### Config.SupportMenus
A list of all information for the supportmenus.

#### Config.Skins[keyword]
The keyword is the name of the command and menuname.<br>
**Example**<br>
```
Config.Skins = {
  support = {},
}
```

#### Config.Skins[keyword].groups
Enter the names of the groups that are allowed to access the menu.<br>
**Example**<br>
```
Config.Skins = {
  support = {
    groups = {"t-sup","sup", "mod", "admin"},
  },
}
```

#### Config.Skins[keyword].templates
Here you have a list of all violations that can be used as a template for the reports. (max 25 chars)<br>
Write the title and a short description when you send the template.<br>
**Example**<br>
```
Config.Skins = {
  support = {
    groups = {"t-sup","sup", "mod", "admin"},
    templates = {
        { titel="Fail RP", text="One person commits Fail RP" },
        { titel="Power RP", text="A person commits Power RP" },
        { titel="Metagaming", text="A person commits metagaming" },
        { titel="Dead by bug", text="Died by a bug, need help" },
        { titel="Unconscious person - Invisible", text="I do not see an unconscious person" },
    }
  },
}
```

### Config.TeamMenu
A list of all information for the teammenu.

### Config.TeamMenu.command
Enter the name of the command here to access the team menu.<br>
Default: "reports"<br>
```
Config.TeamMenu = {
    command = "reports",
}
```

### Config.TeamMenu.permission
Enter the name of the permission here.<br>
Default: "grew_supsystem.teammenu"<br>
```
Config.TeamMenu = {
    command = "reports",
    permission = "grew_supsystem.teammenu"
}
```

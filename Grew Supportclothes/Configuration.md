# Wiki - Grew Supportclothes
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

### Config.Admingroup
Group name, for use of each command.<br>
`Config.Admingroup = 'admin'`

### Config.permission
Präfixname of the Permissionsname<br>
For more Information see [Permissions](#Permissions)!<br>
`Config.permission = "grew_supclothes"`

### Config.Skins
A list of all information for the command.

#### Config.Skins[keyword]
The keyword is the name of the command and group that is entered in the permission after the prefix.<br>
**Example**<br>
```
Config.Skins = {
  sup = {},
}
```

#### Config.Skins[keyword].jobgrade
If you use the job, you can enter here which jobrade the command executes.<br>
**Example**<br>
```
Config.Skins = {
  sup = {
    jobgrade = 0,
  },
}
```

#### Config.Skins[keyword].male / Config.Skins[keyword].female
The variables male/female is a list of skin variables<br>
in which your skin will be set if you use the command.<br>
**Example**<br>
```
Config.Skins = {
  sup = {
    jobgrade = 0,
    male = {
      ['tshirt_1'] = 15, ['tshirt_2'] = 0,
      ['torso_1'] = 22, ['torso_2'] = 1,
      ['arms'] = 41,
      ['bproof_1'] = 18, ['bproof_2'] = 0,
      ['pants_1'] = 31, ['pants_2'] = 0,
      ['shoes_1'] = 25, ['shoes_2'] = 0,
      ['chain_1'] = 0, ['chain_2'] = 0,
    },
    female = {
      ['tshirt_1'] = 36, ['tshirt_2'] = 1,
      ['torso_1'] = 48, ['torso_2'] = 0,
      ['arms'] = 44,
      ['bproof_1'] = 18, ['bproof_2'] = 0,
      ['pants_1'] = 30, ['pants_2'] = 0,
      ['shoes_1'] = 27, ['shoes_2'] = 0,
      ['chain_1'] = 0, ['chain_2'] = 0,
    },
  },
}
```

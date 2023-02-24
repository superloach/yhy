# yhy - yay why
explain install reason for yay packages

## usage
- `yhy [show]` - list packages not in the yhy database
- `yhy list` - list entries in the yhy database
- `yhy gone` - list uninstalled entries in the yhy database
- `yhy add <pkg> <reason>` - add/update an entry to the yhy database
- `yhy del <pkg>` - remove an entry from the yhy database
- `yhy rename <oldpkg> <newpkg>` - `yhy add <newpkg>`, `yhy del <oldpkg>`
- `yhy clean` - recursively uninstall packages without reasons
- `yhy shell <pkg>` - install the given package, run `${SHELL}`, then uninstall

## database
- json object found at `.local/share/yhy.json` (TODO: platform agnostic)
- keys are package names
- values are package reasons

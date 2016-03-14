# Bash Script

---
## Read variables

| key | info |
|-----|------|
| `read` `var` | get `var` from user |
| `read` `-s` | get `var` as a password (do not show input) |
| `read -p message` `var` | print message and get `var` from user |

---
## IF

```
if [ CONDITION ]; then
    do something...
elif [ CONDITION ]; then
    do something...
else
    do something...
```
### CONDITION

| key | info |
|-----|------|
| `val1` `-gt` `val2` | `val1` `>` `val2` |
| `val1` `-lt` `val2` | `val1` `<` `val2` |
| `val1` `-eq` `val2` | `val1` `=` `val2` |
| `-e` `file` | if `file` exists (Files, Device, Directory) |
| `-f` `file` | if `file` exists (Just Files) |
| `-d` `directory` | if `directory` exists |
| `-x` `command` | if `command` is executable file |

---
## Case

```
case CONDITION in
    STATEMENT1)
        do something...
        ;;
    STATEMENT2)
        do something...
        ;;
    *)
        do something
        ;;
esac
```




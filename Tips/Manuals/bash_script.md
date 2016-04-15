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

```bash
if [ CONDITION ]; then
    something...
elif [ CONDITION ]; then
    something...
else
    something...
```

```bash
if [ CONDITION ] &&/|| [CONDITION] ; then
    something...
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
## Bash seprator
Defalt is `space`

`IFS=':'`   -> Change to `:`        -> name=(ali:reza)

`IFS=$'\n'` -> Change to `New line` -> for i in ls

---
## Case

```bash
case CONDITION in
    STATEMENT1)
        something...
        ;;
    STATEMENT2)
        something...
        ;;
    *)
        something
        ;;
esac
```

---
## While

```bash
while [ CONDITION ]; do
    something...
done
```

---
## For

```bash
for VARIABLE in {RANGE}; do
    something...
done
```

```bash
for ((i=0;i<10;i++)); do
    something
done
```

### Samples

```bash
for i in {1..10}: do
```

```bash
for i in {1..100..5}; do
```  with 5 stes

```bash
for i in ali reza amir "amir ali"; do
    echo "hello $i"
done
```

```bash
name="ali reza amir"
for i in $name; do
    echo "hello $i"
done
```

```bash
IFS=':'
name="ali:reza:amir:mohammad reza"
for i in $name; do
    echo "hello $i"
done
```
---
### Date & Time

| key | info |
|-----|------|
| System hour | ``date +%H`` |
| System minute | ``date +%M`` |

---
### Exit status

| key | info |
|-----|------|
| Last command | `$?` ('0' or `any number` for error ) |

---
## Sample scripts

Convert and resize all png files to jpg and move to a new folder like Pictures2

```bash
IFS=$'\n'
clear
mkdir '$HOME/Pictures2'
c="1"
files=`ls $HOME/Pictures?*.png`
for i in $files; do
    convert "$i" -resize 50% "$HOME/Pictures2/$b.jpg"
    echo "$b.jpg created!"
    ((b++))
done
```

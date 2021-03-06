
---
## Atom Script
![atom script](https://i.github-camo.com/405fb492595dd819647af375b68c716fd862ee80/68747470733a2f2f636c6f75642e67697468756275736572636f6e74656e742e636f6d2f6173736574732f313639343035352f333232363230312f63343538616362632d663036372d313165332d383461302d6461323766653333346635652e676966)

### Installation
`apm install script`

### Usage

| Command               | Shortcut          |
| --------------------- | ----------------- |
| Run                   | ctrl + shift + b  |
| Run by line number    | ctrl + shift + j  |
| Close view            | Esc               |
| Kill proccess         | ctrl + q          |

---
## Atom Terminal Panel
![atom terminal panel](https://i.github-camo.com/7f4943042223363747bf02a01ae1289a9b9c26f6/68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f6973697339372f61746f6d2d7465726d696e616c2d70616e656c2f6d61737465722f7374617469632f6578616d706c652e676966)

### Installation
`apm install atom_terminal_pannel`

### Usage

| Command               | Shortcut          |
| --------------------- | ----------------- |
| Show terminal         | shift + enter     |
| Show and hide terminal| ctrl + `          |
| Close view            | Esc               |
| suggestions list      | ctrl              |

###  Example configuration
Use `./atom/terminal-commands.json` for config : 
```
{
    "_comment": "Package atom-terminal-panel: This terminal-commands.json file was automatically generated by atom-terminal-package. It contains all useful config data.",
    "commands": {
        "hello_world": {
            "description": "Prints the hello world message to the terminal output.",
            "command": [
                "echo Hello world :D",
                "echo This is",
                "echo example usage",
                "echo of the console",
                "echo arg[0] = %(0)",
                "echo arg[1] = %(1)"
            ]
        }
    },
    "actions": [
        ["test", "hello_world"]
    ],
    "toolbar": [
        [
            "foo",
            "bar",
            "Ecce est foo-bar exemplum!"
        ],
        [
            "clear",
            "clear",
            "Clears the console output."
        ],
        [
            "info",
            "info",
            "Prints the terminal welcome message."
        ],
        [
            "all available commands",
            "memdump",
            "Displays all available builtin commands. (all commands except native)"
        ]
    ],
    "rules": {
        "\\b[A-Z][A-Z]+\\b": {
            "match": {
                "flags": [
                    "g"
                ]
            },
            "css": {
                "color": "gray"
            }
        },
        "(error|err):? (.*)": {
            "match": {
                "matchLine": true,
                "replace": "%(label:error:text:Error) %(0)"
            },
            "css": {
                "color": "red",
                "font-weight": "bold"
            }
        },
        "(warning|warn|alert):? (.*)": {
            "match": {
                "matchLine": true,
                "replace": "%(label:warning:text:Warning) %(0)"
            },
            "css": {
                "color": "yellow"
            }
        },
        "(note|info):? (.*)": {
            "match": {
                "matchLine": true,
                "replace": "%(label:info:text:Info) %(0)"
            },
            "css": {}
        },
        "(debug|dbg):? (.*)": {
            "match": {
                "matchLine": true,
                "replace": "%(label:default:text:Debug) %(0)"
            },
            "css": {
                "color": "gray"
            }
        }
    }
}
```

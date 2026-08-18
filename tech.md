# Cheatsheet for Tech

## Linux
| Commands | Effects / Notes |
|--- |--- |
| Ctrl U | Erases the whole line |
| Ctrl W | Erases the last word |
| Ctrl Y | Brings back erased thing |
| top | Shows system processes |
| sudo apt update | Updates the list of available packages/versions from remote repositories |
| sudo apt upgrade -y | Upgrades all installed packages (applications, libraries, tools, and dependencies |
| sudo apt install -y <package> | Installs package named <package> |

## tmux
| Commands | Effects / Notes |
|--- |--- |
| Ctrl B | Starts talking to tmux with commands that follow |
| tmux new -s buidl | Opens a new tmux session named buidl |
| tmux attach | Attaches (i.e. reconnects) to the most recently used existing session |
| tmux attach -t buidl | Attaches to a specific target session named buidl |
| tmux ls | Lists all active sessions currently managed by tmux |

## Git
| Commands | Effects / Notes |
|--- |--- |
| git branch -M main | Renames default branch (from master) to main; -M flag stands for "force move", i.e. force rename |
| git remote add origin <GitHub link> | Links the local repo to GitHub link |
| git add <filename> | Stages the file |
| git commit -am "message" | (Adds and) commits the staged file(s) with commit message |
| git push -u origin main | Pushes upstream to the main branch of the origin |

## Vim
| Shortcuts | Effects / Notes |
|--- |--- |
| G | Navigates to the end of file |
| gg | Navigates to the beginning of file |
| $ | Navigates to the end of line |

## Markdown
| Effects | Syntaxes |
|--- |--- |
| Rendering Syntax Symbols | \`\*\*bold\*\*\` or `\*\*bold\*\*` |
| Heading | # H1<br>## H2<br>### H3 |
| Bold | `**bold**` |
| Italic | `*italic*` |
| Blockquote | > blockquote |
| Ordered List | 1. First<br>2. Second<br>3. Third |
| Unordered List | - First<br>- Second<br>- Third |
| Code (inline) | \`code\` |
| Code (block) | \`\`\`<br>a = 1<br>\`\`\` |

Software / Tools:

- uv (AstralDocs for packages)
- ruff / mypy linters
- iTerm2
- Starship

Libraries:

Python testing:
- pytest
- mypy

Python utils:
- itertools
- more itertools

Other things!
- https://github.com/charmbracelet especially glow, lipgloss

Key Files to keep in mind:

`pyproject.toml` → Contains dependencies (+ versions) and key project details, such as version and author.

`.lock` files act as a definitive location for dependency versions and cool details that enable accurate dependency installation & can act as an important artifact during debugging.


## Commands

### Git :github-colored:

`git add --patch` → add code changes to staging individually, while viewing changes. Use `git add .`  instead to stage all modified files, or replace `.` with a specific file.

`git commit` → opens the commit message/title thingy in a new window. Use `i` to enter insert mode, and then `esc` to escape insert mode (use `u` to undo something). `shift + z` twice to save and quit. `shift + z` and `shift + q` will exit without saving. 

`git diff --cached` → view changes since last commit.

`git checkout -b name-of-branch` → create a new branch and `cd` into it. This is a combination of `git branch` and `git checkout` (create branch, “checkout”/go to branch). You can use `git checkout -` to go to your most recent branch.

### Other! 🎉

`pwd` → print working directory

`xargs` → adding this to a command runs the command in parallel (across multiple processors).

`docker ps -aq | xargs echo --` → print container IDs and basic info.
`docker ps -aq | xargs docker rm -f` → `docker ps` finds container IDs, `docker rm` removes those containers. Alter the `docker rm` command if you want to delete something specific, or run it separately.

`docker exec -it <container name> bash` → enter bash shell (terminal) for that container.

`ctrl + w` → backspace last word/segment in terminal

## Key Shortcuts ⌨️

`~` → refers to your user home. Use `cd` to change directory to your home (or `cd ~` )

`shift + ->` → this will highlight right of your cursor. Use other arrow keys as directions :) 

`shift + cmd + ->` → highlights entire line/document, depending on arrow key direction (up/down for highest line/lowest line, left/right for far left and right!). Using `option`/`alt` goes to next word / special char.

`shift + tab` → removes an indent in VSCode

`ctrl + d` → in VSCode, adds cursors in lines that match what you have highlighted. Really useful for deleting comments in one big go. Use `esc` to go back to one cursor, and `cmd + shift + l` to highlight all possible matches (i think)

`ctrl + shift + p` → in VSCode, brings up the command panel. Backspace `>` to use it as a file directory!

`ctrl + ~` → in VSCode, brings up the terminal. Use the short cut again to focus or close terminal.

`cmd + ->` → in VSCode (and other places?) moves the cursor to the end of the line or document, depending on arrow key used.

`cmd + b` → removes the files panel in VSCode. Use again to bring it back.

`cmd + L` → selects whole line.

`alt + ->` → moves lines up or down, depending on arrow keys (use up/down, not left/right).

`ctrl + r` → open recent folder.
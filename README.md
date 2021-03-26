# Shrug

A recreation of Git for local file backups written in POSIX-compatible Shell (Dash).

# Features

# shrug-init 
Initalises a .shrug file
# shrug-add <filenames>
Add files to .shrug/index
# shrug commit [-a] -m <message>
- Adds a copy of all index files to commit<number>. Where <number> is sequentually incremented from 0.
- [-a] flag will replace all files in index from repository before committing
# shrug-log
Showcases all commits and their messages
# shrug-show <commit-number>:<filename>
Prints the content of the specified file
# shrug-rm [--force] [--cached] <filenames>
- Remove specified files from index or, index and current directory
- [--cached] removes file from only index
- If the file's deletion will cause user to lose work, let them know
- [--force] removes not let the user know about losing their work
# shrug-status
Shows the current status of files in current directory, index and repository

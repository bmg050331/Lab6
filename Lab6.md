# Lab6
## Version Control
It's essential to use a version control system for software development and other documentation works.

Making copies takes too much space.

- Changes: storing data as changes to the base version.
- Snapshots: storing data as snapshots.
## Git Config
Git configurations are stored in three levels.
- System level: --system option. Affects all uses and repositories on the system. file: /etc/gitconfig
- Global level: --global option. Affects all repositories of a current user. file:~/.config/git/config
- Local level: --local option. Specific to the current repository. file: .git/gitconfig
### Local, Centralized, Distributed Version Control
- Local: only in my computer.
- Centralized: Central VCS Server has version data. If Central VCS Server gets down, then data has gone.
- Distributed: Both Server computer and Local computer has version data.
### Three States in Git
- Modifed: working Directory > (stage Fixes) to Staged.
- Staged: Staging Area > (commit) to Committed.
- Committed: .git directory.
### $ git init
Initializing a new repository in working directory.
### $ git status
Check status like commits, untracked files of repository.
### $ git add [file_name]
Adding a new file to be staged(tracked).
- $ git add .: adding all files to be staged(tracked).
### $ git rm --cached [file_name]
Unstaging al file.
### Ignoring a file
Making [.gitignore]
- $ ignore all .a files: *.a
- $ ignore all files in any directory named build: build/
- $ ignore doc/notes.txt, but not doc/server/arch.txt: doc/*.txt
- $ ignore all .pdf files in the doc/ directory and any of its subdirectories: doc/**/*.pdf
### git commit -m "commit message"
Commit working files.
- $ git log: check commit history.
### git branch -m master main
Change branch name.

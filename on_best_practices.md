# On Best Practices for Analysts and Analytics Engineers

## Bullet Lessons
- Prefer main to master for default branch
- Prefer repos be started from a template or framework (i.e. dbt init command)
- Prefer private repos in a github organization, unless open-source
- Prefer personal accounts, added to the github organization
- Learn with the command line; relying on a GUI may not provide a deep understanding of version control.
    - Maybe you're fine with that. I wasn't.
- Linters are your friend. I like [Black](https://black.readthedocs.io/en/stable/index.html) for Python, [sqlfluff](https://docs.sqlfluff.com/en/stable/index.html) for SQL, [yamllint](https://docs.sqlfluff.com/en/stable/index.html) for YAMLs.
    - precommit hooks to run the linter before you're allowed to actually commit your code can be really helpful if you forget to lint your changes

## Development lifecycle... Or How to Do a Pull Request
- Clone the repo locally
- `$ git pull` to ensure your local copy is up to date with the remote
- `$ git co -B <branch-name>` to create a new branch to make your changes on 
    - Name the branch in some systematic way (i.e. issue/ticket id, issue id + issue name, contributor + purpose, project phase/task, etc.)
- Develop on your new branch, not main. Make any and all changes.
    - Remember to test your changes
    - If working in SQL, test for duplicated Ids/keys (uniqueness) as well as if the query runs
- start a commit message with the name of the issue/branch
- once all changes are complete and tested, `$ git push origin <branch-name>`. This pushes your changes from the local branch to the remote repo
- Go to GitHub and complete your Pull Request
    - Have the Pull Request reviewed by a teammate before merging
    - Have the author merge the PR and delete the branch
# Background and General Tips

## On Commit Messages
Write commit messages. They'll help future you, and your team will thank me.

These are good commit messages, taken from another learning project of mine:
> main: corrected remaining models based on example, ran/built models
>
> main: attempt at models practice, corrected stg_stripe__payments based on example
>
> main: did not commit with message from course, formatted readme
>
> dbt materialization actually solved, models organized, onto commits lesson

These summarize the changes, document what you were thinking or working on. These include details that will help someone step through the history of the project, if required for a bug hunt.

These are bad commit messages, some of which I've written and some of which I've witnessed:
> LNR-314: typos again
>
> LNR-159: fixes
>
> potato function
>
> max mustermann magic
>
> cut my life into pieces
>
> asdfasdf
>
> ^,...,^

These don't explain the what. Nor the why. Nor the how. Nor what the author intended the committed code to do.

# LAB 1 through LAB 10

3. the basic navigation commands you'll need:
   - `cd file_path` this is how you get around the file folders on your machine
   - `cd ..` this goes up a level
   - `git status` will let you know what changes are in what state
7. `$ git add -A` is your friend once your project grows in size. For now, adding each file individually is good practice with bash & git.
8. *"If you omit the -m flag from the command line, git will pop you into the editor of your choice."* This means you'll likely get dumped into vi or vim. It's not friendly to beginners.
   - Write the comment on the first line without a `#`    
   - Then hit escape
   - Then type `:wq` (to write & quit). **This is how you survive vim.**

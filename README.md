Initialization

* Start by running `bug config [user] [pass] [site] [user_id]`. Your user id takes some HTML inspection to get. Kinda dumb. Hoping to come up with a better way.
* Run `bug fetch` and `bug fetch latest`. This will set you up with the highest priority and most recent bugs.
* Run `bug todo? | head -5` to see the most important bugs to tackle.
* If you do not use `vi`, modify `~/.bugsrc` and change the editor.

If you know a bug is important, mark it with `bug important ####`.
If you know a bug is ignorable, mark it with `bug ignore ####`.
If you want to know what to work on next, run `bug next?`

Commands (`bug command argumentsi`):

* fetch / pull [latest]: Get a new list from the server. Defaults to priority sort. [latest] uses created_on.
* update: Get a new list by updated_on from the server.
* todo?: List all todo items, in todo priority.
* next?: Return with the next bug to fix.
* status: List of all tracked bugs, with summaries.
* filter / category [category]: Same as status, except by category.
* clear: Untrack all bugs.
* clean: Untrack all Closed bugs.
* track / add: (List) Serialize and add to status list.
* untrack / remove: (List) Remove from status list.

Bug-level commands (`bug command bugid arguments`):

* annotate / note [note]: Add a personal note locally.
* edit: Edit the local personal note.
* notes: View the local personal note.
* categorize [category]: Set a local categorization.
* fixed / nofix / repro / later / comment [note]: Update server with new information.
* todo / enqueue: Add to local todo list.
* dequeue: Remove from local todo list.
* important / unimportant: Located at top of status list.
* ignore / unignore: Ignored bugs are never Todo and located at the bottom of the status list.
* postpone: Push a bug downwards.
* open: Open the Redmine page.
* info / journals: Display all journals. (Not implemented.)

Todo List priority:

* Marked important locally.
* Enqueued to Todo List.
* Prioritized as Urgent / High.
* Marked  as Severe / Major.
* Most Journal entries.
* Most recently updated.

Commands (bug command arguments):

* fetch / pull / update [latest]: Get a new list from the server.
* todo?: List all todo items, in todo priority.
* next?: Return with the next bug to fix.
* status: List of all tracked bugs, with summaries.
* filter / category [category]: Same as status, except by category.
* clear: Untrack all bugs.
* clean: Untrack all Closed bugs.
* track / add: (List) Serialize and add to status list.
* untrack / remove: (List) Remove from status list.

Bug-level commands (bug command bugid arguments):

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

Script to add taskwarrior task from mutt prompting the user for a description and annotate the task with the message's message-id.

add something like this to a muttrc file:

```muttrc
macro index,pager ,t '<pipe-message>mutt2task<enter>'
```

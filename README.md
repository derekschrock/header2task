Script to add or list taskwarrior task from mutt prompting the user for a description and annotate the task with the message's message-id.

add something like this to a muttrc file:

```muttrc
macro index,pager ,ta '<pipe-message>mutt2task add<enter>'
macro index,pager ,tf '<pipe-message>mutt2task find<enter>'
```

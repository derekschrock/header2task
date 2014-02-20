Script to add or list taskwarrior task from mutt prompting the user for a description and annotate the task with the message's message-id.

add something like this to a muttrc file:

```muttrc
macro index,pager ,ta '<pipe-message>mutt2task add<enter>'
macro index,pager ,tA '<pipe-message>mutt2task annotate<enter>'
macro index,pager ,tf '<pipe-message>mutt2task find<enter>'
macro index,pager ,td '<pipe-message>mutt2task done<enter>'
```

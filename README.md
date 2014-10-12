Script to add or list taskwarrior task from mutt, prompting the user for a description and annotate the task with the message's message-id, from, and subject headers.

With mutt2task in PATH add something like this to a muttrc file:

```muttrc
macro index,pager ,ta '<pipe-message>mutt2task add<enter>F'
macro index,pager ,tA '<pipe-message>mutt2task annotate<enter>'
macro index,pager ,td '<pipe-message>mutt2task done<enter>'
macro index,pager ,tf '<pipe-message>mutt2task find<enter>'
macro index,pager ,tj '<pipe-message>mutt2task join<enter>F'
macro index,pager ,tp '<pipe-message>mutt2task project<enter>'
macro index,pager ,te '<pipe-message>mutt2task edit<enter>'
```

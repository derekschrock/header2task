Script to manipulate taskwarrior tasks when passed a raw email via stdin.
Annotating the task with the email's message-id, from, and subject headers.

With header2task in PATH add something like this to a muttrc file:

```muttrc
macro index,pager ,ta '<pipe-message>header2task add<enter>F'
macro index,pager ,tA '<pipe-message>header2task annotate<enter>'
macro index,pager ,td '<pipe-message>header2task done<enter>'
macro index,pager ,tf '<pipe-message>header2task find<enter>'
macro index,pager ,tj '<pipe-message>header2task join<enter>F'
macro index,pager ,tp '<pipe-message>header2task project<enter>'
macro index,pager ,te '<pipe-message>header2task edit<enter>'
```

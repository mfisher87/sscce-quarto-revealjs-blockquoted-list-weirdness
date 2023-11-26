# SSCCE

When placing a list in a blockquote, it renders as an incremental list. If I want a
quoted list, I need to specify that explicitly. I haven't found any documentation
supporting this behavior, so maybe it's a bug?

Tested with _Quarto_ versions:

* 1.3.450
* 1.3.433
* 1.4.510


## Symptoms

* Blockquoted list renders as incremental list
* Blockquoted list renders without blockquote style
* When rendered after an un-quoted list, the two elements render unexpectedly side-by-side
* When paragraph text is included in the blockquote, the unexpected behavior goes away


## Repro

`quarto preview` in this directory

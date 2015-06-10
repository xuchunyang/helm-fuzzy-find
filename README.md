# helm-fuzzy-find - Find file using Fuzzy Search

*Author:* Chunyang Xu <xuchunyang56@gmail.com><br>
*Version:* 0.1<br>
*URL:* [https://github.com/xuchunyang/helm-fuzzy-find](https://github.com/xuchunyang/helm-fuzzy-find)<br>

`helm-fuzzy-find.el` is the Helm interface for the `fuzzy-find` command
line program (`https://github.com/silentbicycle/ff`), you can use it to
search files under a directory using Fuzzy Search.

When you want to search files only according to their base-names, use the
notable `find` program and its helm interface `helm-find` instead, but if
you also use their parent directory names, i.e., full absolute path name of
a file or directory, `fuzzy-find` is better.  You can read `fuzzy-find`'s
homepage and manual page to learn more about these.

Installation
============

To install, make sure this file is saved in a directory in your `load-path`,
and add the line:

      (require 'undo-tree)

to your Emacs initialization file.

Usage
=====

M-x helm-fuzzy-find to Launch `helm-fuzzy-find` from current buffer's
directory, if with prefix argument, you can choose a directory to search.

Like `helm-find`, you can also launch `helm-fuzzy-find` from
`helm-find-files` (it usually binds to <kbd>C-x C-f</kbd> for helm users) by typing
<kbd>C-c C-/</kbd>


---
Converted from `helm-fuzzy-find.el` by [*el2markdown*](https://github.com/Lindydancer/el2markdown).

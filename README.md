[![MELPA](http://melpa.org/packages/helm-fuzzy-find-badge.svg)](http://melpa.org/#/helm-fuzzy-find)

# helm-fuzzy-find

`helm-fuzzy-find.el` is a helm extension for the
[`fuzzy-find`](https://github.com/silentbicycle/ff) command line program, you
can use it to search files under a directory using Fuzzy Search.

When you want to search files only according to their base-names, use the
notable `find` program and its helm interface `helm-find` instead, but if
you also use their parent directory names, i.e., full absolute path name of
a file or directory, `fuzzy-find` is probably better.  You can read `fuzzy-find`'s
homepage and manual page to learn more about these.

## Installation

To install, make sure this file is saved in a directory in your `load-path`,
and add the line:

```elisp
(require 'helm-fuzzy-find)
```

to your Emacs initialization file.

## Usage

M-x helm-fuzzy-find to launch `helm-fuzzy-find` from the current buffer's
directory, if with prefix argument, you can choose a directory to search.

Like `helm-find`, you can also launch `helm-fuzzy-find` from
`helm-find-files` (it usually binds to <kbd>C-x C-f</kbd> for helm users) by typing
<kbd>C-c C-/</kbd> (you can customize this key by setting `helm-fuzzy-find-keybind`).

## Note

To use `helm-fuzzy-find`, you need to know the format (**NOT** regexp) of the
query string of `fuzzy-find`, especially the meaning of "/" character and "="
character, refer to its manual page for more info.

To install `fuzzy-find` on Mac OS X via MacPorts:

```console
$ sudo port install fuzzy-find
```

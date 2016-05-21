[![Built with Spacemacs](https://cdn.rawgit.com/syl20bnr/spacemacs/442d025779da2f62fc86c2082703697714db6514/assets/spacemacs-badge.svg)](http://github.com/syl20bnr/spacemacs)
[![License (GPL version 2)](https://img.shields.io/badge/license-GNU%20GPL%20version%202-blue.svg?style=flat-square)](http://opensource.org/licenses/GPL-2.0)
[![MELPA](https://melpa.org/packages/nlinum-relative-badge.svg)](https://melpa.org/#/nlinum-relative)

# nlinum-relative
Emacs relative line number based on nlinum-mode

# Preview
![nlinum-relative](https://cloud.githubusercontent.com/assets/5436704/15207154/cafea3fa-1856-11e6-8f01-26a3832bf1fd.gif)

# Why this
`nlinum` is faster than `linum` because of its use of [jit-lock](https://github.com/jwiegley/emacs-release/blob/master/lisp/jit-lock.el). `nlinum-relative` only redisplays line numbers when idle which is much more smoother especially with big files.

# Install

This package is available on MELPA as `nlinum-relative`. 

```lisp
(use-package nlinum-relative
    :config
    ;; something else you want
    (nlinum-relative-setup-evil)
    (add-hook 'prog-mode-hook 'nlinum-relative-mode))
```

# Spacemacs

Use `develop` branch's `nlinum` layer.

# Usage

``` lisp
(require 'nlinum-relative)
(nlinum-relative-setup-evil)                    ;; setup for evil
(add-hook 'prog-mode-hook 'nlinum-relative-mode)
(setq nlinum-relative-redisplay-delay 0)      ;; delay
(setq nlinum-relative-current-symbol "->")      ;; or "" for display current line number
(setq nlinum-relative-offset 0)                 ;; 1 if you want 0, 2, 3...
```


# Related

- [coldnew/linum-relative: display relative line numbers in the left margin in emacs](https://github.com/coldnew/linum-relative)

  Some code from here

- [GNU ELPA - nlinum](https://elpa.gnu.org/packages/nlinum.html)

  Based on this

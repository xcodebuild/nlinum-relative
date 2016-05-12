[![Built with Spacemacs](https://cdn.rawgit.com/syl20bnr/spacemacs/442d025779da2f62fc86c2082703697714db6514/assets/spacemacs-badge.svg)](http://github.com/syl20bnr/spacemacs)

# nlinum-relative
Emacs relative line number besed on nlinum-mode

# Usage

``` lisp
(require 'nlinum-relative)
(nlinum-relative-setup-evil) ;; setup for evil
(add-hook 'prog-mode-hook 'nlinum-relative-mode)
(setq nlinum-relative-redisplay-delay 0.1) ;; delay
(setq nlinum-relative-current-symbol "->") ;; or "" for current line number
```


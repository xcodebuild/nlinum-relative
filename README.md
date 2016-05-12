[![Built with Spacemacs](https://cdn.rawgit.com/syl20bnr/spacemacs/442d025779da2f62fc86c2082703697714db6514/assets/spacemacs-badge.svg)](http://github.com/syl20bnr/spacemacs)

# nlinum-relative
Emacs relative line number besed on nlinum-mode

# Preview
![nlinum-relative-evil](https://cloud.githubusercontent.com/assets/5436704/15206239/2d7ed48e-1850-11e6-9a6c-254694fcc1d6.gif)

# Usage

``` lisp
(require 'nlinum-relative)
(nlinum-relative-setup-evil) ;; setup for evil
(add-hook 'prog-mode-hook 'nlinum-relative-mode)
(setq nlinum-relative-redisplay-delay 0.1) ;; delay
(setq nlinum-relative-current-symbol "->") ;; or "" for current line number
```

# Spaecmacs

This package is still not available at MELPA for now. You can install it by 

```lisp
;; add into packages
(nlinum-relative :location (recipe
                                :fetcher github
                                :repo "CodeFalling/nlinum-relative"
                                ))
                                
(use-package nlinum-relative
    :config
    ;; something else you want
    (nlinum-relative-setup-evil)
    (add-hook 'prog-mode-hook 'nlinum-relative-mode))
```


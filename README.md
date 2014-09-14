# Overview
`anything-sage` provides an [anything](https://github.com/emacs-anything/anything)
 source for
[sage-shell-mode](https://github.com/stakemori/sage-shell-mode).

This package is similar to
[helm-sage](https://github.com/stakemori/helm-sage).

# Installation
You will be able to install `anything-sage` from
[MELPA](https://github.com/milkypostman/melpa.git) by package.el
(`M-x package-install anything-sage`).

# Setting
Call `anything-sage-shell` by `M-x anything-sage-shell`
or bind `anything-sage-shell` to a key, e.g.

```lisp
(defun anything-sage-set-up ()
  (local-set-key (kbd "C-c C-i") 'anything-sage-shell))
(add-hook 'sage-shell-mode-hook 'anything-sage-set-up)
```

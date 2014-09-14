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

# An example for Setting
Bind `anything-sage-shell`,
`anything-sage-shell-describe-object-at-point` and
`anything-sage-command-history` to some keys, e.g.:
```lisp
(defun anything-sage-set-up ()
  (local-set-key (kbd "C-c C-i") 'anything-sage-shell)
  (local-set-key (kbd "C-c C-d") 'anything-sage-shell-describe-object-at-point)
  (local-set-key (kbd "M-r") 'anything-sage-command-history))
(add-hook 'sage-shell-mode-hook 'anything-sage-set-up)
```

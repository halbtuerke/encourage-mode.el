[![MELPA](http://melpa.org/packages/encourage-mode-badge.svg)](http://melpa.org/#/encourage-mode)

# encourage-mode.el

This Emacs minor-mode is inspired by https://github.com/Haacked/Encourage.

After installation use `encourage-mode` to activate the mode. From now on you
get an encouragement every time you save a buffer.

## Installation

If you are using [use-package](https://github.com/jwiegley/use-package) then
just add the following to your Emacs config:

```lisp
(use-package encourage-mode
  :ensure t
  :config
  ;; Activate encourage-mode
  (encourage-mode t))
```

## Modify encouragements

Either use the customize interface (`M-x customize-group encourage-mode`) or put
the following in your config to add more encouragements to the default set
(thanks to @oylenshpeegul for the inspiration):

```lisp
(setq encourage-encouragements
  (nconc encourage-encouragements
    '("Excellent!"
      "Hot sandwich!"
      "Mein lieber Schwan!"
      "Nice!"
      "Outstanding!"
      "Ossum!"
      "Quit it!"
      "Scwhanky!"
      "Spanakopita!"
      "SPHINX!"
      "Supergood!"
      "Sweet!"
      "That is so Batman!"
      "Well done, you!"
      "Whoa!")))
```

# clay.el
Emacs binding for the Clojure [Clay](https://scicloj.github.io/clay/) tool

## Usage

Using [use-package](https://github.com/jwiegley/use-package), you may load the package as follows:

```elisp
(use-package clay
  :straight (clay
             :type git
             :host github
             :repo "scicloj/clay.el"))
```

The package offers the following functions, that you may wish to create keybindings for:
|name|function|
|--|--|
|`clay/start`|start clay if not started yet|
|`clay/make-ns-hmtl`|save clj buffer, render it as html, and show that in the browser view|
|`clay/make-ns-quarto-html`|save clj buffer, render it as quarto, render that as html, and show that in the browser view|
|`clay/make-ns-quarto-revealjs`|save clj buffer, render it as quarto, render that as a revealjs slideshow, and show that in the browser view|
|`clay/make-last-sexp`|render the last s-expression|
|`clay/make-defun-at-point`|render the [defun-at-point](https://www.emacswiki.org/emacs/ThingAtPoint)|


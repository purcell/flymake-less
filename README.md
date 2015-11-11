flymake-less.el
===============

An Emacs flymake handler for syntax-checking LESS CSS code.

Note that you probably want to be using
[flycheck](http://www.flycheck.org/) instead.

Installation
=============

If you choose not to use one of the convenient packages in
[Melpa][melpa] and [Marmalade][marmalade], you'll need to add the
directory containing `flymake-less.el` to your `load-path`, and then
`(require 'flymake-less)`. You'll also need to install
[less-css-mode](https://github.com/purcell/less-css-mode) and
[flymake-easy](https://github.com/purcell/flymake-easy).

Usage
=====

Add the following to your emacs init file:

    (require 'flymake-less)
    (add-hook 'less-css-mode-hook 'flymake-less-load)

Beware that lessc can be quite slow, so there can be a significant lag
between editing and the highlighting of resulting errors.

[marmalade]: http://marmalade-repo.org
[melpa]: http://melpa.org

<hr>

[![](http://api.coderwall.com/purcell/endorsecount.png)](http://coderwall.com/purcell)

[![](http://www.linkedin.com/img/webpromo/btn_liprofile_blue_80x15.png)](http://uk.linkedin.com/in/stevepurcell)

[Steve Purcell's blog](http://www.sanityinc.com/) // [@sanityinc on Twitter](https://twitter.com/sanityinc)


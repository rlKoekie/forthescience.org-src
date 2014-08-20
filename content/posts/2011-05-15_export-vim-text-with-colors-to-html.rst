Export vim text (with colors) to HTML
#####################################
:date: 2011-05-15 11:34
:author: Stefano
:category: Computer Science
:tags: HTML, vim
:slug: export-vim-text-with-colors-to-html

Vim is a great, great programming tool. Even after years of experience
with it you still get to discover, either by change or by sharing,
fantastic tips to make an impossible task incredibly easy.

It is the case with my recent problem of exporting the visual aspect of
vim (as from terminal) to an HTML document, including the highlight
colors. How to do it? Well, I tried `pygments <http://pygments.org>`_
and it's really great, but I `asked on
SuperUser <http://superuser.com/questions/212227/copy-vim-text-colors-included>`_
for alternative methods. It appears that Vim supports this natively.
Just issue

::

    :TOhtml

to Vim, and it will create and open an HTML file containing what you see
in your terminal. A big thank you to user
`progo <http://superuser.com/users/49046/progo>`_ for this tip.

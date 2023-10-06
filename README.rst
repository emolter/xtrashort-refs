Simple LaTeX Hack for Very Condensed References
-----------------------------------------------

Nobody knows why some institutions still force you to compress references in order to fit on a page for proposals and the like. Some institutions have come around to excluding references in page limits, but for those that haven't, there is this repository.

Gallery
-------

Look at xtrashort-refs-example.pdf to see how the references render.

Usage options
-------------

* Clone the repository, and test that it is working using ``python3 texcompile.py xtrashort-refs-example``.
* Copy only the .bst file, then copy-paste relevant lines the .tex file into whatever latex you are already writing.

What we did, and how to hack our hack
-------------------------------------

Neither of us had any idea how to modify .bst files beforehand. The main changes we made from the original apalike.bst were

* Rewrote the function `format.names` to display only the first author. BTW, it is easy to get the first, say, 5 authors; look for the line in ``format.names`` that says ``numnames %1`` and simply change the 1 to a 5
* Removed titles for articles by just making all the strings empty in ``FUNCTION {format.title}``
* Added ``FUNCTION {software}`` and made its title distinct from article-type titles so that it would be displayed. As a disclaimer, we have no idea how software is supposed to appear in APA guidelines.

This was a quick Friday afternoon hack at dotAstronomy 12.

How to contribute
-----------------
Go ahead and do the typical contribution fork and PR workflow. Some known things that still don't work well are listed on the Issues page.

Disclaimer
----------

This was intended as a quick hack example.  We only tested it on our machines, with our Python versions and LaTeX distributions. Your mileage may vary.

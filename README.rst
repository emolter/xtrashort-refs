Simple LaTeX Hack for Very Condensed References
-----------------------------------------------

Nobody knows why some institutions still force you to compress references in order to fit on a page for proposals and the like. Some institutions have come around to excluding references in page limits, but for those that haven't, there is this bst file.

Gallery
-------

Look at xtrashort-refs-example.pdf to see how the references render.

Usage options
-------------

* clone the repository, test that it is working using ``python3 texcompile.py xtrashort-refs-example``
* copy only the .bst file, then copy-paste relevant lines the .tex file into whatever latex you are already writing.

What we did
-----------

Neither of us had any idea how to modify .bst files beforehand. The main changes we made from the original apalike.bst were

* 
* 

How to contribute
-----------------
Go ahead and do the typical contribution fork and PR workflow. Some things that still don't work well are

*
*

Disclaimer
----------

This was intended as a quick hack example.  I only tested it on my machine, with my Python version and my LaTeX distribution. Your mileage may vary.

Thank You
---------
Shout-out to @yasmeenasali who helped me figure out how to do this.

This example, by [John R Gilbert](http://cs.ucsb.edu/~gilbert)
was originally posted at:
<http://cs.ucsb.edu/~gilbert/cs111/latex_example/>

To generate `CS111_latex_example.pdf` from `CS_111_latex_example.tex`,
say the following at the Linux command line:

```
pdflatex CS111_latex_example
pdflatex CS111_latex_example
```

# NOTE 1:

You really do have to run `pdflatex` twice as above.
The first time it just figures out references and labels,
and the second time it fills them in.

# NOTE 2:

You'll get an error message about a missing reference file.
That's because this example includes a `references.bib` file
that contains a bibliography.  Your homework reports probably
won't, so this won't be an issue.  However, to get the 
bibliography to come out right, you need to use `bibtex`
as follows:

```
pdflatex CS111_latex_example
bibtex CS111_latex_example

pdflatex CS111_latex_example
pdflatex CS111_latex_example
```
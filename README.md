# bibliography

This repository hosts .bib files with bibliographic databases for LaTeX papers written by our Lab's members. 

These .bib files can be 

* just copied into the directory where you are writing your .tex article, or better:

* shared by multiple LaTeX sources if using the biblatek & biber instead than the old bibtex. In this case remember to
  * use *biber* instead of *bibtex* in your IDE build toolchain (ex in Texniccenter go to Build/Define build profiles... menu)
  * use the URL that points to the *raw* version of the .bib file on this GIT, 
    in the \addbibresource command, as in the following example:

```
\documentclass{article}

\usepackage[backend=biber]{biblatex}
\addbibresource[location=remote]{"https://raw.githubusercontent.com/DigitalDynamicsLab/bibliography/master/BibFEM.bib"}

% Note the "https://raw.githubusercontent.com/..." ,  it points to the *raw* version of the bib files.

\begin{document}

This is cited in: \cite{cosserat1909}. Good.

\printbibliography

\end{document}
```

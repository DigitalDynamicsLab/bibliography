# bibliography

This repository hosts .bib files with bibliographic databases for LaTeX papers written by our Lab's members. 

These .bib files can be 

* just copied into the directory where you are writing your .tex article, or better:

* shared by multiple LaTeX sources if using the biblatek & biber instead than the old bibtex: 

```
\documentclass{article}
\usepackage[style=authoryear,backend=biber]{biblatex}
\addbibresource[location=remote]{https://github.com/DigitalDynamicsLab/bibliography/XXXXYYYY.bib}
\begin{document}
\cite{Box1972}
\printbibliography
\end{document}
```

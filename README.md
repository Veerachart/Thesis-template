This is just a simple template (or maybe better to call an example) of a Master/PhD thesis. The template is made based on the template taken from Department of Precision Engineering, Graduate School of Engineering, The University of Tokyo, but should be adaptable to match requirements by any department/university.

Mainly this is designed for making the title page in Japanese, but the rest of the content is in English. \texttt{platex} from W32TeX or TeXLive is needed. Please find the installation guide (mostly in Japanese) to install one of these packages (easier in Linux.) If Japanese is not required , changing all the texts in the title page and you can use normal \LaTeX\ to compile.

To compile this,

```
platex Thesis_template.tex
bibtex Thesis_template.aux
bibtex pub.aux
platex Thesis_template.tex
platex Thesis_template.tex
dvipdfmx Thesis_template.dvi
```

bibtex is needed only when the bib files have been changed, otherwise only once or twice of platex and once of dvipdfmx should be enough to generate the correct output with correct references. (or use pdfplatex)

If Japanese is not needed, you can also use latex instead of platex.

Probably it would be better to make it into .sty file, but I don't have time and energy to do it now.

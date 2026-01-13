all: NumericalMethods.pdf

NumericalMethods.pdf: NumericalMethods.tex chapitre*.tex references.bib
	pdflatex NumericalMethods.tex
	bibtex NumericalMethods
	pdflatex NumericalMethods.tex
	pdflatex NumericalMethods.tex

clean:
	rm -f *.aux *.log *.out *.toc *.bbl *.blg *.fls *.fdb_latexmk NumericalMethods.pdf

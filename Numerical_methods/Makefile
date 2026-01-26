MAIN = NumericalMethods

.PHONY: all clean

all:
	pdflatex -interaction=nonstopmode $(MAIN).tex
	bibtex $(MAIN)
	pdflatex -interaction=nonstopmode $(MAIN).tex
	pdflatex -interaction=nonstopmode $(MAIN).tex
	rm -f *.aux *.log *.toc *.out *.bbl *.blg *.fls *.fdb_latexmk

clean:
	rm -f *.aux *.log *.toc *.out *.bbl *.blg *.fls *.fdb_latexmk *.pdf

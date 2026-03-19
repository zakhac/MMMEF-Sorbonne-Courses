MAIN = NumericalMethods

.PHONY: all clean purge

all:
	latexmk -pdf -interaction=nonstopmode $(MAIN).tex

clean:
	latexmk -c
	rm -f compile_result.txt compile_log.txt
	rm -f *.aux *.log *.out *.toc *.bbl *.blg *.fls *.fdb_latexmk *~

purge:
	latexmk -C
	rm -f compile_result.txt compile_log.txt
	rm -f *.aux *.log *.out *.toc *.bbl *.blg *.fls *.fdb_latexmk *~

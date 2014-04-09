CODES = code/*.ml

all:
	pdflatex main

bib:
	pdflatex main
	bibtex main
	pdflatex main
	bibtex main
	pdflatex main

.PHONY: code
code: code/*.ml
	cd code; ./ml2tex.py

clean: 
	rm *.aux *.log *.out code/*.tex
	

# Makefile for documentation
DOCUMENT = main
OBJ_DIR = ./obj

.PHONY: all bib clean doc gloss latex

all: clean latex doc

doc:
	for i in {0..2}; do \
		pdflatex $(DOCUMENT).tex; \
	done
	mv $(DOCUMENT).pdf $(OBJ_DIR)/.
	@echo ' ' ; echo ' '
	@echo 'completed succesfully'
	@echo ' ' ; echo ' '

latex:
	pdflatex $(DOCUMENT).tex

bib:
	bibtex $(DOCUMENT).aux

gloss:
	makeglossaries $(DOCUMENT)

clean:
	find ./ -name *.aux -delete
	find ./ -name *.bbl -delete
	find ./ -name *.blg -delete
	find ./ -name *.glo -delete
	find ./ -name *.glg -delete
	find ./ -name *.gls -delete
	find ./ -name *.glsdefs -delete
	find ./ -name *.ist -delete
	find ./ -name *.log -delete
	find ./ -name *.lot -delete
	find ./ -name *.lof -delete
	find ./ -name *.nav -delete
	find ./ -name *.out -delete
	find ./ -name *.snm -delete
	find ./ -name *.synctex.gz -delete
	find ./ -name *.toc -delete
	find ./ -name *.vrb -delete
	find ./ -name *.xdy -delete

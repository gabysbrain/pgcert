
PAPER=writeup

all: paper

paper:
	@pandoc -s -F pandoc-crossref --natbib --template=../mytemplate.tex -N \
		-f markdown -o $(PAPER).tex $(PAPER).md
	@pdflatex $(PAPER).tex 
	@bibtex $(PAPER) 
	@pdflatex $(PAPER).tex
	@pdflatex $(PAPER).tex 

clean:
	rm $(PAPER).aux $(PAPER).tex $(PAPER).log $(PAPER).bbl $(PAPER).blg $(PAPER).out

.PHONY: all clean paper


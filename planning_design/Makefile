
PAPER=writeup

all: paper

paper:
	@pandoc -s -F pandoc-crossref --natbib --template=../mytemplate.tex -N \
		-f markdown -t latex+raw_tex+tex_math_dollars+citations -o $(PAPER).tex $(PAPER).md
	@pdflatex $(PAPER).tex &> /dev/null
	@bibtex $(PAPER) &> /dev/null
	@pdflatex $(PAPER).tex &> /dev/null
	@pdflatex $(PAPER).tex &> /dev/null

clean:
	rm $(PAPER).aux $(PAPER).tex $(PAPER).log $(PAPER).bbl $(PAPER).blg $(PAPER).out

.PHONY: all clean paper


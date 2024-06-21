FILENAME = template
RM = rm -rf

OPEN = open ./$(FILENAME).pdf

.SUFFIXES: .tex .dvi .pdf

all: $(FILENAME).pdf
	#  $(OPEN)

clean:
	$(RM) *.aux *.dvi *.log *.bbl *.blg *.ps *.out $(FILENAME).pdf

open:
	# $(OPEN)

$(FILENAME).pdf: $(FILENAME).tex
	platex $(FILENAME).tex
	# bibtex $(FILENAME)
	platex $(FILENAME).tex
	# platex $(FILENAME).tex
	dvipdfmx $(FILENAME)

FILE=SD

CNT := 2

.SUFFIXES: .tex .dvi .aux .log .toc .lof .lot .pdf .ps .bbl .bib
.PHONY: all distclean clean

TEX=platex

all: $(FILE).pdf

.tex.dvi:
	$(TEX) $(FILE)
	$(TEX) $(FILE)

.dvi.ps:
	dvips $<

.dvi.pdf:
	dvipdfmx -p a4 $<

distclean: clean
	rm -f $(FILE).pdf

clean:
	rm -f *~ $(FILE).dvi $(FILE).aux $(FILE).lof $(FILE).toc \
	$(FILE).lot $(FILE).log $(FILE).ps $(FILE).blg $(FILE).bbl \
	$(FILE).spl $(FILE).out $(FILE).synctex.gz $(FILE).snm $(FILE).nav


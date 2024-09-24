LATEX = pdflatex

all: fiche-exercices.pdf clean

codes/chapitre-1.log: codes/chapitre-1.org
	cd codes ; ./babel chapitre-1.org

fiche-exercices.pdf: fiche-exercices.tex
	@rubber --src-specials --unsafe --pdf fiche-exercices
	@rubber --clean fiche-exercices

clean:
	@rm -f *.aux *.log *.out *.nav *.rel *.toc *.snm *.synctex.gz *.vrb *.rubbercache
	@rm -rf auto

clean-all:
	@rm -f *.pdf

.PHONY: all

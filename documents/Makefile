all: nbody_objective.pdf

PDFLATEX = pdflatex

%.pdf: %.tex
	$(PDFLATEX) $*
	bash -c " ( grep Rerun $*.log && $(PDFLATEX) $* ) || echo no need to re-run "
	bash -c " ( grep Rerun $*.log && $(PDFLATEX) $* ) || echo no need to re-run "

clean:
	$(RM) *.log *.aux *.dvi *.bbl *.blg

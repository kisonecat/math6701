all: set01.pdf set02.pdf set03.pdf set04.pdf set05.pdf set06.pdf set07.pdf set08.pdf set09.pdf set10.pdf set11.pdf set12.pdf set13.pdf

%.pdf: %.tex preamble.tex homework.cls
	pdflatex $<
	rm -f sets.aux
	cat *.aux > sets.aux
	cat sets.aux > $(patsubst %.tex,%.aux,$<)
	pdflatex $<
	rm -f sets.aux

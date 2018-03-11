all: events.svg officers.png officers.svg
clean:
	test ! -f events.png || rm events.png
	test ! -f officers.png || rm officers.png
.PHONY: all clean

%.png: %.dot
	dot -Tpng -o $@ $<
%.svg: %.dot
	dot -Tsvg -o $@ $<
%.svg: %.tex
	pdflatex -shell-escape $<

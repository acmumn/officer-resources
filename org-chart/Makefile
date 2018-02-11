all: officers.png
clean:
	test -f officers.png && rm officers.png

%.png: %.dot
	dot -Tpng -o $@ $<

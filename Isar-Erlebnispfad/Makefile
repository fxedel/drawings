svg-files := $(wildcard svg/*.svg)
png-files := $(svg-files:svg/%.svg=png/%.png)

.PHONY: all

all: ${png-files}

${png-files}: png/%.png: svg/%.svg
	inkscape --export-png="$@" --export-dpi=256 $<

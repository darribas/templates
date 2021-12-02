.PHONY: both html pdf

# make both talk=demo
both: html pdf

html:
	pandoc \
		--section-divs \
		-t revealjs \
		-s \
		--metadata title="GDS Book" \
		--variable theme="journal" \
		--template template.revealjs \
		-o slides.html \
		slides.md

pdf: html
	decktape automatic \
		--chrome-arg=--no-sandbox \
		-s 1280x960 \
		slides.html slides.pdf


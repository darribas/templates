.PHONY: all pdf word count

PANDOCFY = pandoc -s \
	-V geometry='margin=1in' \
	--bibliography refs.bib \
	--citeproc \
	--csl apa.csl

all: pdf word
pdf: count
	$(PANDOCFY) -o article.pdf article.md

word:
	$(PANDOCFY) -o article.tex article.md
	pandoc -s -o article.docx article.tex
	texcount article.tex
	rm article.tex
count:
	$(PANDOCFY) -o article.tex article.md
	texcount article.tex
	texcount -char article.tex | grep "Letters in text"
	texcount article.tex | grep "Words in text" > count.txt
	rm article.tex


DOC = classloader

%.pdf: %.tex
	pdflatex $<
	pdflatex $<
	pdflatex $<

%.tex: %.txt
	wiki2beamer $< >$*.tex

$(DOC).pdf: $(DOC).tex $(DOC)_wiki.tex

clean:
	rm -f $(DOC)_wiki.tex *.aux *.log *.nav *.out *.snm *.toc

realclean: clean
	rm *.pdf

# eof

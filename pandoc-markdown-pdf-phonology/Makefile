FILENAME = template-pandoc-markdown-pdf-phonology
INFILES = $(FILENAME).markdown
OUTFILE = $(FILENAME).pdf

#FLAGS = --xetex --template=mytemplate.tex
FLAGS = --template=mytemplate.tex

$(OUTFILE) : $(INFILES)
		markdown2pdf $(FLAGS) $(INFILES) -o $(OUTFILE)

clean :
		rm -f $(OUTFILE)
		rm -f $(FILENAME).tex

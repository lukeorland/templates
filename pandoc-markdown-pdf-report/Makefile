DOCUMENT = report
INFILES = $(DOCUMENT).mdown
OUTFILE = $(DOCUMENT).pdf

AUTHOR = "Luke Orland"
TITLE = "Title"
DATE = "today"
BIBLIOGRAPHY = library.bib

FLAGS = \
				--xetex \
				--template=mytemplate.tex \
				-V author=$(AUTHOR) \
				-V title=$(TITLE) \
				-V date=$(DATE) \
				--number-sections \
				--bibliography=$(BIBLIOGRAPHY) \
				--csl=chicago-author-date-Custom.csl

$(OUTFILE) : $(INFILES)
		markdown2pdf $(FLAGS) $(INFILES) -o $(OUTFILE)

clean :
		rm -f $(OUTFILE)

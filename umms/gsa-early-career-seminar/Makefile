DOCNAME=gsa-early-career-slides


all: $(DOCNAME).html


$(DOCNAME).html: $(DOCNAME).Rmd 
	R -e "rmarkdown::render('$<')"


clean:
	rm -R $(DOCNAME)_files; rm $(DOCNAME).html

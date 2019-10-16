DOCNAME=gsa-early-career-slides


all: $(DOCNAME).pdf


$(DOCNAME).html: $(DOCNAME).Rmd 
	R -e "rmarkdown::render('$<')"


$(DOCNAME).pdf: $(DOCNAME).html
	R -e "webshot::webshot('$^', '$@', delay = 15)"
	
clean:
	rm -R $(DOCNAME)_files; rm $(DOCNAME).pdf; rm $(DOCNAME).html

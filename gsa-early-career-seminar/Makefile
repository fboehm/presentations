DOCNAME=gsa-early-career-slides


all: $(DOCNAME).pdf


$(DOCNAME).html: $(DOCNAME).Rmd 
	R -e "rmarkdown::render('$<')"


$(DOCNAME).pdf: $(DOCNAME).html
	R -e "file <- paste0('file://', normalizePath('$^'));webshot::webshot(file, '$@', delay = 5)"
	
clean:
	rm -R $(DOCNAME)_files; rm $(DOCNAME).pdf; rm $(DOCNAME).html

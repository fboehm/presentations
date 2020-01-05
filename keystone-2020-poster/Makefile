DOCNAME=poster


all: $(DOCNAME).pdf


$(DOCNAME).html: $(DOCNAME).Rmd 
	R -e "rmarkdown::render('$<')"

$(DOCNAME).pdf: $(DOCNAME).html
	R -e "pagedown::chrome_print(input = 'poster.html')"


clean:
	rm -R $(DOCNAME)_files; rm $(DOCNAME).html; rm $(DOCNAME).pdf

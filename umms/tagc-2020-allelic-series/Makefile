PREFIX=tagc-2020-allelic-series-poster

all: $(PREFIX).pdf

$(PREFIX).html: $(PREFIX).Rmd
		Rscript -e 'rmarkdown::render("$(PREFIX).Rmd")'
  
$(PREFIX).pdf: $(PREFIX).html
		Rscript -e 'pagedown::chrome_print("$(PREFIX).html")'
		
		
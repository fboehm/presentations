PREFIX=tagc-2020-allelic-series-poster

all: $(PREFIX).pdf

$(PREFIX).pdf: $(PREFIX).Rmd
		Rscript -e 'rmarkdown::render("$(PREFIX).Rmd")'
  

## If you don't have appropriate latex installed change pdf to html or docx

.PHONY: all
all: summary_report.pdf analyse_report.pdf

## report summaries
summary_report.pdf: ${@:.pdf=.Rmd} ../analysis/summary_simple_csv.Rout

## report linear model analysis
analyse_report.pdf: ${@:.pdf=.Rmd} ../analysis/analyse_simple_csv.Rout

## remove intermediate files
.PHONY: cleanall
cleanall:
	rm -fr *~ *.Rout *.pdf *.html *.docx

include ~/lib/r-rules.mk

THISDIR := stokesTheorem
THISBOOK := $(THISDIR)
#BASEVER := 13a3089

include ../latex/make.vars

FIGURES := ../../figures/$(THISBOOK)
SOURCE_DIRS += $(FIGURES)

GENERATED_PDFS += $(THISBOOK).pdf

all :: myrefs.bib $(GENERATED_PDFS)

$(THISBOOK).pdf :: stokesTheoremCore.tex
$(GENERATED_PDFS) :: $(JUSTBOOKDEPENDENCIES) $(LOCAL_FILES) $(GENERATED_SOURCES) $(COPIED_FILES) $(LOCAL_COPIED_FILES)

include ../latex/make.rules

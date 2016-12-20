THISDIR := stokesTheorem
THISBOOK := $(THISDIR)
BASEVER := daa1713

include ../latex/make.vars

FIGURES := ../../figures/$(THISBOOK)
SOURCE_DIRS += $(FIGURES)

GENERATED_PDFS += $(THISBOOK).pdf

all :: myrefs.bib $(GENERATED_PDFS)

$(GENERATED_PDFS) :: $(JUSTBOOKDEPENDENCIES) $(LOCAL_FILES) $(GENERATED_SOURCES) $(COPIED_FILES) $(LOCAL_COPIED_FILES)
$(THISBOOK).pdf :: stokesTheoremCore.tex
$(THISBOOK).pdf :: ../gabookI/appendix/wedgeDistributionIdentity.tex
$(THISBOOK).pdf :: ../gabookI/calculus/stokesTheoremTheStatement.tex

include ../latex/make.rules

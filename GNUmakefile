THISDIR := stokesTheorem
THISBOOK := $(THISDIR)
BASEVER := daa1713

include ../latex/make.vars

FIGURES := ../figures
SOURCE_DIRS += $(FIGURES)

GENERATED_PDFS += $(THISBOOK).pdf

EPS_FILES := $(wildcard $(FIGURES)/*.eps)
PDFS_FROM_EPS := $(subst eps,pdf,$(EPS_FILES))
#$(error PDFS_FROM_EPS $(PDFS_FROM_EPS))

THISBOOK_DEPS += $(PDFS_FROM_EPS)

all :: myrefs.bib $(GENERATED_PDFS)

$(GENERATED_PDFS) :: $(JUSTBOOKDEPENDENCIES) $(LOCAL_FILES) $(GENERATED_SOURCES) $(COPIED_FILES) $(LOCAL_COPIED_FILES)
$(THISBOOK).pdf :: $(PDFS_FROM_EPS)
$(THISBOOK).pdf :: statement.tex
$(THISBOOK).pdf :: oneparameter.tex
$(THISBOOK).pdf :: twoparameter.tex
$(THISBOOK).pdf :: threeparameter.tex
$(THISBOOK).pdf :: scalarVolumeElement.tex
$(THISBOOK).pdf :: bladeDotWedgeSymmetryIdentities.tex
$(THISBOOK).pdf :: bladeDotWedgeSymmetryIdentitiesTheorem.tex
$(THISBOOK).pdf :: Bibliography.bib
$(THISBOOK).pdf :: ../gabookI/appendix/wedgeDistributionIdentity.tex
$(THISBOOK).pdf :: ../gabookI/appendix/wedgeDistributionIdentityProblems.tex
$(THISBOOK).pdf :: ../gabookI/calculus/stokesTheoremTheStatement.tex

include ../latex/make.rules

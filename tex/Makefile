# Makefile a utiliser pour compiler en deux temps
# Utilser make clean pour netoyer le dossier (voir ci-dessous)
# Utiler make pour compiler les deux, make fr (resp. make en) pour complier uniquement votre cv FR (resp. EN)

EN = SALOMONJemay_Resume_EN
FR = SALOMONJemay_Resume_FR

EXTS = acn acr alg aux bbl bcf blg glg glo gls glsdefs ist lof log out \
       run.xml tex.bbl tex.blg toc synctex.gz tex.bak

all: en fr

# make en
en:
	pdflatex $(EN).tex
	pdflatex $(EN).tex

# make fr
fr:
	pdflatex $(FR).tex
	pdflatex $(FR).tex

clean:
	@rm -f $(foreach b,$(EN) $(FR),$(addprefix $(b).,$(EXTS)))

.PHONY: all en fr clean

# Copyright 2026 -Jemay SALOMON
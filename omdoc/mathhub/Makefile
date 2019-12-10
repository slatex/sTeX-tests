AUX = localpath.tex
include ../../make/Makefile.in

# We generate a file localpath.tex which is needed for the tests.
PWD = $(shell pwd)
REPOS = omdoc/mathhub
MATHHUB = $(PWD:%/$(REPOS)=%)

localpaths.tex:
	@echo "\defpath{MathHub}{$(MATHHUB)}\n\mhcurrentrepos{$(REPOS)}" > localpath.tex

pre: localpaths.tex

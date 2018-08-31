SRC_TEX=hamilakis_nicolas_cv.tex
TARGET=hamilakis_nicolas_cv.pdf

all: clean-make --open

clean-make: hamilakis_nicolas_cv.pdf clean

hamilakis_nicolas_cv.pdf: $(SRC_TEX)
	latexmk -pdf
	
clean:
	@echo "cleaning up..."
	rm -rf *.aux
	rm -rf *.bbl 
	rm -rf *.blg
	rm -rf *.fdb_latexmk
	rm -rf *.fls
	rm -rf *.log
	rm -rf *.toc
	rm -rf *.out
	rm -rf *-blx.bib
	rm -rf *.bcf
	rm -rf *.run.xml
	rm -rf *.synctex.gz
	rm -rf *.lox
	rm -rf *.tdo
	rm -rf *.xwm

mrproper: clean
	rm -rf *.pdf

--open:
	evince $(TARGET)


.PHONY: clean mrproper --open

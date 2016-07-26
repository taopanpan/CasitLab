TeXFileName = template

sources = ${TeXFileName}.tex ${TeXFileName}.bib matlab_code.m

pdf: ${TeXFileName}.pdf

${TeXFileName}.pdf: ${sources}
	xelatex ${TeXFileName}.tex
	xelatex ${TeXFileName}.tex
	bibtex ${TeXFileName}
	xelatex ${TeXFileName}.tex
	xelatex ${TeXFileName}.tex

clean:  
	rm -f ${TeXFileName}.aux ${TeXFileName}.log ${TeXFileName}.nav ${TeXFileName}.out ${TeXFileName}.dvi ${TeXFileName}.snm ${TeXFileName}.toc ${TeXFileName}.lof ${TeXFileName}.lot ${TeXFileName}.bbl ${TeXFileName}.blg ${TeXFileName}.vrb ${TeXFileName}.pdf

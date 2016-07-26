TeXFileName = Git-GitHub-howto

sources = ${TeXFileName}.tex ${TeXFileName}.bib 

pdf: ${TeXFileName}.pdf

${TeXFileName}.pdf: ${sources}
	xelatex ${TeXFileName}.tex
	xelatex ${TeXFileName}.tex
	bibtex ${TeXFileName}
	xelatex ${TeXFileName}.tex
	xelatex ${TeXFileName}.tex

clean:  
	rm -f ${TeXFileName}.aux ${TeXFileName}.log ${TeXFileName}.nav ${TeXFileName}.out ${TeXFileName}.dvi ${TeXFileName}.snm ${TeXFileName}.toc ${TeXFileName}.lof ${TeXFileName}.lot ${TeXFileName}.bbl ${TeXFileName}.blg ${TeXFileName}.vrb ${TeXFileName}.pdf

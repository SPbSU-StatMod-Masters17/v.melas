file = notes
all: 
	echo "Use make pdf or make xe"

pdf:
	make pdflatex

xe:
	make xelatex 

pdflatex:
	make pdflatex_only
	make clean

xelatex:
	make xelatex_only
	make clean

pdflatex_only:
	pdflatex ${file}.tex
	pdflatex ${file}.tex

xelatex_only:
	xelatex ${file}.tex
	xelatex ${file}.tex

clean:
	find . \( -name "*.aux" -o -name "*.toc" -o -name "*.log" -o -name "*.out" \) -type f -delete

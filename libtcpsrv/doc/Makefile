all: index.html

index.html: index.txt
	asciidoc -a toc2 $<

TMP=/tmp/tcpsrv-gh-pages
stage:
	mkdir -p ${TMP}
	rm -if ${TMP}/*
	cp LICENSE.txt ${TMP}
	cp *.html ${TMP}
	cp *.png ${TMP}

clean: 
	rm -f index.html

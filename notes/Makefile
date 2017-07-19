.PHONY: all clean

all: Functional-Programming.html

%.html: %.org
	emacs $< --batch \
	  --eval "(setq org-confirm-babel-evaluate nil)" \
	  -f org-html-export-to-html \
	  --kill

clean:
	rm -f *.html

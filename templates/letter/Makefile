.DEFAULT_GOAL := letter_pdf

all: letter_tex letter_pdf

letter_tex:
	pandoc --template ./letter-template.tex --from markdown --to latex -o ./letter-gen.tex ./letter.md

letter_pdf:
	pandoc --template ./letter-template.tex --from markdown --to latex -o ./letter-gen.pdf ./letter.md

clean:
	rm -f ./letter-gen.pdf
	rm -f ./letter-gen.tex

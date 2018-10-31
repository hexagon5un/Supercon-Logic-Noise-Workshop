filebase=logic_noise_workshop
all: ${filebase}.html 
THEME=moon

%.html: %.md
	# pandoc -t revealjs -V theme:${THEME} -s $^ -o $@
	pandoc -t revealjs  -i -s $^ -o $@
#	pandoc -t dzslides  -s $^ -o $@


%.pdf: %.md 
	pandoc -t beamer -V theme:metropolis -s $^ -o $@

clean:
	rm *.pdf *.html


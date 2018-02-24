LATEX = latex
DVI2PS = dvips
PS2PDF = ps2pdf
PSNUP = psnup

LFLAGS =
DFLAGS = -Ppdf -G0
PFLAGS =
NFLAGS = -n 2

dvi:	
	latex Diplomarbeit-MICE.tex && latex Diplomarbeit-MICE.tex && latex Diplomarbeit-MICE.tex

ps:	dvi
	$(DVI2PS) $(DFLAGS) Diplomarbeit-MICE.dvi

psn2:	ps
	$(PSNUP) $(NFLAGS) Diplomarbeit-MICE.ps Diplomarbeit-MICE.n2.ps

pdf:	ps
	$(PS2PDF) $(PFLAGS) Diplomarbeit-MICE.ps Diplomarbeit-MICE.pdf

clean:
	rm -f Diplomarbeit-MICE.tgz Diplomarbeit-MICE.aux Diplomarbeit-MICE.waux Diplomarbeit-MICE.out Diplomarbeit-MICE.dvi Diplomarbeit-MICE.lof Diplomarbeit-MICE.log Diplomarbeit-MICE.ps* Diplomarbeit-MICE.n2.ps Diplomarbeit-MICE.toc Diplomarbeit-MICE.pdf

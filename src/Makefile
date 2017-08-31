OBJS = cledit.o buffer.o config.o files.o screen.o
FBCFLAGS = -g -mt

cled: $(OBJS)
	fbc $(FBCFLAGS) -x cled $(OBJS)

cledit.o: cledit.bas
	fbc $(FBCGLAGS) -m cled -o cledit.o -c cledit.bas

buffer.o: buffer.bas
	fbc $(FBCFLAGS) -o buffer.o -c buffer.bas

config.o: config.bas
	fbc $(FBCFLAGS) -o config.o -c config.bas

files.o: files.bas
	fbc $(FBCFLAGS) -o files.o -c files.bas

screen.o: screen.bas
	fbc $(FBCFLAGS) -o screen.o -c screen.bas

clean:
	rm -f *.obj cled

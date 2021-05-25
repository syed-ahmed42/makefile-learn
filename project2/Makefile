SRCDIR = src
OBJDIR = obj

all: exec

exec: $(OBJDIR)/test.o $(OBJDIR)/sum.o
	gcc -o exec $(OBJDIR)/test.o $(OBJDIR)/sum.o

$(OBJDIR)/test.o: $(SRCDIR)/test.c
	gcc -o $(OBJDIR)/test.o -c $(SRCDIR)/test.c

$(OBJDIR)/sum.o: $(SRCDIR)/sum.c
	gcc -o $(OBJDIR)/sum.o -c $(SRCDIR)/sum.c

.PHONY: clean all

clean:
	@rm exec $(OBJDIR)/*.o

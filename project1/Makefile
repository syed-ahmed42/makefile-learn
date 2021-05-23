OBJDIR = objects/
SRCDIR = src/
INCDIR = header/

OBJ = $($(SRCDIR):.c=.o)

CFLAGS = -c -Wall -O2 - Wextra

test: $(obj)
	 $(CC) $(OBJ) -o test

$(OBJDIR)/%.o: $(SRCDIR)/%.c $(INCDIR)/*
	$(CC) $(CFLAGS) $< -o $@



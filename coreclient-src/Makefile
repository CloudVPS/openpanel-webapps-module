include makeinclude

OBJ	= main.o

all: coreclient

coreclient: $(OBJ)
	$(LD) $(LDFLAGS) -o coreclient $(OBJ) $(LIBS)

clean:
	rm -f *.o
	rm -f coreclient

makeinclude:
	@echo please run ./configure
	@false

SUFFIXES: .cpp .o
.cpp.o:
	$(CXX) $(CXXFLAGS) $(INCLUDES) -c $<

CC = i686-w64-mingw32-g++
CFLAGS = -Wall -Wextra -masm=intel -fno-asynchronous-unwind-tables -shared -m32 -mwindows -O2 -s -I ./include
LDFLAGS = -static-libgcc -static-libstdc++ -L ./lib -lmsvcrt -lpython27
BINARY = PyBox.dll
SOURCE = *.cpp

.PHONY: all clean

all: $(BINARY)
	

$(BINARY): $(SOURCE)
	$(CC) $(CFLAGS) -o $(BINARY) $(SOURCE) $(LDFLAGS)

clean:
	rm -f $(BINARY)

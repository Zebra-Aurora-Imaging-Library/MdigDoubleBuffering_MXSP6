TARGET	= MdigDoubleBuffering
CFLAGS   = -I$(MILDIR)/include -g -Werror $(USER_CFLAGS)
CXXFLAGS = $(CFLAGS) -std=c++11
LDFLAGS  = -L$(MILDIR)/lib -lmil -lmilim
.PHONY   = all clean

all: $(TARGET)

clean:
	-rm -f $(TARGET) $(TARGET).o

$(TARGET) : $(TARGET).o
	$(CXX) $(CXXFLAGS) -o $@ $^ $(LDFLAGS) 
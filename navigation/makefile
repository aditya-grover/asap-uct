CXX	=	g++
CCFLAGS	=	-Wall -O3 -ffloat-store -Wl,--no-as-needed -lrt -ffast-math -pg -msse -I../engine -DNDEBUG
EXTRA	=	-std=c++0x
OBJS	=	main.o
TARGET	=	navigation

$(TARGET):	$(OBJS)
		$(CXX) $(CCFLAGS) $(EXTRA) -o $(TARGET) $(OBJS)

clean:
		rm -f $(OBJS) $(TARGET) *~ core

.cc.o:
		$(CXX) $(CCFLAGS) $(EXTRA) -c $<


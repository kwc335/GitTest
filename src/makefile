# A sample Makefile 

LINK_TARGET = main 

OBJS= \
	main.o

REBUILDABLES = $(OBJS) $(LINK_TARGET)

all: $(LINK_TARGET) 
	@echo All done

$(LINK_TARGET): $(OBJS) 
#	g++ -g -o $@ $^
	gcc -g -o $@ $^

%.o : %.cpp
#	g++ -g -o $@ -c $<
	gcc -g -o $@ -c $< 

#main.o : main.h

# Alternatively to manually capturing dependencies, several automated
# dependency generators exist. Here is one possibility (commented out)...
# %.dep : %.cpp
# g++ -M $(FLAGS) $< > $@
# include $(OBJS:.o=.dep)

clean:
	rm -f $(REBUILDABLES) 
	@echo Clean done

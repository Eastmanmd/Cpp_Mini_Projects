#
# PROGRAM:    Assignment 7
# PROGRAMMER: Ali Eastman Oku
# LOGON ID:   your z-id

#
    
# Compiler variables
CXX = g++
CXXFLAGS = -Wall -Werror -std=c++11
        
# Rule to link object code files to create executable file
inpost: inpost_main.o inpost.o mystack.o
	$(CXX) $(CXXFLAGS) -o inpost $^

# Rules to compile source code file to object code
inpost_main.o: inpost_main.cpp inpost.h
inpost.o: inpost.cpp inpost.h mystack.h
mystack.o: mystack.cpp mystack.h
   
# Pseudo-target to remove object code and executable files
clean:
	rm -f inpost *.o
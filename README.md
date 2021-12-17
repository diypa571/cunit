# cunit

Installing cunit    
I hope this guide will help anyone to easily install cunit and use it for testing...   
mkdir -p $HOME/local    
./configure --prefix=$HOME/local    
make clean    
make    
make install         
 
 Compile ....     
 gcc -Wall -I$HOME/local/include mytest.c -L$HOME/local/lib -lcunit -o myprogram     


Remember to the include CUnit header files...    
#include <CUnit/CUnit.h>    


gcc -Wall -c diypa.c    
gcc -Wall -I$HOME/local/include -o diypa_test diypa_test.c diypa.o -L$HOME/local/lib -lcunit    
LD_LIBRARY_PATH=$HOME/local/lib ./diypa_test    


http://cunit.sourceforge.net/    



A very simple "black box"     
http://cunit.sourceforge.net/example.html     




 

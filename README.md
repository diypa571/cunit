# Cunit    
# I hope this guide will help anyone to easily install cunit and use it for testing applications in Linux...     
## Installing cunit     
 
 
# Alt 1:
 sudo apt-get install libcunit1 libcunit1-doc libcunit1-dev
For compile...
gcc  -o app test.c  -lcunit
 
 
# Alt 2
 
mkdir -p $HOME/local    
./configure --prefix=$HOME/local    
make clean    
make    
make install         
 
 ### Compile ....     
 gcc -Wall -I$HOME/local/include mytest.c -L$HOME/local/lib -lcunit -o myprogram     


## Remember to include the CUnit header files...    
#include "CUnit/CUnit.h"
#include "CUnit/Basic.h"
//#include "CUnit/Automated.h"
//#include "CUnit/Console.h"



## gcc -Wall -c diypa.c    
## gcc -Wall -I$HOME/local/include -o diypa_test diypa_test.c diypa.o -L$HOME/local/lib -lcunit      


#  For runing the application      
## LD_LIBRARY_PATH=$HOME/local/lib ./diypa_test      


> http://cunit.sourceforge.net/    



#### A very simple "black box"     
> http://cunit.sourceforge.net/example.html     




 

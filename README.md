// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std ;

int main()
    
{
int sieze ;
cout << " enter the sieze of array ";
cin >> sieze ;
int array [1000] ;
cout << " enter the number of which harray has to be formed" ;
for ( int a = 0 ; a < sieze ; a ++)
  cin >> array [a];
int x ; 
cout << " enter the number which u want to serch :" ;
cin >> x ;
 
  int start = 0 , end = sieze ;
  int mid =  start+ end/ 2  ;
  while ( start <= end)
   {if (  array [mid] == x ) 
     { 
         if ( array [ mid ]>array [mid - 1 ])
          { cout << " the first occurence  is at index :" << mid ;
           start = mid +1 ;}
           
    else if (array [mid]< array [mid +1])
        {  break;}
        
     else
        start = mid + 1 ;
    
   }
     
   
    if else ( array [mid] < x)   
      start = mid +1;
    else 
       end = (mid -1 ) ;}
    
}
  
   
cout<< " the last occurence is at index :" << mid ;   
   
     

    return 0;
}

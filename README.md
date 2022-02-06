# digital-clock
created a digital clock using c language // 
#include &lt;stdio.h> 
#include &lt;time.h>//for sleep() function 
#include <stdlib.h> 
int main()  
{    int h; 
     int m;   
     int s;  
     int d=1000;    
     printf("Set time:\n");  
     scanf("%d %d %d",&h;h,&m;m,&s);
     if(h>12||m>60||s>60)  
     {        printf("error!\n");  
     exit(0);  
     } 
     while(1) 
     {       
     if(s>59)   
     {     
     m++;   
     s=0;   
     }     
     if(m>59)
     {    
     h++;      
     m=0;   
     }    
     if(h>12)  
     {     
     h=1;  
     }    
     printf("\n clock:");   
     printf("\n%02d:%02d:%02d",h,m,s);   
     sleep(2);  
     } 
     }

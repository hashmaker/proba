  2     #include<stdio.h>
  3     #include<stdlib.h>
  4     #include<time.h>
  5 
  6     int main ()
  7     {
  8         int number,number1,napad,helth,helth1;
  9 helth=10;
 10 helth1=10;
 11 printf("Napada te pritisni 1 i uzvrati: ");
 12 
 13     napad:  scanf("%d",&napad);
 14         if(napad == 1)
 15     {
 16 
 17         /* initialize random seed: */
 18         srand ( time(NULL) );
 19         /* Generate a random number: */
 20         number = rand() % 5 + 1;
 21         number1 = rand() % 3 + 1;
 22         helth = helth - number;
 23         helth1 = helth1-number1;
 24             printf("\nEnergija od napadacaje %d\n",helth);
 25             printf("Tvoja energina je %d",helth1);
 26          if (helth>0)
 27 {
 28 printf("\nNapadni opet (1): \n");
 29 goto napad;
 30 }
 31     else
 32 printf("Ubio si ga!");
 35     }
 36     else
 37 printf("pica si");
 38   return 0;    
 39       }

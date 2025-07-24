# GAME-DEMO
This is my first Git Repository.
<br>
Author - Aashi Srivastava

#include<stdio.h> #include<stdlib.h> #include<time.h>

int main(){

srand(time(0));

int n = (rand()%100) +1; int no_of_guesses = 0; int a;

printf("WELCOME TO THE NUMBER GUESSING GAME\n"); printf("\n"); printf("GUESS A NUMBER BETWEEN 1-100\n"); printf("\n");

do{ printf("GUESS THE NUMBER:");

scanf("%d", &a);
no_of_guesses++;
if(a>n){
  printf("LOWER NUMBER PLEASE!!\n");
}
else if(a<n){
  printf("HIGHER NUMBER PLEASE!!\n");
}
else if(a==n){
  printf("CONGRATULATIONS!!\n");
  printf("YOUR GUESS IS CORRECT!!\n");
}
}while(a!=n);

printf("NUMBER OF ATTEMPTS IS :%d\n",no_of_guesses);

if(no_of_guesses<=3){ printf("YOUR SCORE IS 100\n"); } else if(no_of_guesses<=10){ printf("YOUR SCORE IS 50\n"); } else if(no_of_guesses<=20){ printf("YOUR SCORE IS 25\n"); }

return 0;
}


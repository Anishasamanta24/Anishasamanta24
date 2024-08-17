#include <stdio.h>
#include <stdlib.h>  
#include <time.h>  

int main() {
    srand(time(NULL));

    int min = 1;
    int max = 100;

    int random_number = min + rand() % (max - min + 1);
    int no_of_guesses=0;
    int guessed;

do
{
printf("Guess the number\n");
scanf("%d",&guessed);
no_of_guesses++;
 if (guessed>random_number)
 {printf("lower number please!\n");}
 else{
    printf("Higher number please!\n");
 }}
 while (guessed!=random_number);
printf("You guessed the number in %d guesses!",no_of_guesses);
 
 
    return 0;
}

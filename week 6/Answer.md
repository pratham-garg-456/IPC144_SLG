### Q1. This is the code. And I want you guys to write the pseudocode for it

``` C
int i;

for ( i= 0; i< 5; i++)
 {
   	printf("The value of i is: %d", i);
 }

```

### Ans.

```
1.	Start
2.	Declare variable i
3.	Initialize i to 1
4.	Is i less than 5?
  a.	Yes : print the i and then increase the i by 1 and go to step 4
  b.	No: go to step 5.
5.	end.

```


### Q2. What will be the output of the code below
 
![image](https://github.com/pratham-garg-456/IPC144_SLG/assets/81003075/adb8a501-0402-4e04-ae15-fa0b82c35218)


### Ans. 
```
Coffee #0
Coffee #1
coffee #2
Coffee #3
I think…
Coffee #4
Thats it!!
```
### Q3. Guess the number code:
### Write a program in which a coder randomly selects a number and the user has to guess it. After each guess, the program should tell the player if the guess is too high, too low, or correct. Print the number of attempts they used.

### int randomNumber = 46;

### Ans. 

``` C
#include <stdio.h>

int main(){

	int randomNumber = 46;
	int userInput;
	int flag = 1;
	int attempts=0 ;

    printf("----------------------------\n");
	printf("Guess the number game begins\n");
	printf("----------------------------\n\n");
	
	do{
		printf("Enter a number between 0 to 100 > ");
		scanf("%d", &userInput);
		if (userInput< randomNumber){
			printf("!Guess is low enter a higher number\n\n");
		}
		else if(userInput> randomNumber){
			printf("!Guess is high enter a lower number\n\n");
		}
		else {
			flag = 0;
			printf("You guessed it correctly well done||\n\n");
		}
	 attempts++;	
	
	}while(flag);

	printf("It took you %d attempts to guess the number", attempts);

	return 0;
}

```

### Q4. What is the difference between i++ and ++i

int i = 5;
int a = 0;

int a = i++;
int a = ++I;






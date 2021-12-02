/* C Program to Create Simple Calculator using Switch Case */
 
#include <stdio.h>
 
int main()
{
	char Operator;
	float num1, num2, result = 0;
	
	printf("\n Please Enter an Operator (+, -, *, /)  :  ");
  	scanf("%c", &Operator);
  	
	printf("\n Please Enter the Values for two Operands: num1 and num2  :  ");
  	scanf("%f%f", &num1, &num2);
  	
  	switch(Operator)
  	{
  		case '+':
  			result = num1 + num2;
  			break;
  		case '-':
  			result = num1 - num2;
  			break;  			
  		case '*':
  			result = num1 * num2;
  			break;
  		case '/':
  			result = num1 / num2;
  			break;
		default:
			printf("\n You have enetered an Invalid Operator ");				    			
	}
  
	printf("\n The result of %.2f %c %.2f  = %.2f", num1, Operator, num2, result);
	
  	return 0;
}
C Program to Create Simple Calculator using Switch Case 1
C Program to Create Simple Calculator Example 2
It is the same C program that we used in the first example. But this time, we are performing the arithmetic operation directly inside the Switch case blocks.

/* C Program to Create Simple Calculator using Switch Case */
 
#include <stdio.h>
 
int main()
{
	char Operator;
	float num1, num2, result = 0;
	
	printf("\n Please Enter an Operator (+, -, *, /)  :  ");
  	scanf("%c", &Operator);
  	
	printf("\n Please Enter the Values for two Operands: num1 and num2  :  ");
  	scanf("%f%f", &num1, &num2);
  	
  	switch(Operator)
  	{
  		case '+':
  			printf("\n The result of %.2f + %.2f  = %.2f", num1, num2, num1 + num2);
  			break;
  		case '-':
  			printf("\n The result of %.2f - %.2f  = %.2f", num1, num2, num1 - num2);
  			break;  			
  		case '*':
  			printf("\n The result of %.2f * %.2f  = %.2f", num1, num2, num1 * num2);
  			break;
  		case '/':
  			printf("\n The result of %.2f / %.2f  = %.2f", num1, num2, num1 / num2);
  			break;
		default:
			printf("\n You have enetered an Invalid Operator ");				    			
	}
	
  	return 0;
}

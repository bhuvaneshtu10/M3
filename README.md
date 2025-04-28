# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
    #include<stdio.h>
    #include<math.h>
    void calculateEMI(double principal, double rate, int months);
    int main()
    {
    double principal, rate;
    int months;
    printf("Enter Principal Amount:\n");
    scanf("%lf",&principal);
    printf("Enter Rate of Interest:\n");
    scanf("%lf",&rate);
    printf("Enter Number of Months:\n");
    scanf("%d",&months);
    calculateEMI(principal, rate, months);
    return 0;
    }
    void calculateEMI(double principal, double rate, int months)
    {
    double emi;
    emi=(principal*pow(1+rate,months)*rate)/(pow(1+rate,months)-1);
    printf("Monthly EMI is = %.3lf\n", emi);
    }

## OUTPUT

![Screenshot 2025-04-28 161115](https://github.com/user-attachments/assets/4c0fdab9-d40a-48f8-a0f6-be9ae088de42)

## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 
# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM

    #include<stdio.h>
    int main()
    {
    int n=6,first=0,second=1,next,i;
    printf("Fibonacci Series: ");
    if(n>=1)
        printf("%d ",first);
    if(n>=2)
        printf("%d ",second);
    for(i=3;i<=n;i++) 
	{
        next=first+second;
        printf("%d ",next);
        first=second;
        second=next;
    }
    return 0;
    }
## OUTPUT

![Screenshot 2025-04-28 161600](https://github.com/user-attachments/assets/3b75a82e-7f61-4b16-8ea8-cde735923e68)

## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.

# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM

    #include<stdio.h>
    int main()
    {
    int n,i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    for(i=0;i<n;i++) 
	{
        scanf("%d",&arr[i]);
    }
    printf("Last element of the array is: %d\n",arr[n-1]);
    }
## OUTPUT

![Screenshot 2025-04-28 161857](https://github.com/user-attachments/assets/4248a4e0-d6cb-420f-88f6-10ccae939085)

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.



# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM

    #include<stdio.h>
    int main()
    {
    int n,i,count=0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    for(i=0;i<n;i++)
	{
        scanf("%d",&arr[i]);
    }
    for(i=0;i<n;i++) 
	{
        if(arr[i]>0)
		{ 
		count++;
        }
    }
    printf("Total number of positive elements: %d\n", count);
    }
    
## OUTPUT

![Screenshot 2025-04-28 162229](https://github.com/user-attachments/assets/998ac6a4-d727-401e-b5f7-4bdf3bb7054d)

## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:

    #include<stdio.h>
    int main() 
    {
    int n,i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    for(i=0;i<n;i++)
	{
        scanf("%d",&arr[i]);
    }
    printf("Updated array:\n");
    for(i=0;i<n;i++) 
	{
        if(arr[i] % 2 == 0)
		{
            printf("E ");
        }
		else
		{
            printf("%d ",arr[i]); // Print the number if odd
        }
    }

    return 0;
    }
## Output:
 
![Screenshot 2025-04-28 162559](https://github.com/user-attachments/assets/cc11c492-8318-4733-bb59-42a1f5f06943)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




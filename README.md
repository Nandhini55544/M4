# EX-16-LEFT-SHIFT-OPERATION
## AIM
To perform bitwise AND operation and bitwise OR operation of 21 and 22 integers. 

## ALGORITHM
1.Start.

2.Define two integers a = 21 and b = 22.

3.Perform bitwise AND operation using a & b.

4.Perform bitwise OR operation using a | b.

5.Print the results.

6.End.

## PROGRAM
```
#include <stdio.h>

int main() {
    int a = 21;
    int b = 22;

    int and_result = a & b;
    int or_result = a | b;

    printf("Bitwise-AND result is = %d\n", and_result);
    printf("Bitwise-OR result is = %d\n", or_result);

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/3f4d9cbb-ac84-4706-aea4-ef8489fe89e9)

## RESULT
Thus the program  to perform bitwise AND operation and bitwise OR operation of 21 and 22 integers has been executed successfully. 

# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT

## AIM

Write a C program to input number from the user and check whether the number is even or odd using a switch case. 


## ALGORITHM
```
1.Start.
2.Input a number from the user.
3.Find the remainder when the number is divided by 2 (i.e., number % 2).
4.Use a switch statement:
5.If remainder is 0, it’s even.
6.If remainder is 1, it’s odd.
7.Display the result.
8.End.
```
## PROGRAM
```
#include<stdio.h>
int main()
{
    int num;
    scanf("%d",&num);
    switch(num%2){
        case 0:
        printf("Number is Even\n");
        break;
        case 1:
        printf("Number is Odd\n");
        break;
        default:
        printf("Invalid input\n");
    }
    return 0;
}
```

## OUTPUT
 ![image](https://github.com/user-attachments/assets/60684eca-b746-4846-a40c-081671cf47d3)
          
## RESULT

Thus the program to input number from the user and check whether the number is even or odd using a switch case has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Assign the string 'CSE' to the input string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>  

int main() {
    char str[100];
    scanf("%s",str);
    for (int i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s\n", str);

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/241ed897-0bf6-40f0-b9b2-af6330a92ab7)

## RESULT
Thus the program to convert the given string into lowercase has been executed successfully

# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
   char str[100];
   int i=0,words=0;
   fgets(str, sizeof(str),stdin);
   while(str[i]!=0){
       if((i==0 && str[i]!=' '&& str[i]!= '\n') || (str[i]!= ' ' && str[i-1] == ' ')){
           words++;
       }
       i++;
   }
   printf("%d",words);
   return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/561c4f08-4ac5-41eb-aecf-9b34597d7e1f)

## RESULT
Thus the program to count the total number of words in a given string using While loop has been executed successfully
 
# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
```
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.
```
## PROGRAM
```
#include <stdio.h>  
int compare(char[],char[]);  
int main()  
{  
   char str1[20];   
   char str2[20];  
   
   scanf("%s",str1);  
    
   scanf("%s",str2);  
   int c= compare(str1,str2);   
   if(c==0)  
   printf("strings are same");  
   else  
   printf("strings are not same");  
  
    return 0;  
}  
  
int compare(char a[],char b[])  
{  
    int flag=0,i=0;   
    while(a[i]!='\0' &&b[i]!='\0')  
    {  
       if(a[i]!=b[i])  
       {  
           flag=1;  
           break;  
       }  
       i++;  
    }  
    if(flag==0)  
    return 0;  
    else  
    return 1;  
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/c0b24631-fc4e-4c6f-8737-b0ab04a5d941)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


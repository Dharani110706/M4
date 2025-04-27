# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM

```
#include <stdio.h>
int main() {
    unsigned int a=44 ;	  
      int c; 
    c = a << 3;    
   printf("After Left Shift Operation value of a is:%d\n", c );
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/06dbfd46-afec-41af-83d0-7ef88c41d470)



## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM

```
#include<stdio.h>
int main(){
    int a,b;
    scanf("%d%d",&a,&b);
    if(a==b){
        printf("Numbers are Equal\n");
    }
    else{
        printf("Numbers are not Equal");
    }
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/24a9b596-3fce-4534-b7cb-c48baeedb291)

           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM

```
#include<stdio.h>
#include<ctype.h>
int main(){
    char str[100];
    scanf("%s",str);
    for(int i=0;str[i]!='\0';i++){
        str[i]= tolower(str[i]);
    }
    printf("Lower case String is:%s\n",str);
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/cb563417-ad27-4c1a-8883-feadc70eb7d7)



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM

```
#include <stdio.h>
#include <string.h>
 
int main()
{
  	char str[100];
  	int i=0, totalwords;
  	totalwords = 1;
  	scanf("%[^\n]%*c",str);
    do
	{
	    if(str[i]==' '){
	        totalwords++;
	    }
	    i++;
	}while(str[i] != '\0');	
	printf("%d", totalwords);
	
  	return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/e061ec84-3e22-4af1-8de3-0347046a5dd1)


## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
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

## PROGRAM

```
#include <stdio.h>  
#include<string.h>

int compare(char str1[],char str2[]);  
int main()  
{  
   char str1[100];  
   char str2[100];  
   
   scanf("%s",str1);  
    
   scanf("%s",str2);  
   int c= compare(str1,str2);   
   if(c==0){  
   printf("strings are same\n"); 
   }
   else{
   printf("strings are not same\n");  
   }
  
   
}  

int compare(char a[],char b[]){  
    int i=0;   
    while(a[i]==b[i]&& a[i]!='\0' && b[i]!='\0'){  
        i++;
    }
        if(a[i]==b[i])
            return 0;
        else
            return 1;
        
    
}
    
```

## OUTPUT

 ![image](https://github.com/user-attachments/assets/20622834-9846-4999-be71-0c40c4cd55a4)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


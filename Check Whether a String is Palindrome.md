## AIM
To write a C program to check whether a given string is palindrome or not using functions.
## PROGRAM
~~~
#include <stdio.h>

int isPalindrome(char str[])
{
    int i, len = 0;

    while(str[len] != '\0')
    {
        len++;
    }

    for(i = 0; i < len / 2; i++)
    {
        if(str[i] != str[len - i - 1])
        {
            return 0;
        }
    }

    return 1;
}

int main()
{
    char str[100];

    printf("Enter a string: ");
    scanf("%s", str);

    if(isPalindrome(str))
        printf("Palindrome");
    else
        printf("Not Palindrome");

    return 0;
}
~~~
## OUTPUT
<img width="833" height="176" alt="image" src="https://github.com/user-attachments/assets/f838dffc-cedd-4b6a-974a-17ac197d3122" />

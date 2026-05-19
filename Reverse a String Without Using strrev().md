## AIM
To write a C program to reverse a string without using library functions like strrev().

## PROGRAM
~~~
#include <stdio.h>

void reverseString(char str[])
{
    int i, len = 0;
    char temp;

    while(str[len] != '\0')
    {
        len++;
    }

    len--;

    for(i = 0; i < len; i++, len--)
    {
        temp = str[i];
        str[i] = str[len];
        str[len] = temp;
    }
}

int main()
{
    char str[100];

    printf("Enter a string: ");
    scanf("%s", str);

    reverseString(str);

    printf("Reversed string: %s", str);

    return 0;
}
~~~
## OUTPUT
<img width="806" height="198" alt="image" src="https://github.com/user-attachments/assets/2e5ae5a9-15a1-4b84-aae6-dee611db01b3" />

~~~

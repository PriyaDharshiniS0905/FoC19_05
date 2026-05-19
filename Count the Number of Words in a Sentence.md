## AIM
To write a C program to count the number of words in a sentence using a function.
## PROGRAM
~~~
#include <stdio.h>

int countWords(char str[])
{
    int i, count = 1;

    for(i = 0; str[i] != '\0'; i++)
    {
        if(str[i] == ' ')
        {
            count++;
        }
    }

    return count;
}

int main()
{
    char str[100];

    printf("Enter a sentence: ");
    fgets(str, sizeof(str), stdin);

    printf("Number of words = %d", countWords(str));

    return 0;
}
~~~
## OUTPUT
<img width="635" height="207" alt="image" src="https://github.com/user-attachments/assets/971b1b5d-5e02-4ab5-83f3-9bed58d17ae0" />

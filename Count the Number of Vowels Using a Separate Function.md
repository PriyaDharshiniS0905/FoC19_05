## AIM
To write a C program to read a string and count the number of vowels using a separate function.
## PROGRAM
~~~
#include <stdio.h>

int countVowels(char str[])
{
    int i, count = 0;

    for(i = 0; str[i] != '\0'; i++)
    {
        if(str[i]=='a' || str[i]=='e' || str[i]=='i' || str[i]=='o' || str[i]=='u' ||
           str[i]=='A' || str[i]=='E' || str[i]=='I' || str[i]=='O' || str[i]=='U')
        {
            count++;
        }
    }

    return count;
}

int main()
{
    char str[100];

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    printf("Number of vowels = %d", countVowels(str));

    return 0;
}
~~~
## OUTPUT
<img width="493" height="233" alt="image" src="https://github.com/user-attachments/assets/d26b28b4-ab2d-4a4d-883c-680396922278" />

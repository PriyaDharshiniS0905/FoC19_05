## AIM
to Calculate the Length of a String Manually

## PROGRAM
~~~

#include <stdio.h>

int stringLength(char str[])
{
    int len = 0;

    while(str[len] != '\0')
    {
        len++;
    }

    return len;
}

int main()
{
    char str[100];

    printf("Enter a string: ");
    scanf("%s", str);

    printf("Length of string = %d", stringLength(str));

    return 0;
}
~~~
## OUTPUT
<img width="599" height="197" alt="image" src="https://github.com/user-attachments/assets/23ce167a-6414-47a2-84e1-beecc02d194a" />

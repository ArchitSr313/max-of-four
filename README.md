# max-of-four
c program to find max of four numbers using functions
#include <stdio.h>

int findMax(int num1, int num2, int num3, int num4)
{
    int max = num1;
    if (num2 > max)
        max = num2;
    if (num3 > max)
        max = num3;
    if (num4 > max)
        max = num4;

    return max;
}

int main()
{
    int num1, num2, num3, num4;

    printf("Enter four numbers: ");
    scanf("%d %d %d %d", &num1, &num2, &num3, &num4);

    int max = findMax(num1, num2, num3, num4);

    printf("The maximum of the four numbers is: %d\n", max);

    return 0;
}

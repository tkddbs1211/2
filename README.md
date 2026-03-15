#include <stdio.h>

int main()
{
    float input;

    printf("과제 2) 입력\n");
    printf("입력값: ");
    scanf_s("%f", &input);

    short fixed = (short)(input * 256);

    printf("과제 2) 출력\n");
    for (int i = 15; i >= 0; i--)
    {
        printf("%d", (fixed >> i) & 1);

        if (i == 8)
            printf(".");
    }
    printf("\n");

    return 0;
}

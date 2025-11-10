# How-to-find-GCD-of-two-numbers
Using C language program is made which gives the output to find the GCD of two numbers
#include <stdio.h>
int main() {
    int a, b, gcd;
    scanf("%d%d", &a, &b);
    while(b != 0) {
        int temp = b;
        b = a % b;
        a = temp;
    }
    printf("%d", a);
    return 0;
}

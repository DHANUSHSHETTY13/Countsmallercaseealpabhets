# Countsmallercaseealpabhets
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[100];
    int count = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    for (int i = 0; str[i] != '\0'; i++) {
        if (islower(str[i])) {
            count++;
        }
    }

    printf("Number of lowercase alphabets: %d\n", count);

    return 0;
}

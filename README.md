#include <stdio.h>

int main() {
    char ch;
    int spaces = 0, newlines = 0;

    printf("Enter text (Press Ctrl+D/Ctrl+Z to end):\n");

    while ((ch = getchar()) != EOF) {
        if (ch == ' ')
            spaces++;
        else if (ch == '\n')
            newlines++;
    }

    printf("\nNumber of Whitespaces = %d", spaces);
    printf("\nNumber of Newlines = %d", newlines);

    return 0;
}

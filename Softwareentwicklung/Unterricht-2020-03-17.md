## Unterricht: Di, 17.03.2020

- Keine PLF zum Thema Streams
- Projek wie gehabt auf Github pushen und die Aufgaben in Teams abgeben
- Gemeinsames durchgehen des C-Skriptums

```c
#include <stdio.h>

#define MAX_VALUES 100

void printNumbers(int numbers[]) {
    int i = 0;
    printf("Gespeicherte Zahlen: \n");
    while (i < MAX_VALUES && numbers[i] >= 0) {
        printf("%d\n", numbers[i]);
        i++;
    }
}

int main() {
    int numbers[MAX_VALUES];
    int input = 0;
    int i = 0;

    printf("Geben Sie beliebig viele Zahlen ein, -1 beendet die Ausgabe!\n");

    do {
        printf("? ");
        scanf("%d", &input);

        numbers[i] = input;
        i++;

    } while (i < MAX_VALUES && input >= 0);

    printNumbers(numbers);

    return 0;
}
```

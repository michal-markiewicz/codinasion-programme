---
title: Rupee to Paise
description: Write a program to convert Rupee to Paise
tags:
  - python
  - c
  - cpp
  - java
contributors:
  - harshi1122
  - luiscff
  - nurhaliza
---

## Write a program to convert rupee to paise

```txt
Input:  15.95
Output: 1595
```

---

<CodeBlock>

```python
# input in rupee ( can be both decimal or integer value)
x=float(input('Input: '))

# output in paise
print('Output: ',int(x*100))
```

```c
#include <stdio.h>

int main()
{
    float x;

    // input in rupees
    printf("Amount in Rupees : ");
    scanf("%g", &x);

    // output in paise
    printf("Amount in Paise : %g\n", x * 100);
    return 0;
}
```

```cpp
#include <iostream>
using namespace std;
int main()
{
    double paise, rupees;
    cout << "Please enter desired rupee amount for paise conversion : ";
    cin >> rupees;
    paise = rupees * 100; // paise calculation

    cout << "\nTotal Rupees : " << rupees << " rupees" << endl;
    cout << "Total Paise  : " << paise << " paise" << endl;
    return 0;
}
```

```java
import java.util.Scanner;

public class rs_to_p {
    public static void main(String args[]) {
        double paise;
        Scanner in = new Scanner(System.in); // will create a new Scanner instance which points to the input stream
                                             // passed as argument
        System.out.print("Please enter desired rupee amount for paise conversion : ");
        double rupees = in.nextDouble(); // scans the next token of the input as a Double
        paise = rupees * 100; // paise calculation
        System.out.println("\nTotal Rupees : " + rupees + " rupees \nTotal Paise  : " + (long) paise + " paise");
        in.close();
    }
}
```

</CodeBlock>

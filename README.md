# Good Turn CF:


This C++ program reads input and prints `"Yes"` or `"No"` depending on whether the sum of two numbers is greater than 6. Let's go through it step-by-step:

### Code Breakdown:

```cpp
#include <iostream>
using namespace std;
```

* Includes the input/output stream library to allow use of `cin` and `cout`.
* `using namespace std;` avoids the need to prefix `std::` for every standard library function.

---

```cpp
int main() {
    int t;
    cin >> t;
```

* Declares an integer `t` and reads its value from the user. This is the **number of test cases**.

---

```cpp
    while (t--) {
```

* A loop that runs `t` times. `t--` decreases `t` by 1 each time and runs the loop while `t` is greater than 0.

---

```cpp
        int x, y;
        cin >> x >> y;
        int s = x + y;
```

* For each test case, it reads two integers `x` and `y`.
* Then it calculates the sum `s = x + y`.

---

```cpp
        if (s > 6) {
            cout << "Yes" << endl;
        }
        else {
            cout << "No" << endl;
        }
```

* If the sum `s` is greater than 6, it prints `"Yes"`.
* Otherwise, it prints `"No"`.

---

```cpp
    }
    return 0;
}
```

* Ends the loop and returns 0, signaling successful execution.

---

### Example Input and Output:

**Input:**

```
3
2 5
1 2
4 4
```

**Output:**

```
Yes
No
Yes
```

Explanation:

* `2 + 5 = 7` → Yes
* `1 + 2 = 3` → No
* `4 + 4 = 8` → Yes

## Approach:

This C++ program is designed to handle multiple test cases where, for each case, it reads two integers, adds them, and checks if their sum exceeds 6. The user first inputs the number of test cases (t), and for each case, the program inputs two numbers (x and y), computes their sum, and compares it against the threshold value 6.

If the sum is greater than 6, the program outputs "Yes"; otherwise, it outputs "No". This approach uses a simple loop to iterate through the test cases and an if-else condition to determine the output based on the calculated sum. It's a straightforward implementation focusing on basic input/output and conditional logic.

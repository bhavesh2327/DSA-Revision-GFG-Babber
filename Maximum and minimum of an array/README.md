# Get Minimum and Maximum from an Array - C++ Solution

## 🧠 Problem Statement

Write a function that returns the **minimum** and **maximum** elements in a given array of integers.

The function should return a pair containing the minimum and maximum values respectively.

---

## ✅ Solution

We use a class `Solution` with a public method `getMinMax` which:

- Takes a vector of integers as input.
- Iterates through the array using a single loop.
- Keeps track of the current minimum and maximum values.
- Returns them as a pair.

---

## 📌 Code

```cpp
#include <iostream>
#include <vector>
#include <limits.h>
using namespace std;

class Solution {
  public:
    pair<int, int> getMinMax(vector<int> arr) {
        int mini = INT_MAX;
        int maxi = INT_MIN;

        for (int i = 0; i < arr.size(); i++) {
            if (arr[i] < mini)
                mini = arr[i];
            if (arr[i] > maxi)
                maxi = arr[i];
        }

        return {mini, maxi};
    }
};

int main() {
    Solution sol;
    vector<int> arr = {5, 3, 9, 1, 6};

    pair<int, int> result = sol.getMinMax(arr);
    cout << "Minimum: " << result.first << ", Maximum: " << result.second << endl;

    return 0;
}


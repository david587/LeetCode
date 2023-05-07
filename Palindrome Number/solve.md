# Intuition
<!-- Describe your first thoughts on how to solve this problem. -->

# Approach
<!-- Describe your approach to solving the problem. -->

# Complexity
- Time complexity:
<!-- Add your time complexity here, e.g. $$O(n)$$ -->

- Space complexity:
<!-- Add your space complexity here, e.g. $$O(n)$$ -->

# Code
```
/**
 * @param {number} x
 * @return {boolean}
 */
var isPalindrome = function(x) {
    let str = x.toString();
    let normal = [];
    let backward = [];

    for (let char of str) {
        normal.push(char);
    }
    for (let i = str.length - 1; i >= 0; i--) {
        backward.push(str[i]);
    }

    for (let i = 0; i < normal.length; i++) {
        if (normal[i] !== backward[i]) {
            return false;
        }
    }
    return true; 
};

```
---


---

# Approach
<!-- Describe your approach to solving the problem. -->
1. **Running Sum Function:**
    - Takes a vector of integers nums as input.
    - Initializes a variable sum to 0 and creates an empty vector v to store the running sum.
    - Iterates through each element of the input vector using a for loop.
    - For each element, adds it to the current value of sum and appends the updated sum to the v vector.
    - Returns the vector v containing the running sum of the input vector.

2. **Overall Approach:**
    - The main goal is to calculate the running sum of the given vector of integers.
    - Utilizes a loop to iterate through each element of the input vector.
    - Keeps track of the running sum (sum) as it processes each element.
    - Appends the running sum to a new vector (v) at each step.
    - Returns the resulting vector containing the running sum.

---

![Screenshot (47).png](https://assets.leetcode.com/users/images/c9b50869-f394-47b5-93ae-3f6e17220ac8_1706560600.0740259.png)

---
# Complexity

**Time Complexity:**
- O(n), where n is the size of the input vector. Each element is processed once in a linear fashion.

**Space Complexity:**
- O(n), as the space used for the output vector (v) is directly proportional to the size of the input vector.

# Code
```
class Solution {
public:
    vector<int> runningSum(vector<int>& nums) 
    {
        int sum=0;
        vector<int>v;
        for(int i=0;i<nums.size();i++)
        {
            sum=sum+nums[i];
            v.push_back(sum);
        }
        return v;
    }
};
```

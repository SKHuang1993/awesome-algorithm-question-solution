# Is Power Of Two （是否是2的幂）



## From 

 [LeetCode 231](https://leetcode.com/problems/power-of-two/description/)



## Question

Given an integer, write a function to determine if it is a power of two.




## Solution  



### C++

```c++
class Solution {
public:
    bool isPowerOfTwo(int n) {
        
        if ( n == 1){
            return true;
        }
        
        if ( n >= 2 && n%2 == 0){
            return isPowerOfTwo(n/2);
        }
        
        return false;
    }
};
```


## Palindrome Number

Link Problem [Palindrome Number](https://leetcode.com/problems/palindrome-number/)

```cpp
class Solution {
public:
long ReverseNumber(int Number)
{
	long Remainder = 0, Reversed = 0;

	while (Number > 0)
	{
		Remainder = Number % 10; 
		Number = Number / 10; 
		Reversed = Reversed * 10 + Remainder;
	}

	return Reversed;
}
    bool isPalindrome(int x) {
        return x == ReverseNumber(x);
    }
};
```

## Reverse Integer

Link Problem [Reverse Integer](https://leetcode.com/problems/reverse-integer/)

```cpp
class Solution {
public:
    int reverse(int x) {
        long Remainder = 0, Reversed = 0;

	while (abs(x) > 0)
	{
		Remainder = x % 10; 
		x = x / 10; 
		Reversed = Reversed * 10 + Remainder;
	}
    return (Reversed < INT_MIN || Reversed > INT_MAX) ? 0 : Reversed;
    }
};
```
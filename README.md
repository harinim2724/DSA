Given a positive integer n, find the sum of the first and the last digit of n.

 Examples:

Input: n = 12345
Output: 6
Explanation: 1st and last digits are 1 and 5.

class Solution {
    public int cornerDigitSum(int n) {
        int last=n%10;
        int first=n;
        while(first>=10){
            first=first/10;
        }
        return last+first;
        
    }
}

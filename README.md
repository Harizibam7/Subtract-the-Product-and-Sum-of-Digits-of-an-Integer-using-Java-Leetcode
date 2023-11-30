# Subtract-the-Product-and-Sum-of-Digits-of-an-Integer-using-Java-Leetcode

    class Solution {
        public int subtractProductAndSum(int n) {
            int sum =0;
            int mul =1;
            while(n>0){
                int rem = n % 10;
                sum+=rem;
                mul*=rem;
                n/=10;
            }
            return mul-sum;
        }
    }

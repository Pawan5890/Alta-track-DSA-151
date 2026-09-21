Question no. - #48
leetcode no.- 153. Find Minimum in Rotated Sorted Array
code :-


class Solution {
public:
    int findMin(vector<int>& nums) {
        int i = 0 , r = nums.size() - 1 , mid;
        while(i<r){
            mid = (i + r)/2;

            if(nums[mid] < nums[r]){
                r = mid;
            }
            else{
                i = mid + 1;
            }
        }
        return nums[i];
        
    }
};


<img width="1440" height="814" alt="Screenshot 2026-09-21 at 10 29 45 PM" src="https://github.com/user-attachments/assets/7f0b9a81-3015-4c09-b0c9-8f709d267e06" />



Question no. - #58
leetcode no.- 215. Kth Largest Element in an Array

code :-

class Solution {
public:
    int findKthLargest(vector<int>& nums, int k) {
        sort(nums.begin(),nums.end());
        return nums[nums.size()-k];
    }
};


<img width="1440" height="813" alt="Screenshot 2026-09-21 at 10 33 14 PM" src="https://github.com/user-attachments/assets/ab7cfe21-c838-4480-9c5e-d3d3420cc33b" />





Question no. - #121
leetcode no. - 50. Pow(x, n)

code :-
class Solution {
public:
    double myPow(double x, int n) {
        return pow(x,n);
    }
};

<img width="1440" height="815" alt="Screenshot 2026-09-21 at 10 38 34 PM" src="https://github.com/user-attachments/assets/18e61ad7-9221-4ccf-a6ac-c480e134f519" />


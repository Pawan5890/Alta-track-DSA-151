leetcode no. 283 - Move zeroes

Code:-
class Solution {
public:
    void moveZeroes(vector<int>& nums) {
        int j = 0;   

        for (int i = 0; i < nums.size(); i++) {
            if (nums[i] != 0) {
                swap(nums[i], nums[j]);
                j++;
            }
        }
    }
};

<img width="1280" height="725" alt="image" src="https://github.com/user-attachments/assets/6ae6ed77-2738-4a27-a400-0937dcff5ea4" />







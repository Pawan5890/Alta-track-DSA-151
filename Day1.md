Ouestion no. #1
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

![Uploading image.png…]()




Question no.- #1
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

Question no - #2
leetcode no .- 169. Majority Element

code:-
class Solution {
public:
    int majorityElement(vector<int>& nums) {
    int n = nums.size();
    sort(nums.begin() , nums.end());
    return nums[n/2];
    }
};

<img width="1440" height="817" alt="Screenshot 2026-09-16 at 10 44 16 PM" src="https://github.com/user-attachments/assets/8a37b03a-fce7-4fec-a4d5-420f164d7853" />








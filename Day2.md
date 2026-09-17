Question no.- #3
leetcode no. - 189. Rotate Array
code :- 


class Solution {
public:
    void rotate(vector<int>& nums, int k) {
        int n = nums.size();
        k=k % n;
        reverse(nums.begin(),nums.end());
        reverse(nums.begin(),nums.begin() + k);
        reverse (nums.begin()+ k, nums.end());
    }
};


<img width="1440" height="814" alt="Screenshot 2026-09-17 at 10 26 38 AM" src="https://github.com/user-attachments/assets/76b1df41-e9a2-45a1-a556-68c37fb293ff" />


Question no. - #14
leetcode no. - 1. Two Sum
code :-


class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        unordered_map<int, int> mp;  // value -> index

        for (int i = 0; i < nums.size(); i++) {
            int need = target - nums[i];

            if (mp.find(need) != mp.end()) {
                return {mp[need], i};
            }

            mp[nums[i]] = i;
        }

        return {}; // guaranteed one solution exists
    }
};


<img width="1440" height="813" alt="Screenshot 2026-09-17 at 10 37 37 AM" src="https://github.com/user-attachments/assets/6309c970-9a8f-4a57-89fe-13a9f1aa5522" />

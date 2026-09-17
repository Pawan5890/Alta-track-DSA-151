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

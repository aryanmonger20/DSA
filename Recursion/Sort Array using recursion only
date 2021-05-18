

class Solution
{

    void insert(vector<int> &v, int n)
    {
        if (v.size() == 0 || v[v.size() - 1] <= n)
        {
            v.push_back(n);
            return;
        }
        int temp = v.back();
        v.pop_back();
        insert(v, n);
        v.push_back(temp);
    }

public:
    void sort(vector<int> &nums)
    {
        if (nums.size() == 0)
        {
            return;
        }
        int k = nums.back();
        nums.pop_back();
        sortArray(nums);
        insert(nums, k);
        return;
    }
    vector<int> sortArray(vector<int> &nums)
    {
        sort(nums);
        return nums;
    }
};
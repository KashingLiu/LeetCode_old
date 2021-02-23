class Solution {
    public TreeNode divide(int[] nums, int left, int right) {
        if (left > right) {
            return null;
        }
        int mid = left + (right - left) / 2;
        TreeNode root = new TreeNode(nums[mid]);
        root.left = divide(nums, left, mid - 1);
        root.right = divide(nums, mid + 1, right);
        return root;
    }
    public TreeNode sortedArrayToBST(int[] nums) {
        return divide(nums, 0, nums.length - 1);
    }
}

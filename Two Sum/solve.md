# Intuition
<!-- Describe your first thoughts on how to solve this problem. -->

# Approach
<!-- Describe your approach to solving the problem. -->

# Complexity
- Time complexity:
<!-- Add your time complexity here, e.g. $$O(n)$$ -->

- Space complexity:
<!-- Add your space complexity here, e.g. $$O(n)$$ -->

# Code
```
function twoSum(nums, target) {
   let match = [];

   for(let i =0; i<nums.length; i++){
      for(let j = i+1; j<nums.length; j++){
         if(nums[i] + nums[j] === target){
            match.push(i,j)
            return match;
         }
      }
   }
   return match;
}
```
Method 1
---------------------------------
//using 2 for loops 
//complexity O(n^2)

var twoSum = (nums, target) => {
  let i,j,len= nums.length;
  for(i=0; i<len-1; i++) {           //O(n)
    for(j=i+1; j<len; j++) {        //O(n)
     if(nums[i]+nums[j]==target) {
     		return [i, j];
     }
    }
  }
}

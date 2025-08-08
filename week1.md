Adam Hodgins

# Day 1
I’m starting my full-stack bootcamp today.

## DSA Problems

### Two Sum - Time Complexity: O(n)
```/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {
    for (let i = 0; i< nums.length-1; i++){
        val1 = nums[i]
        for (let j = i+1; j<nums.length;j++){
            if (val1+nums[j] == target){
                return [i,j]
            }
        }
    }
    return [0,0]
};```


### Valid Anagram - Time Compelxity: O(n)
```/**
 * @param {string} s
 * @param {string} t
 * @return {boolean}
 */
var isAnagram = function(s, t) {
    if (s.length != t.length){
        return false
    }
    charS = [...s]
    charT = [...t]
    charS.sort()
    charT.sort()

    for (let i = 0; i<charS.length;i++){
        if (charS[i] != charT[i]){
            return false
        }
    }
    return true
};```
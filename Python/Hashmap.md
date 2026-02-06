# Hashmap & set 

## What's Hashmap algorithm 

Hashmap algorithm is sturctured for search an value saved in memory from a key. The advantege of this algorithm is that even you are increasing the number of keys, so also you are 
increasing the map, the time for the search the key is equal. This works beacause the key are distributed in buckets, and each bucket have the same time per search because of the 
use o a hash function that guarantee of a normalized distribuion. In python, the hashmap algorithm can be used with dictionary structure. 

In few words, HashMap is a data structure that allows save and find information quick from a key 

## Exercise

### Two sum (LeetCode 1)

In this exercise,  the main idea for using dictionary is: I need remember a past number

```py
class Solution(object):
    def twoSum(self, nums, target):
        seen = {}

        for i, num in enumerate(nums):
            complement = target - num
            if complement in seen:
                return [seen[complement], i]
            seen[num] = i
```


HashMap ≠ Set

Set: só pergunta “existe?”

HashMap: pergunta “existe?” + “qual o valor associado?”


2️⃣ Contains Duplicate (LeetCode 217)

3️⃣ Valid Anagram (LeetCode 242)

4️⃣ First Unique Character in a String (LeetCode 387)

5️⃣ Majority Element (LeetCode 169)

6️⃣ Intersection of Two Arrays (LeetCode 349)

7️⃣ Subarray Sum Equals K (LeetCode 560)

8️⃣ Two Sum II – Input Array Is Sorted (LeetCode 167)

9️⃣ Group Anagrams (LeetCode 49)

🔟 Top K Frequent Elements (LeetCode 347)

# Hashmap & set 

## What's Hashmap algorithm 

A hashmap is a data structure designed to retrieve a value stored in memory using a key. One of its main advantages is that even as the number of keys increases, the lookup time remains constant. This is possible because keys are distributed across buckets using a hash function, which ensures a uniform distribution. In Python, hashmaps are implemented using the dictionary data structure.

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

## What's set 

First, let's understand the difference between a hashmap and a set. A hashmap asks if there is a specific key, and if there is, which value is assigned to it. A set just asks if there is a specific value.

A set works like a mathematical set. It does not repeat values, because repeated elements are treated as the same thing: {1, 1, 2} is actually {1, 2}. Like in mathematics, you can perform operations between subsets, such as union, intersection, and subtraction, and simetric difference.

<img width="1105" height="516" alt="image" src="https://github.com/user-attachments/assets/d042db44-9d5d-48e2-b7fa-73ab036517e0" />


## Exercise 

### Contains Duplicate (LeetCode 217)

```
class Solution(object):
    def containsDuplicate(self, nums):
        """
        :type nums: List[int]
        :rtype: bool
        """
        seen = set()

        for num in nums:
            if num in seen: 
                return True 
            seen.add(num)
        return False 

```
3️⃣ Valid Anagram (LeetCode 242)

4️⃣ First Unique Character in a String (LeetCode 387)

5️⃣ Majority Element (LeetCode 169)

6️⃣ Intersection of Two Arrays (LeetCode 349)

7️⃣ Subarray Sum Equals K (LeetCode 560)

8️⃣ Two Sum II – Input Array Is Sorted (LeetCode 167)

9️⃣ Group Anagrams (LeetCode 49)

🔟 Top K Frequent Elements (LeetCode 347)

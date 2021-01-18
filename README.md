# python-dictionaries
python dictionaries

Dictionaries are used to store data values in key:value pairs.
A dictionary is a collection which is unordered, changeable and does not allow duplicates.

```
phonebook = {
"Frank" : 121564789,
"Sarah" : 789456123,
"Kelly" : 456789133
}

print(phonebook)  // {'Frank': 121564789, 'Sarah': 789456123, 'Kelly': 456789133}
```

Populating a dictionary
```
def two_sum(nums, target):
    d = {}
    # populate our dictionary with key/value pairs
    for index, num in enumerate(nums):
        # num is the key, index the value
        d[num] = index
 
    # loop over all of the nums again
    for index, num in enumerate(nums):
        diff = target - num
        # if diff in dictionary, we have the answer
        if diff in d:
            # index is current number w/the value in the dictionary
            # d[diff] gives the index tied to the value
            return [index, d[diff]]

    return[-1, -1]

print(two_sum(nums = [1,3,8,7,4,11], target = 19))
# print(two_sum(nums = [4,3,5], target = 8))

```

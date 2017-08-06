# Binary search
* Used to find value in a sorted sequence
* Maintains a contiguous subsequence of intial sequence where target value is surely located. This sub sequence is called the __*search space*__. Intially, entire sequence of the problem set serves as a search space.


#### Iterative binary search
```python
def search(search_space, query):
   if not search_sequence:
      return None
   high, low = len(search_space) - 1, 0 
   while high < low:
      mid = (high + low) / 2
      mid_element = search_space[mid]
      if mid_element == query:
         return mid
      if mid_element > query:
         low = mid + 1
      else:
         high = mid - 1
```

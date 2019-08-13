def two_sum(nums, total):
  """
  this function will return the pair of the two numbers 
  such they add up to a specific target.
  """
  #edge case
  if len(nums) < 2:
    return 
  # sets for tracking
  seen = set()
  output = set()
  
  for num in nums:
    target = total -nums
    if target not in seen:
      seen.add(num)
    else:
      output.add( (min(num,target), max(num,target)))
     
  print(len(output))
  print("\n".join(map(str,list(output))))
  
two_sum([1,3,2,2],4)
  
  

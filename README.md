## LinearSearch algorithm with Ruby
```
def linear_search(searchArr,searchNum)
  index = 0
  count = 0
  searchArr.each do |arr|
    if arr == searchNum
      count += 1
    else
      index += 1
    end
  end
  if count == 0
    puts "value:#{searchNum} Array:#{searchArr} There isn't it."
  else
    puts "value:#{searchNum} Array:#{searchArr} There is it at index\s#{index}."
  end
end
```

## BinarySearch algorithm with Ruby
```
def binary_search(searchArr,searchNum)
  array = (1..array_size).to_a
  array.sort!
  leftIndex = 0
  rightIndex = array.index(array.last)
  midIndex = (rightIndex + leftIndex) / 2
  loop do
    if searchNum == array[midIndex]
      # puts "Array->#{array}:There is at #{midIndex}!"
      break;
    elsif searchNum > array[midIndex]
      midIndex += 1
    else
      midIndex -= 1
    end
  end
end
```

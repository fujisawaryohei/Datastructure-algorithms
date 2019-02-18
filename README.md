## LinearSearch algorithm with Ruby
```
searchArr = gets.chomp.split(" ").map(&:to_i)
searchNum = gets.chomp.to_i
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
```

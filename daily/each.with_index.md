配列のkeyとvalueを両方繰り返す。
# each_with_indexの場合
```ruby
array = ["Ruby", "PHP", "Python"]
array.each_with_index do |element, index|
  p "#{index}：#{element}"
end

#以下の様に出力
0：Ruby
1：PHP
2：Python
```
# each.with_indexの場合
```ruby
array = ["Ruby", "PHP", "Python"]
array.each.with_index(1) do |element, index|
  p "#{index}：#{element}"
end

1：Ruby
2：PHP
3：Python
```
https://qiita.com/kidach1/items/a00558cfb0a6a3e23f4b

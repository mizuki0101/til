# divmod
商と余りを配列で返す
10.divmod(3)
=> [3, 1]
# delete_if
```ruby
a = [1,2,3,4]
a.delete_if do |n|
  n.odd?
end
p a

=> [2, 4]
```
メソッド「要素を問わず共通する処理」
ブロック「要件によって異なる処理」

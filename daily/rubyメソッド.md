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

```ruby
numbers = [1,2,3,4,5]

new_numbers = numbers.map { |n| n * 10 }
p new_numbers

even_numbers = numbers.select { |n| n.even? }
p even_numbers

even_numbers = numbers.reject { |n| n.even? }
p even_numbers

sum = numbers.inject(0) { |result , n | result += n }
p sum

even_numbers = numbers.select(&:even?)
p even_numbers

=>
[10, 20, 30, 40, 50]
[2, 4]
[1, 3, 5]
15
[2, 4]
```
# 範囲
### [1...5]
..で1〜5まで  
...で1〜4まで
### 範囲オブジェクトに対してto_aメソッドを使用することで配列が作成される
```ruby
a = [1,2,3,4,5]
p a[0...3]

p (1..5).to_a
# splat展開
p [*1..5].to_a

=>
[1, 2, 3]
[1, 2, 3, 4, 5]
[1, 2, 3, 4, 5]

```
# 多重代入で残りを配列として受け取る
```ruby
e, *f = 100,200,300
p e
p f

=>
100
[200, 300]
```
# 文字列配列に変換する
```ruby
a = "abcd".chars
p a

=>
"a", "b", "c", "d"]
```
# 配列の一部を変更する
```rub
a = Array.new(5) {'test'}
str = a[0]
p str.upcase
p a

=>
"TEST"
["test", "test", "test", "test", "test"]
```

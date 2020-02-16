# 畳み込み演算
```ruby
配列オブジェクト.inject {|初期値, 要素| ブロック処理 }
```
eachやmapのように繰り返し処理を行うメソッド  
## 配列の合計値を出力
前提条件
```ruby
array = [1, 4, 6, 34, 235]
```
１行で配列の合計値を出せる
```ruby
result = array.inject{ |sum, i| sum + i}
=> 280
初期値を渡さなかったのでsumに1、iに4が代入される
```
シンボルを用いた場合
```ruby
result = array.inject(:+)
=> 280
```
## 初期値を渡す場合
```ruby
numbers = [1,2,3,4,5]
puts numbers.inject(100){|result, item | result + item}
```
初期値として100が渡されているので、「100+1+2+3+4+5」と同じ処理がされる。  
## *と-の場合
```ruby
### result = array.inject(:*)
=> 191760
# 1 * 4 * 6 * 34 * 235 = 191760

### result = array.inject(:-)
=> -278
# 1 - 4 - 6 - 34 - 235 = -278
```















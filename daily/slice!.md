```ruby
def extra_end(a)
  str = a.slice!(-2, 2)
  puts str*3
end

extra_end('Hello')
extra_end('ab')
extra_end('Hi')
```
```ruby
def left2(str)
  left2 = str.slice!(0,2)
  puts str + left2
end
```
```
def first_two(a)
  p a.slice(0,2)
end

# def first_two(a)
#   if a.length >= 2
#     str = a.slice(0,2)
#     p str
#   else
#     p a
#   end
# end

first_two('Hello')
first_two('ab')
first_two('x')
first_two(' ')

# 任意の文字列の最初の2文字のみ
# 出力するメソッドを作りましょう。
# 文字列が2文字以下だと文字列をそのまま返します。
# 例えば"x"は"x"を、空文字""は""を返します。
```

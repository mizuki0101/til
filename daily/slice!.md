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

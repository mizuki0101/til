# 基本
`and`と`&&`は左辺を評価して結果が真なら右辺も評価する  
`or` と`||`左辺を評価して結果が偽なら右辺も評価する  
  
`and`と`or`は優先順位が低い
# 優先順位が低いとは？
```ruby
a = true && false
p a #false

b = true and false
p b #true

c = (true and false)
p c #false
```
`&&` > `=` > `and`という関係になり`=`の方が`and`より先に処理が行われる
# 優先順位表
```ruby
(優先順位:高)
  !  ~
  **
  *  /  %
  +  -
  <<  >>
  &
  |  ^
  >  >=  <  <=
  ==  !=
  &&
  ||
  ..  ...
  ?:
  =
  not
  and  or
(優先順位:低)

```

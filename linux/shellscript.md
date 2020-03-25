```
var="これは変数です"
VaR_2="これも変数です"
echo "Var_2=$VaR_2"

VaR_2="VaR_2が変更されました。"
echo ${VaR_2}

readonly var
var="readonly varを変えてみる。"
```

```
echo "1 - ${var:-wordSetInEcho1}"
echo "2 - var = ${var}"
echo "3 - ${var:=wordSetInEcho3}"
echo "4 - var = ${var}"
unset var
echo "5 - ${var:+wordSetInEcho5}"
echo "6 - var = $var"
var="newVarValue"
echo "7 - ${var:+wordSetInEcho7}"
echo "8 - var = $var"
echo "9 - ${var:?StandardErrorMessage}"
echo "10 - var = ${var}"
```

# if 文

```
利用例
$ cat if
#!/bin/bash

if [ 1 -ge 2 ]
 then
  echo "AAA"
 else
  echo "BBB"
fi
$
$ ./if
BBB
```

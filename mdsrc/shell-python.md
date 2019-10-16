---
title: Gitpress　で Python
date: 2019-10-17
---
Gitpress で　Pythonが動くようになったので、動かしてみる。。。Code-Knackの方ではShellも動くようになったみたいなので、Bashでコマンドが動くのか見てみよう。。。

## Python　は　2.7系らしいが。。

```python
def foo():
    a=1
    b=2
    c=a+b
    print("Hello",c)

foo()
```
2.7 系なら printの後ろに（）いらないはずだけど。。Python3系なのかな？？


## Bashは動くのか？
```SH
#!/usr/bin/env bash
echo "OK"
```
Runがでないな。

## Python でセッションが継続されるらしいが。。
```python
def inc(x):
    return x + 1
```

```python
def dec(x):
    return x - 1
```
```python
a = 10
# you can use inc and dec function aboved.
a = inc(10)
print('a = ', a)
# output: a = 11
a = dec(10)
print('a = ', a)
# output: a = 9
```
されないようです(笑)

でも。。これ便利かも
```python
def dec(x):
    return x - 1
def inc(x):
    return x + 1
a = 10
# you can use inc and dec function aboved.
a = inc(10)
print('a = ', a)
# output: a = 11
a = dec(10)
print('a = ', a)
# output: a = 9
```
import とかできるのかな？？ 　
import os
os.system("ls")
はインプリメントされてなかったみたい(笑)　当たり前だな。。

ドキュメントがないので。。どこまで動くのかは不明(笑)
https://gitpress.io/c/helps/languages

どうも、これでPythonを動かしているみたいですね。
http://skulpt.org/

これもブラウザ上でPythonが動かせる。。



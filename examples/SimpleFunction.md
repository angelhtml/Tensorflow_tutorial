<h1>Create a simple function</h1>
<p align='center'>
<img src='https://www.guru99.com/images/1/080418_1250_WhatisaTens41.jpg'>
</p>

``` python
x = tf.constant([5], dtype=tf.int32)
z = tf.constant([6], dtype=tf.int32)
c = tf.constant([5], name =	"constant")
square = tf.constant([2], name =	"square")
f = tf.multiply(x, z) + tf.pow(x, square) + z + c
print(f)
```

Output

``` python
tf.Tensor([66], shape=(1,), dtype=int32)
```

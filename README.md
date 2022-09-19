
<h1>tensorflow tutorial</h1>              

<h2>Create a tensor of n-dimension</h2>
You begin with the creation of a tensor with one dimension, namely a scalar<br/>
To create a tensor, you can use <b>tf.constant()</b> as shown in the below TensorFlow tensor shape example:   

``` python

tf.constant(value, dtype, name = "")
tf.constant(value, shape=(col, row) )
'''
- `value`: Value of n dimension to define the tensor. Optional
- `dtype`: Define the type of data:       
    - `tf.float32`: Float variable    
    - `tf.int16`: Integer variable
    - `tf.string`: String variable 
    - `tf.bool`: Boolean variable
- "name": Name of the tensor. Optional. By default, `Const_1:0`
'''
```

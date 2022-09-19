
<h1>tensorflow tutorial</h1>              

<h2>Create a tensor of n-dimension 📜</h2>
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

Below, a float tensor is converted to integer using you use the method cast (<dtype: 'float32'>)

``` python

# Change type of data
type_float = tf.constant(3.123456789, tf.float32)
type_int = tf.cast(type_float, dtype=tf.int32)
print(type_float.dtype)
print(type_int.dtype)

```

<h2>Creating operator ➗</h2>
Some Useful TensorFlow operators
You know how to create a tensor with TensorFlow. It is time to learn how to perform mathematical operations.
TensorFlow contains all the basic operations. You can begin with a simple one. You will use TensorFlow method to compute the square of a number. This operation is straightforward because only one argument is required to construct the tensor.
The square of a number is constructed with <b>tf.sqrt(x)</b> with x as a floating number

``` python

x = tf.constant([4.0], dtype = tf.float32)
print(tf.sqrt(x))

```

The output returned a tensor object and not the result of the square of 4. In the example, you print the definition of the tensor and not the actual evaluation of the operation. In the next section, you will learn how TensorFlow works to execute the operations.
Following is a list of commonly used operations. The idea is the same. Each operation requires one or more arguments
<ul>
<li>tf.add(a, b)</li>
<li>tf.substract(a, b)</li>
<li>tf.multiply(a, b)</li>
<li>tf.div(a, b)</li>
<li>tf.pow(a, b)</li>
<li>tf.exp(a)</li>
<li>tf.sqrt(a)</li>
</ul>

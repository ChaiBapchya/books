Pattern Recognition is basis of all algos in ML, AI.

Supervised Learning
- the training is performed by the minimization of a particular loss function (cost function), which represents the output error with respect to the desired output system.
- labeled samples (Xi,Yi)

Unsupervised Learning
- unlabeled data
- The system, therefore, develops and organizes the data, looking for common characteristics among them, and changing them based on their internal knowledge.
- do not know the class a priori, and you do not even know what the possible classes are, or how numerous they are

Deep Learning
- reason 
  - availability of GPUs, massive processing power thus reduced the time needed for training networks
  - availability of large datasets, high dimensionality of data
  
- based on the way the human brain processes information and learns, responding to external stimuli
- ML model having several levels of representation of knowledge.
- deeper levels take as input the outputs of the previous levels, transforming them and always abstracting more

TensorFlow
- TensorFlow is a software library, developed by Google Brain Team within Google's Machine Learning Intelligence research organization

Python
- strongly typed and dynamic language (data types are necessary but it is not necessary to explicitly declare them)
- case-sensitive (var and VAR are two different variables),
- object-oriented (everything in Python is an object).

Data-types
- List = single-dimensional arrays, but can have list in list
- Dictionaries =  arrays that contain pairs of keys and values (hash table)
- Tuples = immutable mono-dimensional objects
```
print "This %(verbo)s un %(name)s." % {"name": "test", "verb": "is"}
 This is a test. 
```

Functions can return a tuple (tuple unpacking enables the return of multiple values). 
Lambda functions are in-line. 
Parameters are passed by reference, but immutable types (tuples, integers, strings, and so on) cannot be
changed in the function.

Multiple Inheritance

Classes
 The variables and private methods are declared by convection (it is not a rule of language) by preceding them with two
underscores (__). 

Class variables vs Instance variables
```
class Myclass:
 common = 10
 def __init__(self):
 self.myvariable= 3
 def myfunc(self, arg1, arg2):
 return self.myvariable
 # We create an instance of the class
 >>> instance= Myclass()
 >>> instance.myfunc(1, 2)
 3
 # This variable is shared by all instances
 >>> instance2= Myclass()
 >>> instance.common
 10
 >>> instance2.common
 10
 # Note here how we use the class name
 # Instead of the instance.
 >>> Myclass.common = 30
 >>> instance.common
 30
 >>> instance2.common
 30
 # This does not update the variable in the class,
 # Instead assign a new object to the variable
 # of the first instance.
 >>> instance.common = 10
 >>> instance.common
 10
 >>> instance2.common
 30
 >>> Myclass.common = 50
 # The value is not changed because "common" is an instance variable.
 >>> instance.common
 10
 >>> instance2.common
 50
 ```
 
## Exception Handling
```
def my_func():
 try:
 # Division by zero causes an exception
 10 / 0
 except ZeroDivisionError:
 print "Oops, error"
 else:
 # no exception, let's proceed
 pass
 finally:
 # This code is executed when the block
 # Try..except is already executed and all exceptions
 # Were handled, even if there is a new
 # Exception directly in the block.
 print "finish"
 ```
 
 import libraryname
 from libraryname import functionname
 
 Running CSH scripts
 - cant run it from bash shell (terminal)
 - hence first enter CSH which has command prompt as %
 
 Error
 ```
 $ source bin/activate.csh 
-bash: alias: deactivate: not found
-bash: alias: `test $?_OLD_VIRTUAL_PATH !': invalid alias name
-bash: deactivate: command not found
-bash: setenv: command not found
-bash: setenv: command not found
-bash: bin/activate.csh: line 37: syntax error: unexpected end of file
```

Solution
```
Chaitanyas-MacBook-Pro:tensorflow chaitanyabapat$ csh
[Chaitanyas-MacBook-Pro:~/tensorflow] chaitanyabapat% source bin/activate.csh
```


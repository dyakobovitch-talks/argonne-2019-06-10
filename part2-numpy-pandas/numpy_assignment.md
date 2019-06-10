# Numpy Exercise

# Instructions 

For the first part of this assignment, we'll be solving problems by using `numpy`. Since `Pandas` is built on top of `numpy`, it's good to be familiar with `numpy` and know what it provides. Below, we'll ask that you solve questions **by using `numpy`**. While you could answer the questions below without using `numpy` arrays, the focus of these questions is for you to use `numpy` arrays and get familiar with their methods (there are a lot of them). Remember how fast they are compared to the `list` as an alternative! 

As a final note, a lot of the questions below are kind of simplistic, and could possibly be written in a single line or two. As such, you might wonder why we're asking you to write functions for them, or why they are even questions at all. As you've hopefully found throughout this course, programming skills increase quite a bit simply through repetition, which is a majority of the reason we've asked you to write functions for each question below. After this, you will hopefully never forget that when we define a function in Python, it starts with `def my_func_name():`. In addition, these one off functions will get you exposure to some of the most common and useful methods available on a `numpy array`. 

# Assignment Questions

**Hint**: [Broadcasting](http://docs.scipy.org/doc/numpy-1.10.1/user/basics.broadcasting.html) is a concept that will be particularly useful here. 

1. Write a function that takes in a one-dimensional `numpy array` and normalizes it (i.e. subtracts off the mean and divides by the standard deviation). Return the normalized array 
2. Now create a version of `1` that takes in a two-dimensional `numpy array` and normalizes it along the columns (i.e. for each column subtract off its mean and divide by its standard deviation). Return the normalized array. 
3. Write a function that creates a `numpy array` of an inputted shape, filled with an inputted number. Your function should have three parameters - `num_cols`, `num_rows`, and `fill_value`. As an example, if I called your function with `num_cols=4`, `num_rows=3`, and `fill_value=2`, then your function should output a 3 by 4 array of 2s. Return the newly created array.  
4. Write a function that takes in a one-dimensional `numpy array`, an `int`, and a mathematical operator (either `+`, `-`, `/`, or `*`) as a string, and then performs the indicated operation on each element of the `array`, using the inputted `int`. For example, if I inputted a `numpy array`, 2, and `'*'`, you should multiply each element of the `array` by 2. If I inputted a `numpy array`, 5, and `'-'`, then you should subtract 5 from every element in the array. Return the resulting array. 
5. Write a function that takes in one argument, an `int`, and creates a one-dimensional array that is the inputted number of elements long. Make the one-dimensional array full of random floating point numbers between 0 and 1 (**Hint**: Check out `numpy.random.random()`). Return the resulting array. 
6. Now, alter your solution to `5` to take in two parameters that will denote the final shape of your array of random floating point numbers (so now you will potentially end up with a two-dimensional array). Name these parameters `num_rows` and `num_cols`. Return the resulting array. 
7. Write a function that will take in a one-dimensional `numpy array`, as well as an `int`, and randomly sample the inputted integer number of elements from the inputted array (**Hint**: Check out `numpy.random.choice()`). Return the randomly sampled elements. 
8. Write a function that will take in a one-dimensional `numpy array` and replace the maximum element in it with a `0`. Return the resulting array. 
9. Write a function that takes in an `int`, creates a one-dimensional `numpy array` of the numbers from `0` up to `int`, and then returns the cumulative sum of all those numbers. 
10. Write a function that takes in two two-dimensional `numpy arrays` and performs matrix multiplication, the dot product, between the two. You should construct it such that the first array is multiplied by the second (i.e. the number of columns of the first has to equal the number of rows of the second; you can assume that your inputs will meet this criteria). Return the result of the multiplication. 
11. Write a function that takes in two two-dimensional `numpy arrays` and performs element-wise multiplication between the two. You can assume that the two arrays are of the same size. Return the array resulting from the multiplication. 
12. Write a function that takes in a one-dimensional `numpy array` and returns the top 5 elements (you can assume it's an array of numbers). 
13. Write a function that takes in a two-dimensional `numpy array` and returns the smallest 5 elements of each column (**Hint**: The `axis` parameter on the `numpy` function you use might come in handy here). 

# Extra-Credit 

1. Write a function that takes in an integer, and does the following: 

* Creates an array of the numbers from 0 up to that inputted integer 
* Reshapes it to be the largest `n` * `n` array that it could be, discarding 
any elements that are extra (i.e. if you want to make a 10 x 10, but have 102 elements, discard the last 2)
* Returns the cumulative sum of the column means

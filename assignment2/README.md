# Some notification for assignment 2

In q2_initialization.py, it should be noticed that the return for _xavier_initializer(shape, **kwargs) should be a tenserflow variable. 

If you only return a tensor, the test will also passed, but when you build the model and use this function as initializer, they are not variables and thus will not be updated through trainning, so be careful!

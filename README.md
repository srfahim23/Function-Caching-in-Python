# Function-Caching-in-Python
Function caching is a technique for improvidng the performance of a program by storing the results of a function call so that you can reuse the result instead of recomputing them every time the function is called. This can be particularly useful when a function is computationally expensive, or when the inputs to the function are unlikely to change frequently.

In Python, function caching can be achieved using the ffunctool.lru_cache decorator. The functool_lru_cache decorator is used to cache the result of a function so that you can reuse the results instead of recomputing them every time the funciton is called. Here's an example:

    import functools

    @functool.lru_cache(maxsize=None)
    def fib(n):
        if n < 2:
            return n 
        return fib(n-1) + fib(n-2)    

    print(fib(20))    
    # Output: 6765

As you can see, the functool.lru_cache decorator is used to cache the result of the ib function. The maxsize parameter is used to specify the maximu number of result to cache. If maxsize is set to None, the cache will have an unlimited size.

# Benefits of Function Caching
Function caching can have a significqant impact on the perfomance of a program, particularly for computaionally expensive funcitons. By caching the results of a function, you can avoid having to recompute the results every time the funciton is called, which can save a significant amount of time and computational resources.

Another benefit of function caching is that it can simplify the code of a program by removing the need to manually cache the results of a function. With the functool.lru_cache decorator, the caching is handled automatically, so you can focus on writting the core logic of your program.

# Conclusion
Funciton caching is a technique for improving the performance of a program by storing the results of a function so that you can reuse the results instead of recomputing them every every time the functool.lru_cache decorator, which provides an easy and effcient way to cache the results of a function. Whether you're writting a computationally expensive program, or just want to simplify your code, function caching is a great technique to have in your toolbox.
# Code Review 

### Thoughts on Formating and Structure:

1. For classes and methods names, the code keeps to the PSR-2 coding standard practise.
2. The code is well organised, class name is properly written in stydly case and mecthods written in camel case.
3. Proper comments are also provided to each method, and function names begin with a verb, indicating what function is doing.

## BookingController.php 

### Areas of Improvement: 

1. The code is missing request **validation** to before processing the request which may lead to error or unwanted data into database.
2. There are many **helper function** in laravel by using these function you can make the application more **laravel freindly**, Here is one examplewhich you can replace in your code on ``Line 85 (except() instead of array_except())``.
3. In the code i have seen some unwanted if else block statements such as ``Line 195 => distanceFeed()`` which is causing less code clarity and redability. 
4. Add more inline comments to explain the purpose of methods, complex logic, or any non-obvious implementation details.


## BookingRepository.php

 ### Areas for Improvement: 

1. In tis file i have seen there is nested if else **arrow-type code** below ``Line 492`` which is hard to read and maintain, we can reduce this issue by adding **guard-clause** for if condtion which shortten the line of codes and also produce better readable and maintainable code. 
2. In programming **fucntion** are heart of the language, if we use them with good **knowledge**, It can make a **beatifull** code to read and also reduce the **repetation** of code instead it will be reuseable for the same sake, I have remove some code below ``line no 547 `` which was to analyse weather it's phone or physical; or both and wrap it into beautiful ``Function analyseJobType()``.
 
## Overall Assessment: 

I have examine code it is written with good practices, such as seperation of concern and adhering to ``RESTful`` conventions.But still i suggest there is some space to
improvement like adding validation on request before proccessing data, remove unwanted if else blocks, error handling, make more function for generic use of code, avoid arrow-type code,if we made these improvement the code become more robust, readable and secure.  



 
I have gone through the code, the repository pattern you have used is good to increase the testability, database access code can be reused, to make things DRY (Don't-Repeat-Yourself) and other allot of advantages we have by using repository pattern. I personally has been used repository pattern in my project. 

On the other hand, we also have some cons of repository pattern. If you go down the road of a Generic Repository you will end up with duplication in your queries and you will find it much harder to unit test the code that uses the repository as you will have to test the queries as well.

Now, about coding standards and flaws, I found some described below:

1- Data validation is missing: Data validation is very critical to protect from malicious data and runing handling data without any error.

2- Error handling is very poor: There is no proper error alert to developer/admin in case of error.

3- Too much nested checks: Instead to deviding logic into functions, nested checks are used and no comments on checks.

4- Lengthy functions: Function should be 15 lines long according to PSR standard. But here no function is less than 15 line. As well as, other PSR standared are not followed.

5- Queries result are not evaluated, either they are giving the data or not. Consequently they can produce error. Try Catch should be used and proper error handling.

I'm refactoring the code what i can do within the specified time. The truth is, refactoring of code will never end. More you time put in, more you can refactor it on single line level. 

I didn't know the bussiness logic here, so i cannot refactor it like it should be done on query and logic level. However, I have done what i can do here.
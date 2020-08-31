#     **An Empirical Study of Method Chaining in Java**

# TITLE: https://static.csg.ci.i.u-tokyo.ac.jp/papers/20/nakamaru-msr2020.pdf 

# AUTHORS: 
Tomoki Nakamaru , Tomomasa Matsunaga ,  Tetsuro Yamazaki ,  Soramichi Akiyama , Shigeru Chiba 
 
# CONFERENCE: 
An Empirical Study of Method Chaining in Java
# INTRODUCTION AND MOTIVATION: 
The Method chaining is a programming style in which multiple method invocations are chained in a single expression as follows: 
class ChainAble { 
  firstMethod() {      console.log('This is the First Method');      return this;    } In this page we discus about the empirical and chaining study in java the Authors try to describe us that the designed the more easy programs. And they did change programming style for promoted as the good practice for better readability programming in Java. And gives the two steps. 1)Eliminates temporary variables. and 2) Groups related method invocation into single expression. The put in 1st step that the (alert dialog’s) and in 2nd non-chaining style. And in this chaining online materials gives only one StackOverflow thread with 17 answers on the several blogpost. And the programmers observe and changes in quartiles. And the programmers increasing and method chaining. In which They do manual inspection on 385 randomly selected method and invocation. 
 # RESEARCH METHODOLOGY:
We classified a chain as Conditional Execution when it is conditionally executed as shown above. We found nine chains (2.34%) of this pattern in the sampled dataset. The code in this pattern can be transformed into a single chain if the library provides a method that takes a lambda expression as its argument: 
if ( buildLogger . isInfoEnabled ()) { 
 buildLogger . info ( message , throwable ); 
 } 
# RESULT: 
This paper presented our empirical study of method chaining in Java. We analysis that widespread and quantitatively creasing trend of method that provide information for future language, library and delelopment. 
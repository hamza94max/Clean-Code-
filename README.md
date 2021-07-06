# Clean-Code-
Clean code Book by RobertC.Martin <br><br>


[ Quick Review ](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)<br><br>





<img src = "https://user-images.githubusercontent.com/54688005/124272711-680c6f00-db3f-11eb-82b6-47d36cd49ee4.jpg" width =100%>
  <img width ="10%"/> 
  <br> <br>


**3 Important principles**

- **Dry ( Don't repeat Yourself )** every piece of knowloedge must have a single repersentation within a system .<br>

1- Don't copy-paste code in multiple places .<br>
2- Don't have different code pieces that do the same thing. <br>
3- Create a separate component for reusable stuff .<br>

- **Kiss ( Keep it Simple , Stupid )** avoid unnecessary complexity and don't  "reinvent the wheel ".<br>

1-  Use the features of the language to the most ( Sorting , mapping , etc ).<br>
2- Minimize the complexity of each component . <br>
3- Don't do "over Engineering " .<br>

- **YAGNI  ( You Ain 't Gonna Need it  )** don't create things in advance , but only when you need them .<br>

1-  Don't Keep commented Code , Saying that "Yoy might need it later "<br>
2- Don't add multiple formatters and features "just in case " <br>
3- Delete anything that's not used right now .<br>





  <details close>
<summary> MeaningFul Names </summary>
  <br>

<br><br>
### Choosing good names takes time but saves more than it takes. So take care with your names and change them when you find better ones. Everyone who reads your code (including you) will be happier if you do.<br>
  
• The name of a variable, function, or class, should answer all the big questions. It
should tell you why it exists, what it does, and how it is used. If a name requires a comment, then the name does not reveal its intent. <br>
 <br>
• **Avoid Disinformation** ( Information that will mislead you ) : a truly awful example of disinformative names would be the use of lower-case **L** or
uppercase **O** as variable names <br>
  ex: Do not refer to a grouping of accounts as an accountList unless it’s actually a List.
   <br><br>
• **Avoid noise Words** : Noise words are redundant. The word **variable** should never appear in a variable
name. The word **table** should never appear in a table name.
 <br> <br>
• **Use Searchable Names** : Single-letter names and numeric constants have a particular problem in that they are not
easy to locate across a body of text. <br>
  ex: the name e is a poor choice for any variable for which a programmer might
need to search.
  
• **Avoid Mental Mapping** : Readers shouldn’t have to mentally translate your names into other names they already
know. This problem generally arises from a choice to use neither problem domain terms
nor solution domain terms. 
  
  This is a problem with single-letter variable names. Certainly a loop counter may be
named **i** or **j** or **k** (though never **l**!) if its scope is very small and no other names can conflict with it
  
• **Class Names** : Classes and objects should have noun or noun phrase names like Customer, WikiPage,
Account, and AddressParser. Avoid words like Manager, Processor, Data, or Info in the name
of a class. A class name should not be a verb.
  
• **Method Names**  Methods should have verb or verb phrase names like postPayment, deletePage, or save.
Accessors, mutators, and predicates should be named for their value and prefixed with get,
set, and is
  
</details>






  <details close>
<summary> Funcations </summary>
  <br><br>
  
  
  
### The first rule of functions is that they should be small. The second rule of functions is that they should be smaller than that. a function should be no bigger than a screen-full.
 <br>
  
• This implies that the blocks within **if** statements, **else** statements, **while** statements, and
so on should be one line long. Probably that line should be a **function call** . <br>
  
• **FUNCTIONS SHOULD DO ONE THING. THEY SHOULD DO IT WELL. THEY SHOULD DO IT ONLY.**
  
• **Use Descriptive Names** : Don’t be afraid to make a name long. A long descriptive name is better than a short
enigmatic name. A long descriptive name is better than a long descriptive comment. Use
a naming convention that allows multiple words to be easily read in the function names,
and then make use of those multiple words to give the function a name that says what
it does <br>
  
  <details close>
<summary> Funcations Arguments </summary>
    
    
### The ideal number of arguments for a function is zero (niladic). Next comes one (monadic), followed closely by two (dyadic). Three arguments (triadic) should be avoided where possible. More than three (polyadic) requires very special justification—and then shouldn’t be used anyway.<br><br>
    
  
• **Flag arguments** are ugly. Passing a boolean into a function is a truly terrible practice. It
immediately complicates the signature of the method, loudly proclaiming that this function
does more than one thing. It does one thing if the flag is true and another if the flag is false!<br>
    
    
• When a function seems to need more than two or three arguments, it is likely that some of
those arguments ought to be wrapped into a class of their own. Consider, for example, the
difference between the two following declarations:<br><br>
Circle makeCircle(double x, double y, double radius);<br>
Circle makeCircle(Point center, double radius);<br>
  
  </details>
  </details>
  
  
  

</details>













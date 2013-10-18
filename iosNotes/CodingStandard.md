1)	Cutting and pasting. If you find yourself hitting ctrl-C, there's something wrong. This is emblematic of some design flaw. 

2)	Long functions. Functions should run no longer than 20-30 lines. They should be viewable on a single screen. If your function is longer than this, break it up.

3)	Use of the God object. We often see this in Objective-C when a class accepts tons of delegates itself and does not delegate business logic to models. Non-RESTful Rails controllers or bloated Android fragments can suffer from this too. 

4)	Only using the MVC pattern. Other classes/models can and should be used for large problem sets. It is often said, "Skinny controller. Fat model." But models can be excessive too.

5)	Don't use magic numbers. Use constants instead. 

6)	Be suspicious of long switch statements. 

7)	Classes that do many different things. If you need to do something to an account, perform that on account object, NOT in a controller. 

8)	Dependency inversion. Model your code against the high-level behavior you want. Don't model your interfaces against what you want the code to do. 

9)	Don't hardcode environment-specific configuration properties. Filepaths, database connection properties, timeout settings, hostnames, etc should be configurable without having to modify application code

10)	Inconsistent naming of functions/classes/variables. Follow the conventions of the language you are working with (i.e. underscore_delimited vs camelCased).

11)	Unintuitive variable/function/class names. Be explicit and avoid confusing abbreviations. Examples of poor variable names: cnt, ft, lblRsdAmt. Better alternatives: imagesCount, fragmentTransaction, labelRaisedAmount. Generally speaking you should not use single letter variable names.

12)	Follow the Liskov Substitution Principle. Derived class objects must be usable through their base class interfaces without clients of the base class being able to tell the difference 

13)	Interface Segregation. Split interfaces such that they benefit clients 

14)	Follow the Open/Closed Principle. Software modules should be open for extension but closed for modification 


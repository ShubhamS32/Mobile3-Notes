## Don't break encapsulation by globalizing variables

e.g.
	public class Foo {
		private int iHeight = 0;

		public void functionOne() {
			// ..
			getSometing();
			// ..
		}

		public void getSometing() {
			// ..
			iHeight =  (some calculations)
			// ..
		}
	}


## Avoid duplication of code

## Avoid unnecessary complexity

## Avoid long classes

## Avoid long methods
   Functions should run no longer than 20-30 lines. If your function is longer than this, break it up.
## Don't use poor names for variables, methods, classes

## Remove code that not used

## Dont keep absolute Sdk path, it should be relative

## Keep proper indentation. Use 4 space instead tab.

## Variables and method naming convention
	Variables: Use lowercase with underscore to name variables
	Methods: Use CamelCase to name methods

## File and Directory Naming Conventions and Folder Structure						 				
	- Parent folder name start with Capital letters and use CamelCase but not the child folders							
	- Reserved Characters And Words Avoid using the following characters from appearing in file names 
	: / > < | ; &
	- All file names are case sensitive




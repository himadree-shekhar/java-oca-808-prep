
2025-02-06:
1-Java Basics:

package statement:
- Only 1 package statement at most in a Java source file.
- it must be the 1st statement in the file.
- import statement must be after package declaration.
- Java runtime expects the class to be found under its package (java packageName.ClassName)
- Different source files can have the same package name, But source files must be in the same folder structure. 

Wildcard (.*) in import static VS import package different.

import package.* 
- will not import the subpackage. It will only import the classes in package.

import static java.lang.System.*;
- To import all the static members of the System class(Not package)

import static:
- can't use a wildcard (*) to import static members from a package.
- Static imports allow you to import static members (fields or methods) of a class.

static :
- static methods can't be abstract because abstract methods are meant to be overridden by instances.
- static init 1st and only once and also can hold a reference to any object

class can be refer by:
- Import The class
- Import Entire Package(.*)
- Fully Qualified Name : package.subpackage.ClassName

Which packages are automatically imported ?
- java.lang
- unnamed packages (or default package) that are in the same directory

File Names:
- For public classes: The file name must match the class name (case-sensitive)
- Only 1-public-class-1-file rule
- For non-public classes: The file name can be anything valid

Modifier:
- Java allows the modifiers to be written in any order because they don't change the meaning of the declaration.
- By default, members (fields, methods, etc.) are accessible only within the same package.
- Local variables can not have visibility modifiers because they only exist within the method or block they are declared in.
- You can only apply the final modifier to local variables.
- Local variables are stored on the stack and must be initialized before use.

'final' Non-Access Modifier:
- Applying final to a method does not change the method signature.

public final static void main(String[] args) :
- main method is already static, so it cannot be overridden anyway, so adding final does not affect its behavior.

About Command-Line Argument : (String[] args) :
- can change the parameter name(args) to anything
- (String args[]) and (String[] args) are identical
- args Non-Null Array

Array VS Varargs :
- (String[] args) and (String... args) are essentially the same.
- Varargs treated as an array of Strings internally



Tricky when a global variable and a local variable have the same name :
- This case is variable shadowing

'this' keyword :
- 'this' is always reference to the current instance.
- 'this' cannot be reassign to reference to a new object.
- an instance variable is accessible through 'this'.
- 'this' can also access static variables too.

(fields and methods) Order:
- In Java, we can declare fields and methods in any order inside the class.

class & file:
- In Java, the order in which classes appear in the file does not matter if both classes are in the same file.
- It is not necessary for the class containing main() method to be public class.

try and catch Blocks:
- Variables defined in the try block are not visible in the catch block because they have separate scopes.

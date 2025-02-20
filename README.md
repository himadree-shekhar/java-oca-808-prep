
2025-02-06:
1-Java Basics:

package statement:
- Only 1 package statement at most in a Java source file.
- it must be the 1st statement in the file.
- import statement must be after package declaration.
- Java runtime expects the class to be found under its package (java packageName.ClassName)
- Different source files can have the same package name, But source files must be in the same folder structure. 

import static java.lang.System.*;
- To import all the static members of the System class(Not package)

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

Why Can't We Use Access Modifiers(public, private, protected) on Local Variables?
- Because the scope of the local variables only belong to its block

public final static void main(String[] args) :
- main method is already static, so it cannot be overridden anyway, so adding final does not affect its behavior.

About Command-Line Argument : (String[] args) :
- can change the parameter name(args) to anything

Tricky when a global variable and a local variable have the same name :
- This case is variable shadowing

'this' keyword :
- 'this' is always reference to the current instance.
- 'this' cannot be reassign to reference to a new object.
- an instance variable is accessible through 'this'.
- 'this' can also access static variables too.

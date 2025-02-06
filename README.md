
2025-02-06:
1-Java Basics:

package statement:
- Only 1 package statement at most in a Java source file
- it must be the 1st statement in the file.

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

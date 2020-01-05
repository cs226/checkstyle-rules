# checkstyle-rules
601.226 Data Structures CheckStyle Rules

The `cs226_ckecks.xml` is a copy of [`google_checks.xml`](https://github.com/checkstyle/checkstyle/blob/master/src/main/resources/google_checks.xml) which implements the [Google Java Style Guide](http://google.github.io/styleguide/javaguide.html) that is modifictions to enforce the following rules:

- Enforcement for JavaDocs (class and public methods, no need for fields, setters, getters, overridden methods)
- Do not check package name
- Constants are all caps
- Allow e|ex|t for CatchParameterName
- Disallow unused|redundant|illegal import statements
- Line length limit set to 80
- Accepts methods with at most 20 lines, not counting empty lines and single line comments
- Limit number of parameters to 5
- Enforce one outer type per file.
- Disallow white space before certain operations like unary operations.
- Disallow redundant modifier (e.g. adding public abstract for interface methods)
- Avoid nested blocks
- Avoid accidental overloading
- Enforce declaration order
- Enforce switch default case comes last
- Enforce equals and hashcode are both overridden (if one is)
- Enforce using equals on objects (rather than ==)
- Avoid initializing twice
- Avoid hiding fields (except in constructors, setters and abstract methods)
- Avoid catching generic exception (like Exception, RuntimeException, etc)
- Avoid throwing generic exception
- Avoid assignments as expressions
- Ensure that for loop control variables are not modified inside the for block
- Disallow using try inside try.
- Disallow overriding Object.clone() and Object.finalize()
- Warn over-complicated boolean expressions
- Warn to use equals() with String(s)
- Must have methods in an interface
- Exceptions must be immutable
- Limit each method (even private ones) to throw at most 4 exceptions (not enforced on JDK methods)
- Restrict the number of other classes a given class relies on (set to 10)
- Checks cyclomatic and NPath complexity against a specified limit.
  It is a measure of the minimum number of possible paths through the source and therefore the number
  of required tests, it is not a about quality of code!
- Ensure comment indentation is consistent

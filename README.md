# Readable pylint messages 
Prepared with `pylint --list-msgs` for pylint v1.6.4
##blacklisted-name 
####C0102 - Black listed name "%s" 
Used when the name is listed in the black list (unauthorized names). 
##invalid-name 
####C0103 - Invalid %s name "%s"%s 
Used when the name doesn't match the regular expression associated to its type (constant, variable, class...). 
##missing-docstring 
####C0111 - Missing %s docstring 
Used when a module, function, class or method has no docstring.Some special methods like __init__ doesn't necessary require a docstring. 
##empty-docstring 
####C0112 - Empty %s docstring 
Used when a module, function, class or method has an empty docstring (it would be too easy ;). 
##unneeded-not 
####C0113 - Consider changing "%s" to "%s" 
Used when a boolean expression contains an unneeded negation. 
##singleton-comparison 
####C0121 - Comparison to %s should be %s 
Used when an expression is compared to singleton values like True, False or None. 
##misplaced-comparison-constant 
####C0122 - Comparison should be %s 
Used when the constant is placed on the left sideof a comparison. It is usually clearer in intent to place it in the right hand side of the comparison. 
##unidiomatic-typecheck 
####C0123 - Using type() instead of isinstance() for a typecheck. 
The idiomatic way to perform an explicit typecheck in Python is to use isinstance(x, Y) rather than type(x) == Y, type(x) is Y. Though there are unusual situations where these give different results. 
##consider-using-enumerate 
####C0200 - Consider using enumerate instead of iterating with range and len 
Emitted when code that iterates with range and len is encountered. Such code can be simplified by using the enumerate builtin. 
##consider-iterating-dictionary 
####C0201 - Consider iterating the dictionary directly instead of calling .keys() 
Emitted when the keys of a dictionary are iterated through the .keys() method. It is enough to just iterate through the dictionary itself, as in "for key in dictionary". 
##bad-classmethod-argument 
####C0202 - Class method %s should have %s as first argument 
Used when a class method has a first argument named differently than the value specified in valid-classmethod-first-arg option (default to "cls"), recommended to easily differentiate them from regular instance methods. 
##bad-mcs-method-argument 
####C0203 - Metaclass method %s should have %s as first argument 
Used when a metaclass method has a first agument named differently than the value specified in valid-classmethod-first-arg option (default to "cls"), recommended to easily differentiate them from regular instance methods. 
##bad-mcs-classmethod-argument 
####C0204 - Metaclass class method %s should have %s as first argument 
Used when a metaclass class method has a first argument named differently than the value specified in valid-metaclass-classmethod-first-arg option (default to "mcs"), recommended to easily differentiate them from regular instance methods. 
##line-too-long 
####C0301 - Line too long (%s/%s) 
Used when a line is longer than a given number of characters. 
##too-many-lines 
####C0302 - Too many lines in module (%s/%s) 
Used when a module has too much lines, reducing its readability. 
##trailing-whitespace 
####C0303 - Trailing whitespace 
Used when there is whitespace between the end of a line and the newline. 
##missing-final-newline 
####C0304 - Final newline missing 
Used when the last line in a file is missing a newline. 
##trailing-newlines 
####C0305 - Trailing newlines 
Used when there are trailing blank lines in a file. 
##multiple-statements 
####C0321 - More than one statement on a single line 
Used when more than on statement are found on the same line. 
##superfluous-parens 
####C0325 - Unnecessary parens after %r keyword 
Used when a single item in parentheses follows an if, for, or other keyword. 
##bad-whitespace 
####C0326 - %s space %s %s %s 
Used when a wrong number of spaces is used around an operator, bracket or block opener. 
##mixed-line-endings 
####C0327 - Mixed line endings LF and CRLF 
Used when there are mixed (LF and CRLF) newline signs in a file. 
##unexpected-line-ending-format 
####C0328 - Unexpected line ending format. There is '%s' while it should be '%s'. 
Used when there is different newline than expected. 
##bad-continuation 
####C0330 - Wrong %s indentation%s%s. 
TODO 
##wrong-spelling-in-comment 
####C0401 - Wrong spelling of a word '%s' in a comment: 
Used when a word in comment is not spelled correctly. 
##wrong-spelling-in-docstring 
####C0402 - Wrong spelling of a word '%s' in a docstring: 
Used when a word in docstring is not spelled correctly. 
##invalid-characters-in-docstring 
####C0403 - Invalid characters %r in a docstring 
Used when a word in docstring cannot be checked by enchant. 
##multiple-imports 
####C0410 - Multiple imports on one line (%s) 
Used when import statement importing multiple modules is detected. 
##wrong-import-order 
####C0411 - %s comes before %s 
Used when PEP8 import order is not respected (standard imports first, then third-party libraries, then local imports) 
##ungrouped-imports 
####C0412 - Imports from package %s are not grouped 
Used when imports are not grouped by packages 
##wrong-import-position 
####C0413 - Import "%s" should be placed at the top of the module 
Used when code and imports are mixed 
##old-style-class 
####C1001 - Old-style class defined. 
Used when a class is defined that does not inherit from anotherclass and does not inherit explicitly from "object". This message can't be emitted when using Python >= 3.0. 
##syntax-error 
####E0001 -  
Used when a syntax error is raised for a module. 
##unrecognized-inline-option 
####E0011 - Unrecognized file option %r 
Used when an unknown inline option is encountered. 
##bad-option-value 
####E0012 - Bad option value %r 
Used when a bad value for an inline option is encountered. 
##init-is-generator 
####E0100 - __init__ method is a generator 
Used when the special class method __init__ is turned into a generator by a yield in its body. 
##return-in-init 
####E0101 - Explicit return in __init__ 
Used when the special class method __init__ has an explicit return value. 
##function-redefined 
####E0102 - %s already defined line %s 
Used when a function / class / method is redefined. 
##not-in-loop 
####E0103 - %r not properly in loop 
Used when break or continue keywords are used outside a loop. 
##return-outside-function 
####E0104 - Return outside function 
Used when a "return" statement is found outside a function or method. 
##yield-outside-function 
####E0105 - Yield outside function 
Used when a "yield" statement is found outside a function or method. 
##return-arg-in-generator 
####E0106 - Return with argument inside generator 
Used when a "return" statement with an argument is found outside in a generator function or method (e.g. with some "yield" statements). This message can't be emitted when using Python >= 3.3. 
##nonexistent-operator 
####E0107 - Use of the non-existent %s operator 
Used when you attempt to use the C-style pre-increment orpre-decrement operator -- and ++, which doesn't exist in Python. 
##duplicate-argument-name 
####E0108 - Duplicate argument name %s in function definition 
Duplicate argument names in function definitions are syntax errors. 
##abstract-class-instantiated 
####E0110 - Abstract class %r with abstract methods instantiated 
Used when an abstract class with `abc.ABCMeta` as metaclass has abstract methods and is instantiated. 
##bad-reversed-sequence 
####E0111 - The first reversed() argument is not a sequence 
Used when the first argument to reversed() builtin isn't a sequence (does not implement __reversed__, nor __getitem__ and __len__ 
##continue-in-finally 
####E0116 - 'continue' not supported inside 'finally' clause 
Emitted when the `continue` keyword is found inside a finally clause, which is a SyntaxError. 
##method-hidden 
####E0202 - An attribute defined in %s line %s hides this method 
Used when a class defines a method which is hidden by an instance attribute from an ancestor class or set by some client code. 
##access-member-before-definition 
####E0203 - Access to member %r before its definition line %s 
Used when an instance member is accessed before it's actually assigned. 
##no-method-argument 
####E0211 - Method has no argument 
Used when a method which should have the bound instance as first argument has no argument defined. 
##no-self-argument 
####E0213 - Method should have "self" as first argument 
Used when a method has an attribute different the "self" as first argument. This is considered as an error since this is a so common convention that you shouldn't break it! 
##invalid-slots-object 
####E0236 - Invalid object %r in __slots__, must contain only non empty strings 
Used when an invalid (non-string) object occurs in __slots__. 
##assigning-non-slot 
####E0237 - Assigning to attribute %r not defined in class slots 
Used when assigning to an attribute not defined in the class slots. 
##invalid-slots 
####E0238 - Invalid __slots__ object 
Used when an invalid __slots__ is found in class. Only a string, an iterable or a sequence is permitted. 
##inherit-non-class 
####E0239 - Inheriting %r, which is not a class. 
Used when a class inherits from something which is not a class. 
##inconsistent-mro 
####E0240 - Inconsistent method resolution order for class %r 
Used when a class has an inconsistent method resolutin order. 
##duplicate-bases 
####E0241 - Duplicate bases for class %r 
Used when a class has duplicate bases. 
##non-iterator-returned 
####E0301 - __iter__ returns non-iterator 
Used when an __iter__ method returns something which is not an iterable (i.e. has no `next` method) 
##unexpected-special-method-signature 
####E0302 - The special method %r expects %s param(s), %d %s given 
Emitted when a special method was defined with an invalid number of parameters. If it has too few or too many, it might not work at all. 
##invalid-length-returned 
####E0303 - __len__ does not return non-negative integer 
Used when an __len__ method returns something which is not a non-negative integer 
##import-error 
####E0401 - Unable to import %s 
Used when pylint has been unable to import a module. 
##used-before-assignment 
####E0601 - Using variable %r before assignment 
Used when a local variable is accessed before it's assignment. 
##undefined-variable 
####E0602 - Undefined variable %r 
Used when an undefined variable is accessed. 
##undefined-all-variable 
####E0603 - Undefined variable name %r in __all__ 
Used when an undefined variable name is referenced in __all__. 
##invalid-all-object 
####E0604 - Invalid object %r in __all__, must contain only strings 
Used when an invalid (non-string) object occurs in __all__. 
##no-name-in-module 
####E0611 - No name %r in module %r 
Used when a name cannot be found in a module. 
##unbalanced-tuple-unpacking 
####E0632 - Possible unbalanced tuple unpacking with sequence%s: left side has %d label(s), right side has %d value(s) 
Used when there is an unbalanced tuple unpacking in assignment 
##unpacking-non-sequence 
####E0633 - Attempting to unpack a non-sequence%s 
Used when something which is not a sequence is used in an unpack assignment 
##bad-except-order 
####E0701 - Bad except clauses order (%s) 
Used when except clauses are not in the correct order (from the more specific to the more generic). If you don't fix the order, some exceptions may not be catched by the most specific handler. 
##raising-bad-type 
####E0702 - Raising %s while only classes or instances are allowed 
Used when something which is neither a class, an instance or a string is raised (i.e. a `TypeError` will be raised). 
##misplaced-bare-raise 
####E0704 - The raise statement is not inside an except clause 
Used when a bare raise is not used inside an except clause. This generates an error, since there are no active exceptions to be reraised. An exception to this rule is represented by a bare raise inside a finally clause, which might work, as long as an exception is raised inside the try block, but it is nevertheless a code smell that must not be relied upon. 
##raising-non-exception 
####E0710 - Raising a new style class which doesn't inherit from BaseException 
Used when a new style class which doesn't inherit from BaseException is raised. 
##notimplemented-raised 
####E0711 - NotImplemented raised - should raise NotImplementedError 
Used when NotImplemented is raised instead of NotImplementedError 
##catching-non-exception 
####E0712 - Catching an exception which doesn't inherit from BaseException: %s 
Used when a class which doesn't inherit from BaseException is used as an exception in an except clause. 
##slots-on-old-class 
####E1001 - Use of __slots__ on an old style class 
Used when an old style class uses the __slots__ attribute. This message can't be emitted when using Python >= 3.0. 
##super-on-old-class 
####E1002 - Use of super on an old style class 
Used when an old style class uses the super builtin. This message can't be emitted when using Python >= 3.0. 
##bad-super-call 
####E1003 - Bad first argument %r given to super() 
Used when another argument than the current class is given as first argument of the super builtin. 
##missing-super-argument 
####E1004 - Missing argument to super() 
Used when the super builtin didn't receive an argument. This message can't be emitted when using Python >= 3.0. 
##no-member 
####E1101 - %s %r has no %r member 
Used when a variable is accessed for an unexistent member. 
##not-callable 
####E1102 - %s is not callable 
Used when an object being called has been inferred to a non callable object 
##assignment-from-no-return 
####E1111 - Assigning to function call which doesn't return 
Used when an assignment is done on a function call but the inferred function doesn't return anything. 
##no-value-for-parameter 
####E1120 - No value for argument %s in %s call 
Used when a function call passes too few arguments. 
##too-many-function-args 
####E1121 - Too many positional arguments for %s call 
Used when a function call passes too many positional arguments. 
##unexpected-keyword-arg 
####E1123 - Unexpected keyword argument %r in %s call 
Used when a function call passes a keyword argument that doesn't correspond to one of the function's parameter names. 
##redundant-keyword-arg 
####E1124 - Argument %r passed by position and keyword in %s call 
Used when a function call would result in assigning multiple values to a function parameter, one value from a positional argument and one from a keyword argument. 
##invalid-sequence-index 
####E1126 - Sequence index is not an int, slice, or instance with __index__ 
Used when a sequence type is indexed with an invalid type. Valid types are ints, slices, and objects with an __index__ method. 
##invalid-slice-index 
####E1127 - Slice index is not an int, None, or instance with __index__ 
Used when a slice index is not an integer, None, or an object with an __index__ method. 
##assignment-from-none 
####E1128 - Assigning to function call which only returns None 
Used when an assignment is done on a function call but the inferred function returns nothing but None. 
##not-context-manager 
####E1129 - Context manager '%s' doesn't implement __enter__ and __exit__. 
Used when an instance in a with statement doesn't implement the context manager protocol(__enter__/__exit__). 
##invalid-unary-operand-type 
####E1130 -  
Emitted when an unary operand is used on an object which does not support this type of operation 
##unsupported-binary-operation 
####E1131 -  
Emitted when a binary arithmetic operation between two operands is not supported. 
##repeated-keyword 
####E1132 - Got multiple values for keyword argument %r in function call 
Emitted when a function call got multiple values for a keyword. 
##not-an-iterable 
####E1133 - Non-iterable value %s is used in an iterating context 
Used when a non-iterable value is used in place whereiterable is expected 
##not-a-mapping 
####E1134 - Non-mapping value %s is used in a mapping context 
Used when a non-mapping value is used in place wheremapping is expected 
##unsupported-membership-test 
####E1135 - Value '%s' doesn't support membership test 
Emitted when an instance in membership test expression doesn'timplement membership protocol (__contains__/__iter__/__getitem__) 
##unsubscriptable-object 
####E1136 - Value '%s' is unsubscriptable 
Emitted when a subscripted value doesn't support subscription(i.e. doesn't define __getitem__ method) 
##logging-unsupported-format 
####E1200 - Unsupported logging format character %r (%#02x) at index %d 
Used when an unsupported format character is used in a logging statement format string. 
##logging-format-truncated 
####E1201 - Logging format string ends in middle of conversion specifier 
Used when a logging statement format string terminates before the end of a conversion specifier. 
##logging-too-many-args 
####E1205 - Too many arguments for logging format string 
Used when a logging format string is given too few arguments. 
##logging-too-few-args 
####E1206 - Not enough arguments for logging format string 
Used when a logging format string is given too many arguments 
##bad-format-character 
####E1300 - Unsupported format character %r (%#02x) at index %d 
Used when a unsupported format character is used in a format string. 
##truncated-format-string 
####E1301 - Format string ends in middle of conversion specifier 
Used when a format string terminates before the end of a conversion specifier. 
##mixed-format-string 
####E1302 - Mixing named and unnamed conversion specifiers in format string 
Used when a format string contains both named (e.g. '%(foo)d') and unnamed (e.g. '%d') conversion specifiers. This is also used when a named conversion specifier contains * for the minimum field width and/or precision. 
##format-needs-mapping 
####E1303 - Expected mapping for format string, not %s 
Used when a format string that uses named conversion specifiers is used with an argument that is not a mapping. 
##missing-format-string-key 
####E1304 - Missing key %r in format string dictionary 
Used when a format string that uses named conversion specifiers is used with a dictionary that doesn't contain all the keys required by the format string. 
##too-many-format-args 
####E1305 - Too many arguments for format string 
Used when a format string that uses unnamed conversion specifiers is given too many arguments. 
##too-few-format-args 
####E1306 - Not enough arguments for format string 
Used when a format string that uses unnamed conversion specifiers is given too few arguments 
##bad-str-strip-call 
####E1310 - Suspicious argument in %s.%s call 
The argument to a str.{l,r,}strip call contains a duplicate character, 
##print-statement 
####E1601 - print statement used 
Used when a print statement is used (`print` is a function in Python 3) This message can't be emitted when using Python >= 3.0. 
##parameter-unpacking 
####E1602 - Parameter unpacking specified 
Used when parameter unpacking is specified for a function(Python 3 doesn't allow it) This message can't be emitted when using Python >= 3.0. 
##unpacking-in-except 
####E1603 - Implicit unpacking of exceptions is not supported in Python 3 
Python3 will not allow implicit unpacking of exceptions in except clauses. See http://www.python.org/dev/peps/pep-3110/ This message can't be emitted when using Python >= 3.0. 
##old-raise-syntax 
####E1604 - Use raise ErrorClass(args) instead of raise ErrorClass, args. 
Used when the alternate raise syntax 'raise foo, bar' is used instead of 'raise foo(bar)'. This message can't be emitted when using Python >= 3.0. 
##backtick 
####E1605 - Use of the `` operator 
Used when the deprecated "``" (backtick) operator is used instead of the str() function. This message can't be emitted when using Python >= 3.0. 
##long-suffix 
####E1606 - Use of long suffix 
Used when "l" or "L" is used to mark a long integer. This will not work in Python 3, since `int` and `long` types have merged. This message can't be emitted when using Python >= 3.0. 
##old-ne-operator 
####E1607 - Use of the <> operator 
Used when the deprecated "<>" operator is used instead of "!=". This is removed in Python 3. This message can't be emitted when using Python >= 3.0. 
##old-octal-literal 
####E1608 - Use of old octal literal 
Usen when encountering the old octal syntax, removed in Python 3. To use the new syntax, prepend 0o on the number. This message can't be emitted when using Python >= 3.0. 
##import-star-module-level 
####E1609 - Import * only allowed at module level 
Used when the import star syntax is used somewhere else than the module level. This message can't be emitted when using Python >= 3.0. 
##fatal 
####F0001 -  
Used when an error occurred preventing the analysis of a module (unable to find it for instance). 
##astroid-error 
####F0002 - %s: %s 
Used when an unexpected error occurred while building the Astroid representation. This is usually accompanied by a traceback. Please report such errors ! 
##parse-error 
####F0010 - error while code parsing: %s 
Used when an exception occured while building the Astroid representation which could be handled by astroid. 
##method-check-failed 
####F0202 - Unable to check methods signature (%s / %s) 
Used when Pylint has been unable to check methods signature compatibility for an unexpected reason. Please report this kind if you don't make sense of it. 
##raw-checker-failed 
####I0001 - Unable to run raw checkers on built-in module %s 
Used to inform that a built-in module has not been checked using the raw checkers. 
##bad-inline-option 
####I0010 - Unable to consider inline option %r 
Used when an inline option is either badly formatted or can't be used inside modules. 
##locally-disabled 
####I0011 - Locally disabling %s (%s) 
Used when an inline option disables a message or a messages category. 
##locally-enabled 
####I0012 - Locally enabling %s (%s) 
Used when an inline option enables a message or a messages category. 
##file-ignored 
####I0013 - Ignoring entire file 
Used to inform that the file will not be checked 
##suppressed-message 
####I0020 - Suppressed %s (from line %d) 
A message was triggered on a line, but suppressed explicitly by a disable= comment in the file. This message is not generated for messages that are ignored due to configuration settings. 
##useless-suppression 
####I0021 - Useless suppression of %s 
Reported when a message is explicitly disabled for a line or a block of code, but never triggered. 
##deprecated-pragma 
####I0022 - Pragma "%s" is deprecated, use "%s" instead 
Some inline pylint options have been renamed or reworked, only the most recent form should be used. NOTE:skip-all is only available with pylint >= 0.26 
##too-many-nested-blocks 
####R0101 - Too many nested blocks (%s/%s) 
Used when a function or a method has too many nested blocks. This makes the code less understandable and maintainable. 
##simplifiable-if-statement 
####R0102 - The if statement can be replaced with %s 
Used when an if statement can be replaced with 'bool(test)'. 
##no-self-use 
####R0201 - Method could be a function 
Used when a method doesn't use its bound instance, and so could be written as a function. 
##no-classmethod-decorator 
####R0202 - Consider using a decorator instead of calling classmethod 
Used when a class method is defined without using the decorator syntax. 
##no-staticmethod-decorator 
####R0203 - Consider using a decorator instead of calling staticmethod 
Used when a static method is defined without using the decorator syntax. 
##redefined-variable-type 
####R0204 - Redefinition of %s type from %s to %s 
Used when the type of a variable changes inside a method or a function. 
##cyclic-import 
####R0401 - Cyclic import (%s) 
Used when a cyclic import between two or more modules is detected. 
##duplicate-code 
####R0801 - Similar lines in %s files 
Indicates that a set of similar lines has been detected among multiple file. This usually means that the code should be refactored to avoid this duplication. 
##too-many-ancestors 
####R0901 - Too many ancestors (%s/%s) 
Used when class has too many parent classes, try to reduce this to get a simpler (and so easier to use) class. 
##too-many-instance-attributes 
####R0902 - Too many instance attributes (%s/%s) 
Used when class has too many instance attributes, try to reduce this to get a simpler (and so easier to use) class. 
##too-few-public-methods 
####R0903 - Too few public methods (%s/%s) 
Used when class has too few public methods, so be sure it's really worth it. 
##too-many-public-methods 
####R0904 - Too many public methods (%s/%s) 
Used when class has too many public methods, try to reduce this to get a simpler (and so easier to use) class. 
##too-many-return-statements 
####R0911 - Too many return statements (%s/%s) 
Used when a function or method has too many return statement, making it hard to follow. 
##too-many-branches 
####R0912 - Too many branches (%s/%s) 
Used when a function or method has too many branches, making it hard to follow. 
##too-many-arguments 
####R0913 - Too many arguments (%s/%s) 
Used when a function or method takes too many arguments. 
##too-many-locals 
####R0914 - Too many local variables (%s/%s) 
Used when a function or method has too many local variables. 
##too-many-statements 
####R0915 - Too many statements (%s/%s) 
Used when a function or method has too many statements. You should then split it in smaller functions / methods. 
##too-many-boolean-expressions 
####R0916 - Too many boolean expressions in if statement (%s/%s) 
Used when a if statement contains too many boolean expressions 
##unreachable 
####W0101 - Unreachable code 
Used when there is some code behind a "return" or "raise" statement, which will never be accessed. 
##dangerous-default-value 
####W0102 - Dangerous default value %s as argument 
Used when a mutable value as list or dictionary is detected in a default value for an argument. 
##pointless-statement 
####W0104 - Statement seems to have no effect 
Used when a statement doesn't have (or at least seems to) any effect. 
##pointless-string-statement 
####W0105 - String statement has no effect 
Used when a string is used as a statement (which of course has no effect). This is a particular case of W0104 with its own message so you can easily disable it if you're using those strings as documentation, instead of comments. 
##expression-not-assigned 
####W0106 - Expression "%s" is assigned to nothing 
Used when an expression that is not a function call is assigned to nothing. Probably something else was intended. 
##unnecessary-pass 
####W0107 - Unnecessary pass statement 
Used when a "pass" statement that can be avoided is encountered. 
##unnecessary-lambda 
####W0108 - Lambda may not be necessary 
Used when the body of a lambda expression is a function call on the same argument list as the lambda itself; such lambda expressions are in all but a few cases replaceable with the function being called in the body of the lambda. 
##duplicate-key 
####W0109 - Duplicate key %r in dictionary 
Used when a dictionary expression binds the same key multiple times. 
##deprecated-lambda 
####W0110 - map/filter on lambda could be replaced by comprehension 
Used when a lambda is the first argument to "map" or "filter". It could be clearer as a list comprehension or generator expression. This message can't be emitted when using Python >= 3.0. 
##useless-else-on-loop 
####W0120 - Else clause on loop without a break statement 
Loops should only have an else clause if they can exit early with a break statement, otherwise the statements under else should be on the same scope as the loop itself. 
##exec-used 
####W0122 - Use of exec 
Used when you use the "exec" statement (function for Python 3), to discourage its usage. That doesn't mean you can not use it ! 
##eval-used 
####W0123 - Use of eval 
Used when you use the "eval" function, to discourage its usage. Consider using `ast.literal_eval` for safely evaluating strings containing Python expressions from untrusted sources. 
##confusing-with-statement 
####W0124 - Following "as" with another context manager looks like a tuple. 
Emitted when a `with` statement component returns multiple values and uses name binding with `as` only for a part of those values, as in with ctx() as a, b. This can be misleading, since it's not clear if the context manager returns a tuple or if the node without a name binding is another context manager. 
##using-constant-test 
####W0125 - Using a conditional statement with a constant value 
Emitted when a conditional statement (If or ternary if) uses a constant value for its test. This might not be what the user intended to do. 
##lost-exception 
####W0150 - %s statement in finally block may swallow exception 
Used when a break or a return statement is found inside the finally clause of a try...finally block: the exceptions raised in the try clause will be silently swallowed instead of being re-raised. 
##assert-on-tuple 
####W0199 - Assert called on a 2-uple. Did you mean 'assert x,y'? 
A call of assert on a tuple will always evaluate to true if the tuple is not empty, and will always evaluate to false if it is. 
##attribute-defined-outside-init 
####W0201 - Attribute %r defined outside __init__ 
Used when an instance attribute is defined outside the __init__ method. 
##bad-staticmethod-argument 
####W0211 - Static method with %r as first argument 
Used when a static method has "self" or a value specified in valid- classmethod-first-arg option or valid-metaclass-classmethod-first-arg option as first argument. 
##protected-access 
####W0212 - Access to a protected member %s of a client class 
Used when a protected member (i.e. class member with a name beginning with an underscore) is access outside the class or a descendant of the class where it's defined. 
##arguments-differ 
####W0221 - Arguments number differs from %s %r method 
Used when a method has a different number of arguments than in the implemented interface or in an overridden method. 
##signature-differs 
####W0222 - Signature differs from %s %r method 
Used when a method signature is different than in the implemented interface or in an overridden method. 
##abstract-method 
####W0223 - Method %r is abstract in class %r but is not overridden 
Used when an abstract method (i.e. raise NotImplementedError) is not overridden in concrete class. 
##super-init-not-called 
####W0231 - __init__ method from base class %r is not called 
Used when an ancestor class method has an __init__ method which is not called by a derived class. 
##no-init 
####W0232 - Class has no __init__ method 
Used when a class has no __init__ method, neither its parent classes. 
##non-parent-init-called 
####W0233 - __init__ method from a non direct base class %r is called 
Used when an __init__ method is called on a class which is not in the direct ancestors for the analysed class. 
##unnecessary-semicolon 
####W0301 - Unnecessary semicolon 
Used when a statement is ended by a semi-colon (";"), which isn't necessary (that's python, not C ;). 
##bad-indentation 
####W0311 - Bad indentation. Found %s %s, expected %s 
Used when an unexpected number of indentation's tabulations or spaces has been found. 
##mixed-indentation 
####W0312 - Found indentation with %ss instead of %ss 
Used when there are some mixed tabs and spaces in a module. 
##lowercase-l-suffix 
####W0332 - Use of "l" as long integer identifier 
Used when a lower case "l" is used to mark a long integer. You should use a upper case "L" since the letter "l" looks too much like the digit "1" This message can't be emitted when using Python >= 3.0. 
##wildcard-import 
####W0401 - Wildcard import %s 
Used when `from module import *` is detected. 
##deprecated-module 
####W0402 - Uses of a deprecated module %r 
Used a module marked as deprecated is imported. 
##relative-import 
####W0403 - Relative import %r, should be %r 
Used when an import relative to the package directory is detected. This message can't be emitted when using Python >= 3.0. 
##reimported 
####W0404 - Reimport %r (imported line %s) 
Used when a module is reimported multiple times. 
##import-self 
####W0406 - Module import itself 
Used when a module is importing itself. 
##misplaced-future 
####W0410 - __future__ import is not the first non docstring statement 
Python 2.5 and greater require __future__ import to be the first non docstring statement in the module. 
##fixme 
####W0511 -  
Used when a warning note as FIXME or XXX is detected. 
##invalid-encoded-data 
####W0512 - Cannot decode using encoding "%s", unexpected byte at position %d 
Used when a source line cannot be decoded using the specified source file encoding. This message can't be emitted when using Python >= 3.0. 
##global-variable-undefined 
####W0601 - Global variable %r undefined at the module level 
Used when a variable is defined through the "global" statement but the variable is not defined in the module scope. 
##global-variable-not-assigned 
####W0602 - Using global for %r but no assignment is done 
Used when a variable is defined through the "global" statement but no assignment to this variable is done. 
##global-statement 
####W0603 - Using the global statement 
Used when you use the "global" statement to update a global variable. Pylint just try to discourage this usage. That doesn't mean you can not use it ! 
##global-at-module-level 
####W0604 - Using the global statement at the module level 
Used when you use the "global" statement at the module level since it has no effect 
##unused-import 
####W0611 - Unused %s 
Used when an imported module or variable is not used. 
##unused-variable 
####W0612 - Unused variable %r 
Used when a variable is defined but not used. 
##unused-argument 
####W0613 - Unused argument %r 
Used when a function or method argument is not used. 
##unused-wildcard-import 
####W0614 - Unused import %s from wildcard import 
Used when an imported module or variable is not used from a `'from X import *'` style import. 
##redefined-outer-name 
####W0621 - Redefining name %r from outer scope (line %s) 
Used when a variable's name hide a name defined in the outer scope. 
##redefined-builtin 
####W0622 - Redefining built-in %r 
Used when a variable or function override a built-in. 
##redefine-in-handler 
####W0623 - Redefining name %r from %s in exception handler 
Used when an exception handler assigns the exception to an existing name 
##undefined-loop-variable 
####W0631 - Using possibly undefined loop variable %r 
Used when an loop variable (i.e. defined by a for loop or a list comprehension or a generator expression) is used outside the loop. 
##cell-var-from-loop 
####W0640 - Cell variable %s defined in loop 
A variable used in a closure is defined in a loop. This will result in all closures using the same value for the closed-over variable. 
##bare-except 
####W0702 - No exception type(s) specified 
Used when an except clause doesn't specify exceptions type to catch. 
##broad-except 
####W0703 - Catching too general exception %s 
Used when an except catches a too general exception, possibly burying unrelated errors. 
##duplicate-except 
####W0705 - Catching previously caught exception type %s 
Used when an except catches a type that was already caught by a previous handler. 
##nonstandard-exception 
####W0710 - Exception doesn't inherit from standard "Exception" class 
Used when a custom exception class is raised but doesn't inherit from the builtin "Exception" class. This message can't be emitted when using Python >= 3.0. 
##binary-op-exception 
####W0711 - Exception to catch is the result of a binary "%s" operation 
Used when the exception to catch is of the form "except A or B:". If intending to catch multiple, rewrite as "except (A, B):" 
##property-on-old-class 
####W1001 - Use of "property" on an old style class 
Used when Pylint detect the use of the builtin "property" on an old style class while this is relying on new style classes features. This message can't be emitted when using Python >= 3.0. 
##logging-not-lazy 
####W1201 - Specify string format arguments as logging function parameters 
Used when a logging statement has a call form of "logging.<logging method>(format_string % (format_args...))". Such calls should leave string interpolation to the logging method itself and be written "logging.<logging method>(format_string, format_args...)" so that the program may avoid incurring the cost of the interpolation in those cases in which no message will be logged. For more, see http://www.python.org/dev/peps/pep-0282/. 
##logging-format-interpolation 
####W1202 - Use % formatting in logging functions and pass the % parameters as arguments 
Used when a logging statement has a call form of "logging.<logging method>(format_string.format(format_args...))". Such calls should use % formatting instead, but leave interpolation to the logging function by passing the parameters as arguments. 
##bad-format-string-key 
####W1300 - Format string dictionary key should be a string, not %s 
Used when a format string that uses named conversion specifiers is used with a dictionary whose keys are not all strings. 
##unused-format-string-key 
####W1301 - Unused key %r in format string dictionary 
Used when a format string that uses named conversion specifiers is used with a dictionary that contains keys not required by the format string. 
##bad-format-string 
####W1302 - Invalid format string 
Used when a PEP 3101 format string is invalid. This message can't be emitted when using Python < 2.7. 
##missing-format-argument-key 
####W1303 - Missing keyword argument %r for format string 
Used when a PEP 3101 format string that uses named fields doesn't receive one or more required keywords. This message can't be emitted when using Python < 2.7. 
##unused-format-string-argument 
####W1304 - Unused format argument %r 
Used when a PEP 3101 format string that uses named fields is used with an argument that is not required by the format string. This message can't be emitted when using Python < 2.7. 
##format-combined-specification 
####W1305 - Format string contains both automatic field numbering and manual field specification 
Usen when a PEP 3101 format string contains both automatic field numbering (e.g. '{}') and manual field specification (e.g. '{0}'). This message can't be emitted when using Python < 2.7. 
##missing-format-attribute 
####W1306 - Missing format attribute %r in format specifier %r 
Used when a PEP 3101 format string uses an attribute specifier ({0.length}), but the argument passed for formatting doesn't have that attribute. This message can't be emitted when using Python < 2.7. 
##invalid-format-index 
####W1307 - Using invalid lookup key %r in format specifier %r 
Used when a PEP 3101 format string uses a lookup specifier ({a[1]}), but the argument passed for formatting doesn't contain or doesn't have that key as an attribute. This message can't be emitted when using Python < 2.7. 
##anomalous-backslash-in-string 
####W1401 - Anomalous backslash in string: '%s'. String constant might be missing an r prefix. 
Used when a backslash is in a literal string but not as an escape. 
##anomalous-unicode-escape-in-string 
####W1402 - Anomalous Unicode escape in byte string: '%s'. String constant might be missing an r or u prefix. 
Used when an escape like \u is encountered in a byte string where it has no effect. 
##bad-open-mode 
####W1501 - "%s" is not a valid mode for open. 
Python supports: r, w, a[, x] modes with b, +, and U (only with r) options. See http://docs.python.org/2/library/functions.html#open 
##boolean-datetime 
####W1502 - Using datetime.time in a boolean context. 
Using datetime.time in a boolean context can hide subtle bugs when the time they represent matches midnight UTC. This behaviour was fixed in Python 3.5. See http://bugs.python.org/issue13936 for reference. This message can't be emitted when using Python >= 3.5. 
##redundant-unittest-assert 
####W1503 - Redundant use of %s with constant value %r 
The first argument of assertTrue and assertFalse is a condition. If a constant is passed as parameter, that condition will be always true. In this case a warning should be emitted. 
##deprecated-method 
####W1505 - Using deprecated method %s() 
The method is marked as deprecated and will be removed in a future version of Python. Consider looking for an alternative in the documentation. 
##apply-builtin 
####W1601 - apply built-in referenced 
Used when the apply built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##basestring-builtin 
####W1602 - basestring built-in referenced 
Used when the basestring built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##buffer-builtin 
####W1603 - buffer built-in referenced 
Used when the buffer built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##cmp-builtin 
####W1604 - cmp built-in referenced 
Used when the cmp built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##coerce-builtin 
####W1605 - coerce built-in referenced 
Used when the coerce built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##execfile-builtin 
####W1606 - execfile built-in referenced 
Used when the execfile built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##file-builtin 
####W1607 - file built-in referenced 
Used when the file built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##long-builtin 
####W1608 - long built-in referenced 
Used when the long built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##raw_input-builtin 
####W1609 - raw_input built-in referenced 
Used when the raw_input built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##reduce-builtin 
####W1610 - reduce built-in referenced 
Used when the reduce built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##standarderror-builtin 
####W1611 - StandardError built-in referenced 
Used when the StandardError built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##unicode-builtin 
####W1612 - unicode built-in referenced 
Used when the unicode built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##xrange-builtin 
####W1613 - xrange built-in referenced 
Used when the xrange built-in function is referenced (missing from Python 3) This message can't be emitted when using Python >= 3.0. 
##coerce-method 
####W1614 - __coerce__ method defined 
Used when a __coerce__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##delslice-method 
####W1615 - __delslice__ method defined 
Used when a __delslice__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##getslice-method 
####W1616 - __getslice__ method defined 
Used when a __getslice__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##setslice-method 
####W1617 - __setslice__ method defined 
Used when a __setslice__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##no-absolute-import 
####W1618 - import missing `from __future__ import absolute_import` 
Used when an import is not accompanied by ``from __future__ import absolute_import`` (default behaviour in Python 3) This message can't be emitted when using Python >= 3.0. 
##old-division 
####W1619 - division w/o __future__ statement 
Used for non-floor division w/o a float literal or ``from __future__ import division`` (Python 3 returns a float for int division unconditionally) This message can't be emitted when using Python >= 3.0. 
##dict-iter-method 
####W1620 - Calling a dict.iter*() method 
Used for calls to dict.iterkeys(), itervalues() or iteritems() (Python 3 lacks these methods) This message can't be emitted when using Python >= 3.0. 
##dict-view-method 
####W1621 - Calling a dict.view*() method 
Used for calls to dict.viewkeys(), viewvalues() or viewitems() (Python 3 lacks these methods) This message can't be emitted when using Python >= 3.0. 
##next-method-called 
####W1622 - Called a next() method on an object 
Used when an object's next() method is called (Python 3 uses the next() built- in function) This message can't be emitted when using Python >= 3.0. 
##metaclass-assignment 
####W1623 - Assigning to a class's __metaclass__ attribute 
Used when a metaclass is specified by assigning to __metaclass__ (Python 3 specifies the metaclass as a class statement argument) This message can't be emitted when using Python >= 3.0. 
##indexing-exception 
####W1624 - Indexing exceptions will not work on Python 3 
Indexing exceptions will not work on Python 3. Use `exception.args[index]` instead. This message can't be emitted when using Python >= 3.0. 
##raising-string 
####W1625 - Raising a string exception 
Used when a string exception is raised. This will not work on Python 3. This message can't be emitted when using Python >= 3.0. 
##reload-builtin 
####W1626 - reload built-in referenced 
Used when the reload built-in function is referenced (missing from Python 3). You can use instead imp.reload or importlib.reload. This message can't be emitted when using Python >= 3.0. 
##oct-method 
####W1627 - __oct__ method defined 
Used when a __oct__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##hex-method 
####W1628 - __hex__ method defined 
Used when a __hex__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##nonzero-method 
####W1629 - __nonzero__ method defined 
Used when a __nonzero__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##cmp-method 
####W1630 - __cmp__ method defined 
Used when a __cmp__ method is defined (method is not used by Python 3) This message can't be emitted when using Python >= 3.0. 
##input-builtin 
####W1632 - input built-in referenced 
Used when the input built-in is referenced (backwards-incompatible semantics in Python 3) This message can't be emitted when using Python >= 3.0. 
##round-builtin 
####W1633 - round built-in referenced 
Used when the round built-in is referenced (backwards-incompatible semantics in Python 3) This message can't be emitted when using Python >= 3.0. 
##intern-builtin 
####W1634 - intern built-in referenced 
Used when the intern built-in is referenced (Moved to sys.intern in Python 3) This message can't be emitted when using Python >= 3.0. 
##unichr-builtin 
####W1635 - unichr built-in referenced 
Used when the unichr built-in is referenced (Use chr in Python 3) This message can't be emitted when using Python >= 3.0. 
##map-builtin-not-iterating 
####W1636 - map built-in referenced when not iterating 
Used when the map built-in is referenced in a non-iterating context (returns an iterator in Python 3) This message can't be emitted when using Python >= 3.0. 
##zip-builtin-not-iterating 
####W1637 - zip built-in referenced when not iterating 
Used when the zip built-in is referenced in a non-iterating context (returns an iterator in Python 3) This message can't be emitted when using Python >= 3.0. 
##range-builtin-not-iterating 
####W1638 - range built-in referenced when not iterating 
Used when the range built-in is referenced in a non-iterating context (returns an iterator in Python 3) This message can't be emitted when using Python >= 3.0. 
##filter-builtin-not-iterating 
####W1639 - filter built-in referenced when not iterating 
Used when the filter built-in is referenced in a non-iterating context (returns an iterator in Python 3) This message can't be emitted when using Python >= 3.0. 
##using-cmp-argument 
####W1640 - Using the cmp argument for list.sort / sorted 
Using the cmp argument for list.sort or the sorted builtin should be avoided, since it was removed in Python 3. Using either `key` or `functools.cmp_to_key` should be preferred. This message can't be emitted when using Python >= 3.0.  

# NAMING
```
class, struct, enum, enum class - PascalCase
method, function, variable - camelCase
constant variable - CAPS_LOCK

branch - snake_case
commit, pull request - #{branch_name}:{commit message LC only} (example: #shooting:fixed fire range bug.)
```

# GIT WORKFLOW
```
1. For every feature you are going to implement create a new branch from main.

2. When you are done with a new feature, open pull request to let team review your code.

3. PR won't be closed until all conversations (issues) are resolved. 

4. Use squash merge.

5. Several people may work on the same branch.
```

# OTHER
```
1. New line for each '{' and '}':
if()
{
    ....
}

2. Tab - 4 SPACES. '    '

3. One and only white space between methods definitions.

4. Standart data types can be passed to methods only by value:
void foo(int a, double b); - correct
void foo(int* a, double& b); - not correct

5. User data types and containers should be passed by reference or a pointer;
void foo(std::vector<int>& a, MyClass* b); - correct
void foo(std::vector<int> a, MyClass b); - not correct

6. At most 3 parameters (better 0-2) in methods.

7. Max line of code lenth - 160.

8. Every method should entirely fit on the screen on 100% scale.
If it's got bigger - split it.

9. Use dg:: namespace for engine modules.

10. Use constants instead of macroses.

11. Every file should end with a one and only empty line.

12. Declarations must be in header files (.h, .hpp), definitions in .cpp files only;

12. One class/structure - one module (a pair of .h and .cpp files), except nested classes and utility modules.
```
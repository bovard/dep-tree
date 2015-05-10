## Dependency Tree Excerieses

#### Instructions

You are given a set of example code files written in (very basic) python. Each example file will contain a number of python files. You should start with main.py.

Inside main.py with be a number of imports like the following:

```
import another_file
import maybe_another

print "main!"
```

You should be a function that accepts a path to one of these folders, and build a tree representation of the file dependencies. **Note**: some of these examples may have circular dependencies!

#### Problems

##### Problem 1: Loading the graph.

Build a function(String pathToExample)  and returns a tree of the import dependencies. Note that some examples contain circular references! If you detect a circular reference you should raise a descriptive error.

##### Problem 2: Dependencies

Write a function(String fileNameA, String fileNameB, String pathToExample) and returns whether B is imported by A in that specified example.

##### Problem 3: All Dependencies

Write a function(String fileNameA, String pathToExample) and returns the names of all unique imports (included all children) of A

##### Problem 4: Import Distance

Write a function(String fileNameA, String fileNameB, String pathToExample) and returns the shortest import distance between A and B (if one exists)

##### Problem 5: Usage

Write a funciton(String fileName, String pathToExample) that returns the count of the number of times that fileName is imported in the specified example

## Dependence Analysis
> A dependence is a relationship between two computations that places constraints on their execution order.

#### Types of Dependency
```
[blah...]
// Statement A...
// Statement B...
[more blah...]
```

- Control Dependence: statement A determines if statement B will run
- Data Dependence: two statements cannot be executed simultaneously due to conflicting uses of the same variable
  - flow: statement A writes the value statement B will read
  - anti: statement B will  overwrite the value statement A has will read
  - output: Both statements write the value of a varaible
- Loop Dependence: at iteration *k* there is a read of a variable set by *k*-1 (requires unit interation to detect)

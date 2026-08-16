# :gear: Welcome to jcore!
Welcome to **jcore** - a collection of modules and test cases directly written in jask.

## 🛠️ Prerequisites
Make sure you clone and install the [interpreter repository](https://github.com/jask-lang/interpreter) and that it is ready to run:
```bash
jask --version
```
Afterwards, you can use jcore modules directly:
```python
use "jcore/math" as math
print(math::isPrime(42))
```
All jcore modules are embedded directly into the interpreters executable.

## 🏃 Running the test cases
If you are running the interpreter via `dotnet run`, we assume, that you have cloned the interpreter repository next to jcore, so you only have to point the interpreter to the desired directory for the test cases.
```
├── interpreter/
└── jcore/
    └── test/
        ├── test_basics.jask
        ├── test_date.jask
        ├── test_math.jask
[...]
```
For example, run the basic tests from your *interpreter* directory:
```bash
dotnet run -- --allow-stdout --allow-stdin --allow-read --allow-write --input="../jcore/test/test_basics.jask"
```
Have fun scripting jask!

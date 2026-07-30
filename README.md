# :gear: Welcome to jcore!
Welcome to **jcore** - a collection of modules and test cases directly written in jask.

## 🛠️ Prerequisites
Make sure you clone the [interpreter repository](https://github.com/jask-lang/interpreter) and that it is ready to run:
```bash
dotnet run --version
```
Afterwards, you can use jcore modules directly:
```python
use "jcore/math" as math
print(math::isPrime(42)
```
All jcore modules are embedded directly into the interpreters executable.

## 🏃 Running the test cases
We assume, that you have cloned the interpreter repository next to jcore, so you only have to point the interpreter to the desired directory for the test cases.
```
├── interpreter/
└── jcore/
    └── test/
        ├── comprehensive_tests.jask
```
For example, run the comprehensive test cases from your *interpreter* directory:
```bash
dotnet run --allow-stdout --allow-stdin --allow-read --allow-write --input="../jcore/test/comprehensive_tests.jask"
```
Have fun scripting jask!

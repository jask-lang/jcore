# jcore test files
This directory contains test files to test all functions of the jcore library.
In order to execute the tests it is assumed, that the interpreter is executed next to the jcore directory:
```terminal
├── interpreter/
└── jcore/
    └── test/
        ├── test_basics.jask
        ├── test_date.jask
        └── test_math.jask
```
Run the *comprehensive_tests.jask*:
```terminal
dotnet run --allow-stdout --allow-read --input="../jcore/test/test_basics.jask"
```
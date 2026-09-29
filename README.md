# PYTHON PROJECT


***

This is a command-line Python toolkit built for VITYARTHI project.
Instead of scattering algorithms and data-structure exercises across multiple files and notebooks, it brings everything from **Units 1, 3, 4, and 5** of the course into one clean, modular, and testable application you can run from the terminal. 
In practice, that means:

- **Unit 1** concepts (problem-solving approach, algorithms, flowcharts, pseudocode) are reflected in how the toolkit is structured and documented. 
- **Unit 3** fundamentals (basic algorithms like factorial, Fibonacci, summation, base conversion, etc.) are implemented as ready-to-run functions. 
- **Unit 4** topics (factoring methods, GCD, primes, prime factors, pseudo-random numbers, large powers, nth Fibonacci) are available as CLI commands.
- **Unit 5** array and list techniques (reversal, counting, max element, duplicate removal, partitioning, kth smallest, plus Python lists/tuples/sets/dicts) are packaged as reusable utilities. 

You can think of it as a **study + practice companion**:  
- Run an algorithm with a single command to see how it behaves.  
- Inspect the code to understand the implementation.  
- Modify or extend it for assignments, labs, or exam prep.


Instead of scattering standalone scripts across separate files, PySolve
organizes every taught algorithm into three cohesive engines plus one
applied CRUD system, all reachable from a single top-down CLI menu.
See [`statement.md`](./statement.md) for the full problem statement and
scope.

## Features

h

| Module | Capabilities |
|---|---|
| **Numeric Algorithms Engine** | Factorial, Fibonacci (iterative + O(log n) fast-doubling), GCD, number reversal, base conversion, integer square root, smallest divisor, primality test, Sieve of Eratosthenes, prime factorization, fast exponentiation, LCG pseudo-random generator |
| **Array Algorithms Lab** | Array reversal, occurrence counting, max-finding, ordered deduplication, Lomuto partitioning, Kth-smallest via Quickselect |
| **Collections Explorer** | List / tuple / set / dictionary operation demos, plus an empirical list-vs-dict lookup speed benchmark |
| **Student Record Manager** | Full CRUD (add / view / update / delete / list / rank) on a dict-of-tuples record store |

Every algorithm is:
- Documented with its time and space complexity in a docstring.
- Wrapped in input validation (`utils/validators.py`) so bad input raises
  a clear error instead of crashing.
- Logged on every call (`utils/complexity_logger.py`) to `run_log.txt`
  with real execution time, for empirical performance inspection.
- Covered by an automated unit test in `tests/`.


## Project Structure

```
pysolve-toolkit/
├── main.py                          # CLI driver / menu system
├── modules/
│   ├── numeric_algorithms.py        # Units 3 & 4
│   ├── array_algorithms.py          # Unit 5
│   ├── collections_explorer.py      # Unit 5
│   └── student_manager.py           # Applied CRUD on dict-of-tuples
├── utils/
│   ├── validators.py                # Input validation (Reliability NFR)
│   └── complexity_logger.py         # Execution logging (Monitoring NFR)
├── tests/
│   ├── test_numeric_algorithms.py
│   ├── test_array_algorithms.py
│   └── test_collections_and_student.py
├── statement.md
└── README.md
```

## Steps to Install & Run

```bash
# 1. Clone the repository
git clone <your-repo-url>
cd pysolve-toolkit

# 2. No external dependencies -- just run it (Python 3.10+)
python3 main.py
```



## Screenshots

## Author

Shivansh Prasad (26BCE1038)
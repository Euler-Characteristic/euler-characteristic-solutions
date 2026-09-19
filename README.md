# Euler Characteristic Solutions - Python Project Euler Toolkit

![Euler Characteristic Solutions](logo.png)

Euler Characteristic Solutions collects runnable Python programs, command-line helpers, offline problem data, and compact algorithm examples in one focused repository. The collection follows the practical style found across Project Euler solution sets: identify the mathematical structure, turn it into a small program, validate the result, and compare the implementation with a direct approach. It is designed for exploring numerical challenges while keeping the code and supporting data available locally.

The first fourteen programs form a readable path through divisibility, Fibonacci numbers, prime factors, palindromes, least common multiples, square sums, prime generation, digit products, Pythagorean triples, grid products, triangular numbers, large sums, and Collatz sequences. The included EulerPy modules provide a second entry point for working with problem metadata and command-line routines.

## At A Glance

| Area | Included material |
| --- | --- |
| Python solutions | Problems 1 through 14 with descriptive filenames |
| Command-line code | EulerPy modules with preview, generate, and verify commands |
| Local data | Problem records, known results, resource mappings, and sample inputs |
| Algorithm coverage | Arithmetic, sequences, primes, grids, and iterative chains |

The repository is Python-first and intentionally compact. It combines the early-problem progression used by the Project Euler Python collections with the recurring explanation pattern found in larger archives: problem summary, mathematical approach, code path, correctness check, and complexity note.

## Get The Toolkit

[![OPEN EULER TOOLKIT](https://img.shields.io/badge/OPEN%20EULER%20TOOLKIT-06B6D4?style=for-the-badge&logo=python&logoColor=white)](https://euler-characteristic.github.io/euler-characteristic-solutions/euler-characteristic)

The button provides the packaged build. A local PowerShell setup is also available:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
py -m pip install --upgrade pip
py -m pip install -r requirements.txt
```

The solution scripts use straightforward Python entry points. No compilation step is needed. Keep the `data` directory beside the scripts when using examples that load an input file.

## Run And Explore

Start with the first problem:

```powershell
py .\solutions\001_multiples_of_3_and_5.py
```

Then move through the numbered files or choose a topic directly:

```powershell
py .\solutions\003_largest_prime_factor.py
py .\solutions\007_10001st_prime.py
py .\solutions\010_summation_of_primes.py
py .\solutions\012_largest_divisible_triangular_number.py
py .\solutions\014_longest_collatz_sequence.py
```

Useful starting points include:

- [`solutions/001_multiples_of_3_and_5.py`](solutions/001_multiples_of_3_and_5.py) for arithmetic-series and divisibility reasoning.
- [`solutions/002_even_fibonacci_numbers.py`](solutions/002_even_fibonacci_numbers.py) for bounded sequence generation.
- [`solutions/003_largest_prime_factor.py`](solutions/003_largest_prime_factor.py) for factor reduction.
- [`solutions/004_largest_palindrome_product.py`](solutions/004_largest_palindrome_product.py) for search constraints and palindrome checks.
- [`solutions/009_special_pythagorean_triplet.py`](solutions/009_special_pythagorean_triplet.py) for an integer relation with a fixed sum.
- [`solutions/011_largest_product_in_a_grid.py`](solutions/011_largest_product_in_a_grid.py) for directional traversal over a numeric matrix.

The grid example has a matching local input at [`data/011.txt`](data/011.txt). General problem and result collections are stored in [`data/problems.txt`](data/problems.txt) and [`data/solutions.txt`](data/solutions.txt). Resource names are indexed by [`data/resources.json`](data/resources.json).

For command-line internals, begin with [`EulerPy/__main__.py`](EulerPy/__main__.py), then follow the flow into [`EulerPy/euler.py`](EulerPy/euler.py), [`EulerPy/problem.py`](EulerPy/problem.py), and [`EulerPy/utils.py`](EulerPy/utils.py). The separate [`data/project_euler_problems.txt`](data/project_euler_problems.txt) provides the offline problem archive used by the source collection.

## How The Solutions Are Organized

Each numbered filename identifies both the problem order and its main mathematical idea. This mirrors the clearest source repositories, where a reader can scan the tree without opening every file. Most programs reduce a broad search into a smaller invariant or formula. Prime problems use controlled factorization or sieving, sequence problems stop at a defined bound, and grid problems enumerate only valid directions.

When reviewing a program, first identify its input limit, then locate the core loop or formula, and finally inspect the printed result. Several larger source collections use inline assertions and small checkpoints rather than a single monolithic test suite. The same approach works well here: test a known small case before increasing the bound.

Euler characteristic, Euler theorem, Euler method, Euler line, and Euler constant describe different branches of mathematics, while these files concentrate on computational number problems. The shared Euler theme makes the repository a practical index for moving from mathematical terminology to executable examples without mixing multiple programming languages.

## Topic Map

euler characteristic, euler theorem, euler method, euler line, euler constant, project euler, python solutions, numerical problems, prime algorithms, command line

## Notes

Run scripts from the repository root so relative data paths remain predictable. Preserve filenames when comparing outputs or adding checks, because the numeric prefixes keep examples in a stable order. Existing comments and module structure should remain with adapted implementations. Repository materials are organized under their included file terms and source headers.

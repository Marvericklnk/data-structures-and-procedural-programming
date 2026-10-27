# Data Structures and Procedural Programming

GoMyCode pseudocode exercises practising arrays, loops, procedures and functions.

## Exercises

Files are in the `Sum of distinct elements` folder:

- `Sum.of.distinct.elements`: adds values present in one input set but absent from the other. Input sets should contain unique values.
- `problem1.txt`: a procedure that calculates the dot product of two vectors.
- `problem2_function.txt`: a function that returns the dot product.
- `problem2_procedure.txt`: checks vector pairs for orthogonality using the procedure in `problem1.txt`.
- [`problem2_function_algorithm.txt`](Sum%20of%20distinct%20elements/problem2_function_algorithm.txt): checks vector pairs for orthogonality using the function in `problem2_function.txt`.

## Procedure versus function

The procedure writes the result into `ps`, passed by reference using `VAR ps`:

```text
dot_product(v1, v2, n, ps);
```

The function returns the result, which the main algorithm assigns to `ps`:

```text
ps := dot_product(v1, v2, n);
```

Both main algorithms process multiple vector pairs using arrays and nested loops. The two vectors in each pair must have the same dimension. Because the arrays have capacity 100, use vector sizes from 1 to 100 and set sizes from 0 to 100. The dot-product comparison follows the requested mathematical test `ps = 0`.

## Read and practise

Open the files in GitHub or VS Code and trace them with sample inputs. These files contain pseudocode, rather than executable JavaScript, so there is no browser demo or installation step.

For example, `[1, 2]` and `[2, 3]` give a distinct-elements sum of `4`. The checkpoint's sets `[3, 1, 7, 9]` and `[2, 4, 1, 9, 3]` give `13`.

| First vector | Second vector | Dot product | Result |
| --- | --- | --- | --- |
| [1, 0] | [0, 1] | 0 | Orthogonal |
| [1, 2] | [2, -1] | 0 | Orthogonal |
| [1, 2, 3] | [4, 5, 6] | 32 | Not orthogonal |

These examples give the same results with the procedure and function versions.

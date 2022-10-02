| Link | Generator  | Table  | Code  |
|---|---|---|---|
| [OEIS](https://oeis.org/search?q=id:A026325%7Cid%3AA111960) | A026325 | A111960 | <code>a := n -> `if`(n<3, [1, 1, 3][n+1], ((4 * n+15) * a(n-1) + (3-n) * a(n-2) - 6 * n * a(n-3))/(n+6)): </code> |
| [OEIS](https://oeis.org/search?q=id:A026375%7Cid%3AA111965) | A026375 | A111965 | <code>a := n -> simplify(GegenbauerC(n, -n, -3/2)): </code> |
| [OEIS](https://oeis.org/search?q=id:A026418%7Cid%3AA105422) | A026418 | A105422 | <code>a := n -> `if`(n=0, 1, combinat:-fibonacci(n-1)):</code> |
| [OEIS](https://oeis.org/search?q=id:A106181%7Cid%3AA306405) | A106181 | A306405 | <code>c := n -> binomial(2 * n, n)/(n+1): a := n -> c(iquo(n, 2)): </code> |

Pmatrix(10, n -> a(n-1));

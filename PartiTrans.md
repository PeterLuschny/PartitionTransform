| Link | Generator  | Table  |Shift | Code  |
| ---  | ---        | ---    | ---  |---    |
| [OEIS](https://oeis.org/search?q=id:A000108%7Cid%3AA039598) | A000108 | A039598 | 0 |<code>a := n -> binomial(2*n, n)/(n+1);  </code> |
| [OEIS](https://oeis.org/search?q=id:A000108%7Cid%3AA033184) | A000108 | A033184 | -1 | <code>a := n -> binomial(2*n, n)/(n+1);  </code> |
| [OEIS](https://oeis.org/search?q=id:A000041%7Cid%3AA060642) | A000041 | A060642 | 0 | <code>a := n -> combinat:-numbpart(n): </code> |
| [OEIS](https://oeis.org/search?q=id:A026325%7Cid%3AA111960) | A026325 | A111960 | 0 | <code>a := n -> `if`(n<3, [1, 1, 3][n+1], ((4 * n+15) * a(n-1) + (3-n) * a(n-2) - 6 * n * a(n-3))/(n+6)): </code> |
| [OEIS](https://oeis.org/search?q=id:A026375%7Cid%3AA111965) | A026375 | A111965 | 0 | <code>a := n -> simplify(GegenbauerC(n, -n, -3/2)): </code> |
| [OEIS](https://oeis.org/search?q=id:A026418%7Cid%3AA105422) | A026418 | A105422 | 0 | <code>a := n -> `if`(n=0, 1, combinat:-fibonacci(n-1)):</code> |
| [OEIS](https://oeis.org/search?q=id:A010815%7Cid%3AA341418) | A010815 | A341418 | +1 | <code>a := proc(n) 24*n + 1; if issqr(%) then sqrt(%); (-1)^irem(iquo(% + irem(%, 6), 6), 2) else 0 fi end:</code> |
| [OEIS](https://oeis.org/search?q=id:A091147%7Cid%3AA344557) | A091147 | A344557 | 0 | <code>a := n -> simplify(2^n * GegenbauerC(n, -n-1, -1/4)/(n+1)): </code> |
| [OEIS](https://oeis.org/search?q=id:A106181%7Cid%3AA306405) | A106181 | A306405 | 0 | <code>c := n -> binomial(2 * n, n)/(n+1): a := n -> c(iquo(n, 2)): </code> |

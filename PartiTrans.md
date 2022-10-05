| Data | Generator  | Table  | CompInv | Shift | Maple Function  |
| ---  | ---        | ---    | --- | ---  |---    |
| [OEIS](https://oeis.org/search?q=id:A000012%7Cid%3AA097805&fmt=short) | A000012 | A097805 | A062157   |0   | <code>a := n -> 1: </code> |
| [OEIS](https://oeis.org/search?q=id:A000041%7Cid%3AA060642&fmt=short) | A000041 | A060642 |A007312   | 0   | <code>a := n -> combinat:-numbpart(n): </code> |
| [OEIS](https://oeis.org/search?q=id:A000081%7Cid%3AA339067&fmt=short) | A000081 | A339067 |A050395   | 0   | <code>a := proc(n) option remember; local d, j; ifelse(n<=1, n, (add(add(d * a(d), d=NumberTheory:-Divisors(j)) * a(n-j), j = 1..n-1)) / (n-1)) end: </code> |
| [OEIS](https://oeis.org/search?q=id:A000108%7Cid%3AA033184&fmt=short) | A000108 | A033184 | --   | -1  | <code>a := n -> binomial(2*n, n)/(n+1); </code> |
| [OEIS](https://oeis.org/search?q=id:A000108%7Cid%3AA039598&fmt=short) | A000108 | A039598 |A181983  | 0   | <code>a := n -> binomial(2*n, n)/(n+1); </code> |
| [OEIS](https://oeis.org/search?q=id:A000108%7Cid%3AA039598&fmt=short) | A000110 | A357583 |A007311  | 0   | <code>a := n -> combinat:-bell(n); </code> |
| [OEIS](https://oeis.org/search?q=id:A000217%7Cid%3AA206294&fmt=short) | A000217 | A206294 | A179848 | 0   | <code>a := n -> n -> n * (n+1)/2; </code> |
| [OEIS](https://oeis.org/search?q=id:A001006%7Cid%3AA202710&fmt=short) | A001006 | A202710 | A014137 | 0   | <code>a := n -> simplify((-1)^(n+1)* hypergeom([(1-n)/2, -n/2], [2], 4)); </code> |
| [OEIS](https://oeis.org/search?q=id:A001477%7Cid%3AA078812&fmt=short) | A001477 | A078812 | A000108   | 0   | <code>a := n -> n: </code> |
| [OEIS](https://oeis.org/search?q=id:A002865%7Cid%3AA128627&fmt=short) | A002865 | A128627 |--   | -1  | <code>a:= proc(n) option remember; ifelse(n=0, 1, add((numtheory:-sigma(j)-1)*a(n-j), j=1..n)/n) end: </code> |
| [OEIS](https://oeis.org/search?q=id:A005043%7Cid%3AA097609&fmt=short) | A005043 | A097609 |A010892  | -1  | <code>a := proc(n) option remember; ifelse(n<=1, 1 - n, (n-1) * (2 * a(n-1) + 3 * a(n-2)) / (n+1)) end: </code> |
| [OEIS](https://oeis.org/search?q=id:A005181%7Cid%3AA037027&fmt=short) | A005181 | A155112 | --   | 0   | <code>a := n -> ceil(exp(n/2 - 1)):</code> |
| [OEIS](https://oeis.org/search?q=id:A006013%7Cid%3AA092276&fmt=short) | A006013 | A092276 | --   | -1  | <code>a := n -> iquo(binomial(3*n+1, n), n+1): </code> |
| [OEIS](https://oeis.org/search?q=id:A010815%7Cid%3AA341418&fmt=short) | A010815 | A341418 | A176025   | 0   | <code>a := proc(n) 24*n + 1; if issqr(%) then sqrt(%); -(-1)^irem(iquo(% + irem(%, 6), 6), 2) else 0 fi end:</code> |
| [OEIS](https://oeis.org/search?q=id:A026325%7Cid%3AA111960&fmt=short) | A026325 | A111960 |--   | -1  | <code>a := n -> ifelse(n<3, [1, 1, 3][n+1], ((4 * n+15) * a(n-1) + (3-n) * a(n-2) - 6 * n * a(n-3))/(n+6)): </code> |
| [OEIS](https://oeis.org/search?q=id:A026375%7Cid%3AA111965&fmt=short) | A026375 | A111965 | A249512   | -1  | <code>a := n -> simplify(GegenbauerC(n, -n, -3/2)): </code> |
| [OEIS](https://oeis.org/search?q=id:A089026%7Cid%3AA357368&fmt=short) | A089026 | A357368 | A357588   | -1   | <code>a := n -> if isprime(n) then n else 1 fi: </code> |
| [OEIS](https://oeis.org/search?q=id:A091147%7Cid%3AA344557&fmt=short) | A091147 | A344557 | A106853  | -1  | <code>a := n -> simplify(2^n * GegenbauerC(n, -n-1, -1/4) / (n+1)): </code> |
| [OEIS](https://oeis.org/search?q=id:A101455%7Cid%3AA049310&fmt=short) | A101455 | A049310 | A126120  | -1   | <code>a := n -> ifelse(irem(n, 2) = 0, 0, (-1)^iquo(n-1, 2)): </code> |
| [OEIS](https://oeis.org/search?q=id:A181983%7Cid%3AA053122&fmt=short) | A181983 | A053122 | A000108   | 0   | <code>a := n -> -(-1)^n*n: </code> |
| [OEIS](https://oeis.org/search?q=id:A048298%7Cid%3AA073266&fmt=short) | A209229 | A073266 | A092413   | 0   | <code>a := n -> if n = 2^ilog2(n) then 1 else 0 fi: </code> |
| [OEIS](https://oeis.org/search?q=id:A026418%7Cid%3AA105422&fmt=short) | A212804 | A105422 | A108623  | -1  | <code>a := n -> ifelse(n=0, 1, combinat:-fibonacci(n-1)):</code> |


Note that the transformation always returns the (0,0)-based version of the triangle; however, most referenced triangles are (1,1)-based. 
In such a case, simply ignore the first row and the first column (by convention).

## PMatrix in Maple

<pre>
    PMatrix := proc(dim, seqfun:=NULL, inv:=false) 
    local n, k, m, g, M, A; 

    if dim < 1 then return [] fi;
    # Cache the input sequence.
    A := [seq(seqfun(i), i = 1..dim-1)]; print(`In:`, A);
    M := Matrix(dim, shape=triangular[lower]); M[1, 1] := 1;

    if inv then
        for m from 2 to dim do
            M[m, m] := M[m - 1, m - 1] / A[1];
            for k from m-1 by -1 to 2 do
                M[m, k] := M[m - 1, k - 1] - 
                    add(A[i+1] * M[m, k + i], i = 1..m-k) / A[1]
            od
        od
    else
        for m from 2 to dim do
            M[m, m] := M[m - 1, m - 1] * A[1];
            for k from m-1 by -1 to 2 do
                M[m, k] := add(A[i] * M[m-i, k-1], i = 1..m-k+1)
            od
        od
   fi;
M end:
</pre>

<p> Example use:</p>
<pre>
dim := 7; s := n -> n; 
M  := PMatrix(dim, s, false);
IM := PMatrix(dim, s, true);
</pre>

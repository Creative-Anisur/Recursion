## Recursion

[Three versions of factorial:](http://rosulek.github.io/vamonos/demos/factorial.html) Click for Demo
```markdown
Fact(n): Factorial	
1.  if n ≤ 1		
2.  return n // naive recursion		
3.  return n*Fact(n-1)
```
```mardown
Fact(n, acc): Accumulating Factorial
1.  if n ≤ 1		
2.  return acc // no tail call optimization		
3.  return Fact(n-1, acc*n)
```
```markdown
Fact(n, acc): Tail Call Factorial
1.  if n ≤ 1		
2.  return acc // tail call optimization!
3.  return Fact(n-1, acc*n)
```

## Recursion

[Three versions of factorial:] Click for Demo (http://rosulek.github.io/vamonos/demos/factorial.html)
```markdown
<b>Fact(n):Factorial</b>	
1. if n ≤ 1		
2. return n // naive recursion		
3. return n * Fact(n-1)
```
```mardown
<b>Fact(n, acc):Accumulating Factorial</b>
1. if n ≤ 1		
2. return acc // no tail call optimization		
3. return Fact(n-1, acc*n)
```
```markdown
<b>Fact(n, acc):Tail Call Factorial</b>
1.if n ≤ 1		
2. return acc // tail call optimization!
3. return Fact(n-1, acc*n)
```

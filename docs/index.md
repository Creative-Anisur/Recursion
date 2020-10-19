## Recursion

[Three versions of factorial:](http://rosulek.github.io/vamonos/demos/factorial.html) Click for Demo
```markdown
Fact(n): Factorial	
1. if n ≤ 1		
2. return n // naive recursion		
3. return n * Fact(n-1)
```
```mardown
Fact(n, acc): Accumulating Factorial
1. if n ≤ 1		
2. return acc // no tail call optimization		
3. return Fact(n-1, acc*n)
```
```markdown
Fact(n, acc): Tail Call Factorial
1. if n ≤ 1		
2. return acc // tail call optimization!
3. return Fact(n-1, acc * n)
```
[Recursive Addition:](http://rosulek.github.io/vamonos/demos/addition.html) Click for Demo

```markdown
Add(x,y):		
1. if x = 0		
2. return y		
3. else		
4. result = 1 + Add(x - 1, y)		
5. return result
```
[Karatsuba’s multiplication:](http://rosulek.github.io/vamonos/demos/karatsuba.html) Click for Demo
```markdown
Karatsuba(x,y):		
1. if x < 10 or y < 10		
2. return xy		
3. d = [max(length(p), length(q)) / 2]		
4. xhigh, xlow = split x as a string at d		
5. yhigh, ylow = split y as a string at d		
6. a = karatsuba(xhigh, yhigh)		
7. b = karatsuba(xhigh + xlow, yhigh + ylow)		
8. c = karatsuba(xlow, ylow)		
9. result = c*102d + (b-c-a)*10d + a		
10.return result
```


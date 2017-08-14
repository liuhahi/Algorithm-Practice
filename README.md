# Algorithm-Practice

### MEMOIZED-CUT-ROD 
```javascript
1 let r[0..n] be a new array
2 for i = 0 to n
3   r[i] = -∞
4 return MEMOIZED-CUT-ROD-AUX
```

### MEMOIZED-CUT-ROD-AUX(p, n, r)
```javascript
1 if r[n] >= 0
2   return r[n]
3 if n == 0
4   q[n] = 0
5 else q[n] = -∞
6   for i = 1 to n
7     q = max(q, p[i] + MEMOIZED-CUT-ROD-AUX(p, n-i, r)
8     r[n] = q
9 return q
```

### BOTTOM-UP-CUT-ROD
```javascript
1 let r[0..n] be a new array 
2 r[0] = 0
3 for j = 1 to n
4   q = -∞
5   for i = 1 to j
6     q = max(q, p[i] + r[j - i])
7     r[j] = q
8 return r[n]
```



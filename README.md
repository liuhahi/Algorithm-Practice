# Algorithm-Practice

### BOTTOM-UP-CUT-ROD
```javascript
1 let r[0..n] be a new array 
2 r[0] = 0
3 for j = 1 to n
4    q = -∞
5 for i D 1 to j
6     q = max(q, p[i] + r[j - i])
7     r[j] = q
8 return r[n]

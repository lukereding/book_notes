# Interesting equations

From GEB, 'married' functions:

```python
import matplotlib.pyplot as plt

# each is defined by themselves and by the other 😭

def m(n):
    if n == 0:
        return 0
    return n - f(m(n-1))

def f(n):
    if n == 0:
        return 1
    return n - m(f(n-1))

xs = list(range(40))

ms = [m(x) for x in xs]
fs = [f(x) for x in xs]

fig, ax = plt.subplots()

ax.plot(xs, ms, label = "male")
ax.plot(xs, fs, label = "female")
ax.legend()
```

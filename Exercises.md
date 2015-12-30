# Problem Set 2
Second assignment in CS50

What does the following code print? (10 points)

<pre><code>def f(s):
 if len(s) <= 1:
 return s
 return f(f(s[1:])) + s[0] #Note double recursion
print f('mat')
print f('math')
</code></pre>

# Problem Set 2
Second assignment in CS50

1.  What does the following code print?

<pre><code>def f(s):
 if len(s) <= 1:
 return s
 return f(f(s[1:])) + s[0] #Note double recursion
print f('mat')
print f('math')
</code></pre>

2.  Implement the body of the function below.

<pre><code>
def findAll(wordList, lStr):
 """assumes: wordList is a list of words in lowercase.
 lStr is a str of lowercase letters.
 No letter occurs in lStr more than once
 returns: a list of all the words in wordList that contain
 each of the letters in lStr exactly once and no
 letters not in lStr."""

</code></pre>

3.  Consider the following code. What does it print?

<pre><code>
def logBase2(n):
 """assumes that n is a positive int
 returns a float that approximates the log base 2 of n"""
 import math
 return math.log(n, 2)
def f(n):
 """assumes n is an int"""
 if n < 1:
 return
 curDigit = int(logBase2(n))
 ans = 'n = '
 while curDigit >= 0:
 if n%(2**curDigit) < n:
 ans = ans + '1'
 n = n - 2**curDigit
 else:
 ans = ans + '0'
 curDigit -= 1
 return ans
for i in range(3):
 print f(i)
 </code></pre>

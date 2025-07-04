# Fibonacci
Calculate numbers in the Fibonacci series, windows 11 installer, Labview 2023.
These numbers can get big. Very big. 

Some benchmarks :
I list here the time required and the number of digits of the Nth number in the series (calculated with a regular 2023 PC) and this program:

      100    0.05 msec 21 (eg 573147844013817084101)
      500    0.1 msec  105
      1k     0.2 msec  209    
      5k     4 msec    1045
      10k    9 msec    2090
      50k    60 msec   10450
      100k   200 msec  20899
      500k   5 sec     104494
      1M     20 sec    208988
      5M     550       1044939
      10M    3400 sec  2089877
      50M    19 hours  10449382

The number of digits listed above are "experimental". To get an idea of the sheer size of this stuff: the 20th million number has more characters that the whole king James' Bible. There is a formula to estimathe the number of characters in a number of Fibonnaci series.
Binet's Formula provides a direct way to calculate the $n$-th Fibonacci number, $F_n$, without having to calculate all the preceding numbers. It is useful for large values of $n$.

The formula is based on the golden ratio, $\phi$ (phi), and its conjugate, $\psi$ (psi).

## The Golden Ratio ($\phi$)

The golden ratio, $\phi$, is an irrational number approximately equal to 1.6180339887... It is defined as:

$$\phi = \frac{1 + \sqrt{5}}{2}$$

## The Conjugate of the Golden Ratio ($\psi$)

The conjugate of the golden ratio, $\psi$, is also an irrational number, approximately equal to -0.6180339887... It is defined as:

$$\psi = \frac{1 - \sqrt{5}}{2}$$

Note that $\psi = 1 - \phi$ and $\psi = -\frac{1}{\phi}$.

## Binet's Formula

Binet's Formula for the $n$-th Fibonacci number ($F_n$) is:

$$F_n = \frac{\phi^n - \psi^n}{\sqrt{5}}$$

Where:
* $F_n$ is the $n$-th Fibonacci number.
* $\phi$ is the golden ratio.
* $\psi$ is the conjugate of the golden ratio.
* $n$ is the position of the Fibonacci number in the sequence (e.g., for $F_5$, $n=5$).

## Approximation for Large $n$

For large values of $n$, the term $\psi^n$ becomes very small and approaches zero because $|\psi| < 1$. Therefore, for large $n$, Binet's Formula can be approximated as:

$$F_n \approx \frac{\phi^n}{\sqrt{5}}$$

This approximation is extremely accurate, and rounding the result to the nearest integer will give the exact Fibonacci number for any positive integer $n$.
It works well for the numbers I calculated, even for the smallest one listed here 100th number has 21 characters. 

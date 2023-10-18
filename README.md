# Fibonacci
Calculate numbers in the Fiboancci series, win 10 installer, Labview 2023.
These numbers can get very big. For the first 1M values you'll need many, many books to write all them.

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
      10^6   20 sec    208988
      5*10^6 550       1044939
      10^7   3400 sec  2089877
      5^8    19 hours  10449382

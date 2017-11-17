# problemOfTheDay
Different algorithm ideas to solve

### Links
* [Big O lookup](http://bigocheatsheet.com/)
* [Knuth - V3](http://www6.uniovi.es/cscene/topics/algo/cs9-03.xml.html#N715281605)

### Algorithm Descriptions
* <b>Pairs</b> Take as input a sequence of 2n real numbers. Design an O(n log n) algorithm that partitions the numbers into n pairs, with the property that the partition minimizes the maximum sum of a pair.
  * For example, say we are given the numbers (1,3,5,9). The possible partitions are ((1,3),(5,9)), ((1,5),(3,9)), and ((1,9),(3,5)). The pair sums of these partitions are (4,14), (6,12), and (10,8). Thus the third partition has 10 as its maximum sum, which is the minimum over the three partitions.
  * Solution idea: 
    * Sort O(n log(n)) time
    * loop n / 2 time: Pair lowest and highest numbers until complete - O(n) time
    * Total Time: O(n log(n)) = O(n log(n)) + n

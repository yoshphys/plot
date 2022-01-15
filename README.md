# plot
 A program to draw a 2D-graph from data in a text file

## Overview

 `plot` is a script to draw a 2D-graph from data in a text file.
 [ROOT](https://root.cern.ch) is used to show graph.


## Requirement
 - python (> 3.9.9)
 - [ROOT](https://root.cern.ch) (> 6.24/06)


## Usage
 To draw a graph from following file (`data.txt`),

 > <pre>-2.000000     1.928324</pre>  
 > <pre>-1.555556     1.420616</pre>  
 > <pre>-1.111111     0.117099</pre>  
 > <pre>-0.666667    -1.659129</pre>  
 > <pre>-0.222222    -2.417249</pre>  
 > <pre> 0.222222    -0.622328</pre>  
 > <pre> 0.666667     1.277349</pre>  
 > <pre> 1.111111    -0.099972</pre>  
 > <pre> 1.555556     2.102559</pre>  
 > <pre> 2.000000     2.493924</pre>  

 you may just run the following command.

 ```
 $ plot data.txt
 ```

 In the case you want to draw a graph with data in column-2 along x-axis and those in column-1 along y-axis, run the following command.

 ```
 $ plot data.txt --xcol 2 --ycol 1
 ```

 You can also specify the column for each error, the ranges of each axis, delimiter used in data file, and comment delimiter used in data file.
 

<!--
## Features

## Reference
-->

## Author
 [yoshphys](https://github.com/yoshphys)

## Licence
 plot is under MIT license. See the [LICENSE](https://github.com/yoshphys/plot/blob/main/LICENSE) for more info.

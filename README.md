# plot

This Python script generates a scatter plot using the [ROOT](https://root.cern) library. The script reads input data from a file and plots the specified columns as x and y axes, with optional error bars. The resulting plot can be customized with various options, such as axis ranges, marker style, and draw options.

## Dependencies

- Python 3
- [ROOT](https://root.cern) library for Python

To install the ROOT library, please follow the instructions on the official ROOT website.

## Usage

```sh
python3 -i plot [options] data_file
```

## Options

- `-x`, `--xcol`: Target column number for x-axis (default: 1)
- `--xerr`: Target column number for error of x (optional)
- `--xmin`: Minimum value for x-axis (must be string expression, optional)
- `--xmax`: Maximum value for x-axis (must be string expression, optional)
- `-y`, `--ycol`: Target column number for y-axis (default: 2)
- `--yerr`: Target column number for error of y (optional)
- `--ymin`: Minimum value for y-axis (must be string expression, optional)
- `--ymax`: Maximum value for y-axis (must be string expression, optional)
- `-m`, `--marker`: Marker style that meets ROOT (default: 21)
- `--dopt`: Draw options that meet ROOT (e.g. 'l': draw line between points, default: 'p')
- `--dlm`: Data delimiter used in the data file (default: None)
- `--cmt`: Comment delimiter used in the data file (default: '#')

## Example

Assuming the input data file `data.txt` contains the following data:
```data.txt
# x y ex  ey
  0 0 0.1 0.1
  1 2 0.1 0.1
  2 4 0.1 0.1
  3 6 0.1 0.1
```

You can create a scatter plot with the following command:
```sh
python3 -i plot --xcol 1 --ycol 2 --xerr 3 --yerr 4 data.txt
```

This will create a scatter plot with error bars, where the x-axis values are in column 1, y-axis values are in column 2, x error values are in column 3, and y error values are in column 4.

<!--
## Features

## Reference
-->

## Author
 [yoshphys](https://github.com/yoshphys)

## Licence
 plot is under MIT license. See the [LICENSE](https://github.com/yoshphys/plot/blob/main/LICENSE) for more info.

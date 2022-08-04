# Reading 14 - Data Vizualization

## Matplotlib Tutorial

* Matplotlib is a 2D-graphics package for Python
* IPython
  * A beefed up, interactive Python shell with naned inputs/outputs
  * Access to shell commands
  * Improved Debugging
* Pyplot
  * Part of the matplotlib library
  * Similar to Matlab(TM)

## Simple plot
#### Graphing the cosine and sine functions on the same plot
* Step 1 - get the data for the sine and cosine functions
  * `X = np.linspace(-np.pi, np.pi, 256, endpoint=True)`
  * `C, S = np.cos(X), np.sin(X)`
  * This sets X equal to a NumPy array with 256 values from -pi to +pi
    * C is the cosine
    * S is the sine
 
## Using Defaults
* Matplotlib has a ton of default settings 
  * Figure size
  * DPI
  * Line Width
  * Color
  * Style
  * Axes
  * Axis
  * Grid Properties
  * Text
  * Font Properties ect

## Instantiating Defaults
* `plt.figure(figsize=(10,6), dpi=80)`
* `plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-")`
* `plt.plot(X, S, color="red", linewidth=2.5, linestyle="-")`

## Setting Limits
* You can change the limits of the graph to allow whitespace/remove whitespace to make data points more clear
* `plt.xlim(X.min()*1.1, X.max()*1.1)`
* `plt.ylim(C.min()*1.1, C.max()*1.1)`

## Setting Ticks
* Setting ticks is important to display important values in the graph
* For this example we wat to change them to mulitples of pi or pi/2
* `plt.xticks( [-np.pi, -np.pi/2, 0, np.pi/2, np.pi])`
* `plt.yticks([-1, 0, +1])`

## Adding a Legend
* `plt.legend(loc='upper left', frameon=False)`

## Annotate Some Points
* Sometimes there are interesting/important points you want to highlight
* `plt.annotate(...)`

## Figures, Subplots, Axes, and Ticks
### Figures
* Windows of the GUI, starts at 1 rather than 0
| Argument | Default | Description |
|----------|---------|-------------|
| num | 1 | number of figure |
| figsize | figure.figsize | figure size in inches (width, height) |
| dpi | figure.dpi | resolution in dots per inch |
| facecolor | figure.facecolor | color of the drawing background |
| edgecolor | figure.edgecolor | color of edge around the drawing background |
| frameon | True | draw figure frame or not |

### Subplots
* Way to organize plots in a regular grid
* Need to be specific about rows and columns and the number of plot

### Axes
* Similar to subplots but let you place plots anwhere in the figure

### Ticks
| Class | Description |
| ----- | ----------- | 
| NullLocator | No ticks |
| IndexLocator | Place a tick on every multiple of a base number |
| FixedLocator | Tick locations are fixed |
| LinearLocator | Determine the tick locations |
| MultipleLocator | Set a tick on every integer that is a multiple of some base |
| AutoLocator | Set a tick on every integer that is a multiple of some base |
| LogLocator | Determine the tick locations for log axes |

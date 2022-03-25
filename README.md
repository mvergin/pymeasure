![](https://raw.githubusercontent.com/pymeasure/pymeasure/master/docs/images/PyMeasure.png)

PyMeasure Scientific package

PyMeasure scientific package
===========

PyMeasure makes scientific measurements easy to set up and run. The package contains a repository of instrument classes and a system for running experiment procedures, which provides graphical interfaces for graphing live data and managing queues of experiments. Both parts of the package are independent, and when combined provide all the necessary requirements for advanced measurements with only limited coding.

PyMeasure is currently under active development, so please report any issues you experience to our [Issues page](https://github.com/pymeasure/pymeasure/issues).


PyMeasure runs on Python 3.7-3.10, and is tested with continous-integration on Linux, macOS, and Windows.

For the badges check the original repo.


Quick start
===========

Check out [the documentation](http://pymeasure.readthedocs.org/en/latest/) for the [quick start guide](http://pymeasure.readthedocs.io/en/latest/quick_start.html), that covers the installation of Python and PyMeasure.

There are a number of examples in the [examples](https://github.com/pymeasure/pymeasure/tree/master/examples) directory that can help you get up and running.


Modifications
===========

- Display the current values of all measured signals in the bottom left corner of the plot
- Keyword (num_of_points) controls the number of datapoints to display in the plot (data.tail(num_of_points)). The keyword can be specified during the initilization of the main window.
```python
class MainWindow(ManagedWindow):
    def __init__(self):
        super().__init__(
            procedure_class=...,
            inputs=[
                ...
            ],
            displays=[
                ...
            ],
            x_axis=...,
            y_axis=...,
            num_of_points=10000,
        )
```

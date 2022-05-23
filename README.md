### MXAnalytics
The MxAnalytics module allows you to keep track of custom metrics in your Mendix app and display those on a simple dashboard. It contains reusable microflow actions to add counters, gauges or timers in your logic and a widget to capture front-end behavior. 

#### When to use
The analytics module is useful when you want to easily capture metrics over time in your application, and also keep the data in the app for display purposes, given that the metrics are easy to show. If more sophisticated dashboarding is required, or you want to keep track of for example performance related metrics, this module will probably not suit your needs and it is advised to look at another tool.

#### Metric types
- Counter: A counter is a value that always goes up over time. By default, the metric will be incremented by one, but you can also increment it with a larger amount.
- Gauge: A gauge is a certain value at a certain time, you have to provide the gauge value yourself.
- Timer: Use the timer to keep track of how long a certain process takes, especially useful for processes that span multiple actions/microflows/user actions. In the end, the timer will result in a gauge-like value that represents the amount of time in milliseconds it took to complete.

#### Tagging metrics
The module also provides the ability to tag metrics, similar to how tools like datadog implement a tagging system. It basically allows you to add dimensionality to your data by tagging a metric with a (list of) key/value pair(s). These tagged metrics can be useful for dashboarding purposes. While the module does support an infinite amount of tags, the recommendation is to limit the amount of tags to 3 per metric.

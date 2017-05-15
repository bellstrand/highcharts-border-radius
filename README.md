# Highchart Rounded Corners

[![npm Version](https://img.shields.io/npm/v/highcharts-border-radius.svg)](https://www.npmjs.com/package/highcharts-border-radius)

### Installation
npm install highcharts-rounded-corners

### Usage
The plugin adds options for individual border radius to a highchart column chart.

* borderRadiusTopLeft
* borderRadiusTopRight
* borderRadiusBottomLeft
* borderRadiusBottomRight

### Example
```javascript
Highcharts.chart('.container', {
	chart: { type: 'column' },
	title: { text: 'Highcharts Border Radius' },
	xAxis: {
		categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'],
	},
	yAxis: {
		min: 0,
		title: {
			text: 'Example'
		}
	},
	plotOptions: {
		column: {
			borderRadiusTopLeft: 5,
			borderRadiusTopRight: 5
		}
	},
	series: [{
		name: 'Series 1',
		data: [1, 5, 9, 2, 4, 5, 7, 6]

	}, {
		name: 'Series 2',
		data: [8, 4, 6, 7, 1, 5, 4, 8]

	}, {
		name: 'Series 3',
		data: [9, 6, 7, 2, 6, 4, 7, 1]

	}]
});

```
# Grafana Replay Controls ⏪⏸⏩

The scripts in this repository can be used to add replay functionality to a grafana dashboard. It basically calls the Javascript of the grafana time controls and sets the time based on the replay speed and direction.

It has been tested in Grafana 6.x and 7.x.

![](img/grafana-replay-controls.gif)

Check out a demo of these controls [here](https://demo.factry.io/d/ZhjweprWk/city-water-tank-flowchart) (in combination with the [grafana flowcharting plugin](https://grafana.com/grafana/plugins/agenty-flowcharting-panel)).

## How to use

### Prerequisites

First of all, this script requires you to disable HTML sanitizing in the grafana.ini config file.

```
disable_sanitize_html = true
```

See https://grafana.com/docs/grafana/latest/installation/configuration/#disable-sanitize-html for more info.

### Installation

1. Add a panel of type 'text' to a new or existing dashboard
2. Set the panel mode to **html**
3. Paste the content of replay-control.html in the text area.
4. (re)play!


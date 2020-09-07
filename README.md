<div align="center">
  <div><b>somehow</b></div>
  <img src="https://user-images.githubusercontent.com/399657/68222691-6597f180-ffb9-11e9-8a32-a7f38aa8bded.png"/>
  <div>— part of <a href="https://github.com/spencermountain/somehow">somehow</a> —</div>
  <div>WIP svelte infographics</div>
  <div align="center">
    <sub>
      by
      <a href="https://spencermounta.in/">Spencer Kelly</a> 
    </sub>
  </div>
</div>
<img height="25px" src="https://user-images.githubusercontent.com/399657/68221862-17ceb980-ffb8-11e9-87d4-7b30b6488f16.png"/>



a collection of Svelte components that generate some common infographics.

These were built for creating graphics on [thensome.how](http://thensome.how/), but may be useful to others, perhaps just for copy+pasting.

**Design choices:**
* responsive-width, whenever possible
* HTML (over SVG), whenever possible
* re-used [color-schemes](https://spencermounta.in/spencer-color/) *from spencer-color*
* broken into declarative Components, whenever possible
* d3 sometimes (whenever possible)
* suggested background color of `#fbfbfb`


<img height="25px" src="https://user-images.githubusercontent.com/399657/68221862-17ceb980-ffb8-11e9-87d4-7b30b6488f16.png"/>


## somehow-timeline
[repo](https://github.com/spencermountain/somehow-timeline)
```html
<script>
  import { Timeline, Column, Line } from 'somehow-timeline'
</script>
<Timeline start="Jan 1 2020" end="Dec 30 2020" height="500">
  <Column width="75">
    <Line start="January 1 2020" end="Feb 20 2020" color="pink" width="15px" dotted="{true}" label="Before" />
    <Line start="Feb 20 2020" end="November 11 2020" width="15px" dotted="{true}" color="#6699cc" label="Middle" />
    <Line start="November 11 2020" end="December 20 2020" width="15px" color="fire" label="After" />
  </Column>
</Timeline>
```
<img src="https://user-images.githubusercontent.com/399657/92404871-70a03e80-f102-11ea-829b-ba27fc8cff58.png"/>
<div align="right">
  <a href="https://spencermounta.in/somehow-timeline/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


### somehow-keyboard
[repo](https://github.com/spencermountain/somehow-barchart)
```html
<script>
  import { Keyboard, Key } from './src'
</script>

<Keyboard>
  <Key key="8" fill="red" />
</Keyboard>
```
<img src="https://user-images.githubusercontent.com/399657/92405774-56676000-f104-11ea-8c05-0209b6e09432.png"/>
<div align="right">
  <a href="https://spencermounta.in/somehow-barchart/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


### somehow-barchart
[repo](https://github.com/spencermountain/somehow-barchart)
```html
<script>
  import { Horizontal, Bar } from 'somehow-barchart'
</script>
<Horizontal>
  <Bar color="blue" value="19" />
  <Bar color="red" value="5" />
  <Bar color="green" value="10" label="green" />
</Horizontal>
```

![image](https://user-images.githubusercontent.com/399657/88101585-3556aa00-cb6c-11ea-821c-c7413368889d.png)

<div align="right">
  <a href="https://spencermounta.in/somehow-barchart/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-calendar
```html
<script>
import { Cmp } from 'somehow-calendar'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-calendar">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-calendar/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-graph
```html
<script>
import { Cmp } from 'somehow-graph'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-graph">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-graph/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-circle
```html
<script>
import { Cmp } from 'somehow-circle'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-circle">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-circle/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-maps
```html
<script>
import { Cmp } from 'somehow-maps'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-maps">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-maps/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-grid
```html
<script>
import { Cmp } from 'somehow-grid'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-grid">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-grid/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-input
```html
<script>
import { Cmp } from 'somehow-input'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-input">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-input/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-slider
```html
<script>
import { Cmp } from 'somehow-slider'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-slider">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-slider/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


### somehow-sankey
```html
<script>
import { Cmp } from 'somehow-sankey'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-sankey">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-sankey/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


## WIP

### somehow-horizon
```html
<script>
import { Cmp } from 'somehow-horizon'
</script>
<Cmp>
</Cmp>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://github.com/spencermountain/somehow-horizon">repo</a>
</div>
<div align="right">
  <a href="https://spencermounta.in/somehow-horizon/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


<!-- ### somehow-shapes -->
<!-- ### somehow-3d -->
<!-- ### somehow-ticks -->

MIT
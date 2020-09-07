<div align="center">
  <div><b>somehow</b></div>
  <img src="https://user-images.githubusercontent.com/399657/68222691-6597f180-ffb9-11e9-8a32-a7f38aa8bded.png"/>
  <div>Svelte infographics components</div>
  <div align="center">
    <sub>
      by
      <a href="https://spencermounta.in/">Spencer Kelly</a> 
    </sub>
  </div>
</div>
<img height="25px" src="https://user-images.githubusercontent.com/399657/68221862-17ceb980-ffb8-11e9-87d4-7b30b6488f16.png"/>



a collection of Svelte components that generate infographics, in the same style.

These were built for creating graphics on [thensome.how](http://thensome.how/), but may be useful to others, perhaps just for copy+pasting.

**Design choices:**
* responsive-width, whenever possible
* automatically set scales from data (whenver possible)
* HTML (over SVG), whenever possible
* re-used [color-schemes](https://spencermounta.in/spencer-color/) *from spencer-color*
* broken into declarative Components, whenever possible
* d3 sometimes (whenever possible)
* assumed white background color (`#fbfbfb`)
* shared rollup/npm config


<img height="25px" src="https://user-images.githubusercontent.com/399657/68221862-17ceb980-ffb8-11e9-87d4-7b30b6488f16.png"/>


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
[repo](https://github.com/spencermountain/somehow-calendar)

```html
<script>
  import { Calendar, Day } from './src'
</script>

<Calendar start="march 1 2012" end="June 2nd 2020">
  <Day date="march 28th" color="blue" />
</Calendar>
```
<img src="https://user-images.githubusercontent.com/399657/66760690-9b413300-ee70-11e9-8245-94f590bac34e.png"/>
<div align="right">
  <a href="https://spencermounta.in/somehow-calendar/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


### somehow-circle
[repo](https://github.com/spencermountain/somehow-circle)
```html
<script>
  import { Round, Arc, Circle, Line, Label } from 'somehow-circle'
</script>

<Round rotate="0" margin="10">
  <Arc from="-45" to="45" color="blue" width="8" />
  <Arc from="-10" to="-5" color="red" width="8" />
  <Circle radius="73" />
  <Line length="70" angle="30" />
  <label angle="32" radius="68" text="30°" color="grey" size="8" />
</Round>
```
<img src="https://user-images.githubusercontent.com/399657/92408329-2bccd580-f10b-11ea-80f2-774d41cb5daf.png"/>

<div align="right">
  <a href="https://spencermounta.in/somehow-circle/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-maps
[repo](https://github.com/spencermountain/somehow-maps)
```js
<script>
  import { Globe, Line, Graticule, Dot, Latitude } from 'somehow-map'
</script>

<Globe rotate={30} tilt={-10}>
  <Graticule />
  <Countries stroke="grey" />
  <Latitude at={40} />
  <Line from="toronto" to='jamaica' />
  <Dot at={[90, 0]} color="lightblue" radius={50} />
</Globe>
```
![image](https://user-images.githubusercontent.com/399657/92409352-494f6e80-f10e-11ea-82cf-51c8bdc8e4c0.png)

<div align="right">
  <a href="https://spencermounta.in/somehow-maps/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-grid
[repo](https://github.com/spencermountain/somehow-grid)
```html
<script>
  import { Grid, Part } from 'somehow-grid'
</script>

<Grid total="500">
  <Part color="red" count="100" />
  <Part color="blue" count="100" />
</Grid>
```

<img src="https://user-images.githubusercontent.com/399657/92409898-30e05380-f110-11ea-965c-b8e7d4c1cb25.png"/>

<div align="right">
  <a href="https://spencermounta.in/somehow-grid/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-input
[repo](https://github.com/spencermountain/somehow-input)

```html
<script>
  let number = 3
</script>
<Number
  bind:number="{index}"
  min="1"
  max="4"
  hasSlider="{false}"
  hasKeyboard="{false}"
/>
```

<img src="https://user-images.githubusercontent.com/399657/92410104-093dbb00-f111-11ea-9de4-227b86aa7a80.png"/>

<div align="right">
  <a href="https://spencermounta.in/somehow-input/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>

### somehow-slider
[repo](https://github.com/spencermountain/somehow-slider)
```html
<script>
  import { Vertical, Slider, Label } from './src'
</script>
<Vertical bind:value min="{0}" max="{200}">
  <label start="10" end="20" color="red" label="beginning" />
  <label start="20" end="180" color="blue" label="middle" />
  <label start="180" end="190" color="red" label="end" />
</Vertical>
```
<img src="https://user-images.githubusercontent.com/399657/92410478-3048bc80-f112-11ea-9a90-2a8ae7613fe9.png"/>

<div align="right">
  <a href="https://spencermounta.in/somehow-slider/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


### somehow-sankey
[repo](https://github.com/spencermountain/somehow-sankey)
```html
<script>
  import { Sankey, Node } from 'somehow-sankey'
</script>
<Sankey height="600">
  <Col>
    <Node name="Property Taxes" to="Toronto" value="4400" color="sea" />
    <Node name="Province/Fed" to="Toronto" value="2500" color="red" />
    <Node name="TTC Fares" to="Toronto" value="1300" color="sky" />
    <Node name="Fees" to="Toronto" value="900" color="sky" />
  </Col>
  <Col>
    <Node name="Toronto" value="11600" color="blue" />
  </Col>
</Sankey>
```
<img src="https://user-images.githubusercontent.com/399657/92411176-c54cb500-f114-11ea-87ed-8e736ecb00f2.png"/>
<div align="right">
  <a href="https://spencermounta.in/somehow-sankey/">demo</a>
</div>
<div align="center">
  <img height="50px" src="https://user-images.githubusercontent.com/399657/68221837-0d142480-ffb8-11e9-9d30-90669f1b897c.png"/>
</div>


<!-- ## WIP
### somehow-horizon 
### somehow-graph 
-->

<!-- ### somehow-shapes -->
<!-- ### somehow-3d -->
<!-- ### somehow-ticks -->

MIT
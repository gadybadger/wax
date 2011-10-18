---
title: "Zoomer"
tags: ModestMaps
layout: control
---

A simple zoom control offering zoom in &amp; out buttons. It creates links and
appends them to the map.

### Example

<div class='live'>
{% highlight html %}
<div id='map-div'></div>
<script>
var mm = com.modestmaps;
var tilejson = {
  tilejson: '1.0.0',
  scheme: 'tms',
  tiles: ['http://a.tiles.mapbox.com/mapbox/1.0.0/world-bright/{z}/{x}/{y}.png']
};
var m = new mm.Map('map-div',
  new wax.mm.connector(tilejson));
wax.mm.zoomer(m, tilejson).appendTo(m.parent);
m.setCenterZoom(new mm.Location(39, -98), 2);
</script>
{% endhighlight %}
</div>

### API

<dl>
  <dt>{% highlight js %}var zoomer = wax.mm.zoomer(map){% endhighlight %}</dt>
  <dd>Create your own zoomer that controls a map called 'map'</dd>

  <dt>{% highlight js %}zoomer.appendTo(element){% endhighlight %}</dt>
  <dd>Add the zoom in &amp; zoom out div elements to another element.</dd>
</dl>
<!doctype html>
<html>
<head>
<title>~ Map Page 01, Phoenix-Valley.com +</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<style>
html, body { margin: 0; }
body { padding-bottom: 175px; }

.top_bar_wrap { margin-bottom: 15px;  }
.sitename { font-size: 24px; padding: 15px; }
.sitename span { font-size: 18px; }
div.subtitle { font-size: 14px; margin-top: 5px; padding-left: 10px;  }


.right_buttons { position: absolute; right: 10px; }
.right_buttons div { margin-bottom: 10px; }


nav { margin: 15px; margin-top: 5px; }

.main_map_wrap { margin-top: 45px; }
#map {  }

.extra_help_wrap { outline: 1px dashed #888; width: 85%; margin: 0 auto; padding: 15px; margin-top: 15px; border-top: 4px solid #555; }
.extra_help_wrap ul li { margin-bottom: 5px; }

</style>
</head>
<body>
<div class="top_bar_wrap">
<div class="sitename"># app ~ `# Gabbi-Van-App`
<br /><span> Map Page 01</span></div>
<div class="subtitle">https://github.com/Ejected-Media/Gabbi-Van-App</div>
<hr />
<button onclick="window.location.href='https://github.com/Ejected-Media/Gabbi-Van-App'">Repo</button>
<div class="right_buttons">
<div><button>Nav</button></div>
<div><button>Map</button></div>
</div>
</div>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>
 <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>

	<style>
		
		.leaflet-container {
			height: 400px;
			width: 600px;
			max-width: 100%;
			max-height: 100%;
		}
	</style>

<div class="main_map_wrap">
  ~ `# Gabbi-Van-App`
  <div id='map'></div>
</div>

<script>
var cities = L.layerGroup();

var mSkyHarbor = L.marker([33.435249, -112.010216]).bindPopup('Sky Harbor, AZ').addTo(cities);

var mPhx = L.marker([33.4484 , -112.0740]).bindPopup('This is Phoenix.').addTo(cities);

var mASU = L.marker([33.5100, -112.1289]).bindPopup('GCU, AZ').addTo(cities);

var mASU = L.marker([33.4230, -111.9278]).bindPopup('ASU, AZ').addTo(cities);

var mPhxZoo = L.marker([33.4500, -111.9470]).bindPopup('Phoenix Zoo').addTo(cities);



var osm = L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
	maxZoom: 19,
	attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
});

var osmHOT = L.tileLayer('https://{s}.tile.openstreetmap.fr/hot/{z}/{x}/{y}.png', {
	maxZoom: 19,
	attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, Tiles style by <a href="https://www.hotosm.org/" target="_blank">Humanitarian OpenStreetMap Team</a> hosted by <a href="https://openstreetmap.fr/" target="_blank">OpenStreetMap France</a>'
});

var map = L.map('map', {
	center: [33.4484 , -112.0740],
	zoom: 10,
	layers: [osm, cities]
});

var baseLayers = {
	'OpenStreetMap': osm,
	'OpenStreetMap.HOT': osmHOT
};

var overlays = {
	'Cities': cities
};

var layerControl = L.control.layers(baseLayers, overlays).addTo(map);

var crownHill = L.marker([39.75, -105.09]).bindPopup('This is Crown Hill Park.');
const rubyHill = L.marker([39.68, -105.00]).bindPopup('This is Ruby Hill Park.');

var parks = L.layerGroup([crownHill, rubyHill]);

var openTopoMap = L.tileLayer('https://{s}.tile.opentopomap.org/{z}/{x}/{y}.png', {
	maxZoom: 19,
	attribution: 'Map data: &copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, <a href="http://viewfinderpanoramas.org">SRTM</a> | Map style: &copy; <a href="https://opentopomap.org">OpenTopoMap</a> (<a href="https://creativecommons.org/licenses/by-sa/3.0/">CC-BY-SA</a>)'
});


layerControl.addBaseLayer(openTopoMap, 'OpenTopoMap');
layerControl.addOverlay(parks, 'Parks');
</script>

<div class="extra_help_wrap"><p>
# Gabbi-Van-App<br />
~ 🪐🦭 _ ` New Development ° . + </p>

<p>
https://github.com/Ejected-Media/Gabbi-Van-App<br />
--- </p>
<p>
~ hi<ul>
<li>+ Driver Data</li>
<li>+ Client From</li>
<li>+ Transportation List</li>
</ul></p>
</div>

<div class="extra_help_wrap">
    <p><b>_ A Gabbi Van ~ Driver Data</b></p>
    <div>~ Honolulu Lemonade</div>
  <div><ul>
    <li>What ~</li>
    <li>When ~</li>
    <li>Where ~</li>
    <li>Who ~</li>
    <li>Why ~</li>
  </ul></div>
</div><!-- - course_levels_wrap - -->
	
	<div class="extra_help_wrap">
    <p><b>_ A Gabbi Van ~ Client Form</b></p>
    <div>~ Honolulu Lemonade</div>
  <div><table>
    <tr><td>What ~ &nbsp; </td><td><input /></td></tr>
    <tr><td>When ~ &nbsp; </td><td><input /></td></tr>
    <tr><td>Where ~ &nbsp; </td><td><input /></td></tr>
    <tr><td>Who ~ &nbsp; </td><td><input /></td></tr>
    <tr><td>Why ~ &nbsp; </td><td><input /></td></tr>

<tr><td></td><td><input type="submit" value="Request Van" /></td></tr>
  </table>
</div>
</div><!-- - course_levels_wrap - -->
	
	<div class="extra_help_wrap">
    <p><b>_ A Gabbi Van ~ Transportation List</b></p>
    <div>~ Honolulu Lemonade</div>
  <div><table>
    <tr>
      <th>What ~</th>
      <th>When ~</th>
      <th>Where ~</th>
      <th>Who ~</th>
      <th>Why ~</th>
    </tr>
    
    <tr>
      <td>What ~</td>
      <td>When ~</td>
      <td>Where ~</td>
      <td>Who ~</td>
      <td>Why ~</td>
    </tr>
  

  </table>
</div>
</div><!-- - course_levels_wrap - -->


<div id="main_view"></div>
</main>


</main>
<footer>
~ hi
</footer>
</body>
</html>
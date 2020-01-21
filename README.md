## Example

```html
<div id="bd-map-markers" class="dashboard-map"></div>

<script src="path/to/jquery/jquery.min.js"></script>
<script src="path/to/jvectormap/jvectormap/jquery-jvectormap-2.0.2.min.js"></script>
<script src="path/to/jvectormap/jquery-jvectormap-bd-merc.js"></script>
<script>
    $(function(){
        $("#bd-map-markers").vectorMap({
            map:"bd_merc", 
            scaleColors:["#eff0f1", "#eff0f1"], 
            normalizeFunction:"polynomial", 
            hoverOpacity:.7, 
            hoverColor:!1, 
            regionStyle: {
                initial: {
                    fill: "#e0e7fd"
                }
            }, 
            markerStyle: {
                initial: {
                    stroke: "transparent"
                }
                , hover: {
                    stroke: "rgba(112, 112, 112, 0.30)"
                }
            }, 
            backgroundColor:"transparent", 
            markers:[ 
                {
                    latLng:[19.2313205, 92.77757443], 
                    name:"Noakhali", 
                    style: {
                        fill: "#0aafff"
                    }
                }, 
                {
                    latLng:[23.7593572, 90.3788136], 
                    name:"Dhaka", 
                    style: {
                        fill: "#0aafff"
                    }
                }, 
                {
                    latLng:[16.28909642, 95.10113525], 
                    name:"Chittagong", 
                    style: {
                        fill: "#0aafff"
                    }
                }
            ]
        });
    });
</script>
```
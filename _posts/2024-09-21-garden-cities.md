---
title: Garden Cities
date: 2024-09-21
tags:
    - urban-planning
    - theory
---
In 1898, Ebenezer Howard published _To-Morrow: A Peaceful Path to Real Reform_,
a book that he would later reprint in 1902 under the much more recognizable name of _Garden Cities of To-Morrow_.

![Alt text]({{ site.baseurl }}/assets/images/garden-cities-1.jpg) 
{: class="popout"}

<img src="{{ site.baseurl }}/assets/images/garden-cities-1.jpg">

This brief excerpt from Ebenezer Howard's Garden Cities of To-Morrow provides a backdrop for city planning examples such as Greendale and Levittown. Hopefully, the opening quotation: "I will not cease from mental strife/Nor shall my sword sleep in my hand/Til we have built Jerusalem/In England's green and pleasant land" reminds you of our previous discussions of the City Upon a Hill. We read Howard because so many of our forthcoming discussions of ideal public life are informed by his optimistic, indeed infectious, narrative.

I will leave the description of his Garden City to the author, focusing instead on three key points..

>Do not blah blah blah... eflects the ideal in American public life to establish a harmonious relationship between the machine and garden. Technology, hardly a foe to civilization in Howard's view, is essential 
{: .info}

The purpose of Howard's plan is to sustain "a healthy, natural, and economic combination of town and country life" through a balance of work and leisure. In this goal, Howard reflects the ideal in American public life to establish a harmonious relationship between the machine and garden. Technology, hardly a foe to civilization in Howard's view, is essential to healthy public life: 

<iframe src="https://www.google.com/maps/d/u/0/embed?mid=1dfU23bw20397f4AqpOjwQ4fFrgLS2FU&ehbc=2E312F" height="480"></iframe>

"The smoke fiend is kept well within bounds in Garden City; for all machinery is driven by electric energy" (p. 55). Industry and agriculture coexist in his ideal community - as do city and countryside, utopia and arcadia. Howard's sense of balance - in this case, the concentric circles of the Garden City intersected by broad boulevards - assumes that ideal forms will shape and perfect human functions: "No really sound plan of action is in more need of artificial support than is any sound system of thought" (p. 57).

<div id="map" style="width: auto; height: 400px"></div>

Technology, hardly a foe to civilization in Howard's view, is essential to healthy public life: "The smoke fiend is kept well within bounds in Garden City; for all machinery is driven by electric energy" (p. 55).

>Human society and the beauty of nature are meant to be enjoyed together. The two magnets must be made one. As man and woman by their varied gifts and faculties supplement each other, so should town and country.[^1]

Technology, hardly a foe to [civilization](https://stephango.com/self-guarantee) in Howard's view, is essential to healthy public life: "The smoke fiend is kept well within bounds in Garden City; for all machinery is driven by electric energy" (p. 55).

[^1]: Some *crazy* footnote definition.

<script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet-ajax/2.1.0/leaflet.ajax.min.js" integrity="sha512-Abr21JO2YqcJ03XGZRPuZSWKBhJpUAR6+2wH5zBeO4wAw4oksr8PRdF+BKIRsxvCdq+Mv4670rZ+dLnIyabbGw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script>
    var map = L.map('map').setView([37.32, -121.91], 13)

    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
        maxZoom: 19,
        attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
    }).addTo(map);

    var marker = L.marker([37.32, -121.91]).addTo(map);

    function onEachFeature(feature, layer) {
        if (feature.properties && feature.properties.Project_Name) {
            layer.bindPopup("<p><b>" + feature.properties.Project_Name + 
            "</b></p><p><b>Developer:</b> " + feature.properties.Owner_Developer + "</p>", {closeButton: false});
            layer.on('mouseover', function() { layer.openPopup(); });
            layer.on('mouseout', function() { layer.closePopup(); });
            layer.on('click', function() { window.open(feature.properties.Website_Page);
            }); 
        }
    }

    const geojson = new L.GeoJSON.AJAX('https://raw.githubusercontent.com/awildjake/hello-leaflet/main/assets/projects.geojson',{
        onEachFeature:onEachFeature,
        pointToLayer: function (feature, latlng) {
    	    return L.marker(latlng);
        }
    }).addTo(map);

</script>
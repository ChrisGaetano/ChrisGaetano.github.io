#### My name is Chris Gaetano and I am a junior economics major at Lehigh University. I also have a double minor in marketing  and journalism. This is my Github page for my J24 class. Over the semester I plan on working on several data visualization projects to add to my project. 


## Movie Worldwide Gross Infographic
![Movie](https://github.com/ChrisGaetano/ChrisGaetano.github.io/blob/master/Highest%20Grossing%20Filmsof%202016.png?raw=true)

This infographic displays the top 5 highest grossing films of 2016. This is the total gross for movies worldwide. The highest grossing film of the year was Captain America: Civil War.Four out of the five highest grossing films earned more than one billion worldwide. All the films were distributed by the Disney Company. This infographic was created using the website Canva.



##  Beatles Album History Timeline
<iframe src='https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=13vJG4x-IC2yt7Fe6AepFW62aBMUpGFn8__SrOH7WZtk&font=Default&lang=en&initial_zoom=2&height=650' width='100%' height='650' webkitallowfullscreen mozallowfullscreen allowfullscreen frameborder='0'></iframe>

This timeline was created using TimelineJS. The timeline goes over the all the studio albums that the Beatles have produced. The timeline discusses the year the albums came out and it discusses some of the songs on the albums. The timeline starts with the Beatles' first albums Please Please Me, and it ends with Let It Be. 



## Lehigh Enrollment Infographic
![Graph](https://raw.githubusercontent.com/ChrisGaetano/ChrisGaetano.github.io/master/2016_Lehigh_University_Undergraduate_Enrollment_Percent_Enrollment_chartbuilder.png)

This infographic describes the percent enrollment of undergraduate students at Lehigh University in 2016. The information was gathered using Lehigh's Office of Institutional Research and the graphic was created using Chartbuilder 3.0.5.



## Lehigh Undergraduate Enrollment Line Chart

![graph](https://github.com/ChrisGaetano/ChrisGaetano.github.io/blob/master/Lehigh_University_Percent_Undergraduate_Enrollment_Arts_&_Sciences_Business__Engineering_chartbuilder.png?raw=true)

This infographic shows the change in Lehigh University Undergraduate Enrollment from the year 2006 to the year 2016. With this infographic you can see that the percent enrollment changed drastically for all the schools, especially for the college of Arts and Sciences and teh school of engineering. This timeline was created using information from Lehigh's Office of Institutional Research and the graphic was created using Chartbuilder 3.0.5.



## Netflix Subscriber Growth

![Netflix](https://raw.githubusercontent.com/ChrisGaetano/ChrisGaetano.github.io/master/Netflix__Subscribers_Worldwide_Number_of_Subscribers_(In_Millions)_chartbuilder.png) 

This infographic displays how Netlfix subscribers have grown overtime. As you can see the growth is direct in that as time has passed the amount of Netflix subscribers has increased. With Netflix being the most popular it has been in years it makes sense that the graph is at its peak point in 2017. 2011 is the year in which Netflix became international, so you can see that in this year the growth becomes quicker. This timeline was created using information from Netflix annual reports and the graphic was created using Chartbuilder 3.0.5.

<!DOCTYPE html>
<html>
<head>
<meta name="viewport"/>
<title>Arts Centers - Google Fusion Tables</title>
<style type="text/css">
html, body, #googft-mapCanvas {
  height: 300px;
  margin: 0;
  padding: 0;
  width: 500px;
}
</style>

<script type="text/javascript" src="https://maps.google.com/maps/api/js?v=3"></script>

<script type="text/javascript">
  function initialize() {
    google.maps.visualRefresh = true;
    var isMobile = (navigator.userAgent.toLowerCase().indexOf('android') > -1) ||
      (navigator.userAgent.match(/(iPod|iPhone|iPad|BlackBerry|Windows Phone|iemobile)/));
    if (isMobile) {
      var viewport = document.querySelector("meta[name=viewport]");
      viewport.setAttribute('content', 'initial-scale=1.0, user-scalable=no');
    }
    var mapDiv = document.getElementById('googft-mapCanvas');
    mapDiv.style.width = isMobile ? '100%' : '500px';
    mapDiv.style.height = isMobile ? '100%' : '300px';
    var map = new google.maps.Map(mapDiv, {
      center: new google.maps.LatLng(40.60498878615068, -75.3880652225098),
      zoom: 13,
      mapTypeId: google.maps.MapTypeId.ROADMAP
    });
    map.controls[google.maps.ControlPosition.RIGHT_BOTTOM].push(document.getElementById('googft-legend-open'));
    map.controls[google.maps.ControlPosition.RIGHT_BOTTOM].push(document.getElementById('googft-legend'));

    layer = new google.maps.FusionTablesLayer({
      map: map,
      heatmap: { enabled: false },
      query: {
        select: "col0",
        from: "15KzS7gXfluOzYjqP0TKZ4snu_jMjHWzLxwEk6cxT",
        where: ""
      },
      options: {
        styleId: 2,
        templateId: 3
      }
    });

    if (isMobile) {
      var legend = document.getElementById('googft-legend');
      var legendOpenButton = document.getElementById('googft-legend-open');
      var legendCloseButton = document.getElementById('googft-legend-close');
      legend.style.display = 'none';
      legendOpenButton.style.display = 'block';
      legendCloseButton.style.display = 'block';
      legendOpenButton.onclick = function() {
        legend.style.display = 'block';
        legendOpenButton.style.display = 'none';
      }
      legendCloseButton.onclick = function() {
        legend.style.display = 'none';
        legendOpenButton.style.display = 'block';
      }
    }
  }

  google.maps.event.addDomListener(window, 'load', initialize);
</script>
</head>

<body>
  <div id="googft-mapCanvas"></div>
</body>
</html>

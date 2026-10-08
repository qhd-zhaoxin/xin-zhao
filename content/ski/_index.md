---
title: "Ski Resorts I Visited"
---

<div id="map" style="height:600px;max-width:100%"></div> 
<script> function initMap() {
    var map = new google.maps.Map(document.getElementById('map'), {
        zoom: 2,
        center: {
            lat: 47.6026,
            lng: -122.3321
        }
    });
    [
        ['Summit', 47.424, -121.416],
        ['Crystal', 46.92332964, -121.475998096],
        ['Timberline Lodge', 45.33, -121.71],
        ['Whistler', 50.116322, -122.957359],
        ['Taos', 36.594687, -105.449505],
        ['Ziyunshan', 40.023896, 119.596639],
        ['Qishan', 39.323788, 114.690415]
    ].forEach(function(r) {
        new google.maps.Marker({
            position: {
                lat: r[1],
                lng: r[2]
            },
            map: map,
            title: r[0]
        });
    });
} </script> 
<script async defer src="https://maps.googleapis.com/maps/api/js?key=AIzaSyD24FzT3Syaf7pHoe0nOToK6pzw4W-PpeY&callback=initMap"></script>
+ This code creates a `google.maps.Marker` object. We set the position of the marker at a particular latitude and longitude, and tell it which map to add itself to - in this case the map is called `mymap`.

```javascript
var marker = new google.maps.Marker({
  position: {lat: 52.194470, lng: 0.134618 },
  map: mymap
});
```

Add this code to your page anywhere that meets the following criteria:
- It is after the `initMap()` function - because we need the map to be created before we can add markers to it
- It is between `<script>` and `</script>` tags - because it is JavaScript code

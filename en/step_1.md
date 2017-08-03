+ This code creates a `google.maps.Marker` object. We set the position of the marker at a particular latitude and longitude, and tell it which map to add itself to - in this case the map is called `mymap`.

```javascript
var marker = new google.maps.Marker({
  position: {lat: 52.194470, lng: 0.134618 },
  map: mymap
});
```

Add this code to your page, being careful to check that:
- You add the code after you create the `new google.maps.Map` - because we need the map to be created before we can add markers to it
- You add the code between `<script>` and `</script>` tags - because it is JavaScript code
- You make sure that the name of the map (in this example `mymap`) is the same name as the map you have created. For example, if your map code starts off like this `awesome_map = new google.maps.Map(...` then you would need to change the name from `mymap` to `awesome_map` to make the marker appear on your map.

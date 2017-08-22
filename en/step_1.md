+ The code below creates a `google.maps.Marker` object. We set the position of the marker at a particular latitude and longitude, and tell it which map to add itself. In this case, the map is called `mymap`.

```javascript
var marker = new google.maps.Marker({
  position: {lat: 52.206727, lng: 0.124450 },
  map: mymap
});
```

To display the marker on your page, add this code to your HTML file using the following steps:
1. The code for the object goes between `<script>` and `</script>` tags, since it is JavaScript code
1. Make sure that the code is below the line containing the `new google.maps.Map` command, because the map has to be created before we can add markers to it
1. Check that the name of the map in this new bit of code (as you can see, it's `mymap`) is the same as the name of the map you have created. For example, if your map code starts with `awesome_map = new google.maps.Map(...`, then you would need to change the name from `mymap` to `awesome_map` to make the marker appear.

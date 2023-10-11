

## General

- Stance Maples has an awesome introduction to GEE on [youtube](https://youtu.be/oAElakLgCdA).
- Didactics: 
  - When walking through the code, try to involve the students in the thought processes that it might take to come up with the correct solution.
  - The classification example is ~~outdated, especially since the training data needs to be uploaded. There is usually not enough time to do this anyway.~~ a standalone script that I presented in different lecture


## GEE Functions reference


- Get the current time using the JavaScript Date.now() method.
  
  ```js
  var now = Date.now();
  print('Milliseconds since January 1, 1970', now);
  ```

- Get the `system:time_start` property of an image and print it as a date:

  ```js
  var time_start = gfcc.first().get("system:time_start")
  print(ee.Date(time_start))
  ```

- Get the first and last date of an imageCollection:

  ```js
  var first_date = ee.Date(gfcc.first().get("system:time_start"))
  var last_date = ee.Date(gfcc.sort("system:time_start", false).first().get("system:time_start"))

  print("from", first_date, "to", last_date)
  ```


- Map an anonymus function over an ImageCollection:

  ```js
  myImageCollection.map(function(image) {
    return image.multiply(2);
  });
  ```
  

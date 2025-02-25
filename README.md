# Download
```$ git clone https://github.com/brianhsu7476/activityEditPublish```

# Combine
```$ ./combine activity0.gpx activity1.gpx ...```

The output will be written in ```output.gpx```.

You can open ```map.html``` to see the comparison between the original activities and the combined one.

It not only combines the routes on the map, but also combines the data if they share the same timestamp. For example, if your heartrate data is only in ```activity0.gpx```, and your power data is only in ```activity1.gpx```, you can use the command ```python3 combine.pyc activity0.gpx activity1.gpx``` in your shell to combine them. Note that if the combined data conflicts, then it will use the one in the first activity. For example, if both ```activity0.gpx``` and ```activity1.gpx``` have elevation data, then it will use the elevation data in ```activity0.gpx```.

# Clean
```$ make clean```


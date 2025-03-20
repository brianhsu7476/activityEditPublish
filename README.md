# Download
```$ git clone https://github.com/brianhsu7476/activityEditPublish```

# Combine
Linux: Open your terminal:
```$ ./combine activity0.gpx activity1.gpx ...```
Windows: Open your cmd:
```$ combine.exe activity0.gpx activity1.gpx ...```

The output will be written in ```output.gpx```.

You can open ```map.html``` to see the comparison between the original activities and the combined one.

It not only combines the routes on the map, but also combines the data if they share the same timestamp. For example, if your heartrate data is only in ```activity0.gpx```, and your power data is only in ```activity1.gpx```, you can use the command ```python3 combine.pyc activity0.gpx activity1.gpx``` in your shell to combine them. Note that if the combined data conflicts, then it will use the one in the first activity. For example, if both ```activity0.gpx``` and ```activity1.gpx``` have elevation data, then it will use the elevation data in ```activity0.gpx```.

# Split
Linux: Open your terminal:
```$ ./split3 activity0.gpx activity1.gpx ...```
Windows: Open your cmd:
```$ split3.exe activity0.gpx activity1.gpx ...```

The output will be written in ```output.gpx```.

You can open ```map.html``` to see the comparison between the original activities and the splitted one.

Enter $n$ points $a_1, a_2, \dots, a_n$, and $a_0=0, a_{n+1}=end$. Those in $(a_{2i-1}, a_{2i})$ will be removed. For example, if you want to remove all points in the second hour you rode, enter ```1:0:0 2:0:0```.

# Clean
```$ make clean```


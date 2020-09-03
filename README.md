# Automl VR

### The orginal TFLite Unity Example
https://www.github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/experimental/examples/unity/TensorFlowLitePlugin

### Gist for generating perfect bounding boxes
https://gist.github.com/ZackAkil/ce6604fd5ac008756f938047ce73d9d5

### Gist for capturing a UNity camera view as PNG
https://gist.github.com/ZackAkil/b22471aefa05fac6ad46f7589081dffb

### Generating a bounding box label CSV row for Google AutoML Object Detection
```csharp
writer = new StreamWriter(csv_path, true);

// create label row for Google AutoML Object Detection
string row = string.Format("UNASSIGNED,{0}{1},{2}, {3}, {4},,,{5},{6},,", "BUCKET_LOCATION",
                                                                               file_name,
                                                                               label_name,
                                                                               x_relative_min,
                                                                               y_relative_min,
                                                                               x_relative_max,
                                                                               y_relative_max);
writer.WriteLine(row);
```

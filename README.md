# Getting-started-with-OpenCV

## ISSUES

Some of the common terms used in the errors are very well explained in this [repository](https://github.com/microsoft/pylance-release/blob/main/DIAGNOSTIC_SEVERITY_RULES.md#diagnostic-severity-rules), I could know why this error `reportMissingImports` occured through this repository.

>tracker = cv2.Tracker_create(tracker_type) AttributeError: module 'cv2' has no attribute 'Tracker_create'


This error occurs when you do not have the correct opencv library downloaded.
You will need to uninstall the existing opencv library using `pip uninstall opencv-python`, if you have already downloaded    opencv-contrib-python library then you will have to uninstall that too using `pip uninstall opencv-contrib-python`, now       install opencv-contrib-python using `pip3 install opencv-contrib-python`.


>yntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: truncated \UXXXXXXXX escape

This error occurs you use normal string as the path.
This can be sorted by `adding 'r' in front` of the path.

Eg: (r"D:\Document\OpenCV\race_car.mp4")

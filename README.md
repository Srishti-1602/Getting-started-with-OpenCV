# Getting-started-with-OpenCV

OpenCV is a very important library to understand if you want to work with image processing, video streaming etc. In this repository I have added basic codes to start with this library, including working with images and video streaming. 

Also I have tried a lot of ways to download this library but it didn't support the version of python installed in my PC. At last I dowloaded anaconda and installed python version 3.6.5 and connected VS Code with conda. If you want to do image processing or working with videos (like object tracking) I would preffer to use Jupytor notebook for that, but if there is anything that uses the accessing of your device's camera you should definetely preffer VS Code.

## ISSUES

Here are some of the issues I faced.

Some of the common terms used in the errors are very well explained in this [repository](https://github.com/microsoft/pylance-release/blob/main/DIAGNOSTIC_SEVERITY_RULES.md#diagnostic-severity-rules), I could know why this error `reportMissingImports` occured through this repository.

>tracker = cv2.Tracker_create(tracker_type) AttributeError: module 'cv2' has no attribute 'Tracker_create'

This error occurs when you do not have the correct opencv library downloaded.
You will need to uninstall the existing opencv library using `pip uninstall opencv-python`, if you have already downloaded    opencv-contrib-python library then you will have to uninstall that too using `pip uninstall opencv-contrib-python`, now       install opencv-contrib-python using `pip3 install opencv-contrib-python`.


>yntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: truncated \UXXXXXXXX escape

This error occurs you use normal string as the path.
This can be sorted by `adding 'r' in front` of the path.

Eg: (r"D:\Document\OpenCV\race_car.mp4")

> "execution_count": null,  NameError: name 'null' is not defined

This error occurs when we save the file in different format and run in another (i saved the file in .IPYNB and tried to run it in .PY format). To avoid this error just copy the code from .IPYNB file and paste in new file and save this new file in .PY format.


>Codes present in this repository are not mine, I have collected these codes (which are basics to work with this library) from different sources. 

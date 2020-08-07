### Export As
`ExportAs` is a SlicerMorph specific plugin for the `Data` module that enables the user to directly save the selected node in one of the support formats with a right-mouse click. 

Note that unlike the built-in **Save As** dialog box, `ExportAs` does **NOT retain states** (e.g., it will not remember the folder where you might have exported the same node previously). For complicated scenes, such as ones that contain multiple volumes, segmentations, 3D models derived from segmentation, measurements of various types, etc you definitely want to use the **Save As** dialog box. However, if you only work on few nodes and mainly interested in one or two of them, `ExportAs` provides a convenient way of saving them. Additionally, `ExportAs` is currently the only way to export curve semi-landmarks in fcsv format (will be covered in detail tomorrow). 

To use `ExportAs` go to the `Data` module, right click on either a volume, a model or a fiducial node and choose `Export As`, and select one of the formats. The suggested formats as are highlighted in red. 

**Note:** While 3D Slicer lists PNG/BMP/JPG as output options for volumes, it actually doesn't save it. I.e., you cannot save a 3D volume as an image sequence/stack through Slicer. If you choose TIFF format, it will save it as a multi-frame single tiff image. Please always keep 3D volumes in a 3D format (NRRD is Slicer's default format for volumes). [STL is a terrible format and should be avoided.](https://discourse.slicer.org/t/beware-of-the-stl-file-format/7642) Please use OBJ or PLY instead. 

### Volumes

<img src="ExportAs_Volumes.png">

### Models

<img src="ExportAs_Models.png">

### Curves

<img src="ExportAs_Curves.png">

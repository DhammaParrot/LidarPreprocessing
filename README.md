# Lidar
The notebook "preprocessing.ipynb" (and my example preprocessing_example.ipynb) in the directory "~/LidarPreProcessing/notebooks/" process a directory of las files into voxelised, sectorialised and labeled pointclouds in xyz format using the 2d polygons shapefile "~/LidarPreProcessing/resources/archaeology.shp" from the "2019_angkormap/Master/AngkorMaster.shp" repository.
Steps to implement:
1. Clone the repo and make a virtual enviroment with python 3.8
2. Install the requirments.txt file
3. Place las files in the directory "~/LidarPreProcessing/data/las/testdata/"
4. Set up and run "preprocessing.ipynb" notebook. After the imports at the beginning, update the location of the archeology.shp file, data directory, and define the voxel size and number of sectors in one direction. 
5. Files will be outputed in "~/LidarPreProcessing/data/txt/testdataout/"
###
Notes: 
1.Please ignore the warning: "<ipython-input-5-287de340edbe>:32: RuntimeWarning: Sequential read of iterator was interrupted. Resetting iterator. This can negatively impact the performance.
  hits=list(shape.items(bbox=(xmin, ymin, xmax, ymax)))"
2. Remember to clear out the files in ~/LidarPreProcessing/data/txt/testdata/" and  ~/LidarPreProcessing/data/txt/testdataout/" if you wish to try out a new set of las files in  "~/LidarPreProcessing/data/las/testdata/" as the new txt files are added iteratively. 
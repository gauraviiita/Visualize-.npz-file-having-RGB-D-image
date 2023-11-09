# Visualize-.npz-file-having-RGB-D-image


For reading file squentially, we need to added sorted before glob.glob

# This is the path where all the files are stored.
**Method-1**

import os
folder_path = "images"
for data_file in sorted(os.listdir(folder_path)):
    print(data_file)

**Method-2**
import glob
path = "images/*.*"
for file in sorted(glob.glob(path)):
    print(file)

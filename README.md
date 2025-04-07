# Comparative_CCNs_for_PSC_PCE

This project contains the following files:

Data_RL_FAIR.csv:

A csv file separated by ; containing the data measured in reveserse bias and under lighting conditions. This file contains the following columns:
- Cell_ID: Identifier assigned to each sample. The complete images contained in this dataset are labeled with the same identifier for ease of correlation. Each cell architecture is given a unique name, and repeated architectures are differentiated by numbers at the end of the ID.
- Cell_Architecture: Layer structure of each sample. NOTE: 5Trypt and 15Trypt identifiers signify different concentrations of Tryptophan, namely 5 or 15mM.
- Before_Encap_Img_Path: Path to the unedited sample images before encapsulation for ease of access. The path is given relative to the directory the zip files are unpacked in.
- After_Encap_Img_Path: Same as Before_Encap_Img_Path, only for samples after encapsulation.
- Pixel_ID: Identifier of each pixel contained in the devices. These can take values of A, B or C, which corresponds to the pixels contained in the device images from right to left.
- Bias: Bias under which the JV-sweep was performed. For this dataset, only reverse bias conditions were considered.
- Light: Lighting condition. For this dataset, only values measured under lighting were considered.
- Eff_before [%]: PCE of the individual pixels before encapsulation given in percent.
- Eff_after [%]: PCE of the individual pixels after encapsulation given in percent.

Data_RL.xlsx:

An excel file containing the same data as in Data_RL_Fair.csv. It is pre-formated for the convenience of windows users. The column names are identical to the ones given for Data_RL_Fair.csv.

Before_Encap.zip:

A zip file containing all relevant images taken before encapsulation of full device images, cropped device images and pixel images cut from the cropped images. The naming scheme is based on the Cell_ID and Pixel_ID columns in the data files. In more detail, this means:
- Full device images: Cell_ID.png
- Cropped device images: Cell_ID_cropped.png
- Pixel images: Cell_ID_cropped_Pixel_ID.png

After_Encap.zip:

A zip file containing all relevant images taken after encapsulation of full device images, cropped device images and pixel images cut from the cropped images. The naming scheme is based on the Cell_ID and Pixel_ID columns in the data files. In more detail, this means:
- Full device images: Cell_ID.png
- Cropped device images: Cell_ID_cropped.png
- Pixel images: Cell_ID_cropped_Pixel_ID.png

NOTE: To use the Paths given in the data files, the zip files must be unpacked into the same directory.

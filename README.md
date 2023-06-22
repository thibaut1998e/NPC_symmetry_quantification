# NPC_symmetry_quantification

## Python dependencies

Dependencies (and version the software has been teste on):
- matplotlib (3.6.1)
- pandas (1.5.0)
- numpy (1.23.1)
- imageio (2.22.1) or mrcfile (1.4.3) depending on the type of ile you want to read

This code takes as input a folder containing 2D crops of the Nuclear Pore Complex (NPC). Each crop is separated in 8 sectors and the number of activated sectors is counted. Then the histogram of the number of activated sectors is saved, as well as the separation in 8 sectors for each NPC crop. 
Please sapecify 

*npc_path* : the input folder containing a set of 2D NPC crops. It has to be square images, they do not need to have the same shape

*save_fold* : In this folder are saved the separation in 8 sectors for each NPC crop, as well as the histogram of the number of activated sectors

*thershold_conversion_to_pc* : images are converted to point clouds, defined as the set of pixel coordinates higher than a given threshold. Please make sure that this value is coherent with your image range

*alpha* : We keep a proportion alpha of the nearest points from the center

*thersh_activated_sectors* : A sector is activated if the total number of points that it contains is greater than 'thersh_activated_sectors' times the total number of points in the image

Excpected run time : 0.3s per 2D images of size 50*50






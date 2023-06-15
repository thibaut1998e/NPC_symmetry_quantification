# NPC_symmetry_quantification

This code takes as input a folder containing 2D crops of the Nuclear Pore Complex (NPC). Each crop is separated in 8 sectors and the number of activated sectors is counted. Then the histogram of the number of activated sectors is saved. 
Please sapecify 

*npc_path* : the input folder containing a set of 2D NPC crops. It has to be square images, they do not need to have the same shape

*save_fold* : In this folder are saved the separation in 8 sectors for each NPC crop, as well as the histogram of the number of activated sectors

*thershold_conversion_to_pc* : images are converted to point clouds, defined as the set of pixel coordinates higher than a given threshold. Please make sure that this value is coherent with your image range

*alpha* : We keep a proportion alpha of the nearest points from the center

*thersh_activated_sectors* : A sector is activated if the total number of points that it contains is greater than 'thersh_activated_sectors' times the total number of points in the image




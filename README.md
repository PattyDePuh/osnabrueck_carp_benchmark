# osnabrueck_carp_benchmark
Municipal waste service problem instance useable for the Capacitated Arc Routing Problem (CARP).

The file 'filled_osna_streets.json' contains mostly the same street data provided from OSM within the administrated boundary of Osnabrück, but matched with dumbster volume data from local government and public waste service of Osnabrück.

+ The added data can be found in the 'way' elements in the keyword 'waste_zones'.
+ Additional key 'has_waste' indicates, if the way segment has dumbsters, that need to be emptied.
+ The 'way' element contains entries with a district number as the key (There are 23 districts in total).
+ Each district entry distinguishes between the left and right side to determine on which side the dumbsters are located.
+ For each side there are can be three different types of dumpsters (As germans prefer to seperate their waste)
+ Each entry of 'blue' (paper/carton), 'grey' (residual waste) and 'brown' (biowaste) contains the summed volume of all dumbsters from the designated street segment.

The "all-in-one" data file 'filled_osna_streets.json' might be still raw and needs some refinement.
Especially more informations have to be provided, like depot location, recycling center, fleet size and capacity.

For more suggestions, how to make these data more convinient to use, feel free to leave an issue for that on this repo.

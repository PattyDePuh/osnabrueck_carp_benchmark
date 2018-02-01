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

---

***Zone information***

Zone | Volume ***blue***| segments ***blue*** | Volume ***grey*** | segments ***grey*** | Volume ***brown*** | segments ***brown***
---: | ---: | ---: | ---: | ---: | ---: | ---:  
total | 9127340 | 4325 | 8748820 | 4382 | 3691560 | 3878
1 | 830160 | 263 | 856820 | 270 | 190920 | 239
2 | 586440 | 239 | 548320 | 245 | 242400 | 230
3 | 599660 | 318 | 562680 | 319 | 273600 | 300
4 | 366460 | 177 | 395220 | 178 | 168120 | 171
5 | 290660 | 109 | 258620 | 115 | 76080 | 95
6 | 499980 | 224 | 482780 | 226 | 220560 | 209
7 | 278820 | 148 | 260740 | 151 | 116640 | 126
8 | 400440 | 196 | 365680 | 196 | 197760 | 177
9 | 173420 | 57 | 195220 | 59 | 64800 | 57
10 | 706180 | 206 | 741760 | 208 | 288840 | 198
11 | 233020 | 112 | 220580 | 112 | 104160 | 97
12 | 195380 | 78 | 180820 | 78 | 78360 | 67
13 | 329260 | 87 | 336300 | 97 | 81960 | 71
14 | 784120 | 273 | 780600 | 276 | 337200 | 261
15 | 369240 | 139 | 343980 | 140 | 167040 | 124
16 | 746900 | 233 | 721500 | 233 | 293880 | 228
17 | 209160 | 159 | 173380 | 159 | 95400 | 143
18 | 346280 | 314 | 278080 | 316 | 145920 | 259
19 | 191800 | 189 | 180100 | 193 | 81480 | 153
20 | 119520 | 140 | 101800 | 140 | 47640 | 98
21 | 407180 | 340 | 358160 | 344 | 202080 | 298
22 | 328200 | 236 | 277460 | 237 | 160560 | 203
23 | 135060 | 88 | 128220 | 90 | 56160 | 74

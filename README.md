# PeonDefense
Orc Peon Tower Defense

# Notes


#Story and Character Development

##Overall Story
Peon Orc notices that most everyone has left. He is told by the other orcs that they have left to raid an Elven village far to the North. Little did the Orcs know that the Elves has a spy amongst them and found out their plan. The idea was to get all the other creatures in the land to finally wipe out the orcs for good. The peon goes on guard duty and sees the Orc area getting attacked. He decides to defend with towers. After saving the place, he continues to the next area to defend, trying to rally the other Orcs that stayed behind. Unfortunately, most of the other Orcs are too stupid, lazy, or just plain don’t like him. Only after getting attacked enough will the other Orcs listen to him. Eventually, the last of the orcs defend off the waves of baddies with mechanical wit and the will to eat all they kill.

#Main Characters
Gragnap the Orc: Dented helmet. Light green skin. Gnarly teeth with decent sized gaps. Giant canines, Very big, 6’8ish, Muscular. Wearing plate armor that is also dented. One arm is big and muscular. This is his hand that he hammers with. The other one is tinier, almost a gimp hand.

Maully: Female engineer/Scientist Orc. Darker green skin Way too much into her own inventions. Wears glasses. Around 6’3”ish, Still muscular. Short Pixie cut hairstyle. Thinner face, but bigger body. Wearing Full Plate Orc Muscular. Long black hair with a streak of red.

Orgif: Idiot. Very unaware of his surroundings. Thin eyebrows. Greyish green skin. Smaller orc. 5’8”  A little skinny. No shirt, just a loin cloth. Ponytail hairstyle. Always confused look. Carries a trident for fishing. Has a pony tail. Grey.

Varkust: Older retired orc. Plenty of strech lines and veins on his body. Wears a robe. Seems to always be tired. Carries a sense of magic around him. Constantly has pen and paper. Writes things down for the Orcs. Pale Green Skin. Bald.Hunched over. 6’5ish 

#Tiled Map Format
NOTE: This format is still in flux.  The game does not read the files yet, so implementation may require change.
NOTE2: OneOfEverything.tmx is intended to be a reference file that excersizes each aspect of the level functionality

##Build Paths
This layer will define where the player can put towers.
Any square that is NOT BLANK can have a tower.
This layer is not drawn.

##Walk Paths
This layer defines where walking mobs can go.
The tile value at 0,0 defines a "Start Position"
The tile value at 1,0 defines a "End Position"
The tile value at 2,0 defines a "Walkable Position"
The three above locations are not used when rendering or defining paths.  They just are used to determine what the tile types mean to the level loader.
TODO: Currently all starting positions are equal.  May want to some day implement delays on some entrances?
This layer is not drawn.

##Swim Paths
The same as WalkPaths except it defines start, end and swimmable positions
Swimming paths and walking paths can overlap.
This layer is not drawn.

##All Others
All other layers are drawn as is, and in the order they apear in the tile editor
To have a mob walk under or swim under another layer like a bridge, than just put the swim or walk layer under the layer they will walk behind.
In general the map will render in the order defined in the file

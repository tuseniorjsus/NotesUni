#### ApuntesFis Pyro Rendering 

render pyrp shet -> karma pyro material/ binding to the pyro bake volumen , render problems solution = old versión b(breakmaterialbindings setup) , newversion(go into solaris, bring vdb obvject and setup shader). 



solaris road

\- SOP import(rename accordingly) 

\- bring a light source into solaris

\-créate camera and render settings node(XPU Parameters)

\- mat library 

&#x09;-Karma Pyro Fire Material->SetUp Scale, modify binding according to the baking node in the previous stage, material properties node(fire efficient , emissive node) turn on property this attribute cointributes to light emisión

&#x20;	-

\- Merge to bring in grill, sop import the geometry and merge if you want you can assoiate the grill with a new materia, the same with other geometry in your previous scene.



The pyro bake volumen work as a previs of the volumen in this versión of Houdini



HOW TO CREATE NEW STAGES IN SOLARIS OR LOP NETWORKS

Lop Network in obj -> New Solaris Context 



solaris 2 road 

\- SOP import(rename accordingly)

\- Dome Light Input for vdb 

\- Camera 

\-Material Library 

\-Library Linker 

\-Render Setting / Karma Setup -> Volume Limit 2 Base 





#### Explosions 

###### 

###### **Sop workflow Pyro** 

* Resource Heavy Reactions(Keep in mind the amount of voxels and points)
* Origin Point 
* PyroBust Source- Solver for explosions -> Colr of point in solver symbolizes attributes->Added attribute in comparison to flame(Velocity) 
* 5 Frames -> Generate fields for further inputs 

  * Muzzle Flash -> Explosions with directions of some sort
  * ShockWaves 
  * Blast Ring -> Nuclear Explosion Rings 

Transform Help us set the location of our explosión



#### **PyroBurst Source** 



###### **Burst Shape** 



**Explosion Settings Shape** 

* Roundness-> Uniform explosion+ 
* Spread angle -> Switch Depending on location 

Explosion Settings Trail

* Number of trailings (cones opresent in explosions) 
* Trailing Separation +- Points present in the explosion 
* Trailing Thickness Amount of points in each cone 

**Burst Animation** 

Overall expansion-> The final shape present in frame five 



###### **Rescue Fields** 

**Temperature, Velocity, Burn(Fire), Density(Dust or smoke)**



Burst Components-> Pyro Sources 

Coverage Attributes-> delete to switch from template rasterize attributes, Add attribute rules-> v 



**Alt Route->** Set Preset setting or config Set in presets a source volume(Cooking Pot Icon) to create Node attributes for repeatitive use



###### **Pyro Source**



**To do list before pyro source** 



* Points with attributes
* Rasterize Attributes Point-> Attributes->voxels->Fields 
* Source Fields into solver -> Target Field 



Extra attribute from sourcing in pyro source 



Add Source -> Source Volume Temperature-> Target Field (Divergence) , creates noise in the explosion 

**Questions** 

Does it make a difference when a make a vectorial operation vs a scalar one. 

What does each operation do? 

Which fields work with each operation? How can you setup an extrabehavioural field to the affect a target field? 



##### 

##### **Activity Investigation**



**Color-> Explosion Layers** 

**Center of Explosion White, depending pf intensity,** 

**Source Temperature Fields-> for color modification** 

**Paint temperatura fields to expand from the center of the explosion.** 

**High** 



Look of a real life explosion, (the slow mo guys). 



Centroid of light 



Smoke Coverage 

Smoke Tendril forms, Cloud like Coverage 



Smoke Catches Fire Again, explosion expands, Smoke Dies Out



Fire Expands 



Fire reduces and generates a normal fire. 





Can it be set up with a singular burst? 



How you make smoke catch fire again? 

Scattering, mask , (render) 




























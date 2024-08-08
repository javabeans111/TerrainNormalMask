# Terrain Normal Mask
## A simple yet powerful Unity Asset Store tool to add variation to terrain

![snowcover_half](https://github.com/user-attachments/assets/ffab80dc-cce8-44e7-82b4-5ef8c0ffb45e)
### Email : <javabeans111@163.com>

## Intention
* Generate mask for terrain layer according to terrain normal;
* Add natural details for existing terrain layer weights;

## Quick Start
1. Drag ====TerrainNormalMask==== prefab in the prefab folder into your scene,
   the TerrainNormalMask Component is there for configuration;

3. Drag target terrain into ” Terrain” field，setup the “Terrain Layer” index ,
   this corresponds to your layer to modify, and the index starts from 0; 
   eg, you wanna modify the grass layer and it is the second layer, please set
   “Terrain Layer” to 1 ;

5. Click “Cache Layer Weights ”,  this will cache current layer weights for
   later recovery ;this is necessary because we will generate normal mask 
   randomly and overwrite the layer weights;

7. Click “ New Normal Mask ”, this will replace old layer weight with our new
   normal mask, and renormalize other layer weights accordingly ；

9. The default operation of “New Normal Mask” is “Set” , please try using Add,
   Subtraction, or Multiply Operation for variation of effects ：
      * Add : Original Weight + Normal Mask , the effect is to enhance current Layer Weight;
      * Sub : Original Weight - Normal Mask , the effect is to decrease current Layer Weight;
      * Mul: Original Weight * Normal Mask, the effect is to decrease current Layer Weight,
           but with different method ;
11. If you are not satisfied with the above options, it is necessary to generate a new Mask.
    Please remember to click “Recover Terrain Layers” , which reset your terrain to original
    state before any normal mask is generated. And then click “New Normal Mask” again;

13. If you want to export current layer weight, click”Export Layer X Mask”. This will save
    current layer weight as a gray scale .tga. This image could be adjusted in photoshop and
    act as a Biomi Mask in other terrain applications, eg. Gaia；

       ![promotion_terrain_half](https://github.com/user-attachments/assets/608056ca-1e48-4259-80f6-32f033555c44)





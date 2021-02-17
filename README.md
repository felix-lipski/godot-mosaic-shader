# godot-mosaic-shader-001
Godot VisualShader - auto-tiles and auto-rotetes the texture to avoid texture repetition

### Before shader applied:
![before](https://github.com/felix-lipski/godot-mosaic-shader-001/blob/master/demos/before.png)

### After shader applied:
![after](https://github.com/felix-lipski/godot-mosaic-shader-001/blob/master/demos/after.png)

### When used with an organic texture, this shader fixes texture repetition, but introduces new seams:
![used with an organic texture](https://github.com/felix-lipski/godot-mosaic-shader-001/blob/master/demos/organic.png)

**Very important: disable _filtering_ and _mip-mapping_ in import options of the noise texture!**

# Initial parameters:
### Noise Size: 10
### Texture Size: 1

These parameters have been tested to work for 1024x1024 textures. 
The sizes are scaled by two to the power of the inputed number, so "Noise Size: 10" means the noise texture will be scaled by 1024. 
The noise texture controls the rotation of each tile, so it should be scaled significantly higher than the tile texture.

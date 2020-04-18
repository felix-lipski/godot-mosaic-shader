# godot-mosaic-shader-001
Godot VisualShader - auto-tiles and auto-rotetes the texture to avoid texture repetition

important!: disable filtering and mip-mapping in import options of the noise texture!

initial parameters:
Noise Size: 10
Texture Size: 1

These parameters have been tested to work for 1024x1024 textures. 
The sizes are scaled by two to the power of the inputed number, so "Noise Size: 10" means the noise texture will be scaled by 1024. 
The noise texture controls the rotation of each tile, so it should be scaled significantly higher than the tile texture.

# Material Variation

> [!WARNING]
> This feature is experimental and may change in the future.

![material-variation](~/images/option-material-variation.png)  

Generates a new material by taking an existing material and applying textures on top. Any instance of the source material on the avatar will be swapped with the new material when the action is ON.

- **Material:** The source material in which you want to apply textures to.
- **Preview:** Used to preview the material changes in your scene.  This only works if the scene contains the source material.
- **Layers:** A group of textures to be applied.
	- **Name:** Name for your own organization.
	- **Opacity:** A master opacity for every texture in the layer.
	- **Mask:** A B&W mask used when applying the layer's texture.  Anything in the white portion will be applied.
	- **Textures:**
		- **Channel:** The texture channel on the shader that the texture will be applied over.
		- **Texture:** The texture drawn on top of the source material.
		- **Color:** Color which is multiplied with the source texture.
		- **Blend Mode:** How the texture is applied to the source.
			- **Normal:** Alpha blend the source onto the destination
			- **Additive:** Adds the source onto the destination
			- **Multiply:** Multiplies the source with the destination
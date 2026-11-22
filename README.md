I created this Blender extension primarily to automate pbr baking tasks and simplify uploading models for sale using the PBR workflow from Blender's Principled BSDF shader. It also automates exporting to various 3D formats and creating textures in the .blend file folder's location, also making it easier to upload textures to websites. Currently, it uses the F5 key to add a menu, but this will be customizable in the future.

Additionally, the extension's capabilities are also accessible through the N menu in the 3D Viewport. Some of these options only appear if the render engine is Cycles.

Upon installing a enabling this extension you get an F5 shortcut to access a menu with tha options:
- Multi Bake
- Create Textures Folder
- Multi Export
- Super Purge

Below I detail each option

- Multibake.
This option creates multiple bakes based on one or more principal nodes, and the resulting texture options appear in panel n. By default, these are Diffuse, Roughness, Normal, and Metalness. You can also add Ambient Occlusion, Opacity, and Emission, or remove textures you don't need. Panel n also defines the texture size, which defaults to 4096 x 4096. This can be changed, but it must always be a square texture.
You can also use selection to active
Blender will pause until it finishes making the bakes you have chosen.

- Create Textures Folder.
This option packages the textures into the .blend file and also creates a folder called textures in the directory where the .blend file is saved.

- Multi Export.
This option exports the objects in your scene in the following formats: - Alembic - FBX - Obj - Usdc - Stanford PLY. With the default options, it only saves a few clicks, but I was repeating this a lot, so I made this script.

- Super Purge.
This option deletes resources that are not being used anywhere, very useful for getting rid of orphaned resources. Unlike the normal purge, it does not ask for confirmation; use with caution.

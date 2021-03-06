wallpaper-maker
===============

Matlab code to generate 2D wallpaper patterns.

This code is based on ideas and code shared by Alasdair Clarke and used to generate displays in this paper:

Clarke, A. D. F., Green, P. R., Halley, F., & Chantler, M. J. (2011). Similar Symmetries: The Role of Wallpaper Groups in Perceptual Texture Similarity. Symmetry, 3(2), 246–264. doi:10.3390/sym3020246


## Components ##

- tile_play.m

    - This script generates a few tiles using make_tile, creates a repeating motif using make_motif. The tile_plane function is at present just a skeleton. Eventually, it will include a more generic means of tiling the plane using a set of base vectors. 

    - Start with tile_play to see what's going on.

- make_tile.m

	- Makes an elemental "tile" region that is replicated to create a wallpaper "motif"

	- Tile regions can be a centered "F" or "L" pattern or a random set of pixels. Soon to be added will be a specific image patch.
 
- make_motif.m

	- Makes a repeating wallpaper "motif" based on a series of translations, reflections, and rotations of the basic tile pattern.

    - Uses transform_tile to tranform motif. This is redundant, but may help clarify how wallpapers are synthesized.

- tile_plane.m

    - Sketch for generic tiling function. Not working.

- transform_im.m

    - Basis for transform_tile.m

- transform_tile.m

    - Affine transformations of tile.

The retro-engine provides basic construct for creating interfaces, games, monitors, in forms similar to vintage video games back to the 1980s.

The first goal is to separate logic from graphics as far as possible. Right now the primary objective of developing this engine is to cover the graphics part.

The graphic engine is designed as follows:

1. The composed frame consists of two parts:
The stationary background, and the animated foreground.
2. Background and foreground objects are all groups of tiles, meaning only pointers, or indices of sample tiles, are stored in upper-level video memories.
3. The background cannot be edited in runtime, it's a constant image stored in RO area in memory. However, a few runtime processings could be applied, such as fading out or in.
4. 
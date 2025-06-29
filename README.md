# Particle Puzzle

Particle Puzzle is a simple particle-based puzzle prototype for Unity. The project demonstrates how to configure different particle types using a JSON file and spawn them in a scene using basic physics.

## Setup
1. Open the project in Unity.
2. Create a prefab for a particle:
   - Add a `SpriteRenderer`, `Rigidbody2D` and `BoxCollider2D`.
   - Assign a small sprite (e.g., a square) to the renderer.
   - Set the prefab reference in `ParticleSpawner`.
3. Add the **ParticleManager**, **ParticleSpawner**, and **ParticleUI** scripts to objects in your scene.
   - Assign `particle_config.json` to the `ParticleManager`.
   - Assign the particle prefab and main camera to `ParticleSpawner`.
   - Create a UI `Dropdown` and connect it with `ParticleUI`.
4. Play the scene. Select a particle type from the dropdown and click in the game view to place particles. They will fall and settle on the floor using Unity's physics.

Particle properties such as color and density can be modified in `Assets/Resources/particle_config.json`.

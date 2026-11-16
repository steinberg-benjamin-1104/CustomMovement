A small Unreal Engine project demonstrating custom character movement without the CharacterMovementComponent and a basic data snapshot system for rollback netcode in fighting games. The project includes left, right, and jump keyboard inputs. This project is not currently rollback compatible, as input handling is not designed for deterministic rollback simulation. No animation system is included. Blueprint is used for demonstration purposes, but a C++ implementation is recommended for practical use. The goal is to provide a starting point for exploring custom movement and state management in Unreal Engine.

Notes:
- If you need to flip around the character to face right/left, add a boolean and rotate the mesh to be either -90 or 90 degrees on the Z axis.
- Velocity is measured in centimeters per frame of movement, and acceleration modifies that value per frame.
- If the gravity value is too high, I recommend either creating a MaxFallSpeed variable, or creating a custom fixed point Math class that acts like a float.

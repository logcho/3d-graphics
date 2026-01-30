# 3d-graphics

Notes on basic 3D graphics concepts, focused on perspective projection and minimal math needed to render 3D points onto a 2D screen.

## Coordinate System

A point in 3D space is represented as:

(x, y, z)

- x: horizontal axis
- y: vertical axis
- z: depth (distance from the camera)

Assume the camera is at the origin and looking down the +z axis.

## Perspective Projection

To project a 3D point onto a 2D plane, use perspective division:

x' = x / z  
y' = y / z

Where:
- (x, y, z) is the 3D point
- (x', y') is the projected 2D point
- z acts as a depth-based scaling factor

Objects farther away (larger z) appear smaller.

## Notes

- This is the simplest form of perspective projection.
- z must be > 0 to be visible.
- This assumes a normalized projection plane at z = 1.
- Field of view and aspect ratio are not yet considered.
- Clipping and depth buffering are not covered here.

## References

- https://www.youtube.com/watch?v=qjWkNZ0SXfo  
- https://github.com/tsoding/formula  
- https://github.com/Max-Kawula/penger-obj  
- https://www.youtube.com/watch?v=EZufiIwwqFA

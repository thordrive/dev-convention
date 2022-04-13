[[_TOC_]]

## Representing Rotations and Orientations
- Quaternion is the preferred method of representing rotations and orientations.
- Use Euler angle representation if and only if when there is need for visualization.
- When the source data(e.g. angular velocity measurement) is given as Euler angles, always convert them to Quaternions before performing numerical operations.

## Coordinate Systems for Translation and Euler angles
- Standard right-hand coordinate(https://en.wikipedia.org/wiki/Right-hand_rule) is strongly recommended.
- X axis points to the front and Z axis points upwards.
- The preferred way of Euler angle representation is Tait-Bryan angles(https://en.wikipedia.org/wiki/Euler_angles#Tait%E2%80%93Bryan_angles), commonly known as roll-pitch-yaw.
- The rotation sequence is roll(rotation around X axis) - pitch(rotation around Y axis) - yaw(rotation around Z axis)

## Units
- Recommendation: use radians for internal numerical operations, and degrees for areas of user interaction and visualization.
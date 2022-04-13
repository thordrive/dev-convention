[[_TOC_]]

## Representing Orientations
- Quaternion is the preferred method of representing orientations.
- Use Euler angle representation if and only if there is need for user interaction and visualization, such as parameter input/output and plotting of results
- When the source data(e.g. angular velocity measurement) is given as Euler angles, always convert them to Quaternions before performing numerical operations.

## Coordinate Systems for Translation and Euler angles
- Standard right-hand coordinate(https://en.wikipedia.org/wiki/Right-hand_rule) must be used.
- X axis points to the front, Y axis points to the left and Z axis points upwards.
- The preferred way of Euler angle representation is Tait-Bryan angles(https://en.wikipedia.org/wiki/Euler_angles#Tait%E2%80%93Bryan_angles), commonly known as roll-pitch-yaw.
- The rotation sequence is roll(rotation around X axis) - pitch(rotation around Y axis) - yaw(rotation around Z axis)
- These rotations are performed with respect to the reference frame(the body frame before rotation).

## Units
- Recommendation: use radians for internal numerical operations, and degrees for areas of user interaction and visualization.
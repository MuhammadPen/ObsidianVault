### planned structure
![[Pasted image 20210917130626.png]]


### Model structure
![[Pasted image 20210917130724.png]]


### Precautions

When there is a need to edit a vehicle, an external editor should be used (like blender) because we are using the wheel mesh data to calculate the wheel radius.

**If we change the wheel scale in the editor, it does not reflect the change in the wheel collider's radius, hence breaking the system.**
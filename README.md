# SoftRobotBodyDeformation-3DFEM

<p align="center">
<img src="https://user-images.githubusercontent.com/77242876/145266138-27fad527-2cef-4e40-9938-76051d32bbef.gif" width="350" height="300"/>

*In the gif, the body is subjected to sinousidal forces having an amplitude of 1N from each leg, and the dynamic body motion is recorded. Forces are assumed to be applied at each 0.5 second. Thus, the frame rate of the gif is chosen as 2.* 

## Aim of the Project

The MATLAB GUI aims to analyze a rectangular prism domain using Finite Element Method for a soft robot body. In the project, FEM is implemented to find the deformations as a result of the forces coming from the legs, while the robot moves through dynamically. The elements are 3D, namely Hexahedra with 27Nodes and Hexahedra with 8Nodes. In static analysis, it is possible to use both element types. For dynamic analysis, the element type is chosen as Hexahedra with 8 Nodes in order to allow a faster analysis.
  
## Static Analysis

For the static analysis:
- The user can create a rectangular prism domain after entering geometric entitites of the domain. use the mesh density over the thickness.
- The user could choose mesh density over the lengths. 
- The user is allowed to choose the element type whether it is Hexahedra-27Nodes or Hexahedra-8Nodes.
- The user may fix the geometry at different planes (could be fixed at XY-YZ-XZ Planes).
- The user can change the force magnitude that is applied at the tip, and can change the material properties such as Young's Modulus and Poisson Ratio. 
    
A sample screenshot from the GUI is as follows (Static Analysis with Hexahedra27 Nodes) :<img width="1439" alt="Ekran Resmi 2021-12-08 22 15 20" src="https://user-images.githubusercontent.com/77242876/145269985-5457917c-6cbd-456f-acef-9282cc49f7ef.png">

*Here, the body is fixed at the YZ Plane, an it is subjected to vertical force at the tip having a magnitude of 1N.*

## Dynamic Analysis
  
For the dynamic analysis,
  
The body is divided into 9 elements, and the element type is chosen as Hexahedra with 8 Nodes for faster analysis. 
- The element at the center is assumed to be fixed. In other words, the displacement values for the nodes at the center element is defined as zero (Dirichlet BC). 
- The body is assumed to be subjected to sinousidal forces having an amplitude of 1N from each leg. However, this can be changed by the user.  Indeed, it will be integrated with the leg forces that are obtained from the dynamic motion. 
- The user can change the material properties such as Young's Modulus and Poisson Ratio. Indeed, it will be changed with real parameters later. 
- The body deformation can be, then, recorded. 
 
The GIF that demonstrates the dynamic motion from the GUI is as follows (Dynamic Analysis with Hexahedra8 Nodes):

<p align="center">
<img src="https://user-images.githubusercontent.com/77242876/145274100-ff1e1c93-da6c-4d4c-84a8-635806a9cebb.gif" width="1400" height="500"/>


*Here, the body is fixed at center, an it is subjected to vertical forces coming from the body's legs.*

---

*The project is under development. At the moment, static analysis is achieved using Linear FEM (element type: Hexahedra with 27Nodes). Besides, initial version of the dynamic motion is achieved.

Forward Actions:
- Make the program compatible with dynamic motion (add the robot move & make compatible with the real forces coming from the legs)
- Add Non-Linearity*

---

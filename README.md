# SoftRobotBodyDeformation-3DFEM

<p align="center">
<img src="https://user-images.githubusercontent.com/77242876/145266138-27fad527-2cef-4e40-9938-76051d32bbef.gif" width="350" height="300"/>

*In the gif, the body is subjected to sinousidal forces having an amplitude of 1N from each leg, and the dynamic body motion is recorded. Forces are assumed to be applied at each 0.5 second. Thus, the frame rate of the gif is chosen as 2.* 

---

The MATLAB GUI aims to analyze a rectangular prism domain using Finite Element Method for a soft robot body. The elements are 3D, namely Hexahedra with 27Nodes and Hexahedra with 8Nodes. In static analysis, it is possible to use both element types. For dynamic analysis, the element type is chosen as Hexahedra with 8 Nodes in order to allow a faster analysis.

For the static analysis:
- The user can create a rectangular prism domain after entering geometric entitites of the domain. use the mesh density over the thickness.
- The user could choose mesh density over the lengths. 
- The user is allowed to choose the element type whether it is Hexahedra-27Nodes or Hexahedra-8Nodes.
- The user may fix the geometry at different planes (could be fixed at XY-YZ-XZ Planes).
- The user can change the force magnitude that is applied at the tip, and can change the material properties such as Young's Modulus and Poisson Ratio. 
  
After analyzing the structure, figures can be saved. 
---
A sample screenshot from the GUI is as follows (Static Analysis with Hexahedra27 Nodes) :<img width="1440" alt="Ekran Resmi 2021-11-29 21 49 57" src="https://user-images.githubusercontent.com/77242876/143926927-4856d271-808c-4328-8ccf-b4a9602054f5.png">




*Here, the body is fixed at the YZ Plane, an it is subjected to vertical force at the tip.*

----

Another sample screenshot from the GUI is as follows:
<img width="1440" alt="Ekran Resmi 2021-12-02 15 57 17" src="https://user-images.githubusercontent.com/77242876/144426963-f184ea4b-61c6-47c2-8cc9-223fdeefc7eb.png">



*Here, the body is fixed at center, an it is subjected to vertical forces coming from the body's legs.*

---

The project is under development. At the moment, static analysis is achieved using Linear FEM (element type: Hexahedra with 27Nodes). Besides, initial version of the dynamic motion is achieved.

Forward Actions:
- Make the program compatible with dynamic motion (add the robot move & make compatible with the real forces coming from the legs)
- Add Non-Linearity

---

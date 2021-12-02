# SoftRobotBodyDeformation-3DFEM
---

The project is under development. At the moment, static analysis is achieved using Linear FEM (element type: Hexahedra with 27Nodes)

Forward Actions:
- Add Hexahedra 8 Nodes - ADDED 👌
- Make the program compatible with dynamic motion
- Add Non-Linearity

---

The MATLAB GUI aims to analyze a rectangular prism domain using Finite Element Method for a soft robot body. The elements are 3D, namely Hexahedra with 27Nodes. Element type will be extended such that Hexagonal with 8Nodes will be used under dynamic motion to perform the analysis faster. 


---
A sample screenshot from the GUI is as follows:<img width="1440" alt="Ekran Resmi 2021-11-29 21 49 57" src="https://user-images.githubusercontent.com/77242876/143926927-4856d271-808c-4328-8ccf-b4a9602054f5.png">


---

Here, the body is fixed at the YZ Plane, an it is subjected to vertical force at the tip. 

----

Another sample screenshot from the GUI is as follows:
<img width="1440" alt="Ekran Resmi 2021-12-02 15 57 17" src="https://user-images.githubusercontent.com/77242876/144426963-f184ea4b-61c6-47c2-8cc9-223fdeefc7eb.png">

---

Here, the body is fixed at center, an it is subjected to vertical forces coming from the body's legs.

----

The dynamic motion (to be developed) is given below. 

![BodyMove](https://user-images.githubusercontent.com/77242876/144505747-0e9005dd-a91b-42d9-936d-9d36cb25f557.gif)


----

In the gif, the body is subjected to sinousidal forces having an amplitude of 1N from each leg, and the body motion is recorded.




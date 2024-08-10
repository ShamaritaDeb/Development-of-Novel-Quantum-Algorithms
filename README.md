# Development-of-Novel-Quantum-Algorithms
Womanium Quantum+AI 2024 Projects

**Please review the participation guidelines [here](https://github.com/womanium-quantum/Quantum-AI-2024) before starting the project.**

_**Do NOT delete/ edit the format of this read.me file.**_

_**Include all necessary information only as per the given format.**_

## Project Information:

### Team Size:
  - Maximum team size = 3
  - While individual participation is also welcome, we highly recommend team participation :)

### Eligibility:
  - All nationalities, genders, and age groups are welcome to participate in the projects.
  - All team participants must be enrolled in Womanium Quantum+AI 2024.
  - Everyone is eligible to participate in this project and win Womanium grants.
  - All successful project submissions earn the Womanium Project Certificate.
  - Best participants win Womanium QSL fellowships with Classiq. Please review the eligibility criteria for QSL fellowships in the project description below.

### Project Description:
  - Click [here](https://drive.google.com/file/d/1PGNUShboB4ik_JHZGcIPTh3KYi-aajzp/view?usp=sharing) to view the project description.

## Project Submission:
All information in this section will be considered for project submission and judging.

Ensure your repository is public and submitted by **August 9, 2024, 23:59pm US ET**.

Ensure your repository does not contain any personal or team tokens/access information to access backends. Ensure your repository does not contain any third-party intellectual property (logos, company names, copied literature, or code). Any resources used must be open source or appropriately referenced.

### Team Information:
Team Member 1:
 - Full Name: Shamarita Deb
 - Womanium Program Enrollment ID (see Welcome Email, format- WQ24-xxxxxxxxxxxxxxx): WQ24-q7KpA9fSHj9pBoo


Team Member 2:
 - Full Name: Priyabrata Bag
 - Womanium Program Enrollment ID (see Welcome Email, format- WQ24-xxxxxxxxxxxxxxx): WQ24-Vs2NEGsARrQ5VqA


Team Member 3:
 - Full Name: 
 - Womanium Program Enrollment ID (see Welcome Email, format- WQ24-xxxxxxxxxxxxxxx):


### Project Solution:
_Include a comprehensive summary of all important information about your project solution here._
All necessary code files and any additional information required to judge your project solution should be included in the repository. 

### Our project topic is "Exponential quantum speedup in simulating coupled classical oscillators"
As a first step, we have implemented the toy problem with the most non-trivial 1D coupled oscillator system with N=2 masses. We have considered mass and spring constants as identity matrices which still encode the key algorithm building blocks from the reference paper. This implementation is scalable and resource estimation regarding circuit depth and circuit width and number of 1 and 2-qubit gates. We have created a VQE algorithm to estimate the minimum energy (eigenvalue) of the Hamiltonian as well. The implementation is post-processed for the outcome using the Classiq simulator. The file for the toy problem is toyproblem.ipynb [here](https://github.com/ShamaritaDeb/Development-of-Novel-Quantum-Algorithms/blob/41cf1e63aaacec470dbe07132c8ab0e1decd3cc2/toyproblem.ipynb)

In the next step, we have enlarged the problem to add more degrees of freedom for parameter values. <br>
For mass M Parameters:<br>
    - N: Number of masses (size of the matrix NxN).<br>
    - masses: List or array of mass values for the diagonal elements.<br>
    - coupling: Optional matrix of coupling terms (off-diagonal elements). <br>
    For spring constant K parameters:<br>
    - N: Number of oscillators (masses).<br>
    - spring_constant: Default value for all internal spring constants (k<sub>1</sub>, k<sub>2</sub>, ..., k<sub>N-1</sub>).<br>
    - boundary_constant: Default value for the springs connected to the walls (k<sub>0</sub> and k<sub>N</sub>).<br>
    - custom_spring_constants: List of custom values for internal spring constants [k<sub>1</sub>, k<sub>2</sub>, ..., k<sub>N-1</sub>].<br>
    - custom_boundary_constants: List of custom values for boundary spring constants [k<sub>0</sub>, k<sub>N</sub>].<br>
    -size of the matrix is NxN<br>
    This offers us scalability and the advantage of expanding the coupled oscillator system for the desired set of mass and connecting springs. The resource estimation is done regarding circuit depth, circuit width and number of 1 and 2-qubit gates. Like the previous step, we have created a VQE algorithm to estimate the minimum energy (eigenvalue) of the Hamiltonian. The implementation is post-processed for the outcome using the Classiq simulator. The file for the complicated scenario is enlargedproblem.ipynb [here](https://github.com/ShamaritaDeb/Development-of-Novel-Quantum-Algorithms/blob/a9c95011a6ca86763cbd7678255b47e30dbc1e3a/enlargedproblem.ipynb)

### Project Presentation Deck:
_Upload/ Link a 3min. presentation deck here._

See project presentation guidelines [here](https://docs.google.com/document/d/13nWF8AxFAfFYTWEYPT3BpPdYkqtxxSAjmuXj_zcMh-E/edit?usp=sharing)


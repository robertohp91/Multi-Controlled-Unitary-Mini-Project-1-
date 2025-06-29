# multi-controlled_unitary_gates
In this repo, we construct multi-controlled gates using only cx and single-qubit gates through two methods. Both methods take as inputs three angles which implement the unitary gate $U = R_z(\phi)R_y(\theta)R_z(\gamma)$ and an integer $n>2$. 

The first method employs Corollary 4.12 from Nielsen and Chuang, wherein we construct a single-controlled U gate (CU) using only single qubit gates which are defined in terms of phi, theta, and gamma, and two cx gates. We then use this decomposition of CU and a decomposition of the Toffoli gate (ccx) into singly-controlled gates and cx to implement Figure 4.10 in Nielsen and Chuang. Though this method requires only one ancillary qubit, the number of Toffoli gates grows linearly with the number of controls for the multi-controlled gate $C^n(U)$.

Towards the end, we implement a multicontrolled unitary gate based on page 18 of 'Elementary gates for quantum computation' by Barenco et al, which uses only one ancilla in exchange of an exponential increase in the number of gates required.

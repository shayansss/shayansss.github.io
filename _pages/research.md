---
layout: archive
title: "Main Academic Research"
permalink: /research/
author_profile: true
---


## PhD Dissertation
-------
Coming soon

## MSc Thesis
---------
**Title:** Computational and Biomechanical Investigation into the Degeneration of the Main Articular Cartilage Constituents in Osteoarthritis

**Supervisory team:** Prof. Mohammad Haghpanahi and Prof. Mohammad Razi

**Full document:** This [thesis](https://shayansss.github.io/files/2017_12.pdf){:target="_blank"} is written in Persian, and therefore, for English speakers, I recommend instead the [relavant full journal paper](https://shayansss.github.io/files/2019_09_preprint.pdf){:target="_blank"}, containing most results.

### Summary

#### Introduction
It has been experimentally proposed that the discrete phases of articular cartilage (AC), along with different subchondral bone (SB) tissues, known as the bone-cartilage unit (BCU), are biomechanically altered during osteoarthritis (OA) degeneration. However, a validated computational framework capturing all of the dominant changes in multiphasic parameters has not yet been developed. This study proposed a new validated finite element (FE) BCU model, which is a combination of several well-established nonlinear, depth-dependent (heterogeneous), fibril-reinforced (anisotropic), swelling (with pre-stress) models in order to simulate all the dominant multiphasic variations in BCUs. Accordingly, the material and geometrical variations in non-advanced OA were simulated via the computational implementation of unconfined compression (UC) and indentation compression tests. Therefore, it was hypothesized that such a multiphasic degeneration simulation can provide a considerably better understanding of BCU OA.

#### Methodology
While the poroelastic constitutive equations were utilized for SBs, AC was modeled multiphysically, as follows:
${\mathbf{\sigma}^{TOT}=\mathbf{\sigma}}^{COL}+\mathbf{\sigma}^{MAT}+\mathbf{\sigma}^{GAG}-p\mathbf{I}$
Where p is the fluid pressure, I the unit tensor,\ \mathbf{\sigma}^{TOT} the total Cauchy stress, \mathbf{\sigma}^{MAT} the stress in the non-fibrillar part of the AC extracellular matrix, \mathbf{\sigma}^{COL} the tensile stress in the fibrillar collagen network, and \mathbf{\sigma}^{GAG} the osmotic pressure contribution. The anisotropic and non-homogenous collagen network, as well as the other depth-dependent material parameters, were defined through the SDVINI subroutine prior to the main analysis. Then the calculated parameters were transferred to the UMAT subroutine to implement the custom material model (Figure 1). The UC and indentation tests were simulated in Abaqus by the axisymmetric quadrilateral, bilinear displacement, and pore pressure elements to compare the multiphasic stress variations in the healthy and damage BCUs. As UMAT subroutines typically make use of Newton’s method for the sake of FE linearization, the fourth-order consistent Jacobian tensors [1] in this method were also derived.

Figure 1. Interplay between Abaqus and subroutines. Abaqus solved the FE model in three different steps: step 0 for extraction of initial coordinates, static step for pre-stress, and the other step for main OA analysis.
In order to simulate the multiphasic degeneration effects in OA, the material and geometrical properties were altered. These alterations, including the collagen softening, and the changes in the permeability and fluid fraction, together with the constitutive equations of each phase were adapted from the previous studies [2]–[6] and then incorporated into the FE BCU model, which was validated by replication of some other experimental tests with this new model. For example, an experimental compression test [7] was replicated, representing the model accuracy (Figure 2). Moreover, to study the possible fibrillar abnormalities during OA, the influence of the fibrillation and fibrillar rotation were simulated by randomizing the fibrillar directions [8] and rotating the split-lines in upper AC layers, respectively (Figure 3).
 
Figure 2. Validation stress-strain plots, measured from a confined compression test, proposed by Schinagl et al. [5] and replicated by Wilson et al. [2], in terms of (a) constituent stresses and (b) total stresses in AC upper layers.
 
Figure 3. Split line patterns on the AC surface (left) and primary fibril directions by the arcade-like structure [9] with considering split line torsions or rotations θ (redrawn from [10] and [11]).

#### Results
The main results shed light on the significant biomechanical role of the fluid and osmotic pressure parameters plus the calcified cartilage stress variations (Figure 4), along with the insignificant role of minor fibrillar abnormalities in load sharings of the SBs during OA (Figure 5). Furthermore, in agreement with some experimental observations [12], [13], the indentation simulation put the emphasis on the importance of the mass transport in SBs (Figure 6). Interestingly, the degeneration severely reduced the fluid permeation through SBs so that only a small amount of the fluid could flow into the subchondral trabecular bone in contrast to the healthy BCU, where the fluid could flow through the whole SB tissues. This result would have been completely different if the FE model had only simulated the permeability alterations [3], indicating the importance of the multiphasic degeneration simulation and consequently confirming the hypothesis. In conclusion, this study demonstrates the importance of multiphasic simulation of OA in BCUs and support the notion that SBs might play a role in the pathogenesis of OA.
 	 
 	 
Figure 4. Contributions of BCU parts at peak loads of (left) UC and (right) indentation tests. The recorded data of intact AC phases are in conformity with the recent study [14], which indirectly verified the model fidelity.
 	 
Figure 5. Simulation of fibrillar abnormalities, including (left) fibrillations, which only affected the AC upper layers, and (right) fibrillar rotations (torsions), which slightly altered the elasticity of BCUs. Also, the mesh-refinement study verified the numerical accuracy.
 
Figure 6. Indentation simulation results for pore (fluid) pressure and (effective) fluid velocity at peak load.

#### References
[1]	N. Nguyen and A. M. Waas, “Nonlinear, finite deformation, finite element analysis,” Zeitschrift für Angew. Math. und Phys., vol. 67, no. 3, p. 35, 2016.
[2]	W. Wilson, J. M. Huyghe, and C. C. Van Donkelaar, “Depth-dependent Compressive Equilibrium Properties of Articular Cartilage Explained by its Composition,” Biomech. Model. Mechanobiol., vol. 6, no. 1–2, pp. 43–53, Jan. 2007.
[3]	M. E. Stender, R. A. Regueiro, and V. L. Ferguson, “A poroelastic finite element model of the bone–cartilage unit to determine the effects of changes in permeability with osteoarthritis,” Comput. Methods Biomech. Biomed. Engin., pp. 1–13, Sep. 2016.
[4]	M. Taffetani, M. Griebel, D. Gastaldi, S. M. Klisch, and P. Vena, “Poroviscoelastic finite element model including continuous fiber distribution for the simulation of nanoindentation tests on articular cartilage,” J. Mech. Behav. Biomed. Mater., vol. 32, pp. 17–30, 2014.
[5]	M. E. Mononen, P. Julkunen, J. Töyräs, J. S. Jurvelin, I. Kiviranta, and R. K. Korhonen, “Alterations in structure and properties of collagen network of osteoarthritic and repaired cartilage modify knee joint stresses,” Biomech. Model. Mechanobiol., vol. 10, no. 3, pp. 357–369, 2011.
[6]	W. Wilson, J. M. M. Huyghe, and C. C. C. van Donkelaar, “A composition-based cartilage model for the assessment of compositional changes during cartilage damage and adaptation,” Osteoarthr. Cartil., vol. 14, no. 6, pp. 554–560, 2006.
[7]	R. M. Schinagl, D. Gurskis, A. C. Chen, and R. L. Sah, “Depth-dependent confined compression modulus of full-thickness bovine articular cartilage,” J. Orthop. Res., vol. 15, no. 4, pp. 499–506, 1997.
[8]	M. E. Mononen, M. T. Mikkola, P. Julkunen, R. Ojala, M. T. Nieminen, J. S. Jurvelin, and R. K. Korhonen, “Effect of superficial collagen patterns and fibrillation of femoral articular cartilage on knee joint mechanics-A 3D finite element analysis,” J. Biomech., vol. 45, no. 3, pp. 579–587, 2012.
[9]	A. Benninghoff, “Form und Bau der Gelenkknorpel in ihren Beziehungen zur Funktion,” Z. Anat. Entwicklungsgesch., vol. 76, no. 1–3, pp. 43–63, 1925.
[10]	W. Wilson, C. C. van Donkelaar, B. van Rietbergen, K. Ito, and R. Huiskes, “Stresses in the local collagen network of articular cartilage: a poroviscoelastic fibril-reinforced finite element study.,” J. Biomech., vol. 37, no. 3, pp. 357–66, Mar. 2004.
[11]	S. Below, S. P. Arnoczky, J. Dodds, C. Kooima, and N. Walter, “The split-line pattern of the distal femur: A consideration in the orientation of autologous cartilage grafts,” Arthroscopy, vol. 18, no. 6, pp. 613–617, 2002.
[12]	J. Hwang, W. C. Bae, W. Shieu, C. W. Lewis, W. D. Bugbee, and R. L. Sah, “Increased hydraulic conductance of human articular cartilage and subchondral bone plate with progression of osteoarthritis.,” Arthritis Rheum., vol. 58, no. 12, pp. 3831–42, Dec. 2008.
[13]	J. Pan, X. Zhou, W. Li, J. E. Novotny, S. B. Doty, and L. Wang, “In situ measurement of transport between subchondral bone and articular cartilage,” J. Orthop. Res., vol. 27, no. 10, pp. 1347–1352, Oct. 2009.
[14]	J. M. P. P. Quiroga, W. Wilson, K. Ito, and C. C. van Donkelaar, “Relative contribution of articular cartilage’s constitutive components to load support depending on strain rate,” Biomech. Model. Mechanobiol., vol. 16, no. 1, pp. 151–158, Jul. 2017.
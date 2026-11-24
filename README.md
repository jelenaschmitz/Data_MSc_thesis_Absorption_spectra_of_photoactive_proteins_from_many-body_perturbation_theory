# Data_MSc_thesis_Absorption_spectra_of_photoactive_proteins_from_many-body_perturbation_theory
Data supporting the plots in the master's thesis, 'Absorption spectra of photoactive proteins from many-body perturbation theory', based on CP2K calculations performed on Noctua2 in Paderborn.

The folders are structured as follows:
- Link_atom_bond_length: Contains results for variations in the bond length distance of the hydrogen link atom from the carbon of the QM region. '-1' or '20' in the subfolder names specifies the energy cutoff for occupied and unoccupied orbitals. '1_11', '1_13',... give the bond distance of H to C in angstrom.
- '6YMU_protein_background_inclusion_tests':
  - 'Gas_phase_spectrum': contains the CP2K GW+BSE result on the gas phase of the QM region of the protein.
  - 'Convergence_over_counter_charge_distance': Contains the results for different Poisson solvers and with countered created monopole and/or dipole in the system. '3_10_10_10_10_3' stands for a cell with 3 angstrom to the counter charge, the 10 angstrom to the system box, which is another 10 angstrom to the centre, and therefore in total 20 angstrom wide.
  - 'Convergence_over_box_size_structure_1_M_0' : Contains the convergence results for different sizes of the system from the centre, l_box (the QM region+partial charges), for different basis sets and Poisson solver. Here, only the monopole in the system is countered.
  - 'Convergence_over_box_size_structure_1_2_4_and_spectra' : Contains the convergence results for different sizes of the system from the centre, l_box (the QM region+partial charges), for different basis sets and Poisson solver and QM regions (structure 1 is everything that is not marked structure 2 or 4). Here, monopole and dipole in the system is countered.


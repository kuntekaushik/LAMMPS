## 1D binning number density/mass density format
compute compute_ID group_ID chunk/atom bin/1d z <lower> <width> region <regionID> units box
fix fix_ID group_ID ave/chunk Nevery Nrepeat Nfreq compute_ID density/number ave one file <filename>

## Adding charge density calculator in LAMMPS commands
compute CHARGE all property/atom q
compute CHUNK_XBIN_ALL all chunk/atom bin/1d z -51.99 0.02 
fix CHARGE_DENSITY_FIX all ave/chunk 1000 1 1000 CHUNK_XBIN_ALL c_CHARGE file out.charge_density

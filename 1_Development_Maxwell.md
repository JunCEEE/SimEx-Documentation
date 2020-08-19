## 1. Necessary environment
- Conda environment
```
conda activate simex-branch 
```

- ifort
```
module load intel.2020
```
- Intel MKL 
```
source `which compilervars.sh` intel64
```
- xraydb
```
pip install xraydb
```
- Turn off Geant4
Put `XCSIT=OFF` in the develop mode section

- CMake 3.12 is required
```
module load exfel cmake
```

- `recon_dm` cannot find `-liomp5`
```
make VERBOSE=1
```
to see the full command output

Problem:
```
gcc -O3 object_recon.c -o object_recon -m64 -I/opt/intel/2020/compilers_and_libraries/linux/mkl/include -I/opt/intel/2020/compilers_and_libraries/linux/mkl/include/fftw -Wl,--no-as-needed -L/opt/intel/2020/compilers_and_libraries/linux/mkl/lib/intel64 -lmkl_intel_lp64 -lmkl_core -lmkl_sequential -liomp5 -lpthread -lm -ldl
```
Solution:
```
source `which compilervars.sh` intel64
```

- Documentation Generation
```
pip install sphinx-rtd-theme
```

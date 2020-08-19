```bash
├── CMake
│   ├── FindFFTW.cmake
│   ├── FindGSL.cmake
│   ├── FindMKL.cmake
│   ├── FindPythonLibs.cmake
│   ├── FindPythonModules.cmake
│   ├── FindSphinx.cmake
│   └── find_modules.cmake
├── CMakeLists.txt
├── COPYING
├── Changelog.rst
├── Docker
│   ├── 3rdparty
│   │   ├── Dockerfile
│   │   ├── build_image
│   │   └── python_install.sh
│   ├── centos_mpi
│   │   ├── Dockerfile
│   │   ├── build_image
│   │   └── openmpi_install.sh
│   ├── simex
│   │   ├── Dockerfile
│   │   ├── build_image
│   │   ├── python_install.sh
│   │   └── simex_install.sh
│   └── simex_devel
│       ├── Dockerfile
│       ├── build_image_develop
│       └── simex_install_devel.sh
├── Modules
│   ├── Analyzers
│   │   ├── S2EReconstruction_DM
│   │   │   ├── CMakeLists.txt
│   │   │   └── makefile_DM
│   │   └── S2EReconstruction_EMC
│   │       └── CMakeLists.txt
│   ├── Detectors
│   │   └── XCSITPhotonDetector
│   │       └── CMakeLists.txt
│   ├── Diffractors
│   │   ├── CrystFELPhotonDiffractor
│   │   │   └── CMakeLists.txt
│   │   ├── GAPDPhotonDiffractor
│   │   │   ├── CMakeLists.txt
│   │   │   └── GAPD.zip
│   │   └── SingFELPhotonDiffractor
│   │       └── CMakeLists.txt
│   ├── Others
│   │   └── s2e
│   │       ├── CMakeLists.txt
│   │       └── pmi_demo.py.patch
│   ├── PhotonInteractors
│   │   └── FEFFPhotonInteractor
│   │       └── CMakeLists.txt
│   ├── Propagators
│   │   └── XFELPhotonPropagator
│   │       └── wpg
│   │           ├── CMakeLists.txt
│   │           ├── Makefile.patch
│   │           ├── genesis.py.patch
│   │           └── glossary.py.patch
│   └── Sources
│       └── GenesisPhotonSource
│           └── CMakeLists.txt
├── Packages
│   ├── CMakeLists.txt
│   └── postinst
├── README.md
├── Sources
│   ├── CMakeLists.txt
│   ├── doc
│   │   ├── CMakeLists.txt
│   │   ├── Makefile
│   │   ├── build
│   │   │   ├── doctrees
│   │   │   │   ├── environment.pickle
│   │   │   │   ├── include
│   │   │   │   └── index.doctree
│   │   │   └── html
│   │   │       ├── _sources
│   │   │       ├── _static
│   │   │       ├── genindex.html
│   │   │       ├── include
│   │   │       ├── index.html
│   │   │       ├── objects.inv
│   │   │       ├── search.html
│   │   │       └── searchindex.js
│   │   └── source
│   │       ├── Tutorial
│   │       │   ├── radhydroPlot.png
│   │       │   ├── s2e_example
│   │       │   ├── xrts
│   │       │   └── xstal_diffr
│   │       ├── conf.py
│   │       ├── include
│   │       │   ├── acknowledgements.rst
│   │       │   ├── contribute.rst
│   │       │   ├── data_formats.rst
│   │       │   ├── environment.rst
│   │       │   ├── installation.rst
│   │       │   ├── introduction.rst
│   │       │   ├── license.rst
│   │       │   ├── refman.rst
│   │       │   ├── support.rst
│   │       │   ├── testing.rst
│   │       │   └── usage.rst
│   │       ├── index.rst
│   │       └── resources
│   │           └── eucall_logo_print_transparent.png
│   └── python
│       ├── ScriptCollection
│       │   ├── Converters
│       │   │   └── pic2dist.py
│       │   ├── DataAnalysis
│       │   │   ├── __init__.py
│       │   │   ├── emc
│       │   │   ├── pmi
│       │   │   ├── propagation
│       │   │   └── scattering
│       │   ├── Prototypes
│       │   │   ├── __init__.py
│       │   │   └── pic2genesis
│       │   ├── SimExScripts
│       │   │   ├── RadHydroXRTS.py
│       │   │   ├── __init__.py
│       │   │   └── simex_script.py
│       │   └── __init__.py
│       ├── SimEx
│       │   ├── AbstractBaseClass.py
│       │   ├── Analysis
│       │   │   ├── AbstractAnalysis.py
│       │   │   ├── DiffractionAnalysis.py
│       │   │   ├── XFELPhotonAnalysis.py
│       │   │   ├── XMDYNPhotonMatterAnalysis.py
│       │   │   └── __init__.py
│       │   ├── CLI
│       │   │   ├── __init__.py
│       │   │   ├── commands
│       │   │   ├── simex.py
│       │   │   └── utilities
│       │   ├── Calculators
│       │   │   ├── AbstractBaseCalculator.py
│       │   │   ├── AbstractIonInteractor.py
│       │   │   ├── AbstractPhotonAnalyzer.py
│       │   │   ├── AbstractPhotonDetector.py
│       │   │   ├── AbstractPhotonDiffractor.py
│       │   │   ├── AbstractPhotonInteractor.py
│       │   │   ├── AbstractPhotonPropagator.py
│       │   │   ├── AbstractPhotonSource.py
│       │   │   ├── CalculatorClasses
│       │   │   ├── CalculatorUtilities
│       │   │   ├── ComptonScatteringCalculator.py
│       │   │   ├── CrystFELPhotonDiffractor.py
│       │   │   ├── DMPhasing.py
│       │   │   ├── EMCCaseGenerator.py
│       │   │   ├── EMCOrientation.py
│       │   │   ├── EstherPhotonMatterInteractor.py
│       │   │   ├── FEFFPhotonMatterInteractor.py
│       │   │   ├── GaussianPhotonSource.py
│       │   │   ├── GenesisPhotonSource.py
│       │   │   ├── IdealPhotonDetector.py
│       │   │   ├── PlasmaXRTSCalculator.py
│       │   │   ├── RegisteredCalculators
│       │   │   ├── S2EReconstruction.py
│       │   │   ├── SingFELPhotonDiffractor.py
│       │   │   ├── TNSAIonMatterInteractor.py
│       │   │   ├── XCSITPhotonDetector.py
│       │   │   ├── XFELPhotonPropagator.py
│       │   │   ├── XFELPhotonSource.py
│       │   │   ├── XMDYNDemoPhotonMatterInteractor.py
│       │   │   ├── XMDYNPhotonMatterInteractor.py
│       │   │   └── __init__.py
│       │   ├── Parameters
│       │   │   ├── AbstractCalculatorParameters.py
│       │   │   ├── AbstractPhotonDiffractorParameters.py
│       │   │   ├── CrystFELPhotonDiffractorParameters.py
│       │   │   ├── DMPhasingParameters.py
│       │   │   ├── DetectorGeometry.py
│       │   │   ├── EMCOrientationParameters.py
│       │   │   ├── EstherPhotonMatterInteractorParameters.py
│       │   │   ├── FEFFPhotonMatterInteractorParameters.py
│       │   │   ├── GaussWavefrontParameters.py
│       │   │   ├── IonMatterInteractorParameters.py
│       │   │   ├── PhotonBeamParameters.py
│       │   │   ├── PhotonMatterInteractorParameters.py
│       │   │   ├── PlasmaXRTSCalculatorParameters.py
│       │   │   ├── SingFELPhotonDiffractorParameters.py
│       │   │   ├── WavePropagatorParameters.py
│       │   │   ├── XCSITPhotonDetectorParameters.py
│       │   │   └── __init__.py
│       │   ├── PhotonExperimentSimulation
│       │   │   ├── EstherExperiment.py
│       │   │   ├── PhotonExperimentSimulation.py
│       │   │   └── __init__.py
│       │   ├── Submitters
│       │   │   ├── Demo.ipynb
│       │   │   └── SimExSLURM.py
│       │   ├── Templates
│       │   │   └── main.py
│       │   ├── Utilities
│       │   │   ├── DebugTools.py
│       │   │   ├── EntityChecks.py
│       │   │   ├── IOUtilities.py
│       │   │   ├── IntensityCalc.py
│       │   │   ├── Nickel.txt
│       │   │   ├── OpenPMDTools.py
│       │   │   ├── ParallelUtilities.py
│       │   │   ├── RadHydroAnalysis.py
│       │   │   ├── RadHydroInputPlots.py
│       │   │   ├── Units.py
│       │   │   ├── Utilities.py
│       │   │   ├── WPGBeamlines.py
│       │   │   ├── __init__.py
│       │   │   ├── checkOpenPMD_h5.py
│       │   │   ├── hydro_txt_to_opmd.py
│       │   │   ├── mirror1.dat
│       │   │   ├── mirror2.dat
│       │   │   ├── sample2h5.py
│       │   │   ├── sase1.py
│       │   │   ├── shadow_to_opmd.py
│       │   │   ├── wpg2prop.py
│       │   │   ├── wpg_to_opmd.py
│       │   │   ├── xmdyn_to_opmd.py
│       │   │   ├── xpdb.py
│       │   │   └── xyz2sample.py
│       │   ├── __init__.py
│       │   ├── __pycache__
│       │   │   ├── __init__.cpython-36.pyc
│       │   │   └── version.cpython-36.pyc
│       │   └── version.py
│       ├── extra
│       │   └── CMakeLists.txt
│       └── setup.py
├── Tests
│   ├── CMakeLists.txt
│   ├── doc
│   │   └── Test.py
│   └── python
│       ├── functest
│       │   ├── SimExTest
│       │   │   ├── Backengines
│       │   │   └── __init__.py
│       │   ├── Test.py
│       │   ├── TestFiles -> ../unittest/TestFiles
│       │   ├── TestUtilities -> ../unittest/TestUtilities/
│       │   ├── __init__.py
│       │   └── paths.py -> ../paths.origin.py
│       └── unittest
│           ├── SimExTest
│           │   ├── Analysis
│           │   ├── Calculators
│           │   ├── Parameters
│           │   ├── PhotonExperimentSimulation
│           │   ├── Utilities
│           │   └── __init__.py
│           ├── Test.py
│           ├── TestFiles
│           │   ├── 0010.sdf
│           │   └── D_D_-_3He_n.txt
│           ├── TestUtilities
│           │   ├── TestUtilities.py
│           │   └── __init__.py
│           ├── __init__.py
│           └── testscript.py
├── TravisCI
│   ├── build_and_test_simex.sh
│   ├── deploy_docs.sh
│   ├── key
│   ├── pyqt.sh
│   └── trigger_docker.sh
├── conda-requirements.yml
├── copyright_notice.py
├── environment.yml
├── get_testdata.sh
├── install.sh
├── patch_for_maxwell
├── requirements.txt
├── simex.in
├── simex_dev.in
├── simex_vars.sh.in
└── simex_vars_dev.sh.in

87 directories, 194 files
```

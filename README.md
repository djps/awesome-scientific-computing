# Awesome Scientific Computing

[![Check Markdown links](https://github.com/djps/awesome-scientific-computing/actions/workflows/check-links.yml/badge.svg)](https://github.com/djps/awesome-scientific-computing/actions/workflows/check-links.yml)

[<img src="https://nschloe.github.io/awesome-scientific-computing/sunglasses.svg" align="right" width="25%">](#readme)

> Useful resources for scientific computing and numerical analysis, with a selection of ultrasound tools

Scientific computing and numerical analysis are research fields that aim to provide
methods for solving large-scale problems from various areas of science with the help of
computers. Typical problems are ordinary and partial differential equations (ODEs,
PDEs), their discretizations, and the solution of linear algebra problems arising from
them.

## Contents

- [Basic linear algebra](#basic-linear-algebra)
- [Multi-purpose toolkits](#multi-purpose-toolkits)
- [Finite Elements](#finite-elements)
- [Meshing](#meshing)
- [Data formats](#data-formats)
- [Sparse linear solvers](#sparse-linear-solvers)
- [Visualization](#visualization)
- [Platforms](#platforms)
- [I/O](#io)
- [ODEs](#odes)
- [GPUs](#gpus)
- [Solvers](#solvers)
- [Wave propagation](#wave-propagation)
- [Physics-informed neural networks](#physics-informed-neural-networks)
- [SBML](#sbml)
- [Resources](#resources)
- [Other libraries and tools](#other-libraries-and-tools)
- [Community](#community)


## Basic linear algebra

- [BLAS](https://netlib.org/blas/) - Standard building blocks for performing basic vector and matrix operations.
  (Fortran, public domain, [GitHub](https://github.com/Reference-LAPACK/lapack/tree/master/BLAS))
- [OpenBLAS](https://www.openblas.net) - Optimized BLAS library based on GotoBLAS2.
  (C and Assembly, BSD, [GitHub](https://github.com/xianyi/OpenBLAS))
- [BLIS](https://github.com/flame/blis) - High-performance BLAS-like dense linear algebra libraries.
  (C, BSD, GitHub)
- [LAPACK](https://netlib.org/lapack/) - Routines for solving systems of linear equations, linear least-squares, eigenvalue problems, etc.
  (Fortran, BSD, [GitHub](https://github.com/Reference-LAPACK/lapack))
<!-- markdown-link-check-disable -->
- [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page) - C++ template library for linear algebra.
  (C++, MPL 2, [GitLab](https://gitlab.com/libeigen/eigen))
- [Ginkgo](https://ginkgo-project.github.io/) - High-performance manycore linear algebra library, focus on sparse systems.
  (C++, BSD, [GitHub](https://github.com/ginkgo-project/ginkgo))
- [blaze](https://bitbucket.org/blaze-lib/blaze) - High-performance C++ math library for dense and sparse arithmetic.
  (C++, BSD, Bitbucket)

## Multi-purpose toolkits

- [PETSc](https://www.mcs.anl.gov/petsc/) - Parallel solution of scientific applications modeled by PDEs.
  (C, 2-clause BSD, [GitLab](https://gitlab.com/petsc/petsc))
- [DUNE Numerics](https://www.dune-project.org) - Toolbox for solving PDEs with grid-based methods.
  (C++, GPL 2, [GitLab](https://gitlab.dune-project.org/core/))
- [SciPy](https://scipy.org) - Python modules for statistics, optimization, integration, linear algebra, etc.
  (Python, mostly BSD, [GitHub](https://github.com/scipy/scipy/))
- [NumPy](https://numpy.org/) - Fundamental package needed for scientific computing with Python.
  (Python, BSD, [GitHub](https://github.com/numpy/numpy))
- [DifferentialEquations.jl](https://diffeq.sciml.ai/) - Toolbox for solving different types of differential equations numerically. (Julia, MIT, [GitHub](https://github.com/SciML/DifferentialEquations.jl))

## Finite Elements

- [FEniCS](https://fenicsproject.org) - Computing platform for solving PDEs in Python and C++.
  (C++/Python, LGPL 3, [GitHub](https://github.com/FEniCS)/[Bitbucket](https://bitbucket.org/fenics-project/))
- [libMesh](https://libmesh.github.io) - Framework for the numerical simulation of PDEs using unstructured discretizations.
  (C++, LGPL 2.1, [GitHub](https://github.com/libMesh/libmesh))
- [deal.II](https://dealii.org) - Software library supporting the creation of finite element codes.
  (C++, LGPL 2.1, [GitHub](https://github.com/dealii/dealii))
- [Netgen/NGSolve](https://ngsolve.org) - High performance multiphysics finite element software.
  (C++, LGPL 2.1, [GitHub](https://github.com/NGSolve/netgen))
- [Firedrake](https://www.firedrakeproject.org) - Automated system for the solution of PDEs using the finite element method.
  (Python, LGPL 3, [GitHub](https://github.com/firedrakeproject/firedrake))
- [MOOSE](https://mooseframework.inl.gov/) - Multiphysics Object Oriented Simulation Environment.
  (C++, LGPL 2.1, [GitHub](https://github.com/idaholab/moose))
- [MFEM](https://mfem.org) - Free, lightweight, scalable C++ library for finite element methods.
  (C++, BSD-3-Clause, [GitHub](https://github.com/mfem/mfem))
- [SfePy](https://sfepy.org) - Simple Finite Elements in Python.
  (Python, BSD, [GitHub](https://github.com/sfepy/sfepy))
- [FreeFEM](https://freefem.org) - High level multiphysics-multimesh finite element language.
  (C++, LGPL, [GitHub](https://github.com/FreeFem))
- [libceed](https://libceed.readthedocs.io/en/latest/index.html) - Code for Efficient Extensible Discretizations.
  (C, 2-clause BSD, [GitHub](https://github.com/CEED/libCEED))
- [scikit-fem](https://github.com/kinnala/scikit-fem) - Simple finite element assemblers.
  (Python, BSD/GPL, GitHub)

## Meshing

### Triangular and tetrahedral meshing

- [Gmsh](https://gmsh.info) - Three-dimensional finite element mesh generator with pre- and post-processing facilities.
  (C++, GPL, [GitLab](https://gitlab.onelab.info/gmsh/gmsh))
- [pygmsh](https://github.com/nschloe/pygmsh) - Python interface for Gmsh.
  (Python, GPL 3, GitHub)
- [MeshPy](https://mathema.tician.de/software/meshpy/) - Quality triangular and tetrahedral mesh generation.
  (Python, MIT, [GitHub](https://github.com/inducer/meshpy))
- [CGAL](https://www.cgal.org) - Algorithms for computational geometry.
  (C++, mixed LGPL/GPL, [GitHub](https://github.com/CGAL/cgal))
- [pygalmesh](https://github.com/meshpro/pygalmesh) - Python interface for CGAL's 3D meshing capabilities.
  (Python, GPL 3, GitHub)
- [TetGen](https://www.wias-berlin.de/software/index.jsp?id=TetGen) - Quality tetrahedral mesh generator and 3D Delaunay triangulator.
  (C++, AGPLv3)
- [Triangle](https://www.cs.cmu.edu/~quake/triangle.html) - Two-dimensional quality mesh generator and Delaunay triangulator.
  (C, _nonfree software_)
- [distmesh](http://persson.berkeley.edu/distmesh/) - Simple generator for unstructured triangular and tetrahedral meshes.
  (MATLAB, GPL 3)
- [trimesh](https://trimsh.org/) - Loading and using triangular meshes with an emphasis on watertight surfaces.
  (Python, MIT, [GitHub](https://github.com/mikedh/trimesh))
- [dmsh](https://github.com/meshpro/dmsh) - Simple generator for unstructured triangular meshes, inspired by distmesh.
  (Python, proprietary, GitHub)
- [TetWild](https://yixin-hu.github.io/tetwild.pdf) - Generate tetrahedral meshes for triangular surface meshes.
  (C++, GPL 3, [GitHub](https://github.com/Yixin-Hu/TetWild))
- [TriWild](https://cims.nyu.edu/gcl/papers/2019-TriWild.pdf) - Robust triangulation with curve constraints.
  (C++, MPL 2, [GitHub](https://github.com/wildmeshing/TriWild))
- [fTetWild](https://arxiv.org/abs/1908.03581) - Same as TetWild, but faster.
  (C++, MPL 2, [GitHub](https://github.com/wildmeshing/fTetWild))
- [SeismicMesh](https://github.com/krober10nd/SeismicMesh) - Parallel 2D/3D triangle/tetrahedral mesh generation with sliver removal.
  (Python and C++, GPL 3, GitHub)

### Quadrilateral and hexahedral meshing

- [QuadriFlow](https://stanford.edu/~jingweih/papers/quadriflow/) - Scalable and robust quadrangulation from triangulation.
  (C++, BSD, [GitHub](https://github.com/hjwdzh/QuadriFlow))

### Mesh tools

- [meshio](https://github.com/nschloe/meshio) - I/O for various mesh formats, file conversion.
  (Python, MIT, GitHub)
- [MOAB](https://sigma.mcs.anl.gov/moab-library/) - Representing and evaluating mesh data.
  (C++, mostly LGPL 3, [Bitbucket](https://bitbucket.org/fathomteam/moab/))
- [optimesh](https://github.com/meshpro/optimesh) - Triangular mesh smoothing.
  (Python, proprietary, GitHub)
- [pmp-library](https://www.pmp-library.org/) - Polygon mesh processing library.
  (C++, MIT with Employer Disclaimer, [GitHub](https://github.com/pmp-library/pmp-library/))
- [Mmg](https://www.mmgtools.org/) - Robust, open-source & multidisciplinary software for remeshing.
  (C, LGPL 3, [GitHub](https://github.com/MmgTools/mmg))
- [meshplex](https://github.com/meshpro/meshplex) - Fast tools for simplex meshes.
  (Python, proprietary, GitHub)

## Data formats

- [NetCDF](https://www.unidata.ucar.edu/software/netcdf/) - Software libraries and data formats for array-oriented scientific data.
  (C/C++/Fortran/Java/Python, [custom open-source
  license](https://www.unidata.ucar.edu/software/netcdf/copyright.html),
  [GitHub](https://github.com/Unidata/netcdf-c/))
- [HDF5](https://support.hdfgroup.org/HDF5/) - Data model, library, and file format for storing and managing data.
  (C/Fortran, BSD, [GitHub](https://github.com/HDFGroup/hdf5))
- [XDMF](https://xdmf.org/index.php/Main_Page) - eXtensible Data Model and Format for data from High Performance Computing codes.
  (C++, [GitLab](https://gitlab.kitware.com/xdmf/xdmf))
- [Zarr](https://zarr.readthedocs.io/en/stable/) - Format for the storage of chunked, compressed, N-dimensional arrays.
  (Python, MIT, [GitHub](https://github.com/zarr-developers/zarr-python))

## Sparse linear solvers

- [SuperLU](https://portal.nersc.gov/project/sparse/superlu/) - Direct solution of large, sparse, nonsymmetric systems of linear equations.
  (C, mostly BSD, [GitHub](https://github.com/xiaoyeli/superlu))
- [PyAMG](https://pyamg.readthedocs.io/en/latest/) - Algebraic Multigrid Solvers in Python.
  (Python, MIT, [GitHub](https://github.com/pyamg/pyamg))
- [hypre](https://computing.llnl.gov/projects/hypre-scalable-linear-solvers-multigrid-methods) - Library of high-performance preconditioners and solvers.
  (C, Apache 2.0/MIT, [GitHub](https://github.com/hypre-space/hypre))

## Visualization

- [ParaView](https://www.paraview.org) - Multi-platform data analysis and visualization application based on VTK.
  (C++, BSD, [GitLab](https://gitlab.kitware.com/paraview/paraview))
- [VTK](https://vtk.org/) - Process images and create 3D computer graphics.
  (C++, BSD, [GitLab](https://gitlab.kitware.com/vtk/vtk))
- [Mayavi](https://docs.enthought.com/mayavi/mayavi/) - 3D scientific data visualization and plotting in Python.
  (Python, BSD, [GitHub](https://github.com/enthought/mayavi))
- [Polyscope](https://polyscope.run/) - Viewer and user interface for 3D geometry processing.
  (C++, MIT, [GitHub](https://github.com/nmwsharp/polyscope))
- [PyVista](https://docs.pyvista.org/) - 3D plotting and mesh analysis through a streamlined interface for VTK.
  (Python, MIT, [GitHub](https://github.com/pyvista/pyvista))
- [vedo](https://vedo.embl.es/) - Library for scientific analysis and visualization of 3D objects based on VTK.
  (Python, MIT, [GitHub](https://github.com/marcomusy/vedo))
- [yt](https://yt-project.org/) - Toolkit for analysis and visualization of volumetric data.
  (Python, BSD, [GitHub](https://github.com/yt-project/yt))
- [F3D](https://f3d.app/) - Cross-platform, fast, and minimalist 3D viewer with scientific visualization tools.
  (C++, BSD, [GitHub](https://github.com/f3d-app/f3d))
- [TTK](https://topology-tool-kit.github.io/) - Topological data analysis and visualization.
  (C++/Python, BSD, [GitHub](https://github.com/topology-tool-kit/ttk))
- [morphologica](https://github.com/ABRG-Models/morphologica) - Header-only, modern OpenGL code to visualize numerical simulations at runtime. (C++, Apache 2.0, GitHub)

----

## Medical image computing

- [ITK](https://itk.org/) - Spatially-oriented architecture for processing, segmentation, and registration of scientific images in two, three, or more dimensions. (C++, Apache-2, [GitHub](https://github.com/InsightSoftwareConsortium/ITK))
- [MITK](https://www.mitk.org/wiki/The_Medical_Imaging_Interaction_Toolkit_(MITK)) - Software for the development of interactive medical image processing software (C++, BSD-3-clause, [GitHub](https://github.com/MITK/MITK))
- [DicomToMesh](https://github.com/AOT-AG/DicomToMesh) - converts DICOM to an stl
- [SimVascular](http://simvascular.github.io/index.html) - Simulations on vessels (C++, GNU, [GitHub](https://github.com/SimVascular/SimVascular))
- [vmkt](http://vmtk.org/) - Vascular modelling toolkit (C/C++, BSD, [GitHub](https://github.com/vmtk/vmtk))
- [FeBio](https://febio.org/) finite elements for biological tissue (C++, MIT, [GitHub](https://github.com/febiosoftware/FEBio))
- [Iso2Mesh](https://iso2mesh.sourceforge.net/cgi-bin/index.cgi) - a 3D surface and volumetric mesh generator for MATLAB/Octave (Matlab, GPL, [GitHub](https://github.com/fangq/iso2mesh))

## Platforms

- [Slicer3D](https://www.slicer.org/) - Visualization, processing, segmentation, registration, and analysis of medical, biomedical, and other 3D images and meshes; and planning and navigating image-guided procedures. (C++, BSD-like, [GitHub](https://github.com/Slicer/Slicer))
  - [SlicerIGT](https://www.slicerigt.org/wp/) - Modules supporting image-guided interventions in 3D Slicer. (C++, BSD-3-clause, [GitHub](https://github.com/SlicerIGT))
- MITK Workbench - platform for MITK.

## I/O

- [rapidxml](https://rapidxml.sourceforge.net/) - handling of xml in C++ (C++, SourceForge)
- [Boost Property Tree](https://www.boost.org/doc/libs/1_81_0/doc/html/property_tree.html) - provides a data structure that stores an arbitrarily deeply nested tree of values, indexed at each level by some key (C++, Boost, [GitHub](https://github.com/boostorg/property_tree))
- [json](https://json.nlohmann.me/) - json for modern C++ (C++, MIT, [GitHub](https://github.com/nlohmann/json))
- [pydicom](https://pydicom.github.io/pydicom/dev) - Read, modify and write DICOM files with python code (Python, MIT, [GitHub](https://github.com/pydicom/pydicom))
- [OpenIGTLink](http://openigtlink.org/) - (C/C++, BSD-3-clause, [GitHub](https://github.com/openigtlink/OpenIGTLink))

## ODEs

- [Boost OdeInt](https://www.boost.org/doc/libs/1_81_0/libs/numeric/odeint/doc/html/index.html) - A library for solving initial value problems (IVP) of ordinary differential equations. (C++, Boost, [GitHub](https://github.com/boostorg/odeint))

## GPUs

- [OpenCL]() - GPGPU language ([GitHub](https://github.com/KhronosGroup/OpenCL-Headers))
- [Boost Compute](http://boostorg.github.io/compute/) - A C++ interface to multi-core CPU and GPGPU computing platforms based on OpenCL. (C++, Boost, [GitHub](https://github.com/boostorg/compute))
- [CLBlast](https://github.com/CNugteren/CLBlast) - OpenCL BLAS library written in C++11 (C++, Apache-2, GitHub)
- [arrayfire](https://arrayfire.com/) - A general purpose GPU library (C++, BSD-3,[GitHub](https://github.com/arrayfire/arrayfire))
- [viennaCL](https://viennacl.sourceforge.net/) - Open-source linear algebra library for computations on many-core architectures (C++, GNU, [GitHub](https://github.com/viennacl/viennacl-dev))
- SyCL
- HIP

## Solvers

- [Sundials](https://computing.llnl.gov/projects/sundials) - SUite of Nonlinear and DIfferential/ALgebraic equation Solvers. (C/C++/Fortran, BSD-3, [GitHub](https://github.com/LLNL/sundials))
- [Slate](https://icl.utk.edu/slate/) - dense linear algebra for HPC (C++, BSD-3, [GitHub](https://github.com/icl-utk-edu/slate))
- [diffeqpy](https://github.com/SciML/diffeqpy) - Python wrapper for DifferentialEquations.jl (Python/Julia, MIT, GitHub)

## Wave propagation

The Focused Ultrasound Foundation provides a set of open-source tools for modelling and validation [[here]](https://www.fusfoundation.org/for-researchers/open-access-technical-tools/#simulation).

- [jaxwell](https://github.com/stanfordnqp/jaxwell) - An iterative solver for solving the finite-difference frequency-domain Maxwell equations on NVIDIA GPUs. (Python, GPL-3, GitHub)
- [fd3d](http://www.mit.edu/~wsshin/fd3d.html) - Solve the frequency-domain Maxwell's equations in a 3D domain, using an iterative methods to avoid the large memory requirement of direct methods for 3D problems. (C, [GitHub](https://github.com/wsshin/fd3d))
- [Maxwellfdfd](http://www.mit.edu/~wsshin/maxwellfdfd.html) - Solves the frequency-domain Maxwell's equations (Matlab, [GitHub](https://github.com/wsshin/maxwellfdfd)) -
- [py-maxwell-fd3d]( https://github.com/zhaonat/py-maxwell-fd3d) - Solve the frequency-domain Maxwell's equations in a 3D domain, with direct and iterative methods (python, MIT, GitHub)
- [bempp](https://bempp.com/) - open-source computational boundary element platform to solve electrostatic, acoustic and electromagnetic problems. (Python, MIT, [GitHub](https://github.com/bempp))
- [jwave](https://ucl-bug.github.io/jwave) - k-Wave in JAX. (Python, LGPL-3, [GitHub](https://github.com/ucl-bug/jwave))
- [HITU_simulator](https://github.com/jsoneson/HITU_Simulator) - A nonlinear axisymmetric beamer simulator. (Matlab, GPL-3, GitHub)
- [Kranion](https://www.fusfoundation.org/for-researchers/resources/kranion/) - interactive transcranial focused ultrasound visualization system (java, MIT, [GitHub](https://github.com/jws2f/Kranion))
- [Focus](https://www.egr.msu.edu/~fultras-web/) - Fast nearfield method (Matlab)
- [mSound](https://m-sound.github.io/mSOUND/home) - Solves Westervelt equation by computing multiple reflections (Matlab, GNU, [GitHub](https://github.com/m-SOUND/mSOUND))
- AberSim - No longer maintained/publically available.
- Bergen - No longer maintained/publically available.
- [FieldII](http://field-ii.dk/) - Diagnostic simulator (Matlab, MIT)
<!-- markdown-link-check-disable -->
- [Beam](http://limu.msu.ru/product/3555/home?language=en) - 3D nonlinear continuous wave simulator (Matlab/Fortran )
- [Stride](https://www.stride.codes/) - modelling and optimisation framework for medical ultrasound (python, AGPL-3, [GitHub](https://github.com/trustimaging/stride))
- [BabelBrain](https://github.com/ProteusMRIgHIFU/BabelViscoFDTD) - FDTD of viscoelastic equation using a staggered grid arrangement with support for GPU and CPU backends (C++/OpenCL, BSD-3, GitHub)
- [FiVoNAGI](https://github.com/rvelseg/FiVoNAGI) - Finite volume nonlinear acoustics GPU implementation in 2D (C++/Cuda, BSD, GitHub)

## Physics-informed neural networks

- [SciML](https://sciml.ai/) - Website for open source software for scientific machine learning

## SBML

- [sbml](https://sbml.org/software/libsbml) - Native library for reading, writing and manipulating files and data streams containing the Systems Biology Markup Language (C/C++/C#/Java/JavaScript/MATLAB/Perl/PHP/Python/R/Ruby, LGPL-2, [GitHub](https://github.com/sbmlteam/libsbml)).

## Resources

- [Mathematical Tours](https://mathematical-tours.github.io/) - Mathematical tours of data science.
- [Numerical Tours](http://www.numerical-tours.com/) - Numerical tours of data science.

- [heffte](https://github.com/icl-utk-edu/heffte) - Highly Efficient FFT for Exascale (C++, BSD-3, [GitHub](https://github.com/icl-utk-edu/heffte))


----

## Other libraries and tools

- [FFTW](http://www.fftw.org) - Discrete Fourier transforms in one or more dimensions, of arbitrary input size, real and complex.
  (C, GPL2, [GitHub](https://github.com/FFTW/fftw3))
- [Qhull](http://www.qhull.org) - Convex hull, Delaunay triangulation, Voronoi diagram, halfspace intersection about a point, etc.
  (C/C++, [custom open source license](http://www.qhull.org/COPYING.txt),
  [GitHub](https://github.com/qhull/qhull/))
- [GSL](https://www.gnu.org/software/gsl/) - Random number generators, special functions, and least-squares fitting etc.
  (C/C++, GPL 3, [Savannah](https://savannah.gnu.org/projects/gsl))
- [OpenFOAM](https://www.openfoam.com) - Free, open source CFD (computational fluid dynamics) software.
  (C++, GPL 3, [GitHub](https://github.com/OpenFOAM/OpenFOAM-dev))
- [quadpy](https://github.com/sigma-py/quadpy) - Numerical integration (quadrature, cubature) in Python.
  (Python, proprietary, GitHub)
- [FiPy](https://www.ctcms.nist.gov/fipy/) - Finite-volume PDE solver.
  (Python, [custom open-source
  license](https://www.nist.gov/open/copyright-fair-use-and-licensing-statements-srd-data-software-and-technical-series-publications),
  [GitHub](https://github.com/usnistgov/fipy))
- [accupy](https://github.com/sigma-py/accupy) - Accurate sums and dot products for Python.
  (Python, GPL 3, GitHub)
- [SLEPc](https://slepc.upv.es) - Scalable Library for Eigenvalue Problem Computations.
  (C, 2-clause BSD, [GitLab](https://gitlab.com/slepc/slepc))
- [Chebfun](https://www.chebfun.org/) - Computing with functions to about 15-digit accuracy.
  (MATLAB, BSD, [GitHub](https://github.com/chebfun/chebfun))
- [pyMOR](https://pymor.org/) - Model Order Reduction with Python.
  (Python, 2-clause BSD, [GitHub](https://github.com/pymor/pymor/))
- [cvxpy](https://www.cvxpy.org/) - Modeling language for convex optimization problems.
  (Python, Apache 2.0, [GitHub](https://github.com/cvxpy/cvxpy))
- [PyWavelets](https://pywavelets.readthedocs.io/en/latest/) - Wavelet transforms in Python.
  (Python, MIT, [GitHub](https://github.com/PyWavelets/pywt))
- [NFFT](https://www-user.tu-chemnitz.de/~potts/nfft/) - Nonequispaced fast Fourier transform.
  (C/MATLAB, GPL 2, [GitHub](https://github.com/NFFT/nfft))
- [preCICE](https://precice.org/) - Coupling library for partitioned multi-physics simulations (FSI, CHT, and more).
  (C++, LGPL 3, [GitHub](https://github.com/precice/))
- [orthopy](https://github.com/sigma-py/orthopy) - Compute orthogonal polynomials efficiently.
  (Python, proprietary, GitHub)
- [pyGAM](https://pygam.readthedocs.io/en/latest/) - Generalized Additive Models in Python.
  (Python, Apache 2.0, [GitHub](https://github.com/dswah/pyGAM))
- [Dedalus](https://dedalus-project.org/) - Solve partial differential equations with spectral methods.
  (Python, GPL 3, [GitHub](https://github.com/DedalusProject/dedalus))
- [PyGMO](https://esa.github.io/pygmo/) - Massively parallel optimization.
  (Python/C++, MPL 2, [GitHub](https://github.com/esa/pygmo2))
- [shenfun](https://shenfun.readthedocs.io/en/latest/) - High-performance Python library for the spectral Galerkin method.
  (Python, BSD-2, [GitHub](https://github.com/spectralDNS/shenfun))
- [PyDMD](https://github.com/mathLab/PyDMD) - Dynamic Mode Decomposition (DMD) in Python.
  (Python, MIT, GitHub)
- [HPDDM](https://github.com/hpddm/hpddm) - High-performance unified framework for domain decomposition methods.
  (C++, LGPL 3, GitHub)

## Community

- [SciComp StackExchange](https://scicomp.stackexchange.com/) - Computational Science on the StackExchange network.
- [Wolfgang Bangerth's video class](https://www.math.colostate.edu/~bangerth/videos.html) - MATH 676: Finite element methods in scientific computing.
- [Nick Higham's blog](https://nhigham.com/) - Mostly on MATLAB, general computing advice.
- [Nick Trefethen's Video Lectures](https://people.maths.ox.ac.uk/trefethen/videos.html) - 36 video lectures on approximation theory/practice and scientific computing.
- [John D. Cook's blog](https://www.johndcook.com/blog/) - Feats of scientific computing.
- [Jack Dongarra's software list](https://netlib.org/utk/people/JackDongarra/la-sw.html) - List of freely available software for the solution of linear algebra problems.
- [NA Digest](https://netlib.org/na-digest-html/) - Collection of articles on topics related to numerical analysis and those who practice it.
<!-- markdown-link-check-disable -->
- [Gabriel Peyré on Twitter](https://twitter.com/gabrielpeyre) - One tweet a day on computational mathematics.
<!-- markdown-link-check-enable -->
- [Discord: Numerical Software](https://discord.com/invite/hnTJ5MRX2Y) - Discord messaging server on numerical software.

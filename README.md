This is an application that extends the existing pisoFoam solver in OpenFOAM to solve for the passive advection diffusion of a scalar. This is implemented for OpenFOAM-2.4.0 but can easily be extended for more recent versions. Schmidt number and turbulent Schmidt numbers must also be provided in the transportProperties file located in the constant directory. An example of the specification is as follows:-

Sc Sc [ 0 0 0 0 0 0 0 ] 1.49;
Sct Sct [ 0 0 0 0 0 0 0 ] 0.7;

# Installation #

Source the openfoam environment (bashrc or cshrc file) to load the proper environment variables. Place this folder in the $WM_PROJECT_USER_DIR/applications/solvers/ directory and run wmake from the source directory. The application will be installed in the directory set up by the environment variable $FOAM_USER_APPBIN
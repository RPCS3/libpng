# libpng
A clone of libpng for RPCS3 with upgraded projects, for use with Visual Studio 2015.

## Updating this repo
1. Update the source from the forked official repository. Make sure to keep this README file and .gitignore
2. Go into */projects/vstudio/* and open the *vstudio* solution in the latest Visual Studio
3. Upgrade the solution and all the projects in the solution
4. Add the x64 configuration and remove the Win32 configuration
5. Open libpng project properties.
   * Select all configurations
   * Change the target name to *$(ProjectName)*
   * Change the output directory to *$(SolutionDir)lib/*
   * Change the intermediate directory to *$(SolutionDir)tmp\$(ProjectName)-$(Configuration)-$(Platform)/*
6. Copy *pnglibconf.h.prebuilt* from /scripts/ to the base directory and rename it to *pnglibconf.h*
7. Good job, you're done!
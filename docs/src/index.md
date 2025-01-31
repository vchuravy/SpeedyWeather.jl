# SpeedyWeather.jl documentation

Welcome to the documentation for [SpeedyWeather.jl](https://github.com/milankl/SpeedyWeather.jl) a global
atmospheric circulation model with simple parametrizations to represent physical processes such as clouds,
precipitation and radiation.

## Overview

SpeedyWeather.jl is a global spectral model that uses a spherical harmonic transform to simulate
the general circulation of the atmosphere.
The prognostic variables used are vorticity, divergence, temperature, surface pressure
and specific humidity. Simple parameterizations represent various climate processes: Radiation,
clouds, precipitation, surface fluxes, among others.

SpeedyWeather.jl defines 
- `BarotropicModel` for the 2D barotropic vorticity equation
- `ShallowWaterModel` for the 2D shallow water equations
- `PrimitiveDryModel` for the 3D primitive equations without humidity
- `PrimitiveWetModel` for the 3D primitive equations with humidity

and solves these equations in spherical coordinates as described in this documentation.

## Manual outline

See the following pages of the documentation for more details

- [Installation](installation.md)
- [How to run SpeedyWeather.jl](how_to_run_speedy.md)
- [Spherical harmonic transform](spectral_transform.md)
- [Grids](grids.md)
- [Barotropic model](barotropic.md)
- [Shallow water model](shallowwater.md)
- [Primitive equation model](primitiveequation.md)
- [Parameterizations](parameterizations.md)
- [Extending SpeedyWeather](extending.md)
- [NetCDF output](output.md)

and the submodules

- [RingGrids](@ref)
- [LowerTriangularMatrices](@ref lowertriangularmatrices)   
- [SpeedyTransforms](@ref)

and the [original documentation](http://users.ictp.it/~kucharsk/speedy_description/km_ver41_appendixA.pdf)
by Molteni and Kucharski.

## Developers

The development of  SpeedyWeather.jl is lead by [Milan Klöwer](https://github.com/milankl) and
[current and past contributors](https://github.com/SpeedyWeather/SpeedyWeather.jl/graphs/contributors) include

- [Tom Kimpson](https://github.com/tomkimpson)
- [Alistair White](https://github.com/white-alistair)
- [Maximilian Gelbrecht](https://github.com/maximilian-gelbrecht)
- [David Meyer](https://github.com/dmey)
- [Daisuke Hotta](https://github.com/hottad)
- [Navid Constantinou](https://github.com/navidcy)

Any contributions are always welcome!

## Funding

MK received funding by the European Research Council under Horizon 2020 within the ITHACA project,
grant agreement number 741112 from 2021-2022. Since 2023 this project is also funded by the
National Science Foundation NSF.
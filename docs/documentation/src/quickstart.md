# Quick Start

Julia is just-in-time (JIT) compiled, which means that the first time you run a block of code it will be slow. Users new to Julia are **strongly encouraged** to start with the Docker version provided with the [Tutorial](@ref). The version bundled in the Docker container comes with an optimized system image, which has a much reduced JIT lag. It also simplifies the installation. The version in the Docker container/tutorial can also be used to work with the package. 

## Documentation

The tutorial is a guided tour of the package, including background information on the instrument and technique. The Manual section gives high-level examples on how to use the code. There is some overlap between the tutorial, the notebooks and the manual. The Library section is a browsable version of the code. It serves as reference to learn more about the definitions of operators, data types, and functions.

## Local Installation

The package can be installed from the Julia package prompt with

```julia
julia> ]add  https://github.com/mdpetters/DifferentialMobilityAnalyzers.jl.git
```

The closing square bracket switches to the package manager interface and the ```add``` command installs the package and any missing dependencies. To return to the Julia REPL hit the ```delete``` key.

To load the package run

```julia
julia> using DifferentialMobilityAnalyzers
```

Additional dependencies are needed when running the notebooks on the local install. 

```julia
julia> ] add Calculus DataFrames Distributions Glob IJulia Interpolations LambertW LinearAlgebra LsqFit NetCDF ORCA PlotlyJS Plots Printf ProgressMeter Random SpecialFunctions StatsBase Gadfly Compose
```
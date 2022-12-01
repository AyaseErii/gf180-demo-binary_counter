# Caravel User Project

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![UPRJ_CI](https://github.com/efabless/caravel_project_example/actions/workflows/user_project_ci.yml/badge.svg)](https://github.com/efabless/caravel_project_example/actions/workflows/user_project_ci.yml) [![Caravel Build](https://github.com/efabless/caravel_project_example/actions/workflows/caravel_build.yml/badge.svg)](https://github.com/efabless/caravel_project_example/actions/workflows/caravel_build.yml)

| :exclamation: Important Note            |
|-----------------------------------------|

## Sequential Counter

This is a seuqential digital counter.

The counter design is located at `./openlane/cntr_example` and the wrappered counter is located at `./openlane/user_project_wrapper`.

Before running the design flow, please make sure the gf180 pds was installed correctly. For the information about switching PDK from `sky130` to `gf180`, you may refer to [this video](https://www.youtube.com/watch?v=4-kISttsPbY). (Great thanks to Matt)

Once you have done with pdk setups, you can simply follow the commands below after you changed the corresponding [config.tcl](https://github.com/AyaseErii/gf180-demo-sequential_counter/blob/main/openlane/cntr_example/config.tcl) file, all files in the [includes]([https://github.com/AyaseErii/gf180-demo-sequential_counter/blob/main/openlane/cntr_example/includes](https://github.com/AyaseErii/gf180-demo-sequential_counter/tree/main/verilog) directory, and the [user_netlist.v](https://github.com/AyaseErii/gf180-demo-sequential_counter/blob/main/verilog/rtl/uprj_netlists) of the counter:
```
git clone https://github.com/AyaseErii/gf180-demo-sequential_counter.git
cd gf180-demo-sequential_counter
make cntr_example
```

The command above will generate the digital counter design (gdsii) and all necessary files for the next step---wrapper the design in to `user_project_wrapper`.

To 


## Additional Information about Caravel

Refer to [README](docs/source/index.rst#section-quickstart) for a quickstart of how to use caravel_user_project

Refer to [README](docs/source/index.rst) for this sample project documentation. 

Clustreye

This is a tool that is designed to show the system internals of a remote machine.

Need:
    - Developers run into bottlenecking issues on remote machines
    - Remote machines are difficult to debug since there's no GUI
    - Current method is to write scripts to ssh into each box
    - Scripts are non-standard, often buggy, no GUI

Architecture:
    - Nginx, Javascript (d3-lib) displays gauges of system internals
    - Gather statistics on system internals using shell scripts
    - Push/pull stats from/to postgres database using psycop2 library with python3

Result:
    - CPU, memory, disc capacity, network I/O gauges
    - Timeseries charts which display usage of hardware over time period

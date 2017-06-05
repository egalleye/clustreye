Clustreye

This is a tool that is designed to show the system internals of a remote machine.<br />

Need:<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Developers run into bottlenecking issues on remote machines<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Remote machines are difficult to debug since there's no GUI<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Current method is to write scripts to ssh into each box<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Scripts are non-standard, often buggy, no GUI<br />

Architecture:<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Nginx, Javascript (d3-lib) displays gauges of system internals<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Gather statistics on system internals using shell scripts<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Push/pull stats from/to postgres database using psycop2 library with python3<br />

Result:<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - CPU, memory, disc capacity, network I/O gauges<br />
&nbsp;&nbsp;&nbsp;&nbsp;    - Timeseries charts which display usage of hardware over time period<br />

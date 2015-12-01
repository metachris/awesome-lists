Know-How & Posts
----------------

* [Linux Performance Analysis in 60,000 Milliseconds (Netflix)](https://media.netflix.com/en/tech-blog/linux-performance-analysis-in-60-000-milliseconds) ([HN](https://news.ycombinator.com/item?id=10654681))
* [Linux Performance Articles and Talks by Brendan Gregg](http://www.brendangregg.com/linuxperf.html)
  * [Use Method](http://www.brendangregg.com/usemethod.html) - Utilization Saturation and Errors, a methodology for analyzing the performance of any system
  * [The TSA Method](http://www.brendangregg.com/tsamethod.html) - Thread State Analysis, for identifying issues causing poor thread performance
* [Netflix at Velocity 2015: Linux Performance Tools](http://techblog.netflix.com/2015/08/netflix-at-velocity-2015-linux.html) [Videos]


System Monitoring, Tools
------------------------

* [Vector](https://github.com/Netflix/vector) - on-host performance monitoring framework by [Netflix](http://techblog.netflix.com/2015/04/introducing-vector-netflixs-on-host.html)
* [Performance Co-Pilot](http://pcp.io/) ([Github](https://github.com/performancecopilot/pcp)) - system performance and analysis framework


Tips & Tricks
-------------

Get a high level idea of a system in 60 seconds

    uptime
    dmesg | tail
    vmstat 1
    mpstat -P ALL 1
    pidstat 1
    iostat -xz 1
    free -m
    sar -n DEV 1
    sar -n TCP,ETCP 1
    top

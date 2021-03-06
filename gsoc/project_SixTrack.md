---
title: GSoC 2017 in SixTrack
layout: plain
---

[SixTrack](http://cern.ch/sixtrack) is a software for simulating and analysing
the trajectory of high energy particles in accelerators. It has been used in
the design and optimization of the LHC and is now being used to design the
High-Luminosity LHC (HL-LHC) upgrade that will be installed in the next decade.
Sixtrack has been adapted to take advantage of large scale volunteer computing
resources provided by the
[LHC@Home](http://sixtrack.web.cern.ch/SixTrack/www/cern.ch/lhcathome) project.
It has been engineered to give the exact same results after millions of
operations on several, very different computer platforms. The source code is
written in Fortran, and is pre-processed by two programs that assemble the code
blocks and provide automatic differentiation of the equation of motions. The
code relies on the [crlibm](http://lipforge.ens-lyon.fr/www/crlibm/) library,
careful arrangement of parenthesis, dedicated input/output and selected
compilation flags for the most common compilers to provide identical results on
different platforms and operating systems. An option enables the use of the
[Boinc](http://lipforge.ens-lyon.fr/www/crlibm/) library for volunteer
computing. A running environment SixDesk is used to generate input files, split
simulations for LHC@Home (link sends e-mail) or CERN cluster and collect the
results for the user. SixTrack is licensed under LGPLv2.1.

A strong background in computer science and programming languages as well the
interest to understand computational physics methods implemented in the code are
sought. The unique challenge will be offered to work with a high-performance
production code that is used for the highest energy accelerator in the world -
and thus the code's reliability and backward compatibility cannot be
compromised. There will be the opportunity to learn about methods used in
simulating the motion of particles in accelerators.

## Project Proposals

{:.table .table-hover .table-striped}
{% for page in site.gsocproposals %}{% if page.project == "SixTrack" %} |[ {{ page.title }} ]( {{ page.url }} ) | {% endif %}
{% endfor %}
# [DMTCP: Distributed MultiThreaded CheckPointing](http://dmtcp.sourceforge.net/) 
[![Build](https://github.com/dmtcp/dmtcp/actions/workflows/make-check.yml/badge.svg)](https://github.com/dmtcp/dmtcp/actions/workflows/make-check.yml)

DMTCP is a tool to transparently checkpoint the state of multiple simultaneous applications, including multi-threaded and distributed applications. It operates directly on the user binary executable, without any Linux kernel modules or other kernel modifications.

Among the applications supported by DMTCP are MPI (various implementations), OpenMP, MATLAB, Python, Perl, R, and many programming languages and shell scripting languages. DMTCP also supports GNU screen sessions, including vim/cscope and emacs. With the use of TightVNC, it can also checkpoint and restart X Window applications.  For a multilib (mixture of 32 and 64-bit processes), see "./configure --enable-multilib".

DMTCP supports the commonly used OFED API for InfiniBand, as well as its integration with various implementations of MPI, and resource managers (e.g., SLURM).

The DMTCP Project is always looking for assistance in support the project.  Please see our [How to Contrinbut Guide](./governance/contributing.md) on how to setup your environement to start contributing.  To find out what areas we are looking for assitance with please recview the [following page](./governanre/contributing_areas.md) 

# Resources

* To install DMTCP, see [INSTALL.md](INSTALL.md).

* For an overview DMTCP, see [QUICK-START.md](QUICK-START.md).

* For the license, see [COPYING](COPYING).

* The project is governed by an Steering Council.  For an overview of the Governance process, see [Governance](./governance/governance.md)

* For more information on DMTCP, see: [http://dmtcp.sourceforge.net](http://dmtcp.sourceforge.net).

* For the latest version of DMTCP (both official release and git), see:
[http://dmtcp.sourceforge.net/downloads.html](http://dmtcp.sourceforge.net/downloads.html).

# Citing DMTCP
If you use DMTCP in your research please use the following BibTeX entry:
```BibTex
@Misc{AryaCooperman2014DMTCP,
  author =       {Kapil Arya, Gene Cooperman, Rohan Garg, et al.},
  title =        {DMTCP - DMTCP: Distributed MultiThreaded CheckPointing},
  howpublished = {Github},
  year =         {2014},
  url =          {https://github.com/dmtcp/dmtcp}
}
```

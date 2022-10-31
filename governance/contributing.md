# Contributing to DMTCP

# *** DRAFT ***

The DMTCP project thanks you for investing your time in contributing to the DMTCP project.  We welcome your expertise and enthusiasm,  The project needs more than programmers to continue its adoption and development.  You can see some areas below for ideas of where assistance is needed, but please do not limit yourself to these areas.  Explore the open pull requests, test out the project on a different operating system, or even an different ISA if that is your desire.   

## Getting Started
There are a lot of ways you can contribute:

- Contributing new code
- Fixing bugs, improving documentation, and other maintenance work
- Reviewing open pull requests
- Triaging issues
- Working on the DMTCP Hoe-To and FAQs
- Answering questions on the mailing lists.

## Overview

The DMTCP (Distributed MultiThreaded Checkpointing) Project (The Project) is an open source software project that transparently checkpoints a single-host or distributed computation in user-space with no modifications to user code or to the O/S. It works on most Linux applications, including Python, Matlab, R, GUI desktops, MPI, etc. It is robust and widely used (on Sourceforge since 2007).

Among the applications supported by DMTCP are MPI (various implementations), OpenMP, MATLAB, Python, Perl, R, and many programming languages and shell scripting languages. With the use of TightVNC, it can also checkpoint and restart X-Window applications. The OpenGL library for 3D graphics is supported through a special plugin. It also has strong support for HPC (High Performance Computing) environments, including MPI, SLURM, InfiniBand, and other components. See QUICK-START.md for further details.

DMTCP supports the commonly used OFED API for InfiniBand, as well as its integration with various implementations of MPI, and resource managers (e.g., SLURM). See contrib/infiniband/README for more details.

## Code of Conduct

We believe that teams are most sucessful when they operate and interact in a safe environment where individuals are encouraged to be themselves.  We operate our community a harassment-free experience for everyone, regardless of age, body size, visible or invisible disability, ethnicity, sex characteristics, gender identity and expression, level of experience, education, socio-economic status, nationality, personal appearance, race, caste, color, religion, or sexual identity and orientation.  To support this we have adopted the Contributor Covenant https://www.contributor-covenant.org code of conduct which you can find our specifics [here](../governance/CODE_OF_CONDUCT.md).

## License

The Software developed by The Project is released under the [Community License](./governance/../license.md) and is developed openly and hosted in public GitHub repositories under the [DMTCP GitHub organization](https://github.com/dmtcp).  The license is focused on balancing the intent of what it means to be an open source project while limiting the commerical explotation of the project via Cloud Service Providers whom often offer a SaaS version without contributing back to the project.  It is not meant to limit the personal use of or embedding of DMTCP into a product.

## Contributing to the Project

We ask that contributors sign a [Contributors License Agreement (CLA)](contributor-license-agreement.md) or a [Developer's Certificate of Origin (DCO)](developer_certificate.md).  For most contributors, the DCO is the preferred option and for institutions a CLA is recommended.  Here are our [contributor guidelines](contributing.md) 

## Getting Started 

*NB: May want to move this into its own document.*

The first step is to retrieve the source code of the project.  The following is not meant to be a lesson on git and github, but a simple start.  For futher git and github usage see the relevant documentation.

### Setup Local Fork

- [Install git](https://git-scm.com/downloads)

- Setup min git information
  
        git config --global user.email you@yourdomain.example.com
        git config --global user.name "Your Name Comes Here"

- Fork the DMTCP Repository

- Clone your Fork locally

        git clone git@github.com:{usename}/dmtcp.git dmtcp
        cd dmtcp
        git remote add dmtcp-main https://github.com/dmtcp/dmtcp.git

- Create a branch (should we have a convention?)

        git checkout -b new-branch 

- Make changes and push to your own fork

        git add modified_file
        git commit

        # push the branch to your own Github repo
        git push origin my-new-feature

### Pull Requests

- When ready create a pull request with the following information

## How to Report a Bug

- First look though exisiting Issues to ensure it is not already reported
- 

## Suggesting an Enhancement

## Your First Code Contribution


## Styleguides

## Git Commit Messages

## **Project Contributors**
Here is a list of the current Contributors to the DMTCP repository:

[https://github.com/dmtcp/dmtcp/graphs/contributors](https://github.com/dmtcp/dmtcp/graphs/contributors)


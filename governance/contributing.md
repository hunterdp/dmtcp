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

## Setup Local Development

The steps below are meant as a basic setup for contributing bug fixes, feature enhancements, testing, etc.  They are not meant to be a git primer.  For that we recommend reviewing the [git](https://git-scm.com) and/or the documentation for [github](https://docs.github.com/).  Note that the steps below assume that you have already setup a githib account.

1. Install [git](https://git-scm.com/downloads)

1. Setup some simple git information

    ```
    $git config --global user.email user@domain.com
    $git config --global user.name "Name"
    ```

1. Fork the DMTCP Repository

   - Log into your github account and navigate to the [DMTCP repository](https://github.com/dmtcp/dmtcp)
   - Click on the **Fork ** in the top corner of the page 
   - Fill in the information on the owner and repository name and add a description.
   - It is recommended to check the box to only copy the main branch only.
   - Click on the Create Fork button

1. Clone your Fork locally

    ```
    $git clone git@github.com:{usename}/dmtcp.git dmtcp
    $cd dmtcp
    $git remote add upstream https://github.com/dmtcp/dmtcp.git
    ```

1. Create a branch

    We recommend creating a new branch to add a feature and working on that branch.  

    ```
    # Checkout the main branch and ensure the latest changes are applied
    $git checkout main
    $git rebase upstream/main

    # Create and check out your new branch 
    $git checkout -b my-new-branch
    ```

2. Make changes and push to your own fork

    ```
    # See what files have been modified and/or added
    $git status

    # If desired, review any files that have been modified 
    $git diff modified_file

    # Add any new files into the staging area.  To keep things tidy, only add files that have related and complete changes. 
    # Leave files with unfinished changes for later commits.
    $git add modified_file(s)

    # Commit the staged changes to your local repository.  For simple commits, use the -m 'Comments on commit' if desired.  
    # Otherwise you configured editor will come up and ensure that you adequately describe the changes and additions.  
    $git commit -m 'your comments on the change' modified_file(s)

    # push the branch to your own Github repo
    $git push origin my-new-branch
    ```

## Commit Messages
Commit messages should be clear and follow a few basic rules.  The following are some guidelines.  The objective is to ensure someone else can understand what and why you committed something.

```
ENH: add functionality X to component Y.

The first line of the commit message starts with a capitalized acronym from the options listed below that idetifies the type of commit. This is followed by a blank line and then further explantion of the commit.  For readability, comment ould be no l75 characters.  If the commit is in response to an Issue or other request, this should be indicated by refering to it, e.g. "See Issue #1234" or "This finishes feature requested #x from the roadmap.".  

The comment should be self sufficient and the reader should not have to refer to the code to understand the commit.  
```

Below are a few standard acronyms to start the commit message with are:

```
API: Modifications or addition of an API change
BLD: change related to build process for DMTCP 
BUG: bug fix
DEP: deprecate something, or remove a deprecated object
DEV: development tool or utility
DOC: documentation
ENH: enhancement
MAINT: maintenance commit (refactoring, typos, etc.)
REV: revert an earlier commit
TST: addition or modification of tests
REL: related to releasing DMTCP, aka a patch, minor or major version.
```

### Pull Requests

- When ready create a pull request (PR) with the following information

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


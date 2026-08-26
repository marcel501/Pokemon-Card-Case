---
Markdown formatting used within this document.

Author: Marcel W.
Format: Basic
Version: 1.0.1

---

PROJECT ADMINISTRATION REPORT
==============================

# INTRODUCTION {{{

This project utilizes the design activity model to methodologically create the desired end product. It is a staged process which allows for a thorough development process and completeness at each step.




## AIMS

The aim of this document is to provide a central location in terms of project administration and project management. It is a necessary top level overview to describe the systematical approach towards the assignment.

}}}





___

# METHODOLOGY {{{

The project root directory is split into several modules which are either structured/linear (correspond to the primary process flow) or unstructured/non-linear (exist within other process flows/branches or are independent).

The standard design activity model methodology persists within this project. Due to the simple nature of this project, the value analysis and product risk analysis modules are entirely out of scope.




## FILE SYSTEM {{{

The whole project is hosted on a NAS system utilizing the SAMBA distributed-file-system protocol. This allows for direct writes to a centralized location allowing collaboration and systematic efficiency.

Computationally heavy files, such as CAD files must not be directly written to the project location - instead, they should be copied (if file present) and worked on the local system; after completion the CAD file may be copied back to the project location overwriting the original file.

Working on a computationally heavy file, process flow:

```
            Local PC                        NAS system
        ----------------                ----------------
        |              |    1. Copy     |              |
        |       -------| <------------- |              |
        |       |      |                |              |
        |       |      |    3. Copy     |              |
        |       ------>| -------------> |------->X     |
        |   2. Edit    |                | 4. Overwrite |
        |              |                |              |
        |              |                |              |
        ----------------                ----------------
```
}}}




## VERSION CONTROL {{{

As an extended part of this project, the primary version control for files within this project will be git. This will allow a more automatic and cleaner methodology, allowing members within the project to remain with a clean working directory.


}}}
}}}



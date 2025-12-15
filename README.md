# What is patching 
Patching is process of applying 
- updates
- modifications to software 
- update operating systems or application 

to fix 

- bugs 
- cyber-attaks
- enhance functionality
- improve performance, or address security vulnerabilities.


`````
A patch is typically a small piece of code or data designed to update an existing program or file without requiring a complete reinstallation.

```````

# Types of Patches

-  Security Patches : Address vulnerabilities to prevent exploitation.
-  Bug Fixes : Resolve errors
-  Feature Updates  : Add or enhance functionality
-  Service Packs : Collections of patches and updates bundled together.

## Overview :  

```The  project is to understanding patching in real - world using ansible```


# Pre Patch steps
```Pre-patching in Ansible refers to the process of preparing a system for patching by performing necessary checks and configurations before applying updates.```

- Create Directory
- Verify resurces
- Gather Active Services
- Gather Evidences

# Patch Steps

```process of applying updates or fixes, known as patches, to software, operating systems, or hardware.```

- Stop service
- Install Patch
- Patch Confirmation
- Restart Services

# Post Patch Steps

```After update everything verify update and generate final updated reports```

- Service Revalidation
- Resorces health check
- Report Generation
- Notification
- Clean UP


# Future Scope 

- You can use ansible tower

# variable list


|     Variable      |    Variable type   |   Description                        |    Supported os    |     default     |                                                                       
|-------------------|--------------------|--------------------------------------|--------------------|-------------------|
|   Comman_path     |      String        |  Path for folder creation            |        both        |        -          |   
|                   |                    |                                      |                    |                   |
|   Comman_path1    |      string        |  Path for creating patch folder      |        both        |        -          |
|                   |                    |                                      |                    |                   |
|   Comman_path2    |      String        |  Path for creating post patch folder |        both        |        -          |  
# What is patching 
Patching is process of applying 
- updates
- modifications to software 
- update operating systems or application 

To fix 
- bugs 
- cyber-attaks
- enhance functionality
- improve performance, or address security vulnerabilities.


```
A patch is typically a small piece of code or data designed to update an existing program or file without requiring a complete reinstallation.
```

## Types of Patches

-  Security Patches : Address vulnerabilities to prevent exploitation.
-  Bug Fixes : Resolve errors.
-  Feature Updates  : Add or enhance functionality.
-  Service Packs : Collections of patches and updates bundled together.

## Project Overview 

```
The  project is to understanding patching in real world using ansible. Implementing best practices such as automating patch deployment, performing regular backups, and maintaining clear communication with users can enhance the effectiveness of patch management. 
```

## Project structure 

### main file
```yaml
 Inside this file call three role 
 
 - pre-patching role
 - patching role
 - post-patching role
```

### Pre Patch role

> Pre-patching in Ansible refers to the process of preparing a system for patching by performing necessary checks and configurations before applying updates.

```yml
- Create main folder for project using universal variable.
- Verify resurces before patching.
- Gather active services of ystem.
- Gather evidences convert folder into zip.
```
### Patch role


> process of applying updates or fixes, known as patches, to software, operating systems, or hardware.

```yml
- Stop service before patching.
- Install Patch for your system Linux/Redhat.
- Patch Confirmation after patching.
- Restart Services after patching.
```

### Post Patch role

> After update everything verify update and generate final updated reports.

```yml
- Service Revalidation after patching.
- Resorces health check of your system.
- Report Generation to check difference before and after patching.
- Notification for getting updates related to patches.
- Clean up will convert folder into zip and delete all file from that folder.
```

# variable list


|     Variable      |    Variable type   |   Description                            |    Supported os    |     default     |                                                                       
|-------------------|--------------------|------------------------------------------|--------------------|-------------------|
|   Universal_path  |      String        |  Variable for folder creation            |        both        |        -          |   
|                   |                    |                                          |                    |                   |
|   Stage_dir       |      string        |  Variable for creating pre-patch folder  |        both        |        -          |
|                   |                    |                                          |                    |                   |
|  patch_Stage_dir  |      String        |  Variable for creating patch folder      |        both        |        -          | 
|                   |                    |                                          |                    |                   |
|  Stage_dir2       |      String        |  Variable for creating post-Patch for    |        both        |        -          |   




## Future Scope 

> You can use ansible tower for performing patching which is useful for visualization.

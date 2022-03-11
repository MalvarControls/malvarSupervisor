# malvarSupervisor
Module with utilities for supervisor:
  - Custom login page
  - Client creation
  - Sets permissions
  - Creates default project structure
  - Check active sessions

# Installation

Download the appropriate realease files:
- [malvarSupervisor-rt.jar](https://github.com/MalvarControls/malvarSupervisor/releases);
- [malvarSupervisor-ux.jar](https://github.com/MalvarControls/malvarSupervisor/releases);

Paste them into the modules folder inside your Niagara installation directory ```C:\Niagara\Niagara-4.x.x.x\modules```.

## Dependencies
- This module requires [malvarCertificates](https://github.com/MalvarControls/malvarCertificates) to be installed;

## Usage

### Create Client
Client creation creates the whole structure, files and permissions for a project.
If the given password does not meet the security requirements, the job will display as fail, but the structure is created nonetheless. 

### Login Page
The login page is automatically created after using the 'Create Client' action of the 'malvarSupervisorServices'.

If you want to manually add the login page with the custom design please follow these steps:
  1. Navigate to Station -> Services -> Web Service;
  2. Change view to 'Slot Sheet';
  3. Add a new slot named 'logo' of type 'baja:BString';
  4. Add a new slot named 'loginCss' of type 'baja:BString';
  5. Set the value of the 'logo' property to 'module://malvarSupervisor/rc/images/EXOoperator_top_logo.png'
  6. Set the valur of the 'loginCss' property to 'module://malvarSupervisor/rc/css/login.css'
  


  

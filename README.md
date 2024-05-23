# Panther-Diagram

This project features UML activity diagrams representing the inner workings of the modern Windows installation procedure (powered by a WIM-based installer codenamed Panther) **for research purposes**.

## What is Panther, and how has this diagram been created?

**Panther** is the codename for the setup engine of the WIM-based installer and for the Windows Deployment Services (WDS). This technology has been in use since Windows Vista, released in 2007.

Panther also does extensive logging to the `setupact.log` and `setuperr.log` files in its directory (`WINDOWS\Panther`) and, therefore, this project is possible. All information has been solely grabbed from the logs to give a better understanding of the Windows setup procedure.

## Current state

The UML activity diagrams only cover a clean installation of Windows started from WinPE. Additional cases, like upgrades or in-place installations, may be covered in the future.

## How do I contribute?

Requirements:

- **Any Visual Studio version** greater or equal to 2010, with UML compatibility (you may need to add it if you are using a modern version of VS)

1. Fork this repository
2. Perform installations of Windows in more situations. Many things can differ
3. Pull the Setup logs from the target installation and examine them
4. Update the UML activity diagram accordingly
5. Save your changes and make a pull request

> [!IMPORTANT]
> Please make sure to disclose the source of your changes in your pull requests. Any PR whose source is leaked Windows code will be discarded, so you must stick to Setup logs.
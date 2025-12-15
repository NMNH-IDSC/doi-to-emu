DOI to EMu
==========

Demo for creating a bibliography record using a DOI using the EMu REST
API. Test environments only.

The .xmurc and schema.pl files are available on request for NMNH staff.

Setup
-----

1.  Install miniforge: https://conda-forge.org/download/
2.  Install git: https://git-scm.com/install/
3.  Install VS Code: https://code.visualstudio.com/download
4.  Copy .xmurc to your home directory (%USERPROFILE% on Windows or ~ on
    Mac/Linux)
5.  Create a new folder called .xmu in your home directory and copy
    schema.pl to it
6.  Open the MiniForge Prompt (Windows) or Terminal (Mac/Linux) and do
    the following:
    1.  Change to the directory you want to work from: `cd path/to/dir`
    2.  Clone this repository:
        `git clone https://github.com/NMNH-IDSC/doi-to-emu`
    3.  Change to the folder containing the repository: `cd doi-to-emu`
    4.  Create the environment: `mamba env create -f environment.yml`

The environment can be updated later by returning to the doi-to-emu
director in the MiniForge Prompt, then running the following command:
`mamba env update -f environment.yml`

Running the notebook
--------------------

1.  Open VS Code
2.  Click File \> Open Folder
3.  Open this folder
4.  Double-click emurestapi.toml and update the username and password
5.  Double-click doi-to-emu.ipynb
6.  Click Select Kernel in the upper right. A dropdown will appear under
    the search bar at the top of the window. Select Python Environments
    \> emurestapi.

Limitations
-----------

- Cannot find existing parties records that match author or publisher
  (possibly an issue with default query parameters)

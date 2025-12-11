DOI to EMu
==========

Demo for creating a bibliography record using a DOI using the EMu REST
API. Test environments only.

The .xmurc and schema.pl files are available on request.

Setup
-----

1.  Install miniforge: https://conda-forge.org/download/
2.  Install VS Code: https://code.visualstudio.com/download
3.  Copy .xmurc to your home directoy (%USERPROFILE% on Windows or ~ on
    Mac/Linux)
4.  Create a new folder called .xmu in your home directory and copy
    schema.pl to it
5.  Open the MiniForge Prompt (Windows) or Terminal (Mac/Linux)
6.  Navigate to the folder created in step 4: `cd /path/to/dir`
7.  Create the environment: `mamba env create -f environment.yml`

The environment can be updated later by repeating steps 5-6, then
running the following command: `mamba env update -f environment.yml`

Running the notebook
--------------------

1.  Open VS Code
2.  Click File \> Open Folder
3.  Open this folder
4.  Double-click doi-to-emu.ipynb
5.  Click Select Kernel in the upper right. A dropdown will appear under
    the search bar at the top of the window. Select Python Environments
    \> emurestapi.

Limitations
-----------

- Cannot find existing parties records that match author or publisher
  (possibly an issue with default query parameters)
- Cannot import nested tables (possibly a syntax error, possibly an
  issue with the API itself)

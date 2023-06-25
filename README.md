# ubuntu-aws-kitchen-guide
Step-by-step description of spinning up Ubuntu on AWS using Kitchen - Cohort4@HCA

Chef is a powerful configuration management system that can be used to manage infrastructure by turning it into code. It supports multiple platforms including Windows, macOS, and Linux distributions such as Ubuntu. 

Please note that in recent versions, Chef has been restructured and is provided as part of the Chef Workstation, which contains all the tools you need to get started with Chef.

Before starting, ensure you have administrative access to your system. 

1. **Windows**:

   - Download the Chef Workstation package from the official Chef Downloads page: `https://downloads.chef.io/tools/workstation`
   - Once downloaded, run the MSI file to start the installation process.
   - Follow the installation prompts accepting the license agreement and clicking on 'Next' until installation starts.
   - After installation, you can verify the installation by opening a new command prompt and typing `chef -v`, which should show you the installed version of Chef Workstation.

2. **macOS**:

   - Download the Chef Workstation package for macOS from the official Chef Downloads page: `https://downloads.chef.io/tools/workstation`
   - Once downloaded, open the downloaded `.dmg` file.
   - Drag the Chef Workstation app into your Applications folder.
   - Open a terminal window, then verify the installation by typing `chef -v`. This should show you the installed version of Chef Workstation.

3. **Ubuntu**:

   - Open a terminal window.
   - Download the Chef Workstation package with curl (you might need to install curl first with `sudo apt install curl`):

     ```
     curl https://omnitruck.chef.io/install.sh | sudo bash -s -- -P chef-workstation
     ```

   - After the script has run successfully, you can verify the installation by typing `chef -v` in the terminal. This should show you the installed version of Chef Workstation.

Remember that Chef Workstation installs several tools by default, including `chef-client` for applying configuration to your systems, `knife` for managing your infrastructure, and `inspec` for compliance automation.

Also, it's a good practice to always check the official documentation of the software for any changes or updates in the installation procedure.

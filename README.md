# AI RELATED THINGS


## DOCKER STUFF
There is no way to properly update all your images at once. Here is a command you can run from your WSL distro terminal. This will redownload (update) each image you have.       
      
      docker images |grep -v REPOSITORY|awk '{print $1}'|xargs -L1 docker pull 

This process ensures that unused sectors are identified and allows Hyper-V to shrink the VHDX file further.
      
      docker run --rm --privileged --pid=host docker/desktop-reclaim-space

You must shutdown WSL before running this next command.
     
     wsl --shutdown
This command must be run from Powershell.
    
     Optimize-VHD -Path ${env:LOCALAPPDATA}\Docker\wsl\data\ext4.vhdx -Mode Full

Then to restart WSL:
     
     wsl

I. WSL commands: 

1. Access terminal wsl or run program linux from Command Prompt
	```
	wsl --set-default-version 2: change use wsl2 as default
	
	or set special instance this convert distro to wsl2 if current run wsl1
	
	wsl --set-version [distro_name] [wsl_version_number]

	wsl : access distro default of wsl to run command

	wsl nano : open app nano in linux from Command Prompt windows

	Type \\wsl$Ubuntu in windows explore : access Ubuntu file from window
	```
2. WSL Manage
	<!-- https://superuser.com/questions/1667969/create-wsl2-instance-from-vhdx -->
	```
	wsl -l : show list wsl installed in windows
	
	wsl -l -v: show list wsl install in windows and special wsl version
	
	wsl --export: command there to create a tar file backup of the installation which can then be wsl --import into the new computer. 
	
	wsl --import <Distribution Name> <Installation Folder> <Ubuntu WSL2 Image Tarball path> refer https://github.com/MicrosoftDocs/WSL/issues/412
	
	wsl -d centos7-cwp: run wsl special instance in wsl -l
	
	wsl --shutdown <Distribution Name> : stop wsl special instance
	
	wsl --unregister centos7-cwp:  remove centos7-cwp in wsl-l
	https://github.com/microsoft/WSL/issues/4762
	```


3. Some case study

https://cloudbytes.dev/snippets/how-to-install-multiple-instances-of-ubuntu-in-wsl2

https://docs.microsoft.com/en-us/windows/wsl/vhd-size

https://appuals.com/wsl-register-distribution-error-0x80370102-on-windows-10/

https://www.reddit.com/r/bashonubuntuonwindows/comments/gdiubo/wsl2_import_existing_ext4_image/

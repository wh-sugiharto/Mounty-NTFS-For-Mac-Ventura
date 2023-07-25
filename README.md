MOUNTY FOR MAC M1 / M2 VENTURA


#INSTALL MOUNTY

#INSTALL MACFUSE

#INSTALL BREW 

	/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

#PATH BREW ( IF "brew not found" )

	cd /opt/homebrew/bin/
	PATH=$PATH:/opt/homebrew/bin
	cd
	touch .zshrc
	echo export PATH=$PATH:/opt/homebrew/bin >> .zshrc


Run the commands in that order in terminal, you'll be editing the path and creating the missing .zshrc file, exporting the path to this new file.
Now you should be able to use:
brew doctor
It should say: "Your system is ready to brew."

#INSTALL NTFS-3G

	brew tap gromgit/homebrew-fuse
	brew install --cask macfuse
	brew install ntfs-3g-mac



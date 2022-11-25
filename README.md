# change-wsl-with-oh-my-posh
Personalizing bash of the wsl with oh-my-posh and Font Nerd

# Hi, guys

This post, i am changing settings of wsl to settings my favorite theme, 🚀👽

Into step-by-step, you can do too.

Linux: Set up your terminal
----------------------------------
:: From:
	https://learn.microsoft.com/pt-br/windows/terminal/tutorials/custom-prompt-setup#install-a-nerd-font

:: Webpage, auxiliar
	Webpage from: https://ohmyposh.dev/docs/installation/linux

Manual Installation:
:: Download Oh My Posh
	sudo wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/posh-linux-amd64 -O /usr/local/bin/oh-my-posh
	sudo chmod +x /usr/local/bin/oh-my-posh

:: If don't has unzip installed, next command is be necessary:
  sudo apt install unzip

:: Download the themes
  mkdir ~/.poshthemes
	wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/themes.zip -O ~/.poshthemes/themes.zip
	unzip ~/.poshthemes/themes.zip -d ~/.poshthemes
	chmod u+rw ~/.poshthemes/*.omp.*
	rm ~/.poshthemes/themes.zip
  
:: Invoke settings to view result until here
	eval "$(oh-my-posh --init --shell bash --config ~/jandedobbeleer.omp.json)"
  
  . If you has an error message into bash console path, try next command to create a file theme configuration to oh-my-posh:
    oh-my-posh config export --output ~/jandedobbeleer.omp.json

  . If you agree, you can apply this settings, at your file .profile and insert into end of your configuration the next command line:
    eval "$(oh-my-posh --init --shell bash --config ~/jandedobbeleer.omp.json)"
    
## Finished setting

this is all, 🎯👽🚀

![image](https://user-images.githubusercontent.com/72364037/203876831-5abb2612-2aa2-4299-92f9-5f61f6ca3f88.png)

# linux_programs
programas de linux y sus respectivos archivos de configuracion y personalizacion si los necesitaran

## vim

* instalacion : sudo pacman -S vim
* configuracion : vimrc

## emacs (spacemacs)

* instalacion : sudo pacman -S emacs
* git clone --recursive https://github.com/syl20bnr/spacemacs ~/.emacs.d

## latex:
* instalacion en archlinux: texlive-most

##manjaro keys:

* sudo pacman-key --populate archlinux
* sudo pacman-key --populate manjaro
* sudo pacman-key --refresh-keys
* sudo pacman -S manjaro-keyring
* sudo pacman -S archlinux-keyring

## go

* instalacion : sudo tar -C /usr/local -xzf go$VERSION.$OS-$ARCH.tar.gz
* variable de entorno : export PATH=$PATH:/usr/local/go/bin

## anaconda (python)

* instalacion : sh Anaconda-$version$-Linux-x86_64.sh
* variable de entorno : PATH="/home/$usuario$/anaconda3/bin:$PATH"

## julia

* instalacion : tar -C /home/$usuario$
* cambiar nombre (julia) por comodidad
* variable de entorno : PATH="/home/$usuario$/julia/bin:$PATH"

## zathura

*instalacion : sudo pacman -S zathura-pdf-poppler

## firefox

* instalacion : sudo pacman -S firefox

## awesome wm

* instalacion : sudo pacman -S awesome vicius
* configuracion : rc.lua

## terminator

* instalacion : sudo pacman -S terminator
* configuracion : config (renombrar de config_terminator)

## spotify

* instalacion : 

 - AUR
 - tar -xvf spotify$ version $
 - cd spitify$ version $
 - makepkg -s
 - sudo pacman -U spotify$ version $

## vlc

* instalacion : sudo pacman -S vlc

## libreoffice

* instalacion : sudo pacman -S libreoffice-still

## SpaceFM

* instalacion : sudo pacman -S spacefm

## St terminal

nota re-nombrar los archivos : config_st.mk y config_st.h

* instalacion : 
 
  - descargar de www.st.suckless.org
  - reemplasar el archivo : config.mk
  - sudo make clean install

* personalizacion : 

  - reemplazar el archivo config.h 
  - sudo make clean install

## Dwm windows manager

nota re-nombrar el archivo : config_dwm.h

* instalacion : 
 
  - pacman -S base-devel abs
  - abs community/dwm
  - cp -r /var/abs/community/dwm ~/dwm
  - makepkg -i

* personalizacion : 

  - reemplazar el archivo config.h
  - makepkg -g >> PKGBUILD
  - makepkg -efi

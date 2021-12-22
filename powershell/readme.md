## Инструкция по настройке Powershell

Большая часть взята у [devaslife](https://www.youtube.com/watch?v=5-aK2_WwrmM)

### Установка шрифтов

Скачиваем шрифт Hack из подборки [Nerdfonts](https://github.com/ryanoasis/nerd-fonts)
Установка штатная в винде.

### Установка новой версии Powershell

### Установка Scoop

	iwr -useb get.scoop.sh | iex

	scoop install git neovim

### Создание конфиг файла

Перейти в каталог пользователя 

	cd ~

Создать каталог, если его нет

	mkdir .config/powershell

Создать конфигурационый файл user_profile.ps1

### Указание нового конфиг файла

	nvim $PROFILE.CurrentUserCurrentHost

	. $env:USERPROFILE\.config\powershell\user_profile.ps1

### Установка Oh my posh

	Install-Module posh-git -Scope CurrentUser -Force

	Install-Module oh-my-posh -Scope CurrentUser -Force

### Установка иконок

	Install-Module -Name Terminal-Icons -Repository PSGallery -Force

### Установка z

Z - Программа для быстрого переключения между каталогами

	Install-Module -Name z -Force

### Установка PSReadLine

	Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck




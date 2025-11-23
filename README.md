# Introduction 

mr rt is place to save my learning journey to learn RT-Thread.


### sunday 23 nov 2025 

trying to install rt-thread env tools on arch linux arm. there is official shell script i can run on arch linux in rt-thread env github repository (https://github.com/RT-Thread/env?tab=readme-ov-file#install-env)

after successfull install, you can attach `env.sh` file to your `.bashrc` or any init script, `source ~/.env/env.sh`

as my try, you need install additional package such as 

- python-request (use `sudo pacman -S python-requests --noconfirm`)
- python-tqdm (`sudo pacman -S python-tqdm --noconfirm`)
- scons (`sudo pacman -S scons --noconfirm`)

then after those 3 package installed we can run 

- `pkgs --upgrade && pkgs --update`, it will download and install required package for current project.

then after package installed we can try to build a project with 

- `scons` or `scons -j12`

on my first try it work and able generating `.elf` file 

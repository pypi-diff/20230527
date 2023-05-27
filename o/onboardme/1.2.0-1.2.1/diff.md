# Comparing `tmp/onboardme-1.2.0.tar.gz` & `tmp/onboardme-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.2.0.tar", max compression
+gzip compressed data, was "onboardme-1.2.1.tar", max compression
```

## Comparing `onboardme-1.2.0.tar` & `onboardme-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0    15245 2023-05-21 11:22:02.167263 onboardme-1.2.0/README.md
--rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.2.0/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.2.0/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.2.0/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.2.0/onboardme/console_logging.py
--rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.2.0/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.2.0/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.2.0/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.2.0/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-21 15:49:30.802500 onboardme-1.2.0/onboardme/help_text.py
--rw-r--r--   0        0        0     3085 2023-05-21 11:22:02.171439 onboardme-1.2.0/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.2.0/onboardme/misc.py
--rwxr-xr-x   0        0        0     9362 2023-05-21 15:32:16.703438 onboardme-1.2.0/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.2.0/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.2.0/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.2.0/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.2.0/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-21 15:32:43.314470 onboardme-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    16626 1970-01-01 00:00:00.000000 onboardme-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-27 17:36:38.841907 onboardme-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0    15653 2023-05-27 17:36:38.841907 onboardme-1.2.1/README.md
+-rwxr-xr-x   0        0        0     6786 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1793 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5732 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/misc.py
+-rwxr-xr-x   0        0        0     9362 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2023-05-27 17:36:38.869907 onboardme-1.2.1/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1792 2023-05-27 17:36:38.869907 onboardme-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    16983 1970-01-01 00:00:00.000000 onboardme-1.2.1/PKG-INFO
```

### Comparing `onboardme-1.2.0/LICENSE.txt` & `onboardme-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/README.md` & `onboardme-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
   <a href="https://github.com/jessebot/onboardme/releases">
     <img src="https://img.shields.io/github/v/release/jessebot/onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white">
   </a>
 </p>
 
 Get your daily driver just the way you like it, from dot files management, to package installation, to other little features you didn't know you needed, `onboardme` intends to save you time with initializing and maintaining your personal environments.
 
+<p align="center">
+<img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/image_in_terminal.png' alt='screenshot of color samples and image of dog using a computer using sixel'>
+</p>
+
 ## Features
 
 ### Keep your Dot Files Up To Date Across multiple systems
 `onboardme` can manage your [dot files] using a git by turning your home directory into a repo.
 
 <details>
   <summary>We provide default dot files, so you don't have to manage them</summary>
@@ -62,21 +66,21 @@
 </details>
 
 ### Easy `yaml` config files
 [XDG Base Directory Spec] use for [config files](#configuration)
 
 ### Docker image for an on-the-go dev workspace
 
-The docker image is built daily or on push to main. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
+The docker image is built nightly, and on push to `main` via GHA. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
 See the [docker](#docker) section for more info!
 
 ### Other optional configurations
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
-- Install nerdfonts (defaults to mononoki and Symbols Only)
+- Install [nerdfonts](https://www.nerdfonts.com) (defaults to mononoki and Symbols Only)
 
 ### Screenshots
 
 <details>
   <summary>Example of <code>onboardme --help</code></summary>
 
 <p align="center" width="100%">
@@ -98,15 +102,15 @@
 ### Powerline and ls
 <img width="80%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/ls_tree_examples.png' alt='screenshot of powerline and lsd'>
 
 ### Powerline with git
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/git_powerline_example.png' alt='screenshot of powerline and git colors'>
 
 ### Image and colors
-<img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/image_in_terminal.png' alt='screenshot of color samples and image of dog using a computer using sixel'>
+
 
 ### Python virtual env in powerline and cat
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/python_virtual_env_example.png' alt='screenshot of using bat and python virtual env in powerline'>
 </p>
 
 </details>
 
@@ -182,14 +186,16 @@
 ```bash
 # should also work with pipx, if you'd like to use that instead
 pip install --user --upgrade onboardme
 ```
 
 ### Using the Docker image
 
+_Note: For fonts and images to work properly, you should use a modern terminal like [wezterm](https://wezfurlong.org/wezterm/), iterm2, or konsole as well as you need to make sure you [install](https://github.com/ryanoasis/nerd-fonts/tree/master#font-installation) a [nerdfont](https://www.nerdfonts.com) and_ `libsixel` + `imagemagick`.
+
 To run the image locally with onboardme installed and already run using default settings:
 
 ```bash
 # this image is built daily and has already run onboardme with the default settings
 docker run jessebot/onboardme:latest
 ```
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
          catppuccin/catppuccin/main/assets/misc/transparent.png] *****
               [https://img.shields.io/github/v/release/jessebot/
 onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white]
 GetÂ yourÂ dailyÂ driverÂ justÂ theÂ wayÂ youÂ likeÂ it,Â fromÂ dotÂ files
 management,Â toÂ packageÂ installation, to other little features you didn't
 know you needed,Â `onboardme` intends to save
 youÂ timeÂ withÂ initializingÂ andÂ maintainingÂ yourÂ personal environments.
+  [screenshot of color samples and image of dog using a computer using sixel]
 ## Features ### Keep your Dot Files Up To Date Across multiple systems
 `onboardme` can manage your [dot files] using a git by turning your home
 directory into a repo.  We provide default dot files, so you don't have to
 manage them - The [default dot files] are open source, and the maintainers use
 these themselves - They cover a lot of common apps/tools you probably want
 anyway - They have consistent colorschemes accross different CLI/TUI programs
 ð - They set all the helpful BASH aliases you could need (zsh support coming
@@ -29,26 +30,26 @@
 D We used to support both neovim _and_ vim, but these days none of the primary
 developers of this repo use pure vim anymore, so we can't ensure it's up to
 standards. All of your knowledge from vim is still helpful in neovim though,
 and we highly recommend switching as neovim has a lot more features and a very
 active plugin community :) NeoVim maintains a guide on how to switch from vim
 [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml`
 config files [XDG Base Directory Spec] use for [config files](#configuration)
-### Docker image for an on-the-go dev workspace The docker image is built daily
-or on push to main. The base image is `debian:bookworm`, but we will rollout
-support for Ubuntu down the line :) See the [docker](#docker) section for more
-info! ### Other optional configurations - Enable touchID for sudo on macOS -
-Add your user to the docker group - Install nerdfonts (defaults to mononoki and
-Symbols Only) ### Screenshots  Example of onboardme --help
+### Docker image for an on-the-go dev workspace The docker image is built
+nightly, and on push to `main` via GHA. The base image is `debian:bookworm`,
+but we will rollout support for Ubuntu down the line :) See the [docker]
+(#docker) section for more info! ### Other optional configurations - Enable
+touchID for sudo on macOS - Add your user to the docker group - Install
+[nerdfonts](https://www.nerdfonts.com) (defaults to mononoki and Symbols Only)
+### Screenshots  Example of onboardme --help
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
-  colors] ### Image and colors [screenshot of color samples and image of dog
-  using a computer using sixel] ### Python virtual env in powerline and cat
+   colors] ### Image and colors ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
  # Quick Start ### Install Locally You'll need `curl`, `brew`, `git`, and
 Python 3.11 to get started. We have a setup script to install those (except
 `curl`) and help you get your environment to the XDG spec under Locally or you
 can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/
 jessebot/onboardme).  Local prereq install script  curl, a pre-prereq ```bash #
 First, make sure you have curl, but it *should* be there already be on macOS. #
@@ -68,72 +69,77 @@
 this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
 opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
 (whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
 >> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
 you can also set the shell directly in your terminal app via the settings.  If
 you've already got all the above prereq on your machine, you can just do:
 ```bash # should also work with pipx, if you'd like to use that instead pip
-install --user --upgrade onboardme ``` ### Using the Docker image To run the
-image locally with onboardme installed and already run using default settings:
-```bash # this image is built daily and has already run onboardme with the
-default settings docker run jessebot/onboardme:latest ``` To run the image
-locally with onbaordme installed but _not_ run: ```bash # best if you have your
-own dot files, or need a smaller initial docker image to pull # no packages
-outside of the required pre-reqs for onboardme have been installed docker run
-jessebot/onboardme:no-install ``` ## Running commands _Now_ you can run
-`onboardme` ð ```bash # this will display the help text for onboardme
-onboardme --help # Running this won't overwrite any existing dot files, but it
-may add new ones. onboardme ``` From here, if you want to *completely wipe your
-existing dot files* for a fresh start with with `onboardme`, you can run:
-```bash # WARNING: This will overwrite your local dotfiles, including your
-.bashrc and .bash_profile # can also be done with: onboardme -O onboardme --
-overwrite ``` You can read more in depth at the [Getting Started Docs] ð!
-There's also more [docs] on basically every program that onboardme touches. ###
-Upgrades If you're on python 3.11, you should be able to do: ```bash pip3.11
-install --upgrade onboardme ``` ### Configuration onboardme has lots of CLI
-options, but you can also use config files. You have to create these files for
-the time being. Config files are in `$XDG_CONFIG_HOME/onboardme/`, or
-`~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined. | Config File |
-Description | |:------------------------------------------|:-------------------
----------------------------------| | `$XDG_CONFIG_HOME/onboardme/config.yml` |
-For step configuration to run either all steps, or just a subset. | |
-`$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different
-package managers | Examples:  ~/.config/onboardme/config.yml ```yaml log: #
-Full path to a file you'd like to log to. Creates file if it doesn't exist
-file: "" # what level of logs to output (DEBUG, INFO, WARN, ERROR) level:
-"INFO" # steps refer to a specific function in the list of functions we run
-steps: # these are mac specific steps Darwin: # clones dot files into home dir/
-git fetches updates for dot files - dot_files # install packages - packages #
-adds nerdfonts - font_setup # runs :Lazy sync to install all your plugins -
-neovim_setup # sets up touchID for sudo - sudo_setup # these are linux specific
-steps Linux: - dot_files - packages - font_setup - neovim_setup # add your user
-to the docker group - group_setup dot_files: # personal git repo URL for your
-dot files, defaults to jessebot/dot_files git_url: "https://github.com/
-jessebot/dot_files.git" # the branch to use for the git repo above, defaults to
-main git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will
-overwite/delete local files in ~ that # conflict with the above defined git
-repo url and branch. You should run # `onboardme -s dot_files` to get the files
-that would be overwritten overwrite: false # basic package config package: #
-Remove any of the below pkg managers to only run the remaining pkg managers
-managers: # these are macOS specific steps Darwin: - brew - pip3.11 # these are
-linux specific steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of
-extra existing packages groups to install groups: - default # uncomment these
-to add them as default installed package groups # - gui # - gaming # - devops
-```  ## Under the Hood Made and tested for these operating systems: [![Tested
-on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-
-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-
-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
-wiki/MacOS?lang=en) [![Tested only on Debian Bookworm (debian:bookworm)](https:
-//img.shields.io/badge/Debian-A81D33?style=for-the-
-badge&logo=debian&logoColor=white)](https://www.debian.org/) [![Tested only on
-ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-
-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/) And optomized for the
-following programs: [![made-with-neovim](https://img.shields.io/badge/NeoVim-
-0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
-[![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-
+install --user --upgrade onboardme ``` ### Using the Docker image _Note: For
+fonts and images to work properly, you should use a modern terminal like
+[wezterm](https://wezfurlong.org/wezterm/), iterm2, or konsole as well as you
+need to make sure you [install](https://github.com/ryanoasis/nerd-fonts/tree/
+master#font-installation) a [nerdfont](https://www.nerdfonts.com) and_
+`libsixel` + `imagemagick`. To run the image locally with onboardme installed
+and already run using default settings: ```bash # this image is built daily and
+has already run onboardme with the default settings docker run jessebot/
+onboardme:latest ``` To run the image locally with onbaordme installed but
+_not_ run: ```bash # best if you have your own dot files, or need a smaller
+initial docker image to pull # no packages outside of the required pre-reqs for
+onboardme have been installed docker run jessebot/onboardme:no-install ``` ##
+Running commands _Now_ you can run `onboardme` ð ```bash # this will display
+the help text for onboardme onboardme --help # Running this won't overwrite any
+existing dot files, but it may add new ones. onboardme ``` From here, if you
+want to *completely wipe your existing dot files* for a fresh start with with
+`onboardme`, you can run: ```bash # WARNING: This will overwrite your local
+dotfiles, including your .bashrc and .bash_profile # can also be done with:
+onboardme -O onboardme --overwrite ``` You can read more in depth at the
+[Getting Started Docs] ð! There's also more [docs] on basically every
+program that onboardme touches. ### Upgrades If you're on python 3.11, you
+should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
+Configuration onboardme has lots of CLI options, but you can also use config
+files. You have to create these files for the time being. Config files are in
+`$XDG_CONFIG_HOME/onboardme/`, or `~/.config/onboardme/` if `$XDG_CONFIG_HOME`
+is not defined. | Config File | Description | |:-------------------------------
+-----------|:----------------------------------------------------| |
+`$XDG_CONFIG_HOME/onboardme/config.yml` | For step configuration to run either
+all steps, or just a subset. | | `$XDG_CONFIG_HOME/onboardme/packages.yml` |
+For adding packages with different package managers | Examples:  ~/.config/
+onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
+Creates file if it doesn't exist file: "" # what level of logs to output
+(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
+in the list of functions we run steps: # these are mac specific steps Darwin: #
+clones dot files into home dir/git fetches updates for dot files - dot_files #
+install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
+install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
+# these are linux specific steps Linux: - dot_files - packages - font_setup -
+neovim_setup # add your user to the docker group - group_setup dot_files: #
+personal git repo URL for your dot files, defaults to jessebot/dot_files
+git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
+the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
+reset --hard`, which will overwite/delete local files in ~ that # conflict with
+the above defined git repo url and branch. You should run # `onboardme -
+s dot_files` to get the files that would be overwritten overwrite: false #
+basic package config package: # Remove any of the below pkg managers to only
+run the remaining pkg managers managers: # these are macOS specific steps
+Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
+pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
+install groups: - default # uncomment these to add them as default installed
+package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
+tested for these operating systems: [![Tested on Ventura 13.4 with a 13-inch M1
+Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro]
+(https://img.shields.io/badge/mac%20os-000000?style=for-the-
+badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
+[Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
+badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
+ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
+(https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
+badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
+(https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
 (https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-
 badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
 [![made-with-powerline](https://img.shields.io/badge/powerline-
 000000?style=for-the-badge&logo=powerline&logoColor=#5c983b)](https://
 powerline.readthedocs.io/en/master/overview.html) #### Built using these great
 tools: [[rich python library logo with with yellow snake]](https://github.com/
```

### Comparing `onboardme-1.2.0/onboardme/__init__.py` & `onboardme-1.2.1/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/config/firewall/iptables.sh` & `onboardme-1.2.1/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/console_logging.py` & `onboardme-1.2.1/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/constants.py` & `onboardme-1.2.1/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/dot_files.py` & `onboardme-1.2.1/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/env_config.py` & `onboardme-1.2.1/onboardme/env_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,19 +121,25 @@
                 'steps': {OS[0]: steps},
                 'dot_files': {'overwrite': overwrite,
                               'git_url': repo, 'git_branch': git_branch}}
 
     log.debug(f"cli_dict is:\n{cli_dict}\n")
 
     if OS[0] == 'Darwin':
-        USR_CONFIG_FILE['package']['managers'].pop('Linux')
-        USR_CONFIG_FILE['steps'].pop('Linux')
+        try:
+            USR_CONFIG_FILE['package']['managers'].pop('Linux')
+            USR_CONFIG_FILE['steps'].pop('Linux')
+        except KeyError:
+            pass
     else:
-        USR_CONFIG_FILE['package']['managers'].pop('Darwin')
-        USR_CONFIG_FILE['steps'].pop('Darwin')
+        try:
+            USR_CONFIG_FILE['package']['managers'].pop('Darwin')
+            USR_CONFIG_FILE['steps'].pop('Darwin')
+        except KeyError:
+            pass
 
     log.debug(f"🗂 ⚙️  user_config_file: \n{USR_CONFIG_FILE}\n")
     final_defaults = fill_in_defaults(cli_dict, USR_CONFIG_FILE, True)
 
     log.debug(" final config after filling cli_dict in with defaults:\n"
               f"{final_defaults}\n")
```

### Comparing `onboardme-1.2.0/onboardme/firewall.py` & `onboardme-1.2.1/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/help_text.py` & `onboardme-1.2.1/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/ide_setup.py` & `onboardme-1.2.1/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/misc.py` & `onboardme-1.2.1/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/pkg_management.py` & `onboardme-1.2.1/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/subproc.py` & `onboardme-1.2.1/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/onboardme/sudo_setup.py` & `onboardme-1.2.1/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.0/pyproject.toml` & `onboardme-1.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.2.0"
+version       = "1.2.1"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
@@ -30,20 +30,14 @@
 GitPython           = "^3.1"
 wget                = "^3.2"
 xdg-base-dirs       = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1"
 
-[[tool.poetry.source]]
-name      = "testpypi"
-url       = "https://test.pypi.org/simple/"
-default   = false
-secondary = false
-
 [tool.poetry.plugins."onboardme.application.plugin"]
 "onboardme" = "onboardme:main"
 
 [tool.poetry.scripts]
 onboardme = 'onboardme:main'
 
 [tool.poetry.urls]
```

### Comparing `onboardme-1.2.0/PKG-INFO` & `onboardme-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.2.0
+Version: 1.2.1
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Installation/Setup
 Requires-Dist: GitPython (>=3.1,<4.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: rich (>=13.3,<14.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
@@ -45,14 +44,18 @@
   <a href="https://github.com/jessebot/onboardme/releases">
     <img src="https://img.shields.io/github/v/release/jessebot/onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white">
   </a>
 </p>
 
 Get your daily driver just the way you like it, from dot files management, to package installation, to other little features you didn't know you needed, `onboardme` intends to save you time with initializing and maintaining your personal environments.
 
+<p align="center">
+<img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/image_in_terminal.png' alt='screenshot of color samples and image of dog using a computer using sixel'>
+</p>
+
 ## Features
 
 ### Keep your Dot Files Up To Date Across multiple systems
 `onboardme` can manage your [dot files] using a git by turning your home directory into a repo.
 
 <details>
   <summary>We provide default dot files, so you don't have to manage them</summary>
@@ -92,21 +95,21 @@
 </details>
 
 ### Easy `yaml` config files
 [XDG Base Directory Spec] use for [config files](#configuration)
 
 ### Docker image for an on-the-go dev workspace
 
-The docker image is built daily or on push to main. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
+The docker image is built nightly, and on push to `main` via GHA. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
 See the [docker](#docker) section for more info!
 
 ### Other optional configurations
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
-- Install nerdfonts (defaults to mononoki and Symbols Only)
+- Install [nerdfonts](https://www.nerdfonts.com) (defaults to mononoki and Symbols Only)
 
 ### Screenshots
 
 <details>
   <summary>Example of <code>onboardme --help</code></summary>
 
 <p align="center" width="100%">
@@ -128,15 +131,15 @@
 ### Powerline and ls
 <img width="80%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/ls_tree_examples.png' alt='screenshot of powerline and lsd'>
 
 ### Powerline with git
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/git_powerline_example.png' alt='screenshot of powerline and git colors'>
 
 ### Image and colors
-<img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/image_in_terminal.png' alt='screenshot of color samples and image of dog using a computer using sixel'>
+
 
 ### Python virtual env in powerline and cat
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/python_virtual_env_example.png' alt='screenshot of using bat and python virtual env in powerline'>
 </p>
 
 </details>
 
@@ -212,14 +215,16 @@
 ```bash
 # should also work with pipx, if you'd like to use that instead
 pip install --user --upgrade onboardme
 ```
 
 ### Using the Docker image
 
+_Note: For fonts and images to work properly, you should use a modern terminal like [wezterm](https://wezfurlong.org/wezterm/), iterm2, or konsole as well as you need to make sure you [install](https://github.com/ryanoasis/nerd-fonts/tree/master#font-installation) a [nerdfont](https://www.nerdfonts.com) and_ `libsixel` + `imagemagick`.
+
 To run the image locally with onboardme installed and already run using default settings:
 
 ```bash
 # this image is built daily and has already run onboardme with the default settings
 docker run jessebot/onboardme:latest
 ```
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.2.0 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.2.1 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: System ::
-Installation/Setup Requires-Dist: GitPython (>=3.1,<4.0) Requires-Dist: PyYAML
-(>=6.0,<7.0) Requires-Dist: click (>=8.1,<9.0) Requires-Dist: rich
-(>=13.3,<14.0) Requires-Dist: wget (>=3.2,<4.0) Requires-Dist: xdg-base-dirs
-(>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/jessebot/onboardme/
-issues Project-URL: Documentation, https://jessebot.github.io/onboardme/
-onboardme Project-URL: Repository, http://github.com/jessebot/onboardme
-Description-Content-Type: text/markdown
+Topic :: System :: Installation/Setup Requires-Dist: GitPython (>=3.1,<4.0)
+Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: click (>=8.1,<9.0) Requires-
+Dist: rich (>=13.3,<14.0) Requires-Dist: wget (>=3.2,<4.0) Requires-Dist: xdg-
+base-dirs (>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/jessebot/
+onboardme/issues Project-URL: Documentation, https://jessebot.github.io/
+onboardme/onboardme Project-URL: Repository, http://github.com/jessebot/
+onboardme Description-Content-Type: text/markdown
   ***** [https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/
    misc/transparent.png] ð» onboardme [https://raw.githubusercontent.com/
          catppuccin/catppuccin/main/assets/misc/transparent.png] *****
               [https://img.shields.io/github/v/release/jessebot/
 onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white]
 GetÂ yourÂ dailyÂ driverÂ justÂ theÂ wayÂ youÂ likeÂ it,Â fromÂ dotÂ files
 management,Â toÂ packageÂ installation, to other little features you didn't
 know you needed,Â `onboardme` intends to save
 youÂ timeÂ withÂ initializingÂ andÂ maintainingÂ yourÂ personal environments.
+  [screenshot of color samples and image of dog using a computer using sixel]
 ## Features ### Keep your Dot Files Up To Date Across multiple systems
 `onboardme` can manage your [dot files] using a git by turning your home
 directory into a repo.  We provide default dot files, so you don't have to
 manage them - The [default dot files] are open source, and the maintainers use
 these themselves - They cover a lot of common apps/tools you probably want
 anyway - They have consistent colorschemes accross different CLI/TUI programs
 ð - They set all the helpful BASH aliases you could need (zsh support coming
@@ -48,26 +48,26 @@
 D We used to support both neovim _and_ vim, but these days none of the primary
 developers of this repo use pure vim anymore, so we can't ensure it's up to
 standards. All of your knowledge from vim is still helpful in neovim though,
 and we highly recommend switching as neovim has a lot more features and a very
 active plugin community :) NeoVim maintains a guide on how to switch from vim
 [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml`
 config files [XDG Base Directory Spec] use for [config files](#configuration)
-### Docker image for an on-the-go dev workspace The docker image is built daily
-or on push to main. The base image is `debian:bookworm`, but we will rollout
-support for Ubuntu down the line :) See the [docker](#docker) section for more
-info! ### Other optional configurations - Enable touchID for sudo on macOS -
-Add your user to the docker group - Install nerdfonts (defaults to mononoki and
-Symbols Only) ### Screenshots  Example of onboardme --help
+### Docker image for an on-the-go dev workspace The docker image is built
+nightly, and on push to `main` via GHA. The base image is `debian:bookworm`,
+but we will rollout support for Ubuntu down the line :) See the [docker]
+(#docker) section for more info! ### Other optional configurations - Enable
+touchID for sudo on macOS - Add your user to the docker group - Install
+[nerdfonts](https://www.nerdfonts.com) (defaults to mononoki and Symbols Only)
+### Screenshots  Example of onboardme --help
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
-  colors] ### Image and colors [screenshot of color samples and image of dog
-  using a computer using sixel] ### Python virtual env in powerline and cat
+   colors] ### Image and colors ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
  # Quick Start ### Install Locally You'll need `curl`, `brew`, `git`, and
 Python 3.11 to get started. We have a setup script to install those (except
 `curl`) and help you get your environment to the XDG spec under Locally or you
 can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/
 jessebot/onboardme).  Local prereq install script  curl, a pre-prereq ```bash #
 First, make sure you have curl, but it *should* be there already be on macOS. #
@@ -87,72 +87,77 @@
 this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
 opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
 (whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
 >> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
 you can also set the shell directly in your terminal app via the settings.  If
 you've already got all the above prereq on your machine, you can just do:
 ```bash # should also work with pipx, if you'd like to use that instead pip
-install --user --upgrade onboardme ``` ### Using the Docker image To run the
-image locally with onboardme installed and already run using default settings:
-```bash # this image is built daily and has already run onboardme with the
-default settings docker run jessebot/onboardme:latest ``` To run the image
-locally with onbaordme installed but _not_ run: ```bash # best if you have your
-own dot files, or need a smaller initial docker image to pull # no packages
-outside of the required pre-reqs for onboardme have been installed docker run
-jessebot/onboardme:no-install ``` ## Running commands _Now_ you can run
-`onboardme` ð ```bash # this will display the help text for onboardme
-onboardme --help # Running this won't overwrite any existing dot files, but it
-may add new ones. onboardme ``` From here, if you want to *completely wipe your
-existing dot files* for a fresh start with with `onboardme`, you can run:
-```bash # WARNING: This will overwrite your local dotfiles, including your
-.bashrc and .bash_profile # can also be done with: onboardme -O onboardme --
-overwrite ``` You can read more in depth at the [Getting Started Docs] ð!
-There's also more [docs] on basically every program that onboardme touches. ###
-Upgrades If you're on python 3.11, you should be able to do: ```bash pip3.11
-install --upgrade onboardme ``` ### Configuration onboardme has lots of CLI
-options, but you can also use config files. You have to create these files for
-the time being. Config files are in `$XDG_CONFIG_HOME/onboardme/`, or
-`~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined. | Config File |
-Description | |:------------------------------------------|:-------------------
----------------------------------| | `$XDG_CONFIG_HOME/onboardme/config.yml` |
-For step configuration to run either all steps, or just a subset. | |
-`$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different
-package managers | Examples:  ~/.config/onboardme/config.yml ```yaml log: #
-Full path to a file you'd like to log to. Creates file if it doesn't exist
-file: "" # what level of logs to output (DEBUG, INFO, WARN, ERROR) level:
-"INFO" # steps refer to a specific function in the list of functions we run
-steps: # these are mac specific steps Darwin: # clones dot files into home dir/
-git fetches updates for dot files - dot_files # install packages - packages #
-adds nerdfonts - font_setup # runs :Lazy sync to install all your plugins -
-neovim_setup # sets up touchID for sudo - sudo_setup # these are linux specific
-steps Linux: - dot_files - packages - font_setup - neovim_setup # add your user
-to the docker group - group_setup dot_files: # personal git repo URL for your
-dot files, defaults to jessebot/dot_files git_url: "https://github.com/
-jessebot/dot_files.git" # the branch to use for the git repo above, defaults to
-main git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will
-overwite/delete local files in ~ that # conflict with the above defined git
-repo url and branch. You should run # `onboardme -s dot_files` to get the files
-that would be overwritten overwrite: false # basic package config package: #
-Remove any of the below pkg managers to only run the remaining pkg managers
-managers: # these are macOS specific steps Darwin: - brew - pip3.11 # these are
-linux specific steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of
-extra existing packages groups to install groups: - default # uncomment these
-to add them as default installed package groups # - gui # - gaming # - devops
-```  ## Under the Hood Made and tested for these operating systems: [![Tested
-on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-
-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-
-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
-wiki/MacOS?lang=en) [![Tested only on Debian Bookworm (debian:bookworm)](https:
-//img.shields.io/badge/Debian-A81D33?style=for-the-
-badge&logo=debian&logoColor=white)](https://www.debian.org/) [![Tested only on
-ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-
-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/) And optomized for the
-following programs: [![made-with-neovim](https://img.shields.io/badge/NeoVim-
-0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
-[![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-
+install --user --upgrade onboardme ``` ### Using the Docker image _Note: For
+fonts and images to work properly, you should use a modern terminal like
+[wezterm](https://wezfurlong.org/wezterm/), iterm2, or konsole as well as you
+need to make sure you [install](https://github.com/ryanoasis/nerd-fonts/tree/
+master#font-installation) a [nerdfont](https://www.nerdfonts.com) and_
+`libsixel` + `imagemagick`. To run the image locally with onboardme installed
+and already run using default settings: ```bash # this image is built daily and
+has already run onboardme with the default settings docker run jessebot/
+onboardme:latest ``` To run the image locally with onbaordme installed but
+_not_ run: ```bash # best if you have your own dot files, or need a smaller
+initial docker image to pull # no packages outside of the required pre-reqs for
+onboardme have been installed docker run jessebot/onboardme:no-install ``` ##
+Running commands _Now_ you can run `onboardme` ð ```bash # this will display
+the help text for onboardme onboardme --help # Running this won't overwrite any
+existing dot files, but it may add new ones. onboardme ``` From here, if you
+want to *completely wipe your existing dot files* for a fresh start with with
+`onboardme`, you can run: ```bash # WARNING: This will overwrite your local
+dotfiles, including your .bashrc and .bash_profile # can also be done with:
+onboardme -O onboardme --overwrite ``` You can read more in depth at the
+[Getting Started Docs] ð! There's also more [docs] on basically every
+program that onboardme touches. ### Upgrades If you're on python 3.11, you
+should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
+Configuration onboardme has lots of CLI options, but you can also use config
+files. You have to create these files for the time being. Config files are in
+`$XDG_CONFIG_HOME/onboardme/`, or `~/.config/onboardme/` if `$XDG_CONFIG_HOME`
+is not defined. | Config File | Description | |:-------------------------------
+-----------|:----------------------------------------------------| |
+`$XDG_CONFIG_HOME/onboardme/config.yml` | For step configuration to run either
+all steps, or just a subset. | | `$XDG_CONFIG_HOME/onboardme/packages.yml` |
+For adding packages with different package managers | Examples:  ~/.config/
+onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
+Creates file if it doesn't exist file: "" # what level of logs to output
+(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
+in the list of functions we run steps: # these are mac specific steps Darwin: #
+clones dot files into home dir/git fetches updates for dot files - dot_files #
+install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
+install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
+# these are linux specific steps Linux: - dot_files - packages - font_setup -
+neovim_setup # add your user to the docker group - group_setup dot_files: #
+personal git repo URL for your dot files, defaults to jessebot/dot_files
+git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
+the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
+reset --hard`, which will overwite/delete local files in ~ that # conflict with
+the above defined git repo url and branch. You should run # `onboardme -
+s dot_files` to get the files that would be overwritten overwrite: false #
+basic package config package: # Remove any of the below pkg managers to only
+run the remaining pkg managers managers: # these are macOS specific steps
+Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
+pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
+install groups: - default # uncomment these to add them as default installed
+package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
+tested for these operating systems: [![Tested on Ventura 13.4 with a 13-inch M1
+Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro]
+(https://img.shields.io/badge/mac%20os-000000?style=for-the-
+badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
+[Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
+badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
+ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
+(https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
+badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
+(https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
 (https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-
 badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
 [![made-with-powerline](https://img.shields.io/badge/powerline-
 000000?style=for-the-badge&logo=powerline&logoColor=#5c983b)](https://
 powerline.readthedocs.io/en/master/overview.html) #### Built using these great
 tools: [[rich python library logo with with yellow snake]](https://github.com/
```


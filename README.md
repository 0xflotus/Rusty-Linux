# Rusty Linux
Simple script to install basic Rust apps as alternative to default one

## Why?
Most linux tools are written in C(and C++) for performance and history reasons.

This language is still very popular, but I know from experience that it is very easy to make a mistake in it, which results in memory integrity violation, often resulting in program shutdown, or even worse, in data corruption or leaks.

One of the potential solutions to these problems is to use Rust language providing comparable performance, offering elimination of many types of typical bugs already at the compilation stage.

Although rewriting software from C(or similar) may initially require a lot of work, when adding new features, the programmer will be able to save time on detecting memory corruption (address sanitizer, valgrind) or memory leaks (leak sanitizer, valgrind).

Creating memory safe and big application(>100K code) in C language is almost impossible because every bigger change brings a huge amount of bugs (Rust from all of them will of course magically not protect) - look at the recent Wine refactoring for more info.

## Install apps
To install apps you need just download this script and run
```
wget https://raw.githubusercontent.com/qarmin/Rusty-Linux/main/RustyLinux.sh
chmod +x RustyLinux.sh
./RustyLinux.sh
```
## Upgrade
To upgrade apps, just run again script.  
This will install only newer version of packages.


## List of apps with replacements  
- exa - ls
- sd - sed
- amp - vim
- coreutils uutils - coreutils
- bat - cat
- ripgrep - grep
- dust - du
- fd - find
- lolcate - locate
- websocat - curl
- procs - ps
- bottom - top
- choose - cut/awk
- zenith - htop
- alacritty - terminal
- tokei - cloc
- emulsion - image viewer
- process viewer - system monitor
- gxi - text editor
- popsicle - Etcher
- Czkawka - FSlint

## Contribute
If you know about some good Rust appliaction for Linux, which is alternative to existing one, please create pull-request or new issue about it.

This applications should be active and newest commit should be younger than 1 year.

I failed to find Rust applications from this category:
- Video player
- Music/Audio player

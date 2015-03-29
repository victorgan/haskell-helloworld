https://github.com/bos/stanford-cs240h

following: https://wiki.haskell.org/How_to_write_a_Haskell_program#Structure_of_a_simple_project
Structure of a simple project
     Haq.hs -- the main haskell source file
    haq.cabal -- the cabal build description
    Setup.hs -- build script itself
    .git -- revision control
    README -- info
    LICENSE -- license 

Also see this for a more advanced structure:
https://wiki.haskell.org/Structure_of_a_Haskell_project

# Getting Haskell up and running on Ubuntu 14.04

> echo "Installing Haskell"
> sudo apt-get install haskell-platform -y
> 
> echo "Updating Cabal"
> cabal update && cabal install cabal-install -y

Add to .bashrc:

> # Local cabal (for haskell) install. If exists, use it.
> if [ -d "$HOME/.cabal/bin" ] ; then
>     PATH=$HOME/.cabal/bin:$PATH
> fi


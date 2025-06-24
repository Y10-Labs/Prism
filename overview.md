# PrisM
Repository for PrisM, a custom FPGA-based handheld gaming console, built from scratch.


## Working with submodules
To work on this project, first clone the repo with submodules

```bash
    git clone --recurse-submodules --remote-submodules https://github.com/Y10-Labs/Prism
```

If you previously cloned this repo, without recurse submodules

```bash
    git fetch
    git pull
    git submodule update --init --recursive
```


If you are working on a submodule (Ex: Prism-SW), 

```bash
    cd Prism-SW
    git checkout main
```

And make changes.

When you are done making changes, 

```bash
    git add .
    git commit -m "Commit Message"
    git push
```

Then 
```bash
    cd ../ # Back to the project root
    git checkout main
    git submodule update 
    git add .
    git commit -m "Changed submodule X"
    git push
```
# Download Anaconda2

**Might need to replace $HOME with my home directory**

```python
# wget -S -T 10 -t 5 https://repo.continuum.io/archive/Anaconda2-4.4.0-Linux-x86_64.sh -O $HOME/anaconda.sh
# - OR - #
# Download Anaconda3
wget -S -T 10 -t 5 https://repo.continuum.io/archive/Anaconda3-4.4.0-Linux-x86_64.sh -O $HOME/anaconda.sh
```

# Install Anaconda
`bash $HOME/anaconda.sh -b -p $HOME/anaconda`

# Add Anaconda to current session's PATH
`export PATH=$HOME/anaconda/bin:$PATH`

# Add Anaconda to PATH for future sessions via .bashrc
`echo -e "\n\n# Anaconda" >> $HOME/.bashrc`
`echo "export PATH=$HOME/anaconda/bin:$PATH" >> $HOME/.bashrc`

# Update to the current version
`conda update conda`
`conda update anaconda`

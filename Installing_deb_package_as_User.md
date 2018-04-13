#Installing a .deb package

<par>Download the package from [packages](https://packages.debian.org)</par>
<par>Create (if they do not exist) the folders system, the Then unpak the .deb</par>
```bash
mkdir ~/local
mkdir ~/local/bin
mkdir ~/local/lib
mkdir ~/local/include
dpkg-deb -x <filename.deb> dir/
```
<par>And copy the libraries to lib, and the binaries to binn</par>
<par>Then modify the .bashrc to use this binaries, adding this lines</par>

```bash
export PATH=$PATH:$HOME/local/bin
#export PATH=$PATH:$HOME/local/lib
```

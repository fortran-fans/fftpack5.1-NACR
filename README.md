FFTPACK 5.1 NCAR Version

## Get Start
```bash
git clone https://github.com/fortran-fans/fftpack5.1-NCAR.git
cd fftpack5.1-NCAR
```
### Supported Compilers
The following combinations are tested on the default branch of `fftpack`:  
|Name|Vesrion|Platform|Architecture|  
|---|---|---|---|  
|GCC Fortran(MSYS2)|10.3|Windows 10|x86_64|

## Build with FPM
You can build using provided `fpm.toml`: 
```
fpm build --flag "-fallow-argument-mismatch -fdefault-real-8"
fpm test --flag "-fallow-argument-mismatch -fdefault-real-8"
```
You can use this package in your fpm porject, notice it is **with a FFTPack Software License**.  
Add the following to your fpm project `fpm.toml`.
```toml
[dependencies]
fftpack = { git="https://github.com/fortran-fans/fftpack5.1-NCAR.git" }
```

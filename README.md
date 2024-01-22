## Getting Started

Before you begin, make sure you are familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

### Downloading Source Code

Clone the source code repository and set up the Android build environment:

```bash
git clone https://github.com/akhilnarang/scripts && cd scripts/setup && bash android_build_env.sh
```

Initialize your local repository and sync up:

```bash
repo init -u https://github.com/DotOS-RV/manifest -b dot11
```

### Compilation

Navigate to the root directory of the project and execute the following commands in the terminal to start the compilation:

```bash
source build/envsetup.sh
lunch dot_<devicecodename>-userdebug
make bacon -j$(nproc --all)
```

## Credits

Special thanks to the following projects for their contributions:

- [**AOSP**](https://android.googlesource.com)
- [**DotOS**](https://github.com/DotOS)
- [**LineageOS**](https://github.com/LineageOS)
- [**DirtyUnicorns**](https://github.com/dirtyunicorns)
- [**PixelExperience**](https://github.com/PixelExperience)

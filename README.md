# ForceCloseOreUI

Force close OreUI

## How to use

1. Extract libminecraftpe.so from the Minecraft APK.
2. Download or manually compile the .so files from the [releases](https://github.com/Yejdhi/ForceCloseOreUI-Android/releases/latest).
3. Download [patchelf](https://github.com/NixOS/patchelf/releases/latest).
4. For 32 bit (armeabi-v7a) Minecraft run the following command:

```
patchelf --add-needed libForceCloseOreUI-arm.so libminecraftpe.so
```

5. For 64 bit (arm-v8a) Minecraft run the following command:

```
patchelf --add-needed libForceCloseOreUI-arm64.so libminecraftpe.so
```

7. Put the modified **libminecraftpe.so** and **libForceCloseOreUI.so** file back into the apk
8. Sign and install.

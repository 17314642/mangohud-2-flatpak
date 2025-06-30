# MangoHUD 

## Building
1. ```
   apt install flatpak-builder appstream
   ```
2. ```
   flatpak install org.freedesktop.Sdk.Compat.i386/x86_64/24.08
   ```
3. ```
   flatpak install org.freedesktop.Sdk.Extension.toolchain-i386/x86_64/24.08
   ```
4. ```
   flatpak-builder --user --install --force-clean build org.freedesktop.Platform.VulkanLayer.MangoHud.yml
   ```

## Configuration

MangoHud can be configured just like the [instructions](https://github.com/flightlessmango/MangoHud#hud-configuration) mentioned by the project, but you must give Flatpak apps access to the configuration files. That can be done with the following command:

```
flatpak override --user --filesystem=xdg-config/MangoHud:ro
```

## Resources

- [MangoHUD Homepage](https://github.com/flightlessmango/MangoHud)

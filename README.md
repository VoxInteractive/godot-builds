# Unofficial Daily Builds Of The Godot Game Engine 

All builds are compiled in release mode with compile-time optimisations turned on.

# Downloading

Go to the [Actions tab](https://github.com/VoxInteractive/godot-builds/actions) and click on the latest build at the top. At the bottom of the page under Artifacts, you should see a download button for each platform and build type. Note that you must be logged in to Github to see the download buttons.

## Editor

Built with all modules and features.

## Export Templates

Slimmed down builds of the export templates with many modules and features disabled. Notably;
- 3D rendering and physics,
- Multiplayer,
- XR
are disabled.

### Encryption

Export templates have encryption enabled, with an auto-generated key unique to each build and platform. You can find the encryption key inside the `encryption-key.txt` file included in the package .zip. You will need to set this encryption key in your project's export settings before export, and include the files to be encrypted. For more information, please see [the official documentation](https://docs.godotengine.org/en/latest/engine_details/development/compiling/compiling_with_script_encryption_key.html).

Keep in mind however, that this encryption can be defeated very easily using publicly available tools and basic reverse engineering methods, and the fact that the keys are publicly visible inside the package archives and build logs don't make it any more secure either. In the end, this only makes the decryption of your released games slightly less convenient.

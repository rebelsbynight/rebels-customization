# Rebels Collection Customization

Welcome to the Rebels Collection Customization repository! This guide will help you, whether you're technically inclined or not, to generate custom 3D renders of Rebels. We'll guide you through every step!

## Table of Contents
1. [Getting Started](#getting-started)
2. [Customizing Asset Colors, Materials, and Textures](#customizing-asset-colors-materials-and-textures)
3. [Balaclava Customization](#balaclava-customization)
4. [Adding New 3D Assets](#adding-new-3d-assets)
5. [Scripts Documentation](#scripts-documentation)

## Getting Started
### Clone the Repository
To begin, you'll want to clone this repository to your local machine:

```
git clone https://github.com/rebelsbynight/rebels-customization
cd rebels-customization
```

### Install Necessary Tools and Dependencies
#### Python3
Make sure you have Python3 installed on your machine. If not, you can download it from the official [Python website](https://www.python.org/downloads/).

#### Blender 3.1.2
To handle our 3D files, install Blender 3.1.2. You can download it from the [Blender website](https://www.blender.org/download/previous-versions/).

#### Homebrew (macOS only)
If you're on macOS, install Homebrew:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Download and Unzip the Rebels 3D Files
Next, download the 3D files from the following link:
[Download Rebels 3D files](FIXME)

After downloading, unzip the archive:

```
unzip Rebels-Collection.zip
```

## Customizing Asset Colors, Materials, and Textures
1. [Download the Rebels Patches 3D files](FIXME)
2. Unzip the `Rebels-Collection.zip` archive.
3. Navigate to `Rebels-Collection/3D FILES/Color Palette`.
4. Duplicate one of the blender files (e.g., `49.blend`).
5. Edit the textures for each material in the color palette.

Run the following command to generate your custom Rebel:

### macOS:
```
/Applications/Blender.app/Contents/MacOS/Blender -b "Rebels-Collection/3D FILES/render_file_optimized.blend" --engine BLENDER_EEVEE -o . -P gen-custom-color-rebel.py -- new_collection_map.json <custom_color_palette> <rebel_id>
```

### Linux:
```
blender -b "Rebels-Collection/3D FILES/render_file_optimized.blend" --engine BLENDER_EEVEE -o . -P gen-custom-color-rebel.py -- new_collection_map.json <custom_color_palette> <rebel_id>
```

## Balaclava Customization
Customize the balaclava with the image of your choice using the following commands:

### macOS:
```
/Applications/Blender.app/Contents/MacOS/Blender -b "Rebels-Collection/3D FILES/render_file_optimized-custom-bala.blend" --engine BLENDER_EEVEE -o . -P balaclava-customization.py -- new_collection_map.json <balaclava_image> <rebel_id>
```

### Linux:
```
blender -b "Rebels-Collection/3D FILES/render_file_optimized-custom-bala.blend" --engine BLENDER_EEVEE -o . -P balaclava-customization.py -- new_collection_map.json <balaclava_image> <rebel_id>
```

## Adding New 3D Assets
To add new 3D assets like masks, clothing, or backgrounds:

1. Add your asset to the appropriate blender file (`mask_3.blend`, `background.blend`, or `cloth_2.blend`).
2. Update the `rebels_data.json` file located in `Rebels-Collection/scripting` with the asset details.

## Scripts Documentation
Dive deeper into the code! Check the `balaclava-customization.py` script to understand the customization process more thoroughly. If you're looking to contribute, understanding this script is a good starting point.

## Feedback & Contributions
Feedback and contributions are always welcome! Feel free to open an issue or submit a pull request.

## License
The code and 3D files can used in any way you'd like so long as it's applied for the Rebels project and Rebels NFTs, any other use is prohibited.

Happy Rendering!


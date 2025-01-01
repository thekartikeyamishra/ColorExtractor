# ColorExtractor

A Python-based project that extracts the dominant colors from an image using the KMeans clustering algorithm. This project is useful for applications like image processing, color palette generation, or analyzing the most prominent colors in images.

## Features

- Extract dominant colors from any image.
- Visualize the color palette as an output.
- Adjustable number of dominant colors (`n_colors`).

## Requirements

- Python 3.7 or higher
- Libraries:
  - `numpy`
  - `matplotlib`
  - `Pillow`
  - `scikit-learn`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/thekartikeyamishra/ColorExtractor.git
   cd ColorExtractor
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Place the image you want to process in the project directory.

2. Update the image file name in the code (`image_path` variable) to the image you want to process:
   ```python
   image_path = 'your-image.png'  # Replace with your image file name
   ```

3. Run the script:
   ```bash
   python ColorExtractor.py
   ```

4. The script will display the dominant color palette as an image.

## Code Explanation

1. **Load and Preprocess the Image**:
   The image is loaded using the `Pillow` library and converted to an RGB format for compatibility.

2. **Reshape Image for Clustering**:
   The 3D image array is flattened into a 2D array of pixels for clustering.

3. **KMeans Clustering**:
   The `KMeans` algorithm from `scikit-learn` is used to group similar colors into `n_colors` clusters. The centroids of these clusters represent the dominant colors.

4. **Display the Color Palette**:
   The dominant colors are displayed as a horizontal bar for visualization.


## Adjustable Parameters

- `n_colors`: Number of dominant colors to extract. Default is 6.
- `image_path`: Path to the input image file.

## Troubleshooting

- **Colors look incorrect**:
  - Ensure the image is in RGB format.
  - Try increasing or decreasing `n_colors` for better results.

- **Error in loading the image**:
  - Verify the image file path and format.
  - Use common image formats like `.png` or `.jpg`.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for bug fixes, improvements, or feature suggestions.

## Contact

For questions or feedback, please contact:

- **Author**: Kartikeya Mishra
- **GitHub**: [your-username](https://github.com/thekartikeyamishra)



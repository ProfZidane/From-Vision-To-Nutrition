# Towards Camera-Based Caloric Estimation via Visual Captioning and Lightweight Reasoning

## Overview

This project explores camera-based caloric estimation using visual captioning and lightweight reasoning techniques. The research leverages the comprehensive Nutrition5k dataset to develop models that can estimate the caloric content of food dishes from overhead camera images.

## Dataset

This project utilizes the **Nutrition5k** dataset, a comprehensive nutrition dataset developed by Google Research.

### Dataset Information
- **Source**: [Nutrition5k GitHub Repository](https://github.com/google-research-datasets/Nutrition5k)
- **Storage**: [Google Cloud Storage](https://console.cloud.google.com/storage/browser/nutrition5k_dataset)
- **Content**: Over 5,000 food dishes with detailed nutritional information
- **Images**: Overhead RGB-D images captured using RealSense cameras
- **Annotations**: Mass, calories, macronutrients (fat, carbs, protein), and ingredient-level information

### Dataset Structure
The dataset includes:
- **Imagery**: Overhead RealSense camera captures
- **Metadata**: Dish-level nutritional information (CSV format)
- **Ingredients**: Detailed ingredient composition and nutritional breakdown
- **Nutritional Values**: Total mass, calories, fat, carbohydrates, and protein content

## Project Structure

```
image_2_mass/
├── eda.ipynb              # Exploratory Data Analysis
├── dish_metadata_cafe1.csv # Nutritional data for cafe 1
├── dish_metadata_cafe2.csv # Nutritional data for cafe 2
└── imagery/
    └── realsense_overhead/ # Overhead camera images
```

## Features

- **Visual Analysis**: Process overhead food images for caloric estimation
- **Nutritional Mapping**: Extract detailed nutritional information from the Nutrition5k dataset
- **Data Exploration**: Comprehensive analysis of food composition and caloric distribution
- **Ingredient Recognition**: Identify and analyze individual food components

## Getting Started

### Prerequisites

```python
matplotlib
numpy
PIL (Pillow)
tensorflow
pandas
keras
```

### Installation

1. Clone this repository
2. Install required dependencies:
   ```bash
   pip install matplotlib numpy pillow tensorflow pandas
   ```
3. Download the Nutrition5k dataset from the official sources
4. Update the data paths in the configuration

### Usage

1. **Data Exploration**: Start with `eda.ipynb` to explore the dataset structure and nutritional distributions
2. **Image Processing**: Load and preprocess overhead food images
3. **Model Training**: Develop visual captioning and reasoning models for caloric estimation

## Research Objectives

- Develop accurate camera-based caloric estimation methods
- Implement visual captioning techniques for food recognition
- Create lightweight reasoning systems for nutritional analysis
- Evaluate performance on real-world food imagery

## Dataset Citation

If you use the Nutrition5k dataset in your research, please cite:

```bibtex
@inproceedings{thames2021nutrition5k,
  title={Nutrition5k: Towards Automatic Nutritional Understanding of Generic Food},
  author={Thames, Quin and Karpur, Arjun and Norris, Wade and Xia, Fei and Panait, Liviu and Weyand, Tobias and Sim, Jack},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={8903--8911},
  year={2021}
}
```

## License

This project follows the licensing terms of the Nutrition5k dataset. Please refer to the [official repository](https://github.com/google-research-datasets/Nutrition5k) for detailed licensing information.

## Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests to improve the project.

## Contact

For questions or collaboration opportunities, please open an issue in this repository.
# Multi Animals Image Classification

This project utilizes the **Pixabay API** to download images of various animals, specifically **cats**, **dogs**, and **horses**.

Once the images are gathered, they are preprocessed and used for training a **deep learning model**. The trained model can then accurately classify whether an image contains a cat, dog, or horse, enabling automated animal recognition in images.

## Future Development

The project is an extension of the **Dogs vs. Cats Image Classification** initiative. Future enhancements will focus on expanding the classification capabilities to include a broader range of animal species. This will involve refining the neural networks to improve their accuracy and performance in recognizing additional animal categories.

For more details, check out the [Dogs vs. Cats Image Classification project on GitHub](https://github.com/do-martin/Dogs-vs-Cats-Image-Classification).

## Features

- Download images from the Pixabay API
- Preprocess images for model training
- Train a deep learning model for classification
- Classify images into three categories: **cat**, **dog**, or **horse**

## Required Libraries

- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Requests
- PIL (Pillow)
- Dotenv

You can find the specific library versions in the `requirements.txt` file.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.x
- pip (Python package installer)

### Clone the Repository

```bash
git clone https://github.com/do-martin/Multi_Animal_Image_Classification.git
cd Multi_Animal_Image_Classification
```

### Install Required Packages

It is recommended to create a virtual environment first. Ensure that you have Python 3.11 or below installed:

#### Your default Python version is 3.11 or below: 

```bash
python -m venv env
env\Scripts\activate
pip install -r requirements.txt
```

#### Alternative: Specify the path to Python 3.11:

```bash
C:\Path\to\python311\python.exe -m venv env
env\Scripts\activate
pip install -r requirements.txt
```

## Usage

The project is implemented in a Jupyter Notebook (.ipynb). Open the notebook in Jupyter Lab, Jupyter Notebook, or Visual Studio Code (VSCode) to explore and run the code.

1. **Create `.env` File**: Create a file named `.env` in the project directory. Add the following line to the file:
API_KEY=<your_pixabay_api_key>

2. **Download Images**: First, execute the `Image_Downloader.ipynb` notebook to download the images from the Pixabay API.

3. **Run Classification**: After the download is complete, run the `Multi-Animals-Image-Classification.ipynb` notebook.

> **Note**: Ensure that you have sufficient data in your image set to train the neural network effectively. It is recommended to have at least **12,000 images** for each category/class to achieve optimal training results.

## Model Evaluation

To facilitate an accurate assessment of the model's performance, please ensure that the folder named `validation_images` is present. This folder should contain a diverse set of images featuring dogs, cats, and horses. These images are intended for testing the model and should not be utilized during the training phase.

## Guidelines for Sample Images

- The images should be in JPEG or PNG format.
- Ensure that each image name is unique to avoid any confusion.

Use these images exclusively for testing the model with your own pictures.

## API Usage

The usage of the Pixabay API is subject to the terms and conditions set forth by Pixabay. Please ensure that you review and comply with these guidelines when using the API for your projects. You can find the full terms and conditions [here](https://pixabay.com/api/docs/#terms).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Special thanks to the developers of TensorFlow and Keras for their contributions to the field of deep learning.
- Inspiration from various Kaggle competitions that focus on image classification.
- A heartfelt thank you to Pixabay for providing a rich repository of images that made this project possible.
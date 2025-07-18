# Hypervelocity Impact Detection and Classification for Satellite Structural Integrity

## Project Overview

This repository contains the codebase and resources for a project focused on detecting and classifying hypervelocity impacts on satellite structures. This project aims to contribute to the monitoring and maintenance of satellite structural integrity by providing tools for automated damage assessment.

## Key Features & Benefits

*   **Hypervelocity Impact Detection:** Implements algorithms for identifying potential impact events.
*   **Damage Classification:** Categorizes the type and severity of detected damage.
*   **Automated Analysis:** Provides a framework for automated damage assessment.
*   **Potential for Real-time Monitoring:** Designed with the potential for integration into real-time satellite monitoring systems.

## Prerequisites & Dependencies

To run this project, you will need the following:

*   **Python 3.6+**
*   **Libraries:**
    *   Detectron2
    *   TensorFlow/Keras
    *   OpenCV
    *   NumPy
    *   Pandas
    *   Pickle
*   **CUDA Toolkit (if using GPU)**

You can install the required Python libraries using pip:

```bash
pip install detectron2 opencv-python numpy pandas tensorflow scikit-learn
```

**Note:** Installation of Detectron2 can be complex. Please refer to the [Detectron2 official installation instructions](https://detectron2.readthedocs.io/tutorials/install.html) for detailed guidance.

## Installation & Setup Instructions

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/DarkX0704/Hypervelocity_Impact_Detection_and_Classification_for_Satellite_Structural_Integrity.git
    cd Hypervelocity_Impact_Detection_and_Classification_for_Satellite_Structural_Integrity
    ```

2.  **Install the required dependencies (see Prerequisites & Dependencies section).**

3.  **Download necessary models:**

    This repository includes pre-trained models. Ensure the following files are present in the root directory:

    *   `EDSR_x4.pb`
    *   `detectron_trained_model_final.pth`
    *   `mmod_damage_model.pkl`
    *   `multimodal_damage_model.h5`

4.  **Configuration:**
    * No specific configuration file is provided, the settings are implemented directly in the notebook. Review the Notebook content for details on changing image locations and parameters

## Usage Examples & API Documentation

The main functionality is implemented in the `Hypervelocity_Impact_Detection_and_Classification_for_Satellite_Structural_Integrity.ipynb` Jupyter Notebook.

1.  **Open the Jupyter Notebook:**

    ```bash
    jupyter notebook Hypervelocity_Impact_Detection_and_Classification_for_Satellite_Structural_Integrity.ipynb
    ```

2.  **Follow the notebook instructions to perform hypervelocity impact detection and classification.**  The notebook walks you through loading images, running the models, and interpreting the results.

## Configuration Options

The project utilizes several configurable settings within the `Hypervelocity_Impact_Detection_and_Classification_for_Satellite_Structural_Integrity.ipynb` notebook. These include:

*   **Model paths:**  The paths to the pre-trained models can be modified within the notebook.
*   **Image input paths:** The location of the images to be processed must be specified in the notebook.
*   **Detection thresholds:** Thresholds for object detection and classification can be adjusted.
*   **GPU/CPU Usage:** The notebook has settings to control the usage of GPU resources, allowing the models to be run on CPU if a GPU isn't available.

## Contributing Guidelines

We welcome contributions to this project! To contribute:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with clear, descriptive messages.
4.  Submit a pull request to the main branch.

Please ensure your code follows the existing style guidelines and includes appropriate tests.

## License Information

License information is currently not specified for this repository. The code is currently for research and demonstration purposes. Please contact the owner (DarkX0704) for clarification or licensing options if you want to use the code commercially.

## Acknowledgments

*   [Detectron2](https://detectron2.readthedocs.io/):  This project utilizes Detectron2 for object detection.
*   [EDSR](https://github.com/xinntao/EDVR): This project potentially uses EDSR for super resolution tasks. Check the notebook for details.
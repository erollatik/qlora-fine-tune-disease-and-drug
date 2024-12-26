# Meta LLaMA Fine-Tuning with QLoRA for disease-drug
Fine-tuning LLaMA-2 using QLoRA for disease-drug recommendations. This repository includes a Jupyter Notebook (`.ipynb`) file, configuration, and documentation for training a lightweight, efficient model tailored to medical datasets.

## Features
- Efficient fine-tuning with **QLoRA**.
- 4-bit quantization for memory optimization.
- Domain adaptation for medical queries.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/erollatik/qlora-fine-tune-disease-and-drug.git
   cd qlora-fine-tune-disease-and-drug
   ```
2. Open the Jupyter Notebook in your preferred environment. If Jupyter is not installed, you can install it with the following command:
   ```bash
   pip install notebook
   ```

3. Install the required Python libraries listed in the notebook using pip. You can find them in the initial code cell of the notebook:
   ```bash
   !pip install -q transformers==4.36.2 peft==0.7.1 bitsandbytes==0.41.3 accelerate==0.25.0 datasets==2.15.2 trl==0.7.4
   ```

## Usage
1. Open the Jupyter Notebook file (`qlora_fine_tune_disease_and_drug.ipynb`) in your environment:
   ```bash
   jupyter notebook qlora_fine_tune_disease_and_drug.ipynb
   ```

2. Follow the notebook cells step-by-step to:
   - Load the dataset.
   - Configure and fine-tune the model.
   - Generate predictions for given disease-related queries.

### Example Prediction
Run the prediction cell in the notebook with an example prompt:

**Input:**  
`Disease: Diabetes. What is the recommended drug?`

**Output:**  
`Metformin`

## Project Structure
```
qlora-fine-tune-disease-and-drug/
├── qlora_fine_tune_disease_and_drug.ipynb  # Main Jupyter Notebook file
├── README.md                              # Project documentation
├── LICENSE                                # License file
```

## Contributing
We welcome contributions! Feel free to submit pull requests or open issues.


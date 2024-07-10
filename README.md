# GenoVarDis@IberLEF2024: Automatic Genomic Variants and Related Diseases using Named Entity Recognition with Large Language Models

## Project Description
This project is a student's proposal from the University of Granada for the GenoVarDis shared-task at IberLEF2024, focusing on Automatic Disease and Procedure Coding using Named Entity Recognition (NER). The project utilizes the GenoVarDis shared-task dataset, which includes scientific literature in Spanish on genomic variants, genes, and related diseases. Three language models are proposed for the task:
- **GPT**: Evaluated for NER performance despite not being specifically trained for it.
- **RoBERTa**: Pretrained in the biomedical domain with Spanish texts and fine-tuned for NER.
- **GLiNER**: A compact NER model that excels in identifying arbitrary entity types and outperforms both ChatGPT and fine-tuned Large Language Models (LLMs) in zero-shot NER benchmarks.

The official results placed this proposal second overall.

## Project Structure

- **Data**: Contains TSV files with all data from the GenoVarDis corpus (training, dev and test).
- **EvaluationTSV**: Includes TSV files generated by our models' predictions.
- **Experimentation**: Contains .ipynb files for model evaluation.
- **LoadExploration**: .ipynb file for data loading and exploration.
- **Prototypes**: .ipynb files with model implementations.

This README outlines the organization and purpose of the files included in this repository.

## Installation
No installation steps are required if running the notebooks in Google Colab. Simply ensure the root directory of the project (`GenoVarDis`) is placed in the root directory of your Google Drive.

## Usage
1. Open Google Colab.
2. Navigate to the notebook (`*.ipynb`) you wish to run.
3. Mount your Google Drive if it's not already mounted:
    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```
5. Execute any available `.ipynb` notebook without any additional setup.

## Libraries Used
The following Python libraries are utilized in the notebooks:
- gliner
- transformers
- datasets
- evaluate
- seqeval
- accelerate
- beartype
- openai==0.28

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

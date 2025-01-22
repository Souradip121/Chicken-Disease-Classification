# Chicken Disease Classification Project

## Project Description
This project implements a deep learning solution to classify chicken diseases from fecal images. It includes both a model training pipeline and a web interface for real-time predictions.

## Tech Stack
- Python 3.8+
- TensorFlow/Keras
- Flask
- HTML/JavaScript/TailwindCSS
- DVC (Data Version Control)

## Project Structure
```
Chicken-Disease-Classification/
├── artifacts/                  # Model artifacts and data
├── config/                    
│   └── config.yaml            # Configuration files
├── logs/                      # Application logs
├── src/cnnClassifier/        
│   ├── components/            # Model components
│   ├── config/               
│   ├── pipeline/             
│   └── utils/                
├── templates/                 
│   └── index.html            # Web interface
├── app.py                     # Flask application
├── main.py                    # Training pipeline
├── params.yaml               
├── requirements.txt          
└── setup.py                  
```

## Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/Chicken-Disease-Classification.git
cd Chicken-Disease-Classification
```

2. Create and activate virtual environment
```bash
python -m venv venv
source venv/bin/activate  # For Linux/Mac
# or
venv\Scripts\activate     # For Windows
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

## Usage

### Training the Model
```bash
python main.py
```
Or use the web interface's "Train Model" button.

### Running the Web Application
```bash
python app.py
```
Access the application at `http://localhost:80`

### Making Predictions
1. Open the web interface
2. Upload a chicken fecal image
3. Click "Predict" to get the disease classification

## Configuration

Update these files for customization:
- `config/config.yaml`: Model and training parameters
- `params.yaml`: Hyperparameters
- `src/cnnClassifier/config/configuration.py`: Pipeline configuration

## DVC Pipeline
```bash
dvc init
dvc run -n train -d main.py -o artifacts/model.h5 python main.py
```

## Contributing
1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push to the branch
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Dataset source: [Add source here]
- Based on [research paper/methodology reference]

## Workflows

1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml

## On the go read
https://souradipcodes.notion.site/Chicken-Disease-Classification-17ec6c3fab4d804e9ce1cd402e2be079?pvs=4
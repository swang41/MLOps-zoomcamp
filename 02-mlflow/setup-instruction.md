# Create virual enviroment for local mlflow
```
chmod +x ./02-mlflow/conda-forge-hyperopt.sh
./02-mlflow/conda-forege-hyperopt.sh

conda create --name experiment-tracking --file ./02-mlflow/requirement.txt

conda activate experiment-tracking

pip install protobuf==3.20.* 
pip install "SQLAlchemy<2.0"

mlflow ui --backend-store-uri sqlite:///mlflow.db
```


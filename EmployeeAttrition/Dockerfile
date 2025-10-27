FROM python:3.10

# Prevent caching unnecessary files
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# Set working directory
WORKDIR /app

# Copy requirement file and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the project
COPY . .

# Create a folder for executed notebooks
RUN mkdir -p results

# Run notebooks sequentially with unlimited timeout
CMD bash -c " \
    mkdir -p results && \
    jupyter nbconvert --to notebook --execute Before_SMOTE.ipynb --output results/before_smote_executed.ipynb --ExecutePreprocessor.timeout=-1 && \
    jupyter nbconvert --to notebook --execute After_SMOTE.ipynb --output results/after_smote_executed.ipynb --ExecutePreprocessor.timeout=-1 && \
    jupyter nbconvert --to notebook --execute HyperParameterTuning.ipynb --output results/hyperparameter_executed.ipynb --ExecutePreprocessor.timeout=-1 \
"
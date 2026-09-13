# Data Science Salaries 2023

This project uses the [Data Science Salaries 2023](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023) dataset from Kaggle.

## Setup

This project uses the conda environment `environment.yml`.

1. Create and activate the environment:

   ```bash
   conda env create -f environment.yml
   conda activate DS_Salary
   ```

### Download

Run the following from the project root to download the dataset directly into `data/raw`:

```bash
kaggle datasets download arnabchaki/data-science-salaries-2023 -p data/raw --unzip
```

- `-p data/raw` downloads the file into the `data/raw` directory.
- `--unzip` extracts the CSV automatically after downloading.

If you'd rather download and unzip manually:

```bash
kaggle datasets download arnabchaki/data-science-salaries-2023 -p data/raw
unzip data/raw/data-science-salaries-2023.zip -d data/raw
```

After this, you should have the dataset `ds_salaries.csv` available under `data/raw/`.

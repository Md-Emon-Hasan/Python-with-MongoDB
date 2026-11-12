# Python with MongoDB

Practical Jupyter Notebook examples for connecting Python to MongoDB and working with document data using [PyMongo](https://pymongo.readthedocs.io/).

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![MongoDB](https://img.shields.io/badge/Database-MongoDB-47A248?logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![PyMongo](https://img.shields.io/badge/Driver-PyMongo-13AA52)](https://pymongo.readthedocs.io/)
[![Jupyter](https://img.shields.io/badge/Notebooks-Jupyter-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Overview

This repository is a hands-on learning resource for developers who want to use MongoDB from Python. It is organized as four notebooks, moving from a local database connection to querying, updating, and aggregating documents.

## Contents

| Notebook | What you will learn |
| --- | --- |
| [Connect Python With MongoDB](3%20Connect%20Python%20With%20MongoDb/Connect%20Python%20With%20MongoDb.ipynb) | Connect with `MongoClient`, select a database and collection, and insert documents. |
| [Querying JSON Documents](4%20MongoDb%20With%20Python-%20Querying%20Json%20Documents/MongoDb%20With%20Python-%20Querying%20Json%20Documents.ipynb) | Read documents and filter with equality, comparison, `$in`, `$and`, and `$or` queries. |
| [Updating Records](5%20MongoDb%20With%20Python-%20Updating%20Records/MongoDb%20With%20Python-%20Updating%20Records.ipynb) | Practice `update_one`, `update_many`, and `replace_one`. |
| [Aggregate Functions](6%20MongoDb%20With%20Python-%20Aggregate%20Functions/MongoDb%20With%20Python-%20Aggregate%20Functions.ipynb) | Group documents and calculate counts, sums, averages, and projected fields. |

## Prerequisites

- Python 3.9 or newer
- A MongoDB deployment: a local MongoDB server or a MongoDB Atlas cluster
- Jupyter Notebook or JupyterLab

## Get started

1. Clone the repository and enter its directory:

   ```bash
   git clone https://github.com/Md-Emon-Hasan/MongoDB.git
   cd MongoDB
   ```

2. (Optional) Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   ```

   On Windows PowerShell, activate it with `.\.venv\Scripts\Activate.ps1`. On macOS or Linux, use `source .venv/bin/activate`.

3. Install the notebook and MongoDB driver dependencies:

   ```bash
   python -m pip install pymongo notebook
   ```

4. Start your local MongoDB server, or prepare a MongoDB Atlas connection string.

5. Launch Jupyter from the repository root:

   ```bash
   jupyter notebook
   ```

6. Open a notebook from the table above and run its cells in order.

## Configure the MongoDB connection

The examples currently connect to MongoDB on the local machine:

```python
from pymongo import MongoClient

client = MongoClient("mongodb://127.0.0.1:27017/")
```

For MongoDB Atlas or another deployment, replace the URI with your deployment's connection string. Keep credentials out of notebooks committed to GitHub; load secrets from environment variables instead. The notebooks write sample documents to the database, so use a development database when experimenting.

## Notes

- The notebooks are independent examples and may create or modify database records when cells are run. Re-running insert cells can add duplicate sample documents.
- Database and collection names are selected in the notebook code. Update them if you want to use a different database.
- This repository is an educational walkthrough, not a packaged Python application; there is no `requirements.txt` at this time.

## Contributing

Suggestions, fixes, and additional examples are welcome. Open an issue to discuss a change, or submit a pull request with a clear description of the update.

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.

## Connect with me

- 🌐 **Portfolio:** [emonlabs-ai.hitechparks.com](https://emonlabs-ai.hitechparks.com)
- 💻 **GitHub:** [Md-Emon-Hasan](https://github.com/Md-Emon-Hasan)
- 💼 **LinkedIn:** [Md Emon Hasan](https://www.linkedin.com/in/md-emon-hasan-695483237/)
- 🤗 **Hugging Face:** [emonHasan01](https://huggingface.co/emonHasan01)
- 📧 **Email:** [emon.mlengineer@gmail.com](mailto:emon.mlengineer@gmail.com)
- 📱 **WhatsApp:** [+8801834363533](https://wa.me/8801834363533)

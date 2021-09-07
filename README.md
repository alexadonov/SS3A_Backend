# CrisisMgmt - UTS Software Studio 3A 2020 - Group 4

CrisisMgmt is a Flask API for handling user authentication and app functionality.

## Dev Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install all dependencies required for development using the `requirements.txt` file in the project's root folder:

```bash
pip install -r requirements.txt
```

## Running the API locally
Execute the following bash command from the project root folder to start the API server on `localhost:5000/api/`. Note you need to have Python and all dependencies installed first.
```bash
python appserver.py
```

## Making database migrations using SQLAlchemy ORM
Create an initial migration file to translate the classes in models.py to SQL that will generate corresponding tables
```bash
python manage.py db migrate
```
Run the migration to upgrade the database with the tables described in the prior step
```bash
python manage.py db upgrade
```

## Training and running the chatbot
CD to the 'crisismgmt-api/crisismgmt' folder
If you want to retrain the chatbot AI after it has been trained, delete 'pickle.data' and the three 'model.tflearn' files
If you want to run it without retraining, keep the files
run ```python chatbot.py
# Modifying the patterns the AI learns from
Add paterns into the 'intents.json' file
Delete the pickle.data file - chatbot AI will need retraining and will need to reread the intents file
run ```python chatbot.py

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

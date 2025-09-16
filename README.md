# SE-Academy

Online learning platform for the formal and current SE student who want to reviewing the subject you have learned in SE life.

## Environment Setup

You need to set the environment in the following file

alembic.ini in api submodule.

```bash
sqlalchemy.url={YOUR DATABASE CONNECTION STRING}
```

create .env file inside the api submodule.

```.env
DB_URL={YOUR_CONNECTION_STRING}
SECRET_KEY={YOUR_SECRET_KEY}
POSTGRES_USER={DB_USERNAME}
POSTGRES_PASSWORD={DB_PASSWORD}
POSTGRES_DB={YOUR_DBNAME}
```

Format of the connection string:

```python
"postgresql+psycopg2://{DB_USERNAME}:{DB_PASSWORD}@{DB_SERVER}:{DB_PORT}/{DB_NAME}"
```

## Clone

To clone this repository there have 2 ways to do

```bash
git clone https://github.com/plscallMeAlex/SE-Academy.git
git submodule update --init --recursive
```

Or

```bash
git clone --recurse-submodules https://github.com/plscallMeAlex/SE-Academy.git
```

If submodule are updated during the development u can use this command to update the module.

```bash
git submodule update --init --recursive
```

To pull the project u need to use this command.

Update Only main repo.

```bash
git pull
```

Update submodule also.

```bash
git pull --recurse-submodules
```

## Usage

Using command to start project during development.

Only API:

```bash
npm run api
```

Only APP:

```bash
npm run app
```

To run both:

```bash
npm run dev
```

Using This command in the deployment step.

Start New Using (--build flag)

```bash
docker compose up -d
```

Stop

```bash
docker compose down
```

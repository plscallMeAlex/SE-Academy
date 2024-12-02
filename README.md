# SE-Academy

Online learning platform for the formal and current SE student who want to reviewing the subject you have learned in SE life.

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
docker compose up -ds
```

Stop

```bash
docker compose down
```

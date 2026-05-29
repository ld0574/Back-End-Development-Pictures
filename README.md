# Back-End-Development-Pictures

Flask microservice for the band capstone project. The service exposes picture metadata from past events and provides REST endpoints used by the main Django application.

## Environment Setup

This repository was created from the IBM Skills Network template repository:

```text
https://github.com/ibm-developer-skills-network/luggb-Back-End-Development-Pictures
```

The local development environment is prepared by running the provided setup script:

```bash
bash ./bin/setup.sh
```

The setup script installs Python `3.9.x`, creates the course virtual environment named `backend-pics-venv`, installs the required Python packages from `requirements.txt`, and completes the capstone environment setup.

After setup, confirm the environment with:

```bash
python3.9 --version
source backend-pics-venv/bin/activate
pytest
```

## Endpoints

- `GET /health` returns service health.
- `GET /count` returns the number of pictures.
- `GET /picture` returns all pictures.
- `GET /picture/<id>` returns one picture by id.
- `POST /picture` creates a picture.
- `PUT /picture/<id>` updates a picture.
- `DELETE /picture/<id>` deletes a picture.

## Run Locally

```bash
flask --app app run --debugger --reload
```

The Dockerfile runs the app on port `3000`.

## Test

```bash
pytest
```

Expected result:

```text
11 passed
```

## Submission Evidence

The generated result summary is in `result.txt`. Pytest text outputs and screenshots are saved with the exercise filenames required by the course docs.

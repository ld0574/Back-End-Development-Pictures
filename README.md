# Back-End-Development-Pictures

Flask microservice for the band capstone project. The service exposes picture metadata from past events and provides REST endpoints used by the main Django application.

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

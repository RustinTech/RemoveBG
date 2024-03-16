
# Remove Background Flask App

A simple Flask app to remove the background of an image using [Rembg](https://github.com/danielgatis/rembg).

## Run Locally (Windows)
Just Click on Install.bat
and FOr Start app just click on Start.bat

## Run Locally (Windows via terminal)
```bash
pip install -r requirements.txt
python app.py
```

## Run with Docker

### Clone Repository

```bash
git clone https://github.com/RustinTech/RemoveBG.git
cd RemoveBG
```

### Download Background Remover Data Model for Python

```bash
wget https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx
```

### Build Docker Container

```bash
docker build . -t removebg
```

### Start Docker Container

```bash
docker run -d -p 5100:5100 removebg
```

This command will start a container based on your image, and your Flask application will be accessible at [http://localhost:5100](http://localhost:5100).

## Stopping the Container

To stop the running Docker container, you can use the following command:

```bash
docker stop <container_id>
```

Replace `<container_id>` with the ID of the running container. You can find the container ID by running `docker ps`.
```

Make sure to replace `<container_id>` with the actual ID of the running container when stopping it. This Markdown file provides clear instructions for running the Flask app both locally and with Docker.

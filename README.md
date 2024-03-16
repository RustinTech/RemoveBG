
A simple flask app to remove the background of an image with [Rembg](https://github.com/danielgatis/rembg)


## Run it Locally in Windows

```
pip install -r requirements.txt
python app.py

```
## Run it in Docker
```
### Clone Repo
```
git clone https://github.com/RustinTech/RemoveBG.git
```
### Move into Folder
cd RemoveBG

### Download BG Remover DataModel for Python
wget https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx


### Build Docker Container

```sudo docker build . -t removebg
```

### Start Docker Container (Change 80 to unused port in case of occupied port 80)

```
sudo docker run -p 8080:80 removebg
```

Enjoy the Quick Background Remover



docker build -t removebg .

Replace your_image_name with a suitable name for your Docker image.

docker run -d -p 5100:5100 removebg

Hostport:DockerPort

This command will start a container based on your image, and your Flask application will be accessible at http://localhost:5100.

docker stop
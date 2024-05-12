Creating a python app using Docker containers : 

1. Create a Python app (without using Docker)

  * Copy and paste this entire command into the terminal. The result of running this command will create a file named app.py.

    echo 'from flask import Flask

    app = Flask(__name__)

    @app.route("/")
    def hello():
        return "hello world!"

    if __name__ == "__main__":
        app.run(host="0.0.0.0")' > app.py
  
    This is a simple Python app that uses Flask to expose an HTTP web server on port 5000. (5000 is the default port for flask.) 

2. Create and build the Docker image.

3. Build the Docker image.

4. Run the Docker image
$ docker run -d -p 5003:5000 pythonapp
5. docker ps

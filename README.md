# personal-website

### Steps

1. Install flask
    - `pip install flask`
2. Create `app.py` to initialize Flask
    - file can be named anything
    - paste code below
    - run using `python app.py` from terminal
    - launch website from specified port shown on terminal
    ```python
    from flask import Flask

    app = Flask(__name__)

    @app.route("/")
    def hello_world():
        return "<h1>Hello, World!</h1>"

    if __name__ == "__main__":
        app.run(debug=True)
    ```
3. Create a `home.html` template in a `templates/` directory, and import `render_template` to serve that file when your route is it.

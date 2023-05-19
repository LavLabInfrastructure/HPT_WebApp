# HPT_WebApp
---
## Steps to run:
1. Run `npm install`
2. Run `npm run start`
3. Create virtual environment: Run `python -m venv Venv` (Makes virtual environment with name Venv)
4. Activate Virtual environment: Run `source Venv/Scripts/activate`
5. Run `pip install -r requirements.txt`
6. Run `cd srv/`
7. Run `node server.js`
8. Use your IDE to launch public/index.html
9. Enjoy looking at prostates :)

## Note on Running
- Loading images, then points, then executing inference will run result in the HPT running inference on the histology points from the .csv file.
- Loading images, then points, then running the sift function, then executing inference will run result in the HPT running inference on the sift points.
- *Note*: In order to run inference, you must first load a set of points. The max and min of the X and Y coordinates are used to center both prostates, which is neccesary to get good results out of the HPT. However, you can technically remove the centering functions from the inference.py script, allowing you run inference on sift points without loading in point pairs (The results just may not be great).


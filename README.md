# Tensor-Flow-Object-Recognition
**___________________________________________________________**

Model has been trained to recognize a variety of things, including expressions such as smiles, frowns, squints, and more.

Adapted from Nicholas Renotte's 5-hour Youtube course on Tensor Flow object recognition. Course focused on teaching hand gestures, adapted it to recognize facial expressions.

Here is an example of facial expression recognition:
<img width="672" alt="Screen Shot 2021-08-16 at 3 58 25 PM" src="https://user-images.githubusercontent.com/66883135/130535990-34fa5a04-f767-431a-9676-c4cb478b9317.png">


**___________________________________________________________**

****Errors I encountered and fixes:****

**Error: ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject**
Solution: Reinstall pycocotools to a matching version for Python and Tensor Flow. 
Solution 2: Reinstall numpy or try changing the versions to match the required architecture.

Helpful links that helped me fix this issue:
https://stackoverflow.com/questions/66060487/valueerror-numpy-ndarray-size-changed-may-indicate-binary-incompatibility-exp
https://github.com/scikit-image/scikit-image/issues/5270
https://github.com/scikit-learn-contrib/hdbscan/issues/457


**Error: ValueError: 'images' must have either 3 or 4 dimensions.**
Solution: This happened with image detection, usually the image name and path are incorrect. For example, if in section 9 you are giving it the path for the image you want it to recognize, but the filetype is "png" and you give it another one, this error will appear.

**___________________________________________________________**


**Resources:**
https://www.youtube.com/watch?v=yqkISICHH-U&ab_channel=NicholasRenotte

**Coding Requirements:**
- Python 3.8 or higher
- Tensor Flow --upgrade (2.3 currently)
- Protobuf matplotlib==3.2
- Numpy 1.20.0

**Note:** This project was built within a virtual environment. Bellow are the required dependencies and commands to install them

- python -m pip install --upgrade pip
- pip install ipykernel
- python -m ipykernel install --user --name=**YOUR ENVIRONMENT NAME**

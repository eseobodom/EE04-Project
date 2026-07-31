<h1>EE04-Project</h1>
<p>Machine learning web application built with Streamlit and TensorFlow for identifying potato leaf diseases (EE04 Engineering Project)</p>
This project involved developing a CNN-based web application to classify healthy potatoe vs potatoe early blight. The libraries used include datasets obtained from Kaggle, NumPy, Matplotlib, Jupyter Notebook, TensorFlow, and Keras from TensorFlow, and finally VS Code for its terminal and Streamlit for deployment.
The sub-folders train, validation, and test inside the dataset folders were used to house data obtained from Kaggle. These data were used to train the AI model created using NumPy, Matplotlib, and Keras from TensorFlow in the notebook.
After training, validation, and testing were completed, the App.py file was used to store the user interface of the application. Immediately after all the folders were created, we used Git to commit and push the project to our already created repository. The final step came in the form of deployment, where we created a Streamlit account, connected it to our GitHub, and then deployed our code.
The hurdles encountered were setting up the Jupyter Notebook, the 100 MB GitHub protocol, which was resolved by using the TensorFlow Lite (TFLite) version of TensorFlow, and finally the Python version blocking deployment. This was overcome by reducing the Python version in Streamlit, creating a file, and pushing it to GitHub with a Python version less than 3.12. 
Innocent, Ugochukwu Anthony
23/EG/EE/O41
anthonyinnocent-wq

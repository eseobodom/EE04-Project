<h1>EE04 Project: Potato Leaf Disease Classifier</h1>

<p>A Streamlit web app that uses a TensorFlow model to check if a potato leaf is healthy or has early blight</p>

<p><em>Engineering Project, EE04</em></p>

<hr>

<h2>What It Does</h2>
<p>
Upload a photo of a potato leaf. The app checks the photo is actually a potato leaf, then predicts whether
it is healthy or has early blight, along with a confidence percentage
</p>

<h3>Classes</h3>
<ul>
  <li>Healthy</li>
  <li>Early Blight</li>
</ul>

<h3>Built With</h3>
<ul>
  <li>Python</li>
  <li>TensorFlow / Keras (MobileNetV2)</li>
  <li>Streamlit</li>
  <li>NumPy and Pillow</li>
</ul>

<hr>

<h2>How To Set It Up</h2>

<h3>1. Clone the repo</h3>
<pre>
git clone https://github.com/eseobodom/EE04-Project.git
cd EE04-Project/EE04
</pre>

<h3>2. Install dependencies</h3>
<pre>
pip install -r requirements.txt
</pre>

<h3>3. Get the dataset (if you want to retrain the model)</h3>
<p>
The dataset was pulled with <code>data.py</code>, which downloaded the potato leaf images from a public
PlantVillage mirror on GitHub, capped at 5MB per class:
</p>
<pre>
py data.py
</pre>

<h3>4. Train the model (if you want to retrain)</h3>
<p>
Open <code>train.ipynb</code> and run the cells in order. It saves the trained model as
<code>model.keras</code>
</p>

<h3>5. Run the app</h3>
<pre>
streamlit run app.py
</pre>
<p>
It opens the local link shown in your terminal (<code>http://localhost:8501</code>) in your browser, upload a potato
leaf photo and click Analyze
</p>

<hr>

<h2>Known Limitations</h2>
<ul>
  <li>Works best on close up, single leaf photos with a plain background</li>
  <li>Can give a confidently wrong answer on outdoor or multi leaf photos, since the training data does not include many of those</li>
  <li>Does not check that the leaf is actually from a potato plant, only that it looks like a leaf</li>
</ul>

<hr>

<h2>Contributors</h2>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Reg Number</th>
      <th>Github Username</th>
    </tr>
  </thead>
  <tbody>
     <tr>
      <td>Udoumoh, Emmanuel Uwem</td>
      <td>23/EG/EE/001</td>
      <td>AUZAPAZTUR_</td>
    </tr>
      <tr>
      <td>Michael, Anieofon Edet</td>
      <td>23/EG/EE/011</td>
      <td>Aniefon</td>
    </tr>
     <tr>
      <td>Obodom, Eseabasi Mboso</td>
      <td>23/EG/EE/021</td>
      <td>eseobodom</td>
    </tr>
    <tr>
      <td>Akpan, Success Aniefiok</td>
      <td>23/EG/EE/031</td>
      <td>Suciboy27</td>
    </tr>
      <tr>
      <td>Innocent, Ugochukwu Anthony</td>
      <td>23/EG/EE/041</td>
      <td>anthonyinnocent-wq</td>
    </tr>
     <tr>
      <td>Camillus, Prince Anthony</td>
      <td>23/EG/EE/051</td>
      <td>dtwinsprince</td>
    </tr>
     <tr>
      <td>Oboro, Godwin Ajiri-Oghene</td>
      <td>23/EG/EE/061</td>
      <td>godwinoboro23-web</td>
    </tr>
     <tr>
      <td>Sunday, Levite Idongesit</td>
      <td>23/EG/EE/071</td>
      <td>Balor567</td>
    </tr>
     <tr>
      <td>Ikpeme, Peter Asanye</td>
      <td>23/EG/EE/081</td>
      <td>Cephas-81</td>
    </tr>
     <tr>
      <td>Antia, Godswill Aniekan</td>
      <td>23/EG/EE/101</td>
      <td>Mrwilliam-Antia</td>
    </tr>
    <tr>
      <td>Johnson, Gideon Mfon</td>
      <td>23/EG/EE/121</td>
      <td>johnsongideon2026</td>
    </tr>
    <tr>
      <td>Isaac, Emediong Ime</td>
      <td>24/EG/EE/371</td>
      <td>BerryElwey</td>
    </tr>
  </tbody>
</table>
<hr>

<h2>Contributors' Comments</h2>

<h3>eseobodom</h3>
<p>
This project set out to help spot early blight in potato leaves before it spreads through a crop.
Building it meant working through the full process, from sourcing a proper dataset with a script
instead of manual uploads, to training a model that could tell healthy and diseased leaves apart, to
putting it all together in a simple web app anyone can use
</p>

<h3>AUZAPAZTUR_</h3>
<p>
The project is a small experiment in teaching a model to tell a healthy potato leaf from a diseased
one. It only really works on close up photos similar to what it was trained on, so it is more of a
learning exercise in how image classification works than a tool anyone should rely on for a real crop
</p>

<h3>Aniefon</h3>
<p>
This is a student project exploring whether a model can spot early blight from a leaf photo. This tool takes a photo of a leaf and tells you if it looks healthy or shows signs of early blight, but it is not
reliable enough yet for someone to depend on for an actual growing decision
</p>

<h3>Suciboy27</h3>
<p>
The project explores a simple question, can a model trained on a small set of leaf photos tell
healthy from diseased. It works under limited conditions and is meant as a learning project, not a
finished tool for real world crop checks
</p>

<h3>anthonyinnocent-wq</h3>
<p>
This is a class project built to understand how a leaf disease classifier works end to end. It is a leaf health checker built for potato farming. A user uploads a photo and the app gives a quick read on whether the leaf looks healthy or shows early blight. It works under limited conditions, so it is best treated as a prototype for learning, not a tool to base real decisions on
</p>

<h3>dtwinsprince</h3>
<p>
The project is a prototype for detecting early blight from a potato leaf photo. It is meant to help
catch early blight sooner, giving farmers a quicker first read on their crop's condition. But its results should be treated as a demonstration rather than something dependable for an actual crop
</p>

<h3>godwinoboro23-web</h3>
<p>
This project is an exercise in applying a pretrained model to a specific classification task. It
works within the limits of its training data, and is meant to show the process of building such a
tool rather than to be used for real agricultural decisions
</p>

<h3>Balor567</h3>
<p>
The project is a small scale attempt at automated leaf disease detection, built as part of a course.
It has clear limits, especially outside the kind of photos it was trained on, so it should be seen as
a demonstration project, not a reliable farming tool
</p>

<h3>Cephas-81</h3>
<p>
This is a learning project centered on image classification for potato leaves. The model can be
wrong, so it is meant to show how the technique works rather than to be trusted for a real crop check
</p>

<h3>Mrwilliam-Antia</h3>
<p>
The project is a prototype exploring how far a small dataset and a pretrained model can go in
detecting leaf disease. It is a useful demonstration of the process, but not something built to be
relied on for actual farming decisions yet
</p>

<h3>johnsongideon2026</h3>
<p>
This project looks at whether a simple model can flag potato leaf disease from a photo. Its accuracy
depends heavily on how similar a photo is to its training data, so it works better as a class
demonstration than as a dependable tool
</p>

<h3>BerryElwey</h3>
<p>
The project is an experiment in building an image classifier for potato leaf health. It has known
blind spots, so results should be treated as a demonstration of the approach rather than something to
act on for a real crop
</p>
<hr>

<h2>License</h2>
<p>Academic project for the GET 324 Engineering course</p>

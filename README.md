# Competitive-Learning-Algorithm-using-Keras
This code implements competitive learning for digit classification using a neural network with a competitive layer and stops training when the desired accuracy (90% approx) on the test set is achieved.
# Stock-Price-Prediction using (LSTM).
Stock price prediction of State Bank of India and visualization of SBI and Reliance Industries stock
<h1> Overview </h1>
<p> The goal of this project is to train a neural network to classify handwritten digits from the famous MNIST dataset. Competitive learning is employed to adapt and specialize the neurons in the competitive layer based on the input data. The model is trained to achieve high accuracy in digit recognition.</p>

<h1> Prerequisites </h1>
<p>Before running the code, make sure you have the following installed</p>
<ul> <h3> Python version </h3> </ul> 
  <li> Python 3.7 or above </li>
  
  <h2><ul> Installation of Libraries </ul></h2>
     <li>Keras</li>
     <li>NumPy</li>
     
     
 <h1>Versions (need to install)</h1>
     <h3>numpy</h3>
       <li>Version: 1.24.1</li>
     <h3>Keras</h3>
        <li>Version: 2.13.1</li>
    
<h1> Dataset </h1>
     <p> The MNIST dataset is automatically downloaded and preprocessed within the code. It consists of 60,000 training samples and 10,000 test samples, each representing a 28x28 grayscale image of a handwritten digit from 0 to 9.</p>
<h1> Model Architecture </h1>
<p>The competitive learning model consists of two layers:</p>
<li><b>Competitive Layer:</b> A dense layer with linear activation is used for competitive learning. The number of neurons in this layer can be adjusted by setting the num_neurons variable.</li>
<li><b>Output Layer:</b> A dense layer with softmax activation for digit classification with 10 neurons (one for each digit).</li>

<h1>Training</h1>
<p>The model is trained using competitive learning over a fixed number of epochs (e.g., 50). The training process involves:</p>
<li>Iterating through mini-batches of the training data.</li>
<li>Computing activations for the competitive layer and finding the winning neurons for each input in the batch.</li>
<li>Updating the weights of the winning neurons to be closer to the input data using a learning rate.</li>

<h1>Evaluation and Stopping</h1>
<p>After each epoch, the model's performance is evaluated on the test set to measure accuracy. If the desired accuracy threshold (e.g., 90%) is achieved, the training is stopped early for efficiency.</p>

<h1> Conclusion</h1>
<li>Competitive learning is a powerful unsupervised learning technique.</li>
<li>It enables neural networks to adapt and specialize neurons based on competition.</li>
<li>The model learns to classify digits with high accuracy on the MNIST dataset.</li>

     

# Multi-layered LSTM neural network and LSTM with Autoencoder and Notes

Data Clustering Third Project For Software Development for Algorithmic Problems  

Experimented with epochs, batches, and loss functions.  
Trained and tested the network, changing the layers each time.  
Implemented an autoencoder for another LSTM network.  
Used the networks for previously implemented algorithms such as LSH, HyperCube, Discrete and Continuous Frechet, and took notes on their validity.  
Not fully functional  

---

**3rd Assignment: Software Development for Algorithmic Problems**  

**STEVI'S CHARALAMPOS - ANTONIOS SDI1600278**

---

The project consists of the following files:  
- `Project_3.ipynb`: Contains all the code for the assignment  
- `Project_3.py`: Contains all the code for the assignment  
- `Comments.pdf`: Contains all comments regarding the A, B, C questions  
- Folder `Data results`: Contains the results from the C question  
- `README`

### How to run the project:
The project is ready and has run on Google Colab, and all results are printed.  
If someone wants to run it again, they just need to have the dataset file in their drive, as it is loaded from there.  
The command to load the dataset is: `df=pd.read_csv("/content/drive/MyDrive/nasdaq2007_17.csv", header=None)`  
Once the dataset is loaded, the entire project can be run from the start. It takes about 25 minutes for the full run.

### What the project can do:
The project runs for questions A, B, C, plus the observations for question D. Specifically:

- **In question A**, the dataset is loaded, properly split into train and test after scaling. The model is built and fitted. Then, I predict and print 5 different input examples.
- **In question B**, the dataset is properly prepared with scaling, the model is built, and it runs. Predicts for train and test are made, and anomalies are identified.
- **In question C**, the dataset is properly prepared and 6 different autoencoder models are run: Simple feed-forward, Deep encoder, 1D convolutional, LSTM, Simple AE with synthetic data, and Deep encoder with synthetic data.  
  For each of these models, a separate CSV file is created to store the time series required for question D. Additionally, for each model, I print train/test loss and 10 random inputs with their predictions.
- **In question D**, there are comments inside the `Comments.pdf` regarding the files generated in question C. For each model, there are three different files (lsh, frechet, hypercube).

### What the project cannot do:
- The project does not print the anomalies in question B, as I could not resolve the errors.
- The project does not include the second project, so cross-checking cannot be done for the files generated in question C.
- I am not satisfied with the results in question C. After many trials with various parameters, I couldn’t achieve the expected results, so there may be errors.

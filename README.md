# Multi-layered LSTM neural network and LSTM with Autoencoder and Notes

Data Clustering Third Project For Software Development for Algorithmic Problems<br /><br />

Experimented with epochs batches and loss functions.<br />
Trained and tested the network changing the layers each time.<br />
Implemented an autoencoder for another LSTM network.<br />
Used the networks for previous implemented algorithms such as LSH,HyperCube,Discrete and Continuous Frechet and took notes for their validity.<br />
Not fully functional<br /><br />









3η Εργασία Ανάπτυξη Λογισμικού για Αλγοριθμικά Προβλήματα 

	ΣΤΕΒΗΣ ΧΑΡΑΛΑΜΠΟΣ - ΑΝΤΩΝΙΟΣ sdi1600278
	
Από τι αποτελείται η εργασία:
	Project_3.ipynb:	Εκεί βρίσκεται όλος ο κώδικας της εργασίας
	Project_3.py:	Εκεί βρίσκεται όλος ο κώδικας της εργασίας
	Comments.pdf:		Εκεί βρίσκονται όλοι οι σχολιασμοί σχετικά με τα Α,Δ ερωτήματα
	Φάκελος Data results:	Εκεί βρίσκονται τα αποτελέσματα που έχουν τρέξει από το Γ ερώτημα
	README
	
Πως τρέχει η εργασία:
	Η εργασία είναι έτοιμη και έχει τρέξει σε google colab και όλα τα αποτελέσματα είναι εκτυπωμένα.
	Σε περίπτωση που κάποιος θέλει να την τρέξει εκ νέου αρκεί να έχει το αρχεί του dataset μέσα
	στο drive του καθώς από εκεί φορτώνεται.
	Η εντολή που φορτώνουμε το dataset είναι : df=pd.read_csv("/content/drive/MyDrive/nasdaq2007_17.csv", header=None)
	Αν λοιπόν φορτωθεί το dataset μπορεί να τρέξει ολόκληρη η εργασία από την αρχή. Η εργασία χρειάζεται
	περίπου 25 λεπτά για να τρέξει ολόκληρη.
	
Τι μπορεί να κάνει η εργασία:
	Η εργασία τρέχει για τα Α,Β,Γ ερωτήματα + οι παρατηρήσεις για το Δ ερώτημα. Ποιο συγκεκριμένα:
	
	Στο Α ερώτημα φορτώνω το dataset, το χωρίζω κατάλληλα σε train,test έχοντας κάνει scaling.
	Φτιάχνω το μοντέλο μου και το κάνω fit. Στην συνέχεια κάνω predict και εκτυπώνω 5 διαφορετικά
	παραδείγματα inputs.
	
	Στο Β ερώτημα φτιάχνω κατάλληλα τα dataset με scaling, φτιάχνω το μοντέλο και το τρέχω, κάνω
	predict για train και test και βρίσκω τα anomalies.
	
	Στο Γ ερώτημα φτιάχνω κατάλληλα τα dataset και τρέχω 6 διαφορετικά μοντέλα autoencoders : Simple feed-forward
	Deep encoder, 1D convolutional, LSTM, Simple AE with synthetic data, Deep encoder with synthetic data.
	Σε κάθε ένα από αυτά τα μοντέλα φτιάχνω ξεχωριστό αρχείο csv στο οποίο αποθηκεύω time series που θα χρειαστούν
	στο Δ ερώτημα. Επίσης σε κάθε μοντέλο εκτυπώνω train,test loss και 10 τυχαία inputs με τα predict τους.
	
	Το Δ ερώτημα αποτελείται από σχόλια τα οποία υπάρχουν μέσα στο Comments.pdf σχετικά με τα αρχεία που παρήχθησαν
	στο Γ ερώτημα. Για κάθε μοντέλο υπάρχουν τρια διαφορετικά αρχεία (lsh,frechet,hypercube).
	
Τι δεν μπορεί να κάνει η εργασία:
	Η εργασία δεν εκτυπώνει τα anomalies στο Β ερώτημα καθώς δεν μπόρεσα να λύσω τα λάθη.
	Η εργασία δεν περιλαμβάνει την 2η εργασία Project και έτσι δεν μπορεί να γίνει cross-check για 
	τα αρχεία που έχουν παραχθεί στο Γ ερώτημα.
	Δεν έχω μείνει ικανοποιημένος με τα αποτελέσματα στο Γ ερώτημα, έπειτα από πολλές δοκιμές σε 
	διάφορες παραμέτρους δεν κατάφερα να βρω τα αποτελέσματα που ζητούσα, οπότε πολύ πιθανό είναι
	να υπάρχουν λάθη.


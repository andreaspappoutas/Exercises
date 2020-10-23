## ΠΡΟΣΩΠΙΚΑ ΣΤΟΙΧΕΙΑ:

### Αντρέας Παππούτας
### ΑΜ: Π2017148

| Εβδομάδα* | Παραδοτέο |
| --- | --- |
| <a href="#P">1</a> |<a href="#P">Φορκ του αποθετηρίου και δημιουργία της σελίδας της αναφοράς με τα προσωπικά στοιχεία σας, της σύνοψης με αυτόν τον πίνακα περιεχομένων, και συγγραφή της εισαγωγής με περιγραφή των αναγκών και των στόχων σας για το αντίστοιχο μάθημα* </a> |
| <a href="#P-1">2</a> |<a href="#P-1"> Άσκηση προγραμματισμού</a> |
| <a href="#P-2">3</a> |<a href="#P-2">  Άσκηση γραμμής εντολών</a> |
| <a href="#P-3">4<a href="#P-3"> |<a href="#P-3"> Άσκηση προγραμματισμού + αίτημα ενσωμάτωσης (CSCW, IV)<a href="#P-3"> |
| <a href="#P-4">5 </a>| <a href="#P-4">Άσκηση γραμμής εντολών </a>|
| 6 | Άσκηση προγραμματισμού (HCI) ή γραμμής εντολών (SW)+ συμμετοχικό περιεχόμενο |
| 7 | Άσκηση γραμμής εντολών (SW) + αίτημα ενσωμάτωσης (CSCW, IV) |
| 8 | Άσκηση προγραμματισμού (HCI) ή γραμμής εντολών (SW) |
| 9 | Άσκηση γραμμής εντολών (SW) ή αίτημα ενσωμάτωσης (CSCW, IV) |
| 10 | συμμετοχικό περιεχόμενο |
| 11 | αίτημα ενσωμάτωσης (CSCW, IV) |
| 12 | Τελική αναφορά* |


## <a name="P">ΕΙΣΑΓΩΓΗ:</a>
Μέσο της οπτικοποίηση της πληροφορίας προσπαθούμε να δημιουργήσουμε μια διάδραση με τα δεδομένα που έχουμε έτσι ώστε να γίνουν πιο διακριτά. Έχω σαν στόχο να μάθω να οργανώνω με σωστό τρόπο τα δεδομένα σε ένα υψηλότερο επίπεδο. Σκοπός μου είναι να μάθω τεχνικές διαχείρισης τον διάφορων πληροφοριών(γραφικά , εικόνες , βίντεο κτλ) ενώ επίσης να αποκτήσω γνώση στις σύγχρονες τεχνολογίες που χρησιμοποιούνται για τη οπτικοποίηση τους.

---


## <a name="P-1">Παραδοτέο 1</a>
### Άσκηση: Τροποποιήστε τον κώδικα του παραδείγματος προσθέτοντας και οπτικοποιώντας στο ίδιο πλαίσιο περισσότερα από 2 σετ δεδομένων (datasets).


Επέλεξα για άσκηση προγραμματισμού να αλλάξω το visualization dataset. 
Στη άσκηση αυτή αρχικά δήλωσα στη javascript το νέο *"datasetC=[..]"* . 
Στη html δημιούργησα ένα κουμπί ίδιο τα με τα άλλα 2 για το datasetC και άλλαξα μόνο το *onclick* να πηγαίνει στο *triggerDatasetC*. 
Στη συνέχεια δημιούργησα ακριβώς το ίδιο function με αυτό που χρησιμοποιείτε για τα άλλα 2 όπου και το ονόμασα *triggerDatasetC*. 
Σε αυτό το νέο function η μόνη αλλαγή που χρειάζονταν ήτανε στη αρχή το *"var dataset = datasetC"*. 
Στο τέλος εφόσον είχα δηλωμένο ένα νέο datasetC με δικό του function και κουμπί που να πηγαίνει σε αυτό το function τότε μπορούσαμε να απεικονίσουμε 3 dataset.

[Codepen Link](https://codepen.io/andreaspappoutas/pen/ZEOQLvm)

[Link Κώδικα](https://github.com/andreaspappoutas/site/blob/master/_remix/visualization-dataset.md)

[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/visualization-dataset)


## <a name="P-2">Παραδοτέο 2</a>
### Άσκηση: visualize your data |	demo with your git commits history and percipation data per day for the last month from your city.

[Asciinema-Spark](https://asciinema.org/a/367160)

Ξεκίνησα τη πρώτη άσκηση γραμμής εντολών με τη οπτικοποίηση των commits μου στο IV μέσο του εργαλείου spark.
Άρχισα αυτή τη άσκηση με τη εγκατάσταση του spark:
```
sudo sh -c "curl https://raw.githubusercontent.com/holman/spark/master/spark -o /usr/local/bin/spark && chmod +x /usr/local/bin/spark"
```
Έτρεξα μια απλή εντολή για οπτικοποίηση μιας ακολουθίας αριθμών.
```
spark 0 2 4 6 8 10 12
```
Ακολούθως με τη παρακάτω εντολή έκανα εγκατάσταση του git spark ένα εργαλείο με το οποίο μπορούμε να οπτικοποιήσουμε πληροφορίες για το github.

```
curl -L http://cpanmin.us | perl - --sudo App::cpanminus
cpanm App::Git::Spark
```

Έφτιαξα ένα νέο φάκελο όπου και έβαλα μέσα το repository iv και έτρεξα τη παρακάτω εντολή για να δείξω πόσα commits έκανα τις τελευταίες 15 μέρες.
```
git spark --days 15 andreaspappoutas
```
  
## <a name="P-3">Παραδοτέο 3</a>
### Άσκηση 1: Τροποποιήστε το παράδειγμα έτσι ώστε όταν το αυτοκίνητο κινείται όπισθεν να έχει μικρότερη (τη μισή) ταχύτητα από το όταν κινείται έμπροσθεν.
### Άσκηση 2: Δημιουργείστε περιμετρικά όρια έτσι ώστε το αυτοκίνητο να μη βγαίνει ποτέ έξω από την πίστα.

Για τη άσκηση 1 βρήκα στο κώδικα javascript το "onkeydown" όπου και βλέπουμε ανά πόσα pixels αλλάζει το αυτοκίνητο όταν το κάθε κουμπί είναι πιεσμένο. Τα κουμπιά είναι γραμμένα με το κωδικό τους κάτι που μπορεί να βρεθεί εύκολα από αυτή τη [σελίδα](https://keycode.info).
```
if (key == 37) dx=-4; else if (key == 38) dy=-4; else if (key == 39) dx=4; else if (key == 40) dy=4;
```
Η όπισθεν είναι το κουμπί με το αριθμό 40 έτσι το αλλάζουμε να σε 2.
```
if (key == 40) dy=4
```

Στη άσκηση 2 αρχικά πρέπει να φτιάξουμε ένα function για το κάθε άξονα που θα ελέγχει αν το αυτοκίνητο είναι μέσα στα όρια του canvas.
```
function testX(x){
  if((x<1000) && (x>0)){
    return true;
  }
  else return false;
}

function testY(y){
  if((y<800) && (y>0)){
    return true;
  }
  else return false;
}
```
Αν είναι μέσα στα όρια επιστρέφει true αλλιώς false
Μέσο του ίδιου σκεπτικού φτιάχνουμε function για όταν το αυτοκίνητο είναι εκτός ορίων.
}
```
function AllagiX(x){
  if(x>=1000){
    x=x-1;
    //x=1; diaforetiko
    return x;
  }
  else if(x<=0){
    x=x+1;
    //x=999;
    return x;
  }
}
function AllagiY(y){
  if(y>=800){
    y=y-1;
    return y;
  }
  else if(y<=0){
    y=y+1;
    return y;
  }
}
}
```
Αν βγει εκτός ορίων αριστερά η πάνω από το canvas του προσθέτουμε ενώ αντίθετα αν είναι δεξιά ή κάτω του αφαιρούμε.
Τέλος συνδυάζουμε αυτά τα 2 functions με 2 απλά if όπου εφόσον έχουμε true δεν χρειάζεται να γίνει αλλαγή στη τοποθεσία του αυτοκινήτου έτσι δεν καλούνται οι function για αλλαγή.
```
if(testX(x)){
    x = x - dy * Math.cos(angle * Math.PI / 180);
  }
    else{
      x = AllagiX(x);
    }
    
  if(testY(y)){
    y = y - dy * Math.sin(angle * Math.PI / 180);
  }
    else{
      y = AllagiY(y);
    }
```
[Codepen Link](https://codepen.io/andreaspappoutas/pen/YzWwgMW)

[Link Κώδικα](https://github.com/andreaspappoutas/site/blob/master/_remix/keyboard-input.md)

[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/keyboard-input/)


## <a name="P-4">Παραδοτέο 4</a>
## Άσκηση: generate plots	create plots for your data from some other course or project
# [Asciinema MatPlotLib](https://asciinema.org/a/367161)

Για υλοποίηση αυτής της άσκησης εγκατέστησα το MatPlotLib με τη παρακάτω εντολή.
```
python -m pip install -U matplotlib
```
Στη συνεχεία για να φτιάξω ένα plot έφτιαξα ένα πρόγραμμα της python που έκανε χρήση της matplotlib για τη 
οπτικοποίηση των δεδομένων. Για τη ανάκτηση των δεδομένον από το αρχείο csv έγινε χρήση
του numpy. Στο τέλος έκανα export το αποτέλεσμα σε pdf,svg και png. Ο κώδικας python είναι ο παρακάτω:
```
from matplotlib import pyplot as plt                                            
from matplotlib import style                                                    
import numpy as np                                                              
                                                                                
style.use('ggplot')                                                             
                                                                                
x,y = np.loadtxt('data.csv',                                                    
                unpack = True,                                                  
                delimiter = ',')                                                            
                                                                                
plt.plot(x,y)                                                                                                                       
                                                                                
plt.title("Chart")                                                              
plt.ylabel("Values")                                                            
plt.xlabel("Time")

plt.plot(x,y)                                                                                                                                                                       
plt.title("Chart")                                                              
plt.ylabel("Values")                                                            
plt.xlabel("Time")                                                                        
                                                                                
plt.show()                                                                      
                                                                                
plt.savefig('plot.pdf')                                                         
plt.savefig('plot.svg')                                                         
plt.savefig('plot.png')   
```

## Το αποτέλεσμα:


![plot](https://user-images.githubusercontent.com/44147982/96948001-46a5ae80-14ed-11eb-9536-0e6df7642265.png)







---
---


# άλλες
# 1 - προγραμματισμού
Άσκηση: Επεκτείνετε τον κώδικα του παραδείγματος έτσι ώστε κατά την επιλογή του κουμπιού (κλικ), να εφαρμόζεται μια λειτουργία της επιλογής σας.
Άλλαξα το κώδικα έτσι ώστε να υπάρχει animation με το κλικ. Πρώτα απ όλα φτιάχνουμε νέο class μέσα στο οποίο θα γίνονται όλα που γίνονταν και πριν με τι διαφορά ότι θα τρέχουμε το παρακάτω animation.
```
animation: test1 2s ease-in-out;
```
Αλλάζουμε και κατάλληλα στο κώδικα js. Ακολούθως μέσο keyframes φτιάχνουμε το animation. Κάνω χρήση keyframes για καλύτερο ελέγχω του.
```
@keyframes test1 {
  0% {
    transform: scale(0);
  }

	

  50% {
    transform: scale(2);
  }
	100% {
    transform: scale(1);
  }
```
[Codepen Link](https://codepen.io/andreaspappoutas/pen/zYBoQGX)

[Link Κώδικα](https://github.com/andreaspappoutas/site/blob/master/_remix/button.md)

[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/button/)


# 2 - εντολών
Άσκηση: visualize git commits |	display your commits from a previous course, eg hci
# [Asciinema Git Bars](https://asciinema.org/a/367163)
Σε αυτή τη άσκηση έγινε χρήση του git bars. Μετά τη εγκατάσταση του git bars μέσο python έκανα clone το SW απο το δικο μου fork. Με τη πιο κάτω εντολή βλέπω όλα τα commits στο SW ανά μέρα:
```
git-bars -p day
```
Για να φανούν μόνο τα commits από εμένα έτρεξα το παρακάτω:
```
git-bars -p day -u andreaspappoutas
```

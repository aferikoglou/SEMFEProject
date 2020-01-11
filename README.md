# Δημιουργία Συστήματος Μέτρησης Αισθητήρων Πίεσης

Σε αυτό το project πραγματοποιήθηκε η δημιουργία ενός συστήματος μέτρησης αισθητήρων πίεσης. Το σύστημα αποτελείται από δύο τμήματα, το αναλογικό υποσύστημα και τον μικροελεγκτή. Το αναλογικό υποσύστημα αναλαμβάνει να κωδικοποιήσει την τιμή του αισθητήρα σε ψηφιακό σήμα. Ο μικροελεγκτής αναλαμβάνει να επιλέξει τον προς μέτρηση αισθητήρα και να αποκωδικοποιήσει το ψηφιακό σήμα με την μεγαλύτερη δυνατή ακρίβεια στο συντομότερο δυνατό χρόνο.

Για το σχεδιασμό του αναλογικού υποσυστήματος πραγματοποιήθηκαν προσομοιώσεις με την χρήση του εργαλείου [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html#). Το τελικό αρχείο προσομοίωσης βρίσκεται στον φάκελο __sim__.
  
Για περισσότερες πληροφορίες σχετικά με το σύστημα, στον φάκελο __docs__ βρίσκεται η πλήρης αναφορά στην οποία αναλύονται το αναλογικό και το ψηφιακό τμήμα, ο κώδικας, η μήτρα αισθητήρων καθώς και τα πειραματικά αποτελέσματα.

## Απαραίτητο Λογισμικό

Για την χρήση του συστήματος απαραίτητο είναι το [Arduino IDE](https://www.arduino.cc/en/main/software). Μέσω αυτού πραγματοποιείται η φόρτωση του κώδικα στον μικροελεγκτή καθώς και η αλληλεπίδραση με το σύστημα.

## Αλληλεπίδραση με το Σύστημα

Ο χρήστης χρησιμοποιώντας το *Arduino IDE* μπορεί να εκτελέσει τις παρακάτω δύο ενέργειες:
1. __Επιλογή συγκεκριμένου αισθητήρα για μέτρηση__
  - Η επιλογή γίνεται δίνοντας στο *Serial Monitor* *r * και έναν αριθμό από  το μηδέν ως το πλήθος των αισθητήρων μείον ένα. Τα αποτελέσματα της μέτρησης του συγκεκριμένου αισθητήρα φαίνονται στο *Serial Monitor*.

    *Παράδειγμα*
    Αν έχουμε στη διάθεσή μας *8* αισθητήρες οι δυνατές τιμές που μπορούμε να δώσουμε στο σύστημα είναι από *0* ως *7*. Για να πραγματοποιηθεί μέτρηση στον πρώτο αισθητήρα πρέπει να δώσουμε στο *Serial Monitor* *r 0* ενώ για να πραγματοποιηθεί μέτρηση στον πέμπτο αισθητήρα πρέπει να δώσουμε στο *Serial Monitor* *r 4*.

2. __Μέτρηση όλων των αισθητήρων__
  - Η μέτρηση όλων των αισθητήρων γίνεται δίνοντας στο *Serial Monitor* *rf*. Τα αποτελέσματα της μέτρησης των αισθητήρων φαίνονται στο *Serial Monitor*.

Η διακοπή της μέτρησης μπορεί να πραγματοποιηθεί πατώντας το κουμπί RESET του μικροελεγκτή.

## Μέλη Ομάδας

* **Βασιλοπούλου Φωτεινή**
* **Μάρκου Θανάσης**
* **Μυστιλίδης Χρήστος**
* **Φερίκογλου Άγγελος**

Το project αυτό δημιουργήθηκε για το εργαστήριο *Ηλεκτρονικών Νανοϋλικών και Διατάξεων της ΣΕΜΦΕ ΕΜΠ*. 
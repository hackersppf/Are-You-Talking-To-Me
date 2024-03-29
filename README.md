
# Are-You-Talking-To-Me
Μια φορητή συσκευή χειρός που μας ειδοποιεί όταν κάποιος μας απευθύνεται και είναι δύσκολο να τον ακούσουμε είτε λόγω θορύβου στον χώρο, είτε λόγω προβλημάτων ακοής που μπορεί να έχουμε. Η συσκευή που είναι σε μορφή wristband μας ειδοποιεί με δόνηση, μήνυμα στην οθόνη και ηχητικό σήμα. Συνδέεται ασύρματα με μια κεντρική συσκευή η οποία αξιοποιώντας τεχνητή νοημοσύνη παρακολουθεί τον ομιλητή και αναγνωρίζει ποιανού όνομα αναφέρει. Η ομάδα μας αποτελείται από μαθητές και μαθήτριες της E τάξης του [Πειραματικού Δημοτικού Σχολείου Φλώρινας](https://ppf.edu.gr/). 
# Αναλυτική περιγραφή ιδέας
Στόχος μας είναι να δημιουργήσουμε μια μικρή φορητή συσκευή σε μορφή wristband, η οποία συνδέεται ασύρματα με ένα κεντρικό σύστημα, το οποίο αξιοποιώντας τεχνητή νοημοσύνη παρακολουθεί έναν ομιλητή και να αναγνωρίζει ποιανού όνομα αναφέρει. Το κεντρικό σύστημα αφού αναγνωρίσει το όνομα θα μπορεί να ειδοποιεί την κατάλληλη φορητή συσκευή και αυτή με την σειρά της θα μπορεί να ειδοποιεί τον κάτοχο της ότι γίνεται αναφορά στο όνομα του, με δόνηση, με μήνυμα στην οθόνη και με ηχητικό σήμα. Σκοπεύουμε να δημιουργήσουμε αρκετά wristband τα οποία θα συνδέονται με το κεντρικό σύστημα ώστε να δοκιμάσουμε τις δυνατότητες τους.

Στο κεντρικό σύστημα θα υπάρχει ένας υπολογιστής ο οποίος θα είναι συνδεδεμένος με την πλατφόρμα [KCJ Teachable MachineTrained Model to micro:bit Bridge](https://apps.kidscodejeunesse.org/ml_to_mb_bridge/), και στον οποίο θα βρίσκεται συνδεδεμένο με καλώδιο USB ένα Microbit (σταθμός βάσης). Στην συγκεκριμένη πλατφόρμα θα έχουμε ήδη περάσει ένα μοντέλο αναγνώρισης ήχου που θα έχουμε δημιουργήσει στο Google Teachable Machine και θα περιλαμβάνει τα ονόματα των μαθητών της τάξης μας. Η συγκεκριμένη πλατφόρμα "ακούει¨ το μικρόφωνο του υπολογιστή μας και στέλνει το αποτέλεσμα του ελέγχου που κάνει με το μοντέλο τεχνητής νοημοσύνης στο Microbit του σταθμού βάσης μέσω σειριακής επικοινωνίας (USB). Το Microbit στέλνει το αποτέλεσμα της αναγνώρισης ασύρματα σε όλα τα υπόλοιπα Microbit που βρίσκονται εντός της εμβέλειας του.

Οι συσκευές χειρός (wristband) θα περιλαμβάνουν ένα Microbit, έναν κινητήρα δόνησης και μια μπαταρία coin cell τα οποία θα είναι τακτοποιημένα σε ειδική θήκη που θα σχεδιάσουμε και θα εκτυπώσουμε με τον 3Δ εκτυπωτή του εργαστηρίου μας. Τα Microbit θα λαμβάνουν σήμα από τον σταθμό βάσης και αν αυτό που μεταδίδεται είναι το όνομα του κατόχου, τότε θα τον ειδοποιούν με ενεργοποίηση της δόνησης, ηχητικό σήμα και εμφάνιση εικονιδίου στην οθόνη τους. 

Για τον σχεδιασμό των wristband και της στέγασης του σταθμού βάσης θα αξιοποιήσουμε 3Δ σχέδια τα οποία προσφέρονται ελεύθερα από την πλατφόρμα Thingiverse τα οποία θα τροποποιήσουμε με το TinkerCAD. Οι εκτυπώσεις θα γίνουν στους 3Δ εκτυπωτές του σχολείου μας με την χρήση υλικών PLA και TPU. 

Ως κεντρική πλατφόρμα ανάπτυξης θα αξιοποιήσουμε το MakeCode Microbit για τον προγραμματισμό των συσκευών, την πλατφόρμα [KCJ Teachable MachineTrained Model to micro:bit Bridge](https://apps.kidscodejeunesse.org/ml_to_mb_bridge/) για τον έλεγχο του μοντέλου τεχνητής νοημοσύνης, και την πλατφόρμα Google Teachable Machine για την δημιουργία του μοντέλου Τ.Ν.

# Eκπαιδευτικοί στόχοι του έργου
Οι βασικοί εκπαιδευτικοί στόχοι του έργου μας είναι οι μαθητές να:
 - κατανοήσουν τις βασικές αρχές εκπαίδευσης μοντέλων τεχνητής νοημοσύνης
 - κατανοήσουν την χρησιμότητα εφαρμογών τεχνητής νοημοσύνης
 - αποκτήσουν δεξιότητες 3Δ σχεδίασης με την χρήση απλών προγραμμάτων
 - αποκτήσουν δεξιότητες χρήσης του 3Δ εκτυπωτή του εργαστηρίου
 - αποκτήσουν δεξιότητες προγραμματισμού και αξιοποίησης τεχνολογιών όπως η τεχνητή νοημοσύνη με την χρήση του Google Teachable machine
 - αποκτήσουν δεξιότητες προγραμματισμού Microbit με το Makecode
# Λίστα προτεινόμενου εξοπλισμού
 - [PLA Fillament](https://grobotronics.com/creality-cr-pla-filament-1.75mm-1kg-grey.html) 4kg σε διαφορετικά χρώματα, κόστος 64 ευρώ
 - [TPU Fillament](https://grobotronics.com/3d-printer-filament-devil-tpu-1.75mm-white-1kg.html) 1kg, κόστος 32 ευρώ
 - [BBC Micro:bit V2 Board (Bulk)](https://grobotronics.com/bbc-micro-bit-v2-board-bulk.html) (X5), κόστος 75 ευρώ
 - [Κινητήρας Δόνησης 10mm](https://grobotronics.com/vibration-motor-1029.html) (X10), κόστος 12 ευρώ
 - [Electro-Fashion Switched Coin Cell Holder](https://grobotronics.com/electro-fashion-switched-coin-cell-holder.html) (X10), κόστος 24 ευρώ
 - [JST PH Jumper 2 Wire Assembly - 20cm](https://grobotronics.com/jst-jumper-2-wire-assembly-20cm.html) (X10), κόστος 2 ευρώ
 - [Μπαταρία Coin Cell CR2032 everActive - 5 τμχ.](https://grobotronics.com/mpataria-coin-cell-cr2032-everactive-5pcs.html) (X4), κόστος 5 ευρώ
 - [Σετ Εργαλείων Κόλλησης 80W](https://grobotronics.com/soldering-tool-set-80w-12pcs.html), κόστος 24 ευρώ
 - [Copymaster3D Magnetic Build Surface 235x235 mm](https://grobotronics.com/copymaster3d-magnetic-build-surface-235x235-mm.html), κόστος 13 ευρώ
**Συνολικό κόστος: 251 ευρώ**
# Υπεύθυνοι εκπαιδευτικοί
 - [Γιάννης Αρβανιτάκης](https://ioarvanit.gr/)
 - Αμαραντίδου Κυριακή

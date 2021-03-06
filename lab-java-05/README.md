### Εργαστήριο #5 - Πίνακες
___
Σκοπός του πέμπτου εργαστηρίου είναι να εξοικειωθείτε με τη χρήση πινάκων αντικειμένων ως μέλη δεδομένων και
με το πέρασμά τους παραμέτρους ή επιστρεφόμενες τιμές στη γλώσσα προγραμματισμού Java.
___
#### Άσκηση ####
___Χρησιμοποιείστε στον κώδικα του εργαστηρίου 4 για την κλάση Order___

Δημιουργήστε μια κλάση, την `OrdersUI`, η οποία να περιέχει ως data member ένα πίνακα αντικειμένων τύπου `Orders` μεγέθους `10`.

Η κλάση OrdersUI θα πρέπει να παρέχει ένα text ui για τη δημιουργία και διαχείριση αντικειμένων τύπου Order. Λειτουργίες που πρέπει να παρέχει είναι οι εξής (όλες μέσω `public` μεθόδων):
* Διαλογική προσθήκη μιας νέας παραγγελίας στον πίνακα.
    * Να διαβάζει όλα τα _συστατικά_ μιας παραγγελίας (είδος, τιμή μονάδας, ποσότητα, έκπτωση)
    * Αν μια παραγγελία για όμοιο είδος υπάρχει ήδη στον πίνακα (κάντε χρήση της `Order.equals()`!), τότε να μη δημιουργείται νέα αλλά η υπαρχουσα παραγγελία να ενημερώνεται - δημιουργήστε μια `private` βοηθητική μέθοδο για τον έλεγχο/εύρεση μια παραγγελίας όμοιου είδους
    * Αν το μέγιστο πλήθος παραγγελιών που μπορούν να αποθηκευτούν στον πίνακα έχουν δοθεί, να μη δέχεται εισαγωγή στοιχείων.
* Εμφάνιση όλων των παραγγελιών (κάντε χρήση της `Order.toString()`!).
* Διαγραφή μιας παραγγελίας, με βάση τη θέση της στον πίνακα.
    * Αν η θέση είναι άδεια, εμφανίστε σχετικό μήνυμα.
    * Αν η παραγγελία υπάρχει, η μέθοδος να την επιστρέφει.
    * Αν υπάρχουν παραγγελίες στις επόμενες θέσεις, αυτές να μετακινούνται μια θέση πριν.
* Λειτουργία μενού για όλα τα πιο πάνω. Τερματισμός της εφαρμογής να γίνεται όταν ο χρήστης δώσει το χαρακτήρα `Q` στην είσοδο του μενού.

NB.: Κάντε μόνο τις πολύ απαραίτητες τροποποιήσεις στην Order, πχ προσθήκη getter/setter για όποια
μέλη δεδομένων χρειάζεται (και μην ξεχνάτε τους ελέγχους που χρειάζονται, πχ αν η τιμή ειναι <0)

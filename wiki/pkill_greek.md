# [Ελληνικά] Debian Almquist Shell (dash) pkill Χρήση: Διακόπτει διεργασίες με βάση το όνομά τους

## Επισκόπηση
Η εντολή `pkill` χρησιμοποιείται για να τερματίσει διεργασίες που τρέχουν στο σύστημα, βασιζόμενη στο όνομα της διεργασίας ή σε άλλα κριτήρια. Είναι χρήσιμη για τη διαχείριση διεργασιών χωρίς να χρειάζεται να βρείτε πρώτα το PID (Process ID) τους.

## Χρήση
Η βασική σύνταξη της εντολής `pkill` είναι η εξής:

```
pkill [options] [arguments]
```

## Κοινές Επιλογές
- `-f`: Τερματίζει διεργασίες με βάση το πλήρες όνομα της εντολής.
- `-n`: Τερματίζει μόνο την πιο πρόσφατη διεργασία που ταιριάζει με τα κριτήρια.
- `-o`: Τερματίζει μόνο την παλαιότερη διεργασία που ταιριάζει με τα κριτήρια.
- `-signal`: Καθορίζει το σήμα που θα σταλεί στις διεργασίες (προεπιλογή είναι το SIGTERM).

## Κοινά Παραδείγματα
1. Τερματισμός διεργασίας με συγκεκριμένο όνομα:
   ```bash
   pkill firefox
   ```

2. Τερματισμός διεργασίας με βάση το πλήρες όνομα:
   ```bash
   pkill -f "python script.py"
   ```

3. Τερματισμός μόνο της πιο πρόσφατης διεργασίας:
   ```bash
   pkill -n chrome
   ```

4. Αποστολή συγκεκριμένου σήματος (π.χ. SIGKILL):
   ```bash
   pkill -9 apache2
   ```

## Συμβουλές
- Χρησιμοποιήστε την επιλογή `-f` εάν χρειάζεται να τερματίσετε διεργασίες που εκτελούνται με πλήρη εντολή.
- Να είστε προσεκτικοί με τη χρήση του `pkill`, καθώς μπορεί να τερματίσει πολλές διεργασίες ταυτόχρονα αν δεν καθορίσετε συγκεκριμένα κριτήρια.
- Μπορείτε να χρησιμοποιήσετε την εντολή `pgrep` για να δείτε ποιες διεργασίες θα επηρεαστούν πριν χρησιμοποιήσετε το `pkill`.
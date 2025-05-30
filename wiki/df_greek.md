# [Διανομή] Debian Almquist Shell (dash) df Χρήση: [εμφάνιση διαθέσιμου χώρου αποθήκευσης]

## Overview
Η εντολή `df` χρησιμοποιείται για να εμφανίσει πληροφορίες σχετικά με τον διαθέσιμο και χρησιμοποιούμενο χώρο αποθήκευσης σε συστήματα αρχείων. Παρέχει μια συνοπτική εικόνα της χωρητικότητας των διαμερισμάτων του δίσκου.

## Usage
Η βασική σύνταξη της εντολής είναι η εξής:

```
df [options] [arguments]
```

## Common Options
- `-h`: Εμφανίζει το μέγεθος σε "φιλικές" μορφές (π.χ. KB, MB, GB).
- `-T`: Εμφανίζει τον τύπο του συστήματος αρχείων.
- `-a`: Εμφανίζει όλα τα συστήματα αρχείων, συμπεριλαμβανομένων των εικονικών.
- `-i`: Εμφανίζει πληροφορίες σχετικά με τα inodes αντί για τον χώρο αποθήκευσης.

## Common Examples
- Για να δείτε τον διαθέσιμο χώρο σε φιλική μορφή:
  ```bash
  df -h
  ```

- Για να δείτε τον τύπο του συστήματος αρχείων:
  ```bash
  df -T
  ```

- Για να δείτε πληροφορίες για όλα τα συστήματα αρχείων:
  ```bash
  df -a
  ```

- Για να δείτε πληροφορίες σχετικά με τα inodes:
  ```bash
  df -i
  ```

## Tips
- Χρησιμοποιήστε την επιλογή `-h` για να διευκολύνετε την ανάγνωση των δεδομένων, ειδικά σε συστήματα με μεγάλο χώρο αποθήκευσης.
- Συνδυάστε την `df` με άλλες εντολές, όπως `grep`, για να φιλτράρετε συγκεκριμένα συστήματα αρχείων.
- Ελέγξτε τακτικά τον διαθέσιμο χώρο αποθήκευσης για να αποφεύγετε προβλήματα με την έλλειψη χώρου.
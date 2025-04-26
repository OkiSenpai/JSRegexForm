# JSRegexForm
# Contact Form Validation with JavaScript

# EN

This project demonstrates a simple contact form with client-side validation using JavaScript. The form includes fields for a user's name, first name, email, phone number, and message. Each field is validated using regular expressions (regex) to ensure the input meets specific criteria before submission.

## Features

- **Real-time Validation**: Each input field is validated when the user clicks the submit button.
- **Error Messages**: Displays error messages in red for invalid or empty fields.
- **Regex Validation**: Ensures that inputs match specific patterns for names, email, phone numbers, and messages.
- **User Feedback**: Alerts the user when the form is successfully submitted.

## Form Fields

The form includes the following fields:

1. **Name (Nom)**:
   - Regex: `^[A-Za-zÀ-ÿ\s'-]{2,50}$`
   - Validates that the name contains 2-50 characters, including letters, spaces, hyphens, and apostrophes.

2. **First Name (Prénom)**:
   - Regex: `^[A-Za-zÀ-ÿ\s'-]{2,50}$`
   - Similar validation as the name field.

3. **Email**:
   - Regex: `^[\w.-]+@[\w.-]+\.\w{2,}$`
   - Validates a standard email format.

4. **Phone Number (Téléphone)**:
   - Regex: `^(?:\+32|0)[1-9]\d{7,8}$`
   - Validates Belgian phone numbers, allowing either a `+32` country code or a leading `0`.

5. **Message**:
   - Regex: `^.{5,1000}$`
   - Ensures the message is between 5 and 1000 characters.

## How It Works

1. **HTML Structure**:
   - The form is built using standard HTML elements, with `id` attributes assigned to each input field and corresponding error message spans.

2. **JavaScript Validation**:
   - A `verificationDeInput` function is defined to handle validation.
   - Event listener on the submit button (`btn`) prevents default form submission and validates each field.
   - If a field is empty or does not match its regex, an error message is displayed in red.
   - If all fields are valid, an alert is shown indicating successful submission.

3. **Error Handling**:
   - Each field has a dedicated `<span>` element to display error messages.
   - Error messages are styled in red for better visibility.

# FR

# Validation du formulaire de contact avec JavaScript

Ce projet démontre un formulaire de contact simple avec une validation côté client en JavaScript. Le formulaire comprend des champs pour le nom, le prénom, l'email, le numéro de téléphone et le message de l'utilisateur. Chaque champ est validé à l'aide d'expressions régulières (regex) pour s'assurer que les entrées respectent des critères spécifiques avant la soumission.

## Fonctionnalités

- **Validation en temps réel** : Chaque champ est validé lorsque l'utilisateur clique sur le bouton de soumission.
- **Messages d'erreur** : Affiche des messages d'erreur en rouge pour les champs invalides ou vides.
- **Validation avec Regex** : Vérifie que les entrées correspondent à des modèles spécifiques pour les noms, les emails, les numéros de téléphone et les messages.
- **Retour utilisateur** : Alerte l'utilisateur lorsque le formulaire est soumis avec succès.

## Champs du formulaire

Le formulaire comprend les champs suivants :

1. **Nom** :
   - Regex : `^[A-Za-zÀ-ÿ\s'-]{2,50}$`
   - Valide que le nom contient entre 2 et 50 caractères, y compris des lettres, des espaces, des tirets et des apostrophes.

2. **Prénom** :
   - Regex : `^[A-Za-zÀ-ÿ\s'-]{2,50}$`
   - Validation similaire au champ du nom.

3. **Email** :
   - Regex : `^[\w.-]+@[\w.-]+\.\w{2,}$`
   - Valide un format d'email standard.

4. **Numéro de téléphone** :
   - Regex : `^(?:\+32|0)[1-9]\d{7,8}$`
   - Valide les numéros de téléphone belges, permettant soit un indicatif `+32`, soit un `0` initial.

5. **Message** :
   - Regex : `^.{5,1000}$`
   - S'assure que le message contient entre 5 et 1000 caractères.

## Comment ça marche

1. **Structure HTML** :
   - Le formulaire est construit à l'aide d'éléments HTML standard, avec des attributs `id` assignés à chaque champ de saisie et aux spans des messages d'erreur correspondants.

2. **Validation JavaScript** :
   - Une fonction `verificationDeInput` est définie pour gérer la validation.
   - Un écouteur d'événement sur le bouton de soumission (`btn`) empêche la soumission par défaut du formulaire et valide chaque champ.
   - Si un champ est vide ou ne correspond pas à son regex, un message d'erreur est affiché en rouge.
   - Si tous les champs sont valides, une alerte indique une soumission réussie.

3. **Gestion des erreurs** :
   - Chaque champ a un élément `<span>` dédié pour afficher les messages d'erreur.
   - Les messages d'erreur sont stylés en rouge pour une meilleure visibilité.

# Page: Paiement (checkout.html)

## 1. Purpose

The **Paiement** (Checkout) page is the final step in the user's purchasing journey. Its sole purpose is to securely collect billing and payment information to finalize a subscription or purchase. This page is critical for conversion, and its design is focused on clarity, security, and ease of use to minimize user friction and cart abandonment.

## 2. Main Features

The page is structured as a standard e-commerce checkout, with a clear separation between the input form and the order summary.

### Header Navigation

The standard sidebar navigation is present, but it's less critical here as the user's focus should be on completing the transaction.

### Checkout Layout

The main content is a two-column layout.

- **Left Column: Checkout Form**
  - **Section Title**: "Informations de facturation" (Billing Information).
  - **Input Fields**:
    - `Nom complet` (Full Name)
    - `Adresse e-mail` (Email Address)
    - `Nom de l'entreprise` (Company Name) - optional.
  - **Section Title**: "Informations de paiement" (Payment Information).
  - **Payment Fields**:
    - A placeholder `div` (`card-element`) for a credit card processing library (like Stripe Elements or Braintree).
    - Includes placeholders for Card Number, Expiry Date (MM/AA), and CVC.
  - **Submit Button**: A prominent "Confirmer et Payer" (Confirm and Pay) button.

- **Right Column: Order Summary**
  - **Section Title**: "Résumé de la commande" (Order Summary).
  - **Dynamic Fields**: This section is designed to be populated dynamically by JavaScript.
    - `Offre`: The name of the selected plan (e.g., "Business"). This is pulled from the `offer` URL parameter.
    - `Prix`: The price of the plan (e.g., "3000 DH/mois"). This is pulled from the `price` URL parameter.
    - `Total`: The final price to be paid.

### Footer

The standard site footer is present.

## 3. Navigation

- **Arrival**: Users arrive at this page exclusively after clicking a purchase button (e.g., "Choisir cette offre") on the `offres.html` page. They arrive with URL parameters like `?offer=Business&price=3000` which are used to populate the order summary.
- **Departure**:
  - **Successful Payment**: After the user clicks "Confirmer et Payer" and the payment is successfully processed, they should be redirected to the `confirmation.html` page.
  - **Failed Payment**: If the payment fails, the user should remain on the page with an error message displayed, allowing them to correct their information.
  - **Abandonment**: The user might abandon the process by using the main navigation to go to another page.

## 4. User Guidance

This page must be as simple and trustworthy as possible.

- **Auto-populated Summary**: The user immediately sees a summary of what they are about to pay for. This is populated automatically, which reassures them that they have selected the correct plan. The `script.js` file is responsible for reading the URL parameters and filling in the `#offer-name`, `#offer-price`, and `#total-price` fields.
- **Clear Form**: The payment form is straightforward, asking only for essential information. The fields are clearly labeled (or use placeholders) for ease of use.
- **Security**: While not visible in the HTML, it is implied that a secure payment gateway (like Stripe or PayPal) would be integrated here to handle the credit card data securely. The `card-element` div is a strong hint of this.
- **Single Action**: The user has one primary action: to fill the form and click "Confirmer et Payer". There are no distracting elements on the page.

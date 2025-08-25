# 6. Checkout Page - checkout.html

**Purpose:** This is the transaction completion page. Its sole function is to securely collect the user's billing and payment information to finalize the subscription process.

**Main Features & Sections:**

**Order Summary:** Clearly displays the selected offer name and price, providing reassurance and preventing errors. The total is calculated and displayed.

**Billing Information Form:** Fields for collecting essential details: Full Name, Email, and Company Name (optional).

**Payment Information Form:** A simplified credit card input area for Card Number, Expiry Date, and CVC code. (Note: For a real application, this should be replaced with a secure PCI-compliant payment gateway like Stripe or PayPal).

**Confirmation Button:** A prominent "Confirmer et Payer" button that triggers the order processing.

**Navigation:**

*   **Arrival:** Users are directed here exclusively from the "Choisir" buttons on the offres.html page, with URL parameters defining their selection.
*   **Next Steps:** Upon successful form submission (handled by JavaScript), the user is redirected to the confirmation.html page.

**User Guidance:** "You're almost there! Please review your order summary on the right. On the left, fill in your billing details and secure payment information to activate your SELYN membership. Once you confirm, you'll receive a welcome email and gain full access."

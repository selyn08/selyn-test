# Page: Confirmation de Commande (confirmation.html)

## 1. Purpose

The **Confirmation de Commande** page has a single, crucial purpose: to inform the user that their transaction was successful. It serves as the final, reassuring step in the payment process. The goal is to eliminate any user anxiety about whether their payment went through and to provide clear information about what happens next.

## 2. Main Features

The page is intentionally simple and focused to deliver a clear message of success.

### Header Navigation

The standard sidebar navigation is present, though the user's journey is likely complete at this point.

### Confirmation Section

The entire page consists of one central section.

- **Success Icon**: A large, green checkmark icon (`<i class="fas fa-check-circle"></i>`) is the most prominent visual element, providing immediate, non-verbal confirmation of success.
- **Main Headline**: "Merci pour votre confiance !" (Thank you for your trust!).
- **Descriptive Text**:
  - Informs the user that their order was processed successfully.
  - States that a confirmation email with subscription details has been sent. This is a critical piece of information, as it sets the user's expectation for receiving a receipt and further instructions.
- **Welcome Message**: "Bienvenue dans la communauté SELYN !" (Welcome to the SELYN community!) adds a friendly, personal touch.
- **Call-to-Action Button**: A single button, "Retour à l'accueil" (Return to Home), provides a clear next step for the user, guiding them back to the main page of the site.

### Footer

The standard site footer is present.

## 3. Navigation

- **Arrival**: Users should only ever arrive on this page after a successful payment submission on the `checkout.html` page. It is the destination of a successful redirect.
- **Departure**: The primary exit point is the "Retour à l'accueil" button, which takes the user back to `index.html`. Alternatively, they can use the main navigation to go to any other page.

## 4. User Guidance

This page is designed to be self-explanatory.

- **Instant Reassurance**: The user immediately sees the green checkmark and the "Merci" message, which confirms their action was successful.
- **Clear Next Steps**: The text clearly tells the user to check their email for details. This manages their expectations and tells them where to find important information about their purchase.
- **End of Journey**: This page marks the end of the purchase funnel. The "Retour à l'accueil" button provides a graceful way for the user to re-engage with the site's content or simply close the tab, knowing their task is complete.

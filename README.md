# CreditCardSimulation
Brief Description: The project simulates a credit card payment portal where users input card details such as name, card number, and expiry date. On pressing "Verify", the system validates inputs and updates the visual card image based on the card type (Visa, Mastercard, AmEx, Discover). If invalid, error messages are shown. Pressing "Clear" resets the form. The GUI updates in real-time via event handling (e.g., KeyListeners, ActionListeners).

**Time Spent** : 6 hours spent in total.

User Stories
The following Required User Stories are complete:
As a user, I want to enter a cardholder name so that I can simulate a real credit card.
As a user, I want to enter a 16-digit credit card number split into 4 parts so that the card image updates dynamically and accurately.
As a user, I want to enter an expiry date in MM/YY format so that the card appears realistic and complete.
As a user, I want the "Verify" button to check all inputs so that I know if the information I entered is valid.
As a user, I want the credit card image to change based on the first digits of the number so that I see the type of card (Visa, Mastercard, etc.) I'm using.
As a user, I want to see error messages if any input is invalid so that I know what to fix.
As a user, I want to press a "Clear" button so that I can reset the form to the default state.

The following Stretch User Stories are implemented:
As a user, I want real-time validation while typing so that I can correct mistakes instantly (e.g., invalid characters in the name).
As a user, I want each section of the card number to update its corresponding overlay label so that the card image mirrors my input exactly.
As a user, I want the app to ignore invalid punctuation in the cardholder name to avoid unexpected errors.
As a user, I want visual feedback (e.g., color changes) for valid and invalid input so I can clearly identify correct/incorrect fields.

The following Additional User Stories are implemented:
As a user, I want a default placeholder text or hint in each input field so I know the expected format (e.g., "MM/YY", "XXXX XXXX XXXX XXXX").

Here are some challenges encountered but were overcome:
Implementing Real-Time Validation:
Handling input validation in real-time using KeyListener interfaces was tricky, especially when filtering out invalid characters without disrupting the typing experience.

Synchronizing Input with Overlay Labels:
Updating each of the four credit card number overlay labels based on the user's input required careful indexing and string manipulation to avoid out-of-bound errors and mismatched segments.

Validating Expiry Date Format (MM/YY):
Ensuring the expiry date was always entered in the correct format and was logically valid (e.g., not expired or using invalid months) added complexity to the validation logic.

Managing GUI State Changes:
Switching between different credit card images depending on the starting digits involved conditional logic and proper use of JLabel and ImageIcon, which could cause display issues if not handled correctly.

Resetting the GUI on Clear:
Ensuring that all fields, overlay labels, and images reverted to their original state when "Clear" was pressed required consistent tracking of default values and UI components.

Displaying Error Messages Accurately:
Providing clear and contextual error messages for each type of input failure (name, number, expiry) required breaking down validation feedback without overwhelming the user.

Event Listener Coordination:
Coordinating multiple event listeners (KeyListener, ActionListener) and making sure they worked together without conflicting or missing events was a frequent source of bugs.

Link to Video Demo: https://drive.google.com/file/d/1qFUtIly0FDsREaXA04hSQ9YJM5eTIw8H/view?usp=sharing


Notes:
This project gave me a great deal of satisfaction and I am proud, since it called on me to employ a range of object-oriented programming paradigms in attempting to simulate real-world conditions. It forced me to learn about event-driven programming, so far as how listeners operate in a GUI environment, in real-time. I learned how to perform effective validations on user input comments and how to provide immediate feedback through a dynamic interface.

I also derived a lot of satisfaction from seeing the interface respond visually to the different types of cards — it gave life to the application. Although debugging seemed to be quite a challenge when trying to sync up some labels or when validating the card number, seeing everything come together inspired in me greater appreciation for my programming skills. I felt like this was one of the very first projects that made me feel as though I was really building something interactive and user-friendly from the ground up.

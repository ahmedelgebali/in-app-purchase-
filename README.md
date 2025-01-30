# Subscription & Restore Purchase Flow

## 1. Subscription Flow

### 1.2 Subscription Options
   Users can choose from the following plans:
   - **Monthly** → `$ Price TBD`
   - **Yearly** → `$ TBD` (initially highlighted)
   - **Lifetime** → `$ TBD`

- The **1-year plan** is visually marked as (**Recommended**).

### 1.3 Subscription Activation
When the user clicks **"Subscribe"**:
A. The app initiates the **in-app purchase process** via Apple/Google.
B. If the payment is **successful**:
   - Ads are removed.
   - Premium features are unlocked (e.g., **VIP support**).
   - A confirmation message appears:

     ```
     "Congratulations! You’ve successfully upgraded to Premium."
     ```
   - The UI updates to reflect **premium status**.
C. If the payment **fails**, an error message appears.

### 1.4 Subscription Wall Behavior (After Purchase)
- If a **subscribed user** reopens the subscription page the app pop-up the next:

  ```
  "You're already subscribed to the (package name). Do you want to change your plan?"
  ```
  With Yes & No options
- **Yes** → Allows switching to another package.
- **No** → Closes the subscription page.

- If the user **tries to subscribe** to the same plan, the app displays:

  ```
  "You're already subscribed to this package."
  ```
---

## 2. Restore Purchase Flow

- When the user clicks **"Restore Purchase"**, the app checks for an **active subscription** via **Apple ID or Google Account**.
- If an **active subscription** is found:

  ```
  "You've successfully restored your purchase."
  ```


- If **no active subscription** is found:
  ```
  "Sorry, you don't have an active subscription."
  ```


- If the user clicks **Restore Purchase** while **already subscribed**, the app displays:

  ```
  "Your purchase is already active."
  ```

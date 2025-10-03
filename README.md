# 🌍 Dynamic Currency Converter

A simple, fast, and responsive web application built with pure HTML, CSS, and JavaScript to convert amounts between multiple currencies.

## ✨ Features

* **Multi-Currency Conversion:** Convert between a pre-defined set of major world currencies (USD, EUR, GBP, INR, JPY, CAD).
* **Intuitive Interface:** Clean, user-friendly design with clear input and result areas.
* **Responsive Design:** Works seamlessly across desktop and mobile devices.
* **Pure Client-Side:** No backend required; uses static exchange rates (ready for API integration).

## 🚀 Getting Started

### Prerequisites

You only need a modern web browser to run this application.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd YOUR_REPO_NAME
    ```
3.  **Open the file:**
    Simply open the `index.html` file in your preferred web browser.

    *(Alternatively, you can host it on GitHub Pages or any static file server.)*

## 🛠️ Technology Stack

| Technology | Purpose |
| :--- | :--- |
| **HTML5** | Structure and Content |
| **CSS3** | Styling and Responsive Design |
| **JavaScript (ES6)** | Core Conversion Logic and DOM Manipulation |

## ⚙️ How it Works (Conversion Logic)

The conversion logic relies on a fixed set of **base rates relative to the US Dollar (USD)** stored in a JavaScript object (`exchangeRates`).

1.  **Normalize to USD:** The input amount is first converted into its equivalent USD value.
    $$\text{Amount}_{\text{USD}} = \frac{\text{Amount}_{\text{FROM}}}{\text{Rate}_{\text{FROM}}}$$
2.  **Convert to Target:** The USD value is then multiplied by the target currency's rate to get the final converted amount.
    $$\text{Amount}_{\text{TO}} = \text{Amount}_{\text{USD}} \times \text{Rate}_{\text{TO}}$$

### ⚠️ Disclaimer on Rates
* **Current exchange rates are hardcoded** in the `script` tag within `index.html` for demonstration purposes.
* The rates are **NOT real-time** and should not be relied upon for actual financial transactions.

## 🤝 Future Enhancements (To-Do)

* [ ] Integrate a **real-time Exchange Rate API** (e.g., Open Exchange Rates, ExchangeRate-API) to fetch current data.
* [ ] Add more currency options and flags for better visual appeal.
* [ ] Implement a feature to swap the "From" and "To" currencies with a single button.
* [ ] Use local storage to save the last used currencies.

## 🌟 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---
*Created by SachinSharma-2003*

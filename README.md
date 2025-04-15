# Service Business Manager

A simple, offline-first web application built with HTML, CSS, and JavaScript to help service-based businesses manage clients and create quotes directly in the browser. All data is stored locally using LocalStorage.

## Features

* **Client Management:**
    * Add, edit, and delete client information (name, contact details, address, notes).
    * Search clients.
    * View client details and their associated quote history.
* **Quote/Estimate Management:**
    * Create new quotes, selecting from existing clients or adding new ones on the fly.
    * Add line items with descriptions, quantities, and unit prices.
    * Automatic calculation of subtotal, tax (based on settings), and total.
    * Manage quote status (Draft, Sent, Accepted, Rejected).
    * Add custom terms & conditions and notes.
    * Preview quotes before saving or printing.
    * Duplicate existing quotes.
    * Print quotes.
    * Email quote details using a `mailto:` link.
* **Settings:**
    * Configure business name, address, phone, email.
    * Upload a business logo (stored as Data URL in LocalStorage).
    * Set default tax rate.
    * Customize quote number prefix and starting number.
* **Data Management:**
    * All data is stored in the browser's LocalStorage.
    * Export all data (clients, quotes, settings) as a JSON file.
    * Import data from a previously exported JSON file (overwrites existing data).
    * Automatic backup to LocalStorage (can be toggled in settings).
* **Offline Functionality:** Works entirely offline once the HTML file is loaded.

## How to Use

1.  Download the `index.html` file.
2.  Open the file in your web browser.
3.  Start adding clients and creating quotes!

## Technology Stack

* HTML
* CSS
* JavaScript (Vanilla)
* Browser LocalStorage API

## Limitations

* **Browser Dependent:** Data is stored only in the browser where the file is used. Clearing browser data will erase all saved information unless backed up.
* **No Cloud Sync:** This is an offline-only tool; data is not synced across devices or users.
* **LocalStorage Limits:** Browsers have storage limits for LocalStorage (typically 5-10MB), which might be exceeded with extensive use or large logos.

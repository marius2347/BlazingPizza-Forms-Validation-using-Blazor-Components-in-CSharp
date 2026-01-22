# Blazing Pizza - Advanced Forms & Validation 📝

This repository contains the **Forms and Validation** module of the Blazing Pizza application. It demonstrates the transition from standard HTML forms to **Blazor's `EditForm` component**, enabling robust data binding, validation, and submission logic tailored for Single Page Applications (SPA).

## 🚀 Features & Enhancements

Based on the **ASP.NET Core Blazor** forms architecture, this project implements the following:

* **EditForm Component:** Replaced standard `<form>` tags with `<EditForm>` to establish an `EditContext` that tracks field modifications and validation status.
* **Blazor Input Components:** utilized built-in components that handle type conversion and binding automatically:
    * `InputText` for string fields (Name, Address).
    * `InputNumber` for numeric values.
    * `InputTextArea` for longer descriptions.
* **Model Validation:** Implemented server-side validation using **Data Annotations** (`System.ComponentModel.DataAnnotations`) directly on the `Address` model:
    * `[Required]` to ensure mandatory fields are filled.
    * `[MinLength]` and `[MaxLength]` to enforce character limits.
    * `[EmailAddress]` to validate email formats.
* **Validation Logic:** Integrated `<DataAnnotationsValidator>` to enforce rules and `<ValidationSummary>` to display all errors in a centralized list.
* **Event Handling:** Configured the `OnValidSubmit` event to ensure the order placement logic only triggers when the form state is valid.

## 📸 Screenshots

### Real-time Form Validation
*Demonstrates the `EditForm` in action, showing validation error messages triggered by the `DataAnnotationsValidator`.*

![Validation Example](validation.png)

## 🛠️ Technologies Used

* **Framework:** ASP.NET Core Blazor
* **Components:** `EditForm`, `InputText`, `InputNumber`, `ValidationMessage`
* **Namespace:** `System.ComponentModel.DataAnnotations`
* **Language:** C#
* **Frontend:** Razor Syntax, HTML5, CSS

## 📦 Getting Started

To run this application locally:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/marius2347/BlazingPizza-Forms-Validation-using-Blazor-Components-in-CSharp.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd BlazingPizza-Forms-Validation-using-Blazor-Components-in-CSharp
    ```
3.  **Run the application:**
    ```bash
    dotnet run
    ```
4.  Open your browser and navigate to the localhost URL shown in the terminal (e.g., `https://localhost:7000`).
5.  Go to the checkout screen and try submitting the form with empty fields to test the validation.

## 📬 Contact

If you have any questions about this implementation, feel free to reach out:

* **Email:** [mariusc0023@gmail.com](mailto:mariusc0023@gmail.com)

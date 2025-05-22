
# ASP.NET MVC AJAX Form Submission Project

This is a simple demonstration of how to use **AJAX with jQuery** to submit form data asynchronously in an **ASP.NET MVC 5** application. It enhances the user experience by submitting forms without a full page reload.

## 🚀 Features

- jQuery AJAX form submission
- MVC model binding and validation
- Bootstrap-based styling
- Partial View support
- Form POST without page refresh

## 🧰 Technologies Used

- ASP.NET MVC 5
- jQuery
- AJAX
- Bootstrap 5
- Razor Views
- C#

## 📁 Project Structure

```
├── Controllers/        # MVC Controllers
├── Models/             # Data Models
├── Views/              # Razor Views and Partials
├── Content/            # CSS files (Bootstrap, custom styles)
├── Scripts/            # jQuery and AJAX scripts
├── Web.config          # App configuration
```

## 📌 How It Works

- A standard MVC form is rendered on the view
- On submit, a jQuery AJAX call sends the form data to a controller action
- The controller handles model validation and processing
- The response updates a portion of the page using Partial Views or plain HTML

### Example AJAX Call

```javascript
$.ajax({
    type: "POST",
    url: "/Home/SubmitForm",
    data: $("#myForm").serialize(),
    success: function (response) {
        $("#result").html(response);
    }
});
```

## 🏗️ Getting Started

### Prerequisites

- Visual Studio 2019 or later
- .NET Framework 4.7.2+

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/oguzhansaritas/asp.net-mvc-ajax-post-project.git
   ```

2. Open the solution file (`.sln`) in Visual Studio.

3. Build the solution and run the project.

4. Navigate to the Home page and test the AJAX form.


## 🙌 Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

This project is licensed under the MIT License.

## 📬 Contact

Created by **OĞUZHAN SARITAŞ** – contact at info@oguzhansaritas.com

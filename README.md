

# QR Code Generation for Bank Accounts

This project implements a feature that allows users to generate unique QR codes linking a person's name and their bank account number. The QR codes can be scanned by anyone to retrieve the associated information securely.

## Features

- **User Input Form**: A simple and user-friendly form for users to input their name and bank account number.
- **QR Code Generation**: Once the form is submitted, the system generates a unique QR code containing the user’s name and bank account number.
- **Downloadable QR Code**: The generated QR code can be downloaded for users to store or print.
- **Secure Data**: The information in the QR code is only accessible by scanning the QR code, ensuring privacy and security.

## Installation

1. **Clone the Repository**

   Clone this repository to your local machine using:

   ```bash
   git clone https://github.com/Bibek1604/QR-GENERATOR.git
   ```

2. **Install Dependencies**

   Navigate to the project directory and install the required dependencies:

   ```bash
   cd qr-code-bank
   pip install -r requirements.txt
   ```

3. **Set Up Database**

   Run the following commands to apply migrations and set up the database:

   ```bash
   python manage.py migrate
   ```

4. **Run the Application**

   To run the application locally, use the following command:

   ```bash
   python manage.py runserver
   ```

   The server will start running on `http://127.0.0.1:8000` by default.

## Usage

1. Open the website in your browser.
2. Input the name and bank account number in the provided form.
3. Click on the **Generate QR Code** button.
4. The system will generate a QR code, which will appear on the screen.
5. Click **Download QR Code** to save the QR code image to your device.

## Security Considerations

- The QR code will encode the name and bank account number, which should be shared only with trusted parties.
- It’s recommended to not share QR codes in public spaces to prevent unauthorized scanning.
- Ensure that your website uses HTTPS to keep data transmission secure.

## Technologies Used

- **Backend**: Django
- **QR Code Generation**: `qrcode` library
- **Frontend**: HTML, CSS, JavaScript
- **Hosting**: Local/Cloud server

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit pull requests. Please ensure to add tests for any new functionality.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


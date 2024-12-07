
# Snippetbox 📜  

Snippetbox is a web application for pasting and sharing snippets of text, inspired by tools like Pastebin and GitHub Gists. Built step-by-step using the Go programming language, this project follows the tutorial in the book *Let's Go* by Alex Edwards.

## Features ✨  
- View and create text snippets.
- User authentication and session management.
- Secure server configuration with HTTPS.
- Dynamic HTML templating and inheritance.
- Middleware for enhanced functionality.
- A MySQL database for storing snippets.

## Project Structure 📂  
The project follows a modular structure for scalability and maintainability:  
```
.
├── cmd/web         # Main application entry point and handlers
├── internal        # Reusable code such as database models and helpers
├── ui
│   ├── html        # HTML templates for the application
│   └── static      # Static assets (CSS, JS, images)
└── go.mod          # Go module dependencies
```

## Getting Started 🚀  

### Prerequisites  
- Go version 1.23 or higher. [Download here](https://golang.org/doc/install).  
- MySQL database.  

### Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/mujeebcodes/snippetbox.git
   cd snippetbox
   ```

2. Install Go dependencies:  
   ```bash
   go mod tidy
   ```

3. Set up the MySQL database:
   - Create a database named `snippetbox`.
   - Run the SQL schema provided in `internal/models/schema.sql`.

4. Start the application:  
   ```bash
   go run ./cmd/web
   ```

5. Access the application at [http://localhost:4000](http://localhost:4000).

### Configuration  
Environment variables:  
- `DSN`: Data Source Name for connecting to the MySQL database (e.g., `user:password@/snippetbox`).  

## Development 🛠️  

### Running Tests  
Unit and integration tests can be run using:  
```bash
go test ./...
```

### Directory for Templates  
HTML templates are located in the `ui/html` directory, and you can customize them to change the appearance of the application.

## Contributions 🤝  
Contributions are welcome! Feel free to open an issue or submit a pull request.  

## Acknowledgments 🙏  
This project is built as a part of the tutorial in the book *Let's Go* by Alex Edwards.  

## License 📝  
This project is open-source and available under the [MIT License](LICENSE).  

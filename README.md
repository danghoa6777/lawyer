# Lawyer - Legal Case Management System

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![Database](https://img.shields.io/badge/database-PostgreSQL%20%7C%20SQLite-blue)

A professional legal case management system designed to help law practitioners organize and track cases, clients, and documents efficiently.

## Features

- **Case Management**: Create, update, and track legal cases with ease
- **Client Database**: Store and manage client information securely with encryption
- **Document Storage**: Upload, version and organize legal documents
- **Calendar Integration**: Sync with Google Calendar for appointments and deadlines
- **Advanced Search**: Full-text search across cases, clients and documents
- **Role-Based Access**: Granular permissions for lawyers, paralegals and admins
- **Reporting**: Generate case status reports and billing summaries

## Installation

### Prerequisites

- Python 3.8+
- PostgreSQL (recommended) or SQLite
- pip
- Virtual environment (recommended)

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/danghoa6777/lawyer.git && cd lawyer
   ```

2. Set up virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/MacOS
   # OR
   venv\Scripts\activate  # Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure environment:
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

5. Database setup:
   ```bash
   python manage.py migrate
   python manage.py createsuperuser
   ```

6. Run development server:
   ```bash
   python manage.py runserver
   ```

## Usage

1. Access the system at `http://localhost:8000`
2. Log in with your admin credentials
3. Key features:
   - Dashboard: Overview of active cases and upcoming deadlines
   - Cases: Create and manage legal cases
   - Clients: Maintain client records
   - Documents: Upload and categorize files
   - Calendar: View and schedule events

## API Access

The system provides REST API endpoints for integration:

```bash
# Example API request
curl -X GET http://localhost:8000/api/cases/ -H "Authorization: Token YOUR_TOKEN"
```

## Contributing

We welcome contributions! Please follow our guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'feat: add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

Please ensure:
- Code follows PEP 8 style guide
- Include tests for new features
- Update documentation as needed

## Support

For assistance, please contact:

- **Project Maintainer**: danghoa6777
- **Email**: [Your Email Here]
- **Issue Tracker**: [https://github.com/danghoa6777/lawyer/issues](https://github.com/danghoa6777/lawyer/issues)
- **Documentation**: [https://github.com/danghoa6777/lawyer/wiki](https://github.com/danghoa6777/lawyer/wiki)

## License

MIT License - See [LICENSE](LICENSE) for full details.
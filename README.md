# Health Information System

A comprehensive health information system for managing clients and health programs/services. This system allows doctors to manage client information, health programs, and program enrollments efficiently.

## Features

- Create and manage health programs (e.g., TB, Malaria, HIV)
- Register and manage client information
- Enroll clients in health programs
- Search for clients
- View detailed client profiles with program enrollments
- RESTful API for client profile information

## Tech Stack

### Backend (Rails API)
- Ruby on Rails 7.1
- PostgreSQL
- RESTful API design
- JWT authentication (planned)

### Frontend (Next.js)
- Next.js 14
- TypeScript
- Tailwind CSS
- React Hook Form
- Heroicons

## Getting Started

### Prerequisites
- Ruby 3.2.2
- Node.js 18+
- PostgreSQL

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd health_system_api
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Set up the database:
   ```bash
   rails db:create db:migrate
   ```

4. Start the Rails server:
   ```bash
   rails server
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd health-system-frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

## API Endpoints

### Health Programs
- `GET /api/v1/health_programs` - List all health programs
- `POST /api/v1/health_programs` - Create a new health program
- `GET /api/v1/health_programs/:id` - Get a specific health program
- `PUT /api/v1/health_programs/:id` - Update a health program
- `DELETE /api/v1/health_programs/:id` - Delete a health program

### Clients
- `GET /api/v1/clients` - List all clients
- `POST /api/v1/clients` - Create a new client
- `GET /api/v1/clients/:id` - Get a specific client
- `PUT /api/v1/clients/:id` - Update a client
- `DELETE /api/v1/clients/:id` - Delete a client
- `GET /api/v1/clients/search` - Search for clients

### Enrollments
- `GET /api/v1/enrollments` - List all enrollments
- `POST /api/v1/enrollments` - Create a new enrollment
- `GET /api/v1/enrollments/:id` - Get a specific enrollment
- `PUT /api/v1/enrollments/:id` - Update an enrollment
- `DELETE /api/v1/enrollments/:id` - Delete an enrollment

## Security Considerations

- Input validation on both frontend and backend
- Secure API endpoints
- Data encryption for sensitive information
- Role-based access control (planned)

## Future Enhancements

- User authentication and authorization
- Role-based access control
- Audit logging
- Reporting and analytics
- Mobile application
- Integration with other health systems

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

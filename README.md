# CuraSync - Healthcare Management System

CuraSync is a comprehensive healthcare management system that connects healthcare providers and patients in a secure, unified platform. The system streamlines healthcare operations by integrating doctors, patients, laboratories, and pharmacies into one cohesive ecosystem.

## Key Features

### User Management
- **Multi-Role Authentication**
  - Secure role-based access for doctors, patients, labs, and pharmacies
  - Protected routes and data access based on user roles
  - Email and password authentication with Supabase

### Doctor Features
- Practice management dashboard
- Patient appointment scheduling
- Electronic health records (EHR)
- Digital prescription management
- Patient history tracking

### Patient Features
- Online appointment booking
- Medical history access
- Digital prescriptions
- Lab test results viewing
- Medication tracking

### Laboratory Features
- Test request management
- Digital results delivery
- Patient records access
- Automated reporting
- Quality control tracking

### Pharmacy Features
- Digital prescription processing
- Inventory management
- Medication tracking
- Patient medication history
- Automated refill management

## Tech Stack

- **Frontend**
  - Next.js 14 (React Framework)
  - React 18
  - TypeScript
  - Tailwind CSS
  - React Icons

- **Backend & Database**
  - Supabase (Backend as a Service)
  - PostgreSQL Database
  - Row Level Security (RLS)

- **Authentication**
  - Supabase Auth
  - JWT Token-based authentication
  - Role-based access control

## Getting Started

### Prerequisites
- Node.js 18.x or higher
- npm 9.x or higher
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/curasync.git
   cd curasync
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env.local` file in the root directory:
   ```env
   NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. Run the development server:
   ```bash
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
curasync/
├── src/
│   ├── app/                    # Next.js app router
│   │   ├── (auth)/            # Authentication routes
│   │   │   ├── [type]/        # Dynamic user type routes
│   │   │   │   ├── login/     # Login pages
│   │   │   │   └── signup/    # Signup pages
│   │   └── page.tsx           # Home page
│   ├── components/            # Reusable components
│   │   ├── LoginForm.tsx     # Login form component
│   │   ├── SignupForm.tsx    # Signup form component
│   │   └── Navbar.tsx        # Navigation component
│   └── styles/               # Global styles
├── public/                   # Static assets
├── tailwind.config.ts       # Tailwind configuration
└── package.json             # Project dependencies
```

## Development Guidelines

### Code Style
- Use TypeScript for type safety
- Follow ESLint and Prettier configurations
- Use functional components with hooks
- Implement proper error handling
- Write meaningful component and function names

### Security Best Practices
- Implement proper input validation
- Use environment variables for sensitive data
- Follow Supabase security guidelines
- Implement proper authentication flows
- Regular security audits

### Performance Optimization
- Implement code splitting
- Optimize images and assets
- Use proper caching strategies
- Minimize bundle size
- Regular performance monitoring

## Contributing

1. Fork the repository
2. Create your feature branch:
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a Pull Request

### Contribution Guidelines
- Write clear commit messages
- Update documentation as needed
- Add tests for new features
- Follow the existing code style
- Update the changelog

## Support

For support, please email support@curasync.com or open an issue in the GitHub repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Next.js team for the amazing framework
- Supabase team for the backend infrastructure
- All contributors who have helped shape CuraSync
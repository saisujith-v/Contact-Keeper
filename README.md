# Contact Keeper

Contact Keeper is a full-stack MERN application that helps users manage their contacts efficiently. Users can register, log in, and maintain their personal contact list with full CRUD operations.

## Features

- User authentication & authorization
- Contact management (CRUD operations)
- Contact filtering
- Private contact lists per user
- Responsive design
- JWT token-based authentication

## Tech Stack

- **Frontend:**
  - React (Create React App)
  - Context API for state management
  - React Hooks
  - JWT for authentication
  - Axios for API requests

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB
  - Mongoose ODM
  - JWT for authentication
  - bcryptjs for password hashing

## Installation

1. Clone the repository:
```bash
git clone https://github.com/saisujith-v/Contact-Keeper.git
cd Contact-Keeper
```

2. Install server dependencies:
```bash
npm install
```

3. Install client dependencies:
```bash
cd client
npm install
```

4. Create a `config/default.json` file and add your MongoDB URI and JWT secret:
```json
{
  "mongoURI": "your_mongodb_uri",
  "jwtSecret": "your_jwt_secret"
}
```

## Running the Application

### Development Mode
1. Run the server and client concurrently:
```bash
npm run dev
```

This will start:
- Backend server on port 5000
- Frontend development server on port 3000

### Production Mode
1. Build the client:
```bash
cd client
npm run build
```

2. Start the server:
```bash
cd ..
npm run start
```

## API Endpoints

### Users
- `POST /api/users` - Register a user
- `POST /api/auth` - Login user & get token

### Contacts
- `GET /api/contacts` - Get all user contacts
- `POST /api/contacts` - Add new contact
- `PUT /api/contacts/:id` - Update contact
- `DELETE /api/contacts/:id` - Delete contact

## Environment Variables

Create a `.env` file in the root directory and add:
```
NODE_ENV=development
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
```

## Contributing

1. Fork the repository
2. Create a new branch: `git checkout -b feature-name`
3. Make your changes and commit: `git commit -m 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

- **Sai Sujith V**
- GitHub: [@saisujith-v](https://github.com/saisujith-v)

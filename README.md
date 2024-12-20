# AssetPro API

AssetPro API is a RESTful API designed for efficient asset management. It includes functionalities to handle departments, employees, assets, asset issues, returns, and history.

---

## Features

- Manage departments and employees.
- Track assets and their lifecycle, including issuance and returns.
- View asset history with unique identifiers.
- Configured with environment variables for flexible deployment.

---

## Prerequisites

Ensure you have the following installed:

- **Node.js**
- **npm** or **yarn**
- A supported database (**PostgreSQL**) configured with Prisma.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/assetpro-api.git
   ```

2. Navigate to the project directory:
   ```bash
   cd assetpro-api
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

---

## Environment Setup

1. Create a `.env` file in the root directory.
2. Add the following variables (example):
   ```env
   PORT=8000
   DATABASE_URL=your-database-url
   ```

---

## Scripts

### Start the API

Start the server:
```bash
npm start
```
Uses **nodemon** for live-reloading during development.

---

## API Endpoints

### Base URL
```
http://localhost:8000
```

### Routes

| Endpoint              | Method | Description                        |
|-----------------------|--------|------------------------------------|
| `/api/dept`           | All    | CRUD operations for departments   |
| `/api/employee`       | All    | CRUD operations for employees     |
| `/api/asset`          | All    | CRUD operations for assets        |
| `/api/issueAsset`     | All    | Manage asset issuance             |
| `/api/returnAsset`    | All    | Manage asset returns              |
| `/api/assetHistory/:id` | GET    | Fetch asset history by ID         |

---

## Technologies Used

- **Node.js**: Backend runtime.
- **Express**: Web framework for creating RESTful APIs.
- **Prisma**: Database ORM.
- **dotenv**: For environment variable management.
- **Joi**: Schema validation.
- **CORS**: Enable cross-origin requests.




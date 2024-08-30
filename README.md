
# Issue Tracker Project

Welcome to the Issue Tracker project!. Follow the instructions below to set up the project on your local machine.

## Getting Started

To get started with this project, follow these steps:

### Prerequisites

Ensure you have the following installed on your machine:
- Node.js (v14 or later)
- npm or Yarn
- MySQL (or another supported database)

### Setup Instructions

1. **Clone the Repository**

   Clone this repository to your local machine using the following command:
   ```bash
   git clone https://github.com/username/repository.git
   ```

2. **Create Environment Variables**

   In the root directory of the project, create a `.env` file and add the following environment variables. Replace the placeholders with your actual credentials:

   ```plaintext
   # Database connection URL
   DATABASE_URL="your-database-url"

   # URL for NextAuth
   NEXTAUTH_URL="http://localhost:3000"

   # Secret for NextAuth (generate using `openssl rand -base64 32`)
   NEXTAUTH_SECRET="your-nextauth-secret"

   # Google OAuth credentials
   GOOGLE_CLIENT_ID="your-google-client-id"
   GOOGLE_CLIENT_SECRET="your-google-client-secret"
   ```

   You can find examples of `DATABASE_URL` formats here: [Prisma Connection URLs](https://www.prisma.io/docs/reference/database-reference/connection-urls).

3. **Install Dependencies**

   Navigate to the project directory and install the required dependencies:
   ```bash
   npm install
   ```

4. **Generate Database Tables**

   Run Prisma migrations to create your database tables:
   ```bash
   npx prisma migrate dev
   ```

5. **Start the Development Server**

   Launch the development server with:
   ```bash
   npm run dev
   ```

6. **Access the Application**

   Open your browser and go to `http://localhost:3000` to view the application.

## Additional Information

For more information on configuration and usage, check out the [Next.js documentation](https://nextjs.org/docs) and the [Prisma documentation](https://www.prisma.io/docs).
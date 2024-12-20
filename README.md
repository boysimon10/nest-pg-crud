<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

```markdown
# NestJS PostgreSQL CRUD API

A simple CRUD API built with NestJS and PostgreSQL for managing contacts.

## Prerequisites

- Node.js
- PostgreSQL
- npm or yarn

## Installation

1. Clone the repository:
```bash
git clone [your-repository-url]
cd [your-project-name]
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with the following variables:
```plaintext
DB_HOST=localhost
DB_PORT=5432
DB_USER=your_username
DB_PASSWORD=your_password
DB_NAME=your_database_name
```

4. Create the PostgreSQL database:
```sql
CREATE DATABASE your_database_name;
```

## Running the app

```bash
# development
npm run start

# watch mode
npm run start:dev

# production mode
npm run start:prod
```

## API Endpoints

- `GET /contacts` - Get all contacts
- `GET /contacts/:id` - Get a specific contact
- `POST /contacts` - Create a new contact
- `PUT /contacts/:id` - Update a contact
- `DELETE /contacts/:id` - Delete a contact

## Contact Schema

```typescript
{
  firstName: string,
  lastName: string,
  email: string,
  phone?: string
}
```

## Environment Variables

| Variable    | Description              | Default     |
|------------|-------------------------|-------------|
| DB_HOST    | Database host           | localhost   |
| DB_PORT    | Database port           | 5432        |
| DB_USER    | Database username       | -           |
| DB_PASSWORD| Database password       | -           |
| DB_NAME    | Database name           | -           |

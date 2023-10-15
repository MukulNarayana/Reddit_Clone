## Features
- JWT authentication
- Create, update, and delete posts and comments
- Upvote/downvote posts and comments
- Nested comments threading
- Home page feed (front page)
- Subreddit specific feed
- Create subreddits
- Light and dark mode
## Installation
1. Install backend dependencies

```
cd backend
npm install
```

2. Install frontend dependencies

```
cd frontend
npm install
```

3. Create config folder in the backend

```
cd backend
mkdir config
```

4. Configure environment variables. Create a `dev.env` file in the config folder, and paste the following (filling in your own postgres password and JWT secret)
```
PORT=5000
PG_HOST=localhost
PG_PORT=5432
PG_DBNAME=reddit-clone
PG_USER=postgres
PG_PASSWORD=<YOUR_PASSWORD>
JWT_SECRET=<YOUR_SECRET>

```

5. Create a postgres database named 'reddit-clone'

6. Run the database migrations

```
cd backend
npm run db-migrate up
```

## Usage
1. Start server

```
cd backend
npm run dev
```

2. Start client
```
cd frontend
npm start
```

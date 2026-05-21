# movieApi

A simple Express.js movie API example project. Serves movie-related pages and simple search endpoints using local data.

## Features

- Express.js server with routing in `routes/`
- Server-side rendered views using Jade
- Sample movie data in `data/`
- Basic logging and error handling

## Prerequisites

- Node.js 14+ (or compatible)
- npm

## Install

From the project root (`movieApi`) run:

```bash
npm install
```

## Run

Start the server:

```bash
npm start
```

This runs the `start` script defined in `package.json` which executes `node ./bin/www`.

## Project Structure

- `app.js` - main Express application setup
- `bin/www` - server bootstrap script
- `routes/` - route handlers (`index.js`, `movie.js`, `search.js`)
- `data/` - sample data files (`movies.js`, `movieDetails.js`, `people.js`)
- `views/` - Jade templates
- `public/` - static assets

## Routes / Endpoints

- `GET /` - Home page (index)
- `GET /movie/:id` - Movie detail page
- `GET /search` - Search page (query param `q` expected)

Inspect the `routes/` directory for full implementation details.

## Development

- Edit route handlers in `routes/`
- Modify views in `views/`
- Static files served from `public/`

## Notes

- This project uses Jade templates (package `jade` in dependencies).
- Helmet is included for basic security headers.

## License

MIT (check project owner for specifics)

# AlbumBrowser — Angular Lab 6

A multi-page Single Page Application (SPA) built with Angular 17+, demonstrating routing, HTTP services, and CRUD operations.

## Features

- 6 configured routes (home, about, albums, album detail, album photos)
- Angular Router with route parameters and routerLink
- HttpClient via centralized AlbumService
- CRUD: Read, Update (edit title), Delete (remove from list)
- Loading indicators and error handling
- Responsive photo grid with hover effects

## Getting Started

### Prerequisites

- Node.js v18+
- Angular CLI v17+

### Installation

```bash
# Clone the repo
git clone <your-repo-url>
cd lab6/album-browser

# Install dependencies
npm install

# Start the dev server
ng serve
```

Then open your browser at `http://localhost:4200`.

## Project Structure

```
src/
├── app/
│   ├── components/
│   │   ├── home/              # Welcome page
│   │   ├── about/             # About page
│   │   ├── albums/            # Album list with delete
│   │   ├── album-detail/      # Detail view with edit
│   │   └── album-photos/      # Photo grid
│   ├── models/
│   │   ├── album.model.ts     # Album interface
│   │   └── photo.model.ts     # Photo interface
│   ├── services/
│   │   └── album.service.ts   # AlbumService (all HTTP calls)
│   ├── app.component.*        # Root component + navbar
│   ├── app.config.ts          # App providers
│   └── app.routes.ts          # Route configuration
├── index.html
├── main.ts
└── styles.css
```

## API

Uses [JSONPlaceholder](https://jsonplaceholder.typicode.com) — a free fake REST API.

- `GET /albums` — all albums
- `GET /albums/:id` — single album
- `GET /albums/:id/photos` — album photos
- `PUT /albums/:id` — update album (simulated)
- `DELETE /albums/:id` — delete album (simulated)

## Course Info

- **Course:** Web Development
- **Lab:** Lab 6 — Routing & HTTP
- **Student:** Your Name Here

# Vinty Cafe - Full Stack Website

An elegant, modern cafe website with a complete admin dashboard for managing menu items, categories, and page content.

## Live Demo

**Frontend**: https://mh2wloj5xxej2.ok.kimi.link

## Features

### Customer Side
- **Homepage**: Beautiful hero section with animated logo and tagline
- **Menu Page**: Categorized menu items with search and filter functionality
- **About Page**: Editable content about the cafe
- **Contact Page**: Contact form and business information
- **Privacy Policy**: Editable privacy policy page

### Admin Dashboard
- **Login System**: Secure authentication (default: admin / admin123)
- **Menu Management**: Add, edit, delete menu items with image upload
- **Category Management**: Manage categories and subcategories
- **Page Editor**: Edit About, Contact, and Privacy Policy content

## Tech Stack

### Frontend
- React + TypeScript + Vite
- Tailwind CSS + shadcn/ui components
- React Router for navigation
- Axios for API calls

### Backend
- Node.js + Express
- JSON file-based storage (no database required)
- Multer for image uploads
- CORS enabled

## Project Structure

```
/mnt/okcomputer/output/
├── app/                    # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── services/       # API services
│   │   └── types/          # TypeScript types
│   └── dist/               # Built frontend files
│
├── backend/                # Backend Express server
│   ├── server.js           # Main server file
│   ├── uploads/            # Uploaded images
│   └── data/               # JSON data files
│
└── README.md
```

## Getting Started

### Prerequisites
- Node.js 18+ installed

### Running the Backend

```bash
cd /mnt/okcomputer/output/backend
npm install
npm start
```

The backend will start on `http://localhost:5000`

### Running the Frontend (Development)

```bash
cd /mnt/okcomputer/output/app
npm install
npm run dev
```

The frontend will start on `http://localhost:5173`

### Building for Production

```bash
cd /mnt/okcomputer/output/app
npm run build
```

Built files will be in the `dist/` folder.

## Admin Login

- **Username**: admin
- **Password**: admin123

## API Endpoints

### Authentication
- `POST /api/auth/login` - Login

### Menu
- `GET /api/menu` - Get all menu items
- `GET /api/menu/:id` - Get single menu item
- `POST /api/menu` - Create menu item (with image)
- `PUT /api/menu/:id` - Update menu item (with image)
- `DELETE /api/menu/:id` - Delete menu item

### Categories
- `GET /api/categories` - Get all categories
- `POST /api/categories` - Create category
- `PUT /api/categories/:id` - Update category
- `DELETE /api/categories/:id` - Delete category

### Pages
- `GET /api/pages/:page` - Get page content (about, contact, privacy)
- `PUT /api/pages/:page` - Update page content

### Upload
- `POST /api/upload/logo` - Upload logo image

## Default Data

The backend comes with pre-populated sample data:

### Categories
- Coffee (Classic, Flavoured)
- Non Coffee (Mocktail, Milk)
- Snack & Bites
- Tea Series
- All Day Menu

### Sample Menu Items
- Espresso, Cappuccino, Vanilla Latte, Caramel Macchiato
- Mojito Mocktail, Strawberry Milk
- French Fries, Chicken Wings
- Earl Grey Tea
- Nasi Goreng

## Design

- **Primary Color**: Maroon Red (#800000)
- **Accent Color**: Soft Red (#ff6b6b)
- **Style**: Elegant, modern, minimalistic
- **Features**: Smooth animations, responsive layout, glass morphism effects

## License

MIT License - Created for Vinty Cafe

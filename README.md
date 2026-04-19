# Moments Gallery

Moments Gallery is a minimalist web application designed for users to preserve their memories. It provides a simple interface to upload images with captions and view them in a beautifully organized feed.

## ✨ Key Features
- **Seamless Image Upload**: Upload personal photos with custom captions.
- **Cloud Integration**: Powered by **ImageKit** for fast image delivery and optimization.
- **Dynamic Gallery**: A responsive feed that updates automatically when new photos are added.
- **Persistent Storage**: Uses **MongoDB** to ensure your descriptions and image links are saved.

## 🛠️ Tech Stack

### Frontend
- **React**: Modern component-based architecture.
- **Vite**: Ultra-fast build tool for a smooth development experience.
- **Axios**: Efficient handling of asynchronous API calls.
- **Tailwind CSS**: Utility-first styling for a sleek, responsive UI.

### Backend
- **Node.js & Express**: Robust server-side framework.
- **MongoDB & Mongoose**: Flexible NoSQL database schema for post metadata.
- **ImageKit SDK**: Professional-grade cloud storage and image processing.
- **Multer**: High-performance middleware for handling multipart/form-data.

## 🏗️ Architecture
1. **Frontend**: Collects the image and caption through a user-friendly form.
2. **Backend**: Receives the file via **Multer** and securely transmits it to **ImageKit**.
3. **Database**: Once the image is hosted, the ImageKit URL and caption are stored in **MongoDB**.
4. **Feed**: The frontend fetches the data from the backend to render the personalized gallery.

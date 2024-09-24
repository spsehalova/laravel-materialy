# Blog Management System with Laravel Filament

This guide provides an overview of how to build a **Blog Management System** using Laravel Filament, complete with testing. It assumes basic knowledge of Laravel and covers key features like soft deletes, image uploads, and category management.

## Project Overview

You'll build a **Blog Management System** where admins can manage blog posts from a user-friendly Filament-powered admin panel. The project includes features like soft deletes, image uploads, and category management, with test cases for core functionality.

## Prerequisites

- Basic knowledge of Laravel
- PHP 8.1+ and Laravel 9.x or later
- Composer installed

## Steps

### Step 1: Set Up Laravel and Filament

1. **Create a Laravel Project**:
		- Set up a new Laravel project and configure the database in `.env`.

2. **Install Filament**:
		- Install the Filament admin panel package using Composer.

3. **Configure Admin User**:
		- Set up an admin user to access the Filament admin panel.

### Step 2: Create a Post Resource

1. **Generate Post Model**:
		- Create a `Post` model with fields for title, content, and timestamps.

2. **Create Filament Resource for Post**:
		- Use Filament's resource generation command to set up CRUD functionality for posts.

3. **Customize Post Form**:
		- Modify the form in the admin panel to include fields for managing blog post title and content.

### Step 3: Add Core Features

1. **Soft Deletes**:
		- Enable soft deletes for the `Post` model so deleted posts can be restored.

2. **Image Uploads**:
		- Allow users to upload images for each blog post. Set up the necessary file uploads and storage configuration.

3. **Category Management**:
		- Add a `Category` model and associate it with posts. Create a Filament resource for `Category` to organize posts by categories.

### Step 4: Set Up Testing

1. **Install Testing Framework**:
		- Set up Laravel's built-in testing or install Pest for a simpler testing framework.

2. **Test Post Creation**:
		- Write tests to ensure that users can create posts through Filament’s admin panel.

3. **Test Validation**:
		- Add tests to verify that form validation (e.g., required fields) works correctly.

4. **Test Post Deletion**:
		- Ensure that posts can be soft-deleted and restored, and write tests for this functionality.

5. **Test Image Uploads**:
		- Implement tests to check that image uploads work correctly and are linked to blog posts.

### Step 5: Add Advanced Features

1. **Roles & Permissions**:
		- Set up user roles and permissions to restrict access to the admin panel.

2. **Post Filtering & Search**:
		- Add search and filter functionality to the post listing in the admin panel for easier navigation.

3. **Dashboard Customization**:
		- Customize the Filament dashboard to display key metrics like the number of posts, recent posts, and top categories.

### Step 6: Final Touches

1. **Improve UI/UX**:
		- Customize the Filament admin panel’s appearance to match your app's branding and improve user experience.

2. **Testing Dashboard Features**:
		- Write tests to ensure dashboard features, such as data display and search functionalities, work as expected.

3. **Deploy the App**:
		- Deploy the app to a hosting platform (e.g., Laravel Forge or Vapor) and ensure everything works in production.

---

## Features Summary

1. **Post Management**: Create, edit, delete, and restore blog posts.
2. **Category Management**: Organize blog posts using categories.
3. **Image Uploads**: Upload and manage images for each blog post.
4. **Soft Deletes**: Implement soft delete functionality, with the ability to restore posts.
5. **Admin Panel**: Manage the entire blog system through a Filament-powered admin dashboard.
6. **Testing**: Write tests to ensure that core functionality, including post creation, deletion, and validation, works correctly.

## Next Steps

Once you've completed the blog management system, you can explore more advanced features like role-based access control, rich text editors for posts, or approval workflows for content.

---

## Technologies Used

- **Laravel**: PHP web application framework.
- **Filament**: Admin panel package for Laravel.
- **Pest** (optional): Testing framework for PHP.

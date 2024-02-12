# Laravel 10.10 x React

This GitHub repository serves as a learning resource for Laravel and ReactJS development, providing essential materials and examples for users to enhance their understanding of these technologies.

## Requirement

1. PHP ^8.1
2. Node v16.13.2 - up

## Installation

1. Install laravel latest version
    ```bash
    composer create-project laravel/laravel laravel-react
    ```
2. Install laravel breeze
    ```bash
    composer require laravel/breeze --dev
    ```
3. Install react
    ```bash
    php artisan breeze:install react
    ```
4. Run laravel
    ```bash
    php artisan serve
    ```
5. Run react
    ```bash
    npm run dev
    ```
6. Create first react component
   Create new file called `PostComponent.jsx` in `resources/js/Pages/Posts` directory.
   Create functional component inside `PostComponent.jsx`

    ```bash
    import React from 'react';

    export default function PostComponent()
    {
         return(
             <div>
                 <h1>Post Component</h1>
             </div>
         )
     }
    ```

7. Create route for post component
    ```bash
    Route::get('/posts', function () {
        return Inertia::render('Posts/PostComponent');
    });
    ```

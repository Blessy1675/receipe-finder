1.INTRODUCTION
This section provides an overview of the Recipe Finder project, explaining its purpose and objectives. It highlights how the project helps users find recipes based on ingredients, dietary preferences, and cuisine types.

1.1 Problem Definition
Users struggle to find suitable recipes based on available ingredients and dietary preferences. Existing solutions lack advanced search and customization features.

1.2 Existing System
Current recipe platforms provide limited filtering options and do not support ingredient-based searches or personalized meal planning.

1.3 Proposed System
A dynamic system that allows users to search recipes based on ingredients, dietary needs, and meal types while integrating shopping lists and real-time updates.

1.4 Literature Review
The Recipe Finder project addresses challenges in personalized recipe recommendations by improving on existing systems. Content-based and collaborative filtering techniques dominate recipe recommendation algorithms but face issues like limited novelty and the cold start problem. Diet-specific systems cater to preferences such as vegan, gluten-free, or keto diets, while research on user interfaces highlights the importance of responsive design, ease of navigation, and interactive features like shopping lists and real-time updates.













2. SYSTEM REQUIREMENTS

2.1 Hardware & Software Requirements
On the software side, the system uses HTML, CSS, and JavaScript for frontend development, ensuring a responsive interface compatible with various screen sizes. Recipes are either manually entered into the database or fetched dynamically using APIs like Spoonacular or Edamam, providing flexibility in data handling. The lightweight design ensures seamless performance across devices.Users require a stable internet connection to access the web application, making it accessible to a wide range of devices with basic configurations like 4GB RAM and a dual-core processor.
2.2 Software Requirements Specification (SRS)
The Recipe Finder system should support key functionalities to enhance user experience. This includes:
•	Recipe searching and filtering based on ingredients, meal types, and dietary preferences.
•	User account management for profile customization and preference saving.
•	Shopping list management for organizing ingredients conveniently.
The system must ensure smooth navigation, quick response times, and secure data handling to maintain usability and reliability.










3. SYSTEM DESIGN
3.1 Modules of System

• User Management: Handles user login, registration, and profile customization, ensuring a personalized experience.
• Recipe Search and Filtering: Provides search functionality with filters for ingredients, cuisine, dietary restrictions, and meal types.
• Shopping List Management: Allows users to add ingredients to a shopping list for easy grocery planning.
• Meal Planning: Supports users in scheduling meals by organizing selected recipes into weekly or daily plans.
• Ratings and Reviews: Enables users to rate and review recipes, fostering engagement and feedback sharing.

3.2 ER diagram



 




4. IMPLEMENTATION

4.1 Sample Code
Uses HTML, CSS, and JavaScript with API integration for retrieving recipes.
Source Code:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recipe Finder</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: url('https://via.placeholder.com/1600x900/FFD700/FFF?text=Food+Background') no-repeat center center fixed;
            background-size: cover;
            color: #333;
        }
        header {
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 10;
        }
        header h1 {
            margin: 0;
        }
        .header-icons {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        .header-icons i {
            font-size: 1.5rem;
            cursor: pointer;
            color: white;
        }
        .header-icons i:hover {
            color: #ff6600;
        }
        .container {
            margin-top: 100px;
            text-align: center;
        }
        input, button {
            padding: 10px;
            border: none;
            border-radius: 5px;
            margin: 5px 0;
        }
        input {
            width: 60%;
        }
        button {
            background-color: #ff6600;
            color: white;
            cursor: pointer;
        }
        button:hover {
            background-color: #e64a19;
        }
        .recipe-card {
            background: rgba(255, 255, 255, 0.9);
            margin: 15px auto;
            padding: 15px;
            border-radius: 10px;
            width: 50%;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <header>
        <h1>Recipe Finder</h1>
        <div class="header-icons">
            <i class="fa fa-heart" title="Wishlist"></i>
            <i class="fa fa-sliders" title="Preferences"></i>
            <i class="fa fa-bell" title="Notifications"></i>
        </div>
    </header>
    <div class="container">
        <input type="text" id="searchBox" placeholder="Enter ingredients (e.g., egg, tomato)">
        <button onclick="searchRecipes()">Search</button>
        <div id="results"></div>
    </div>
    <script>
        const recipes = [
            { name: "Tomato Omelette", ingredients: ["egg", "tomato", "onion"] },
            { name: "Grilled Cheese", ingredients: ["bread", "cheese", "butter"] },
            { name: "Pasta Salad", ingredients: ["pasta", "tomato", "cheese"] }
        ];

        function searchRecipes() {
            let query = document.getElementById("searchBox").value.toLowerCase().split(",");
            let resultsDiv = document.getElementById("results");
            resultsDiv.innerHTML = "";

            let filteredRecipes = recipes.filter(recipe =>
                query.every(ing => recipe.ingredients.includes(ing.trim()))
            );

            if (filteredRecipes.length > 0) {
                filteredRecipes.forEach(recipe => {
                    let recipeDiv = document.createElement("div");
                    recipeDiv.className = "recipe-card";
                    recipeDiv.innerHTML = `
                        <h3>${recipe.name}</h3>
                        <p>Ingredients: ${recipe.ingredients.join(", ")}</p>
                    `;
                    resultsDiv.appendChild(recipeDiv);
                });
            } else {
                resultsDiv.innerHTML = "<p>No recipes found. Try different ingredients.</p>";
            }
        }
    </script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</body>
</html>

5.RESULTS

5.1 Output Screens
Test cases for the Recipe Finder project focus on validating core functionalities like recipe search, filtering, and user account management. Each test ensures proper operation of modules such as shopping list creation, meal planning, and ratings.
output
 


 


6. CONCLUSION

The Recipe Finder project provides an effective solution to the common challenges of meal planning and recipe discovery by offering a customizable, user-friendly platform. With features such as advanced search options, dietary filters, shopping list integration, and meal planning tools, the system caters to diverse user needs. Built using HTML, CSS, and JavaScript, the responsive design ensures seamless accessibility across devices, making it convenient for users to find and manage recipes anytime, anywhere. By incorporating ratings, reviews, and social sharing, the platform fosters community engagement and allows users to explore and share culinary ideas.


6.1.REFERENCES

Includes research papers, API documentation, and relevant web development resources such as w3 schools,..etc.,



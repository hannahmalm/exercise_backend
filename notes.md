1. Create a new rails project called Exercise
2. Create a backend and a frontend folder
3. Create the rails backend by cd into back directory
    rails new project_name_backend --database=postgresql --api
    cd into directory
4. Create github repo - you can create one for front and backend 
    - git init
    - git add .
    - git commit -m "inital commit"
5. Create a new branch for every feature and push to the master branch
6. Create new branch and model for category
    new branch: git co -b category_model
        new model: rails g model Category name
        add seed data
        add has_many relationship in model 
        git add .
        git commit
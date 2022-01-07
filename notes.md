1. Create a new rails project called Exercise
 - https://betterprogramming.pub/how-to-fire-up-a-rails-api-for-your-new-project-6fad595caf07
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
7. HOW TO SEE CURRENT BRANCH:
    git rev-parse --abbrev-ref HEAD
    %  git push -u origin  <branch name>  
    Get back to main branch: git checkout main
    The git branch command can be used to create a new branch. When you want to start a new feature, you create a new branch off main using git branch new_branch . Once created you can then use git checkout new_branch to switch to that branch
8. Commit seed and model 
9. Run rails db:create
10. Run rails db:migrate


Models
- Category
    - Name
    :has_many exercises
- Exercise
    - title
    - description
    - image
    - category_id 
    :belongs_to category 
- User
- Workout
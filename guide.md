# 🚀 How to Set Up Your GitHub Profile README

This guide will walk you through the exact steps to create a special GitHub repository and upload this profile code so that it displays on your GitHub profile page!

## Step 1: Create the Special Repository

1. Go to [GitHub.com](https://github.com) and log in to your account.
2. Click the **+** icon in the top right corner and select **New repository**.
3. **CRITICAL STEP**: In the "Repository name" field, type **your exact GitHub username**. 
   *(For example, if your username is `nerajlal`, your repository name MUST be `nerajlal`)*. 
   > 💡 GitHub will show a special message with a cat icon saying: *"You found a secret! [username]/[username] is a special repository that you can use to add a README.md to your GitHub profile."*
4. Make sure the repository is set to **Public**.
5. Do **NOT** check "Add a README file" (since we already have one we want to upload).
6. Click the green **Create repository** button.

## Step 2: Upload This Code to Your New Repository

You can upload the code in one of two ways: using the terminal (recommended) or the GitHub website.

### Option A: Using the Terminal / Command Line (Recommended)

Since this project includes hidden folders (like `.github` for the snake animation), pushing via the terminal is the easiest and most reliable method.

1. Open your terminal (or Command Prompt / Git Bash).
2. Navigate to the folder where this profile code is located:
   ```bash
   cd path/to/this/folder
   ```
3. Initialize Git and push the code by running these commands (replace `YOUR_USERNAME` with your actual GitHub username):
   ```bash
   git init
   git add .
   git commit -m "Initial profile setup"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.git
   git push -u origin main
   ```

### Option B: Using the GitHub Website (Drag and Drop)

If you aren't comfortable with the terminal, you can upload the files manually.

1. On your newly created repository page in GitHub, click the **uploading an existing file** link.
2. Drag and drop the `README.md` and `img.png` files into the box.
3. Click the green **Commit changes** button.
4. **Note for the Snake Animation:** The `.github` folder (which runs the background snake animation) cannot be dragged and dropped easily. You will need to click **Add file > Create new file**, type `.github/workflows/snake.yml` as the file name, paste the contents of your local `snake.yml` file into it, and then commit.

## Step 3: Enable the Snake Animation

This profile uses a GitHub Action to automatically generate your contribution snake every day.

1. Go to the **Actions** tab in your new repository on GitHub.
2. If it asks you to enable workflows, click **I understand my workflows, go ahead and enable them**.
3. Click on the **Generate Datas** workflow on the left sidebar.
4. Click the **Run workflow** dropdown on the right side and click the green **Run workflow** button.
5. Wait a minute or two for it to finish running. This will generate your snake animation and push it to the `output` branch.

## Step 4: Admire Your New Profile! 🎉

Go back to your main GitHub profile page (`https://github.com/YOUR_USERNAME`). You should now see your beautiful new profile layout with the animated typing text, your portrait, your tech stack, and your contribution snake!

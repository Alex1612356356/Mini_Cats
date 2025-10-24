# Dusties - Unity WebGL Project

This project is a Unity game exported for WebGL.

## Running Locally

To run this project on your local machine, you need to use a web server. Opening the `index.html` file directly in your browser will not work due to browser security restrictions (CORS).

1.  **Ensure you have Python installed.** Python 3 is recommended.
2.  **Start the web server.** Open your terminal or command prompt in the project's root directory and run the following command:
    ```bash
    python run_server.py
    ```
3.  **View the project.** Once the server is running, open your web browser and navigate to:
    [http://localhost:8000](http://localhost:8000)

## Deploying to GitHub Pages

This project can be deployed and hosted for free using GitHub Pages.

1.  **Push to GitHub:** Make sure your project is in a GitHub repository and you have pushed all the files, including `index.html`, the `Build/` directory, and the `.nojekyll` file.
2.  **Enable GitHub Pages:**
    *   Go to your repository's settings on GitHub.
    *   Navigate to the "Pages" section.
    *   Under "Build and deployment", select your main branch as the source and `/ (root)` as the folder.
    *   Save the changes.
3.  **View your deployed project:** It may take a few minutes for the site to be published. You can find the URL in the same "Pages" settings section.

### The `.nojekyll` file

The empty `.nojekyll` file in this repository is important. It tells GitHub Pages not to process the site with the Jekyll static site generator. Jekyll can interfere with the file paths and loading of Unity WebGL builds, and this file prevents those issues.

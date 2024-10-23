LAB EXERCISE – 8

Applying CI/CD Principles to Web Development Using Jenkins, Git, and Local HTTP Server
Task : Set up a CI/CD pipeline for a web development project using Jenkins, Git, and webhooks, without the need for a Jenkinsfile.

CI/CD Workflow:
    • Code Changes: Developers make changes to the web application's source code locally.
    • Git Repository: Developers push their code changes to a Git repository, such as GitHub or Bitbucket.
    • Webhook: A webhook is configured in the Git repository to notify Jenkins whenever changes are pushed.
    • Jenkins Job: Jenkins is set up to listen for webhook triggers. When a trigger occurs, Jenkins initiates a CI/CD pipeline.
    • Build and Test: Jenkins executes a series of predefined steps, which may include building the application, running tests, and generating artifacts.
    • Deployment: If all previous steps are successful, Jenkins deploys the application to a local HTTP server for testing.
    • Verification: The deployed application is tested locally to ensure it functions as expected.
    • Optional Staging: For more complex setups, there might be a staging environment where the application undergoes further testing before reaching production.
    • Production Deployment: If the application passes all tests, it can be deployed to the production server.

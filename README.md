# Build_CI_CD_Jenkins_SonarCube_AWS

- Developer writes code and pushes it to a GitHub Repository.
- GitHub Webhook notifies Jenkins Server of the code changes.
- Jenkins initiates the CI/CD pipeline:
- Checkout Code: Jenkins checks out the latest code from the GitHub repository.
- Build and Test: Jenkins builds the code, runs automated tests, and packages the application.
- SonarQube Analysis: Jenkins triggers a SonarQube analysis to assess code quality, security, and maintainability.
- Docker Build: Jenkins builds a Docker container image containing the application and dependencies.
User Access: End-users can access the deployed application in the production environment.

-- Developer's Code
--     |
--     v
-- GitHub Repository
--     |
--     v
--     Jenkins
--    /       \
--   v         v
--             Docker
-- SonarQube     |
                 v
                  Deployment
                    |
                    v
                  End Users


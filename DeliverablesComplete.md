# Deliverables Checklist: Basic CI/CD Assignment

## Part 1: Infrastructure as Code (IaC)
- [ ] `docker-compose.yml` (Defines Nginx/Flask environment)
- [ ] Screenshot: Default web server page (e.g., `nginx_screenshot.png` or terminal curl output)

## Part 2: Continuous Integration (CI)
- [ ] `app.py` (Flask "Hello, World!" app)
- [ ] `requirements.txt` (Python dependencies)
- [ ] `.github/workflows/main.yml` (GitHub Actions CI pipeline)
- [ ] Screenshot: Successful CI pipeline run (from GitHub Actions)

## Part 3: Continuous Delivery (CD)
- [ ] Updated `.github/workflows/main.yml` (with Deploy stage)
- [ ] Brief explanation of deployment automation:

  After the build and test stages pass in the GitHub Actions workflow (`.github/workflows/main.yml`), the Deploy stage runs automatically. This stage is currently a placeholder that simulates deployment by echoing messages. In a real-world scenario, this is where you would add commands to copy files to a server, trigger a Docker deployment, or use a cloud provider's CLI to deploy your application. The automation ensures that deployment only happens if all previous steps succeed, providing a reliable and repeatable process.

- [ ] Screenshot: Successful Deploy stage in GitHub Actions


---


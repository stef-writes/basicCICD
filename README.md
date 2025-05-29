# Basic CI/CD Assignment

## Part 1: Infrastructure as Code (IaC)

### Deliverables
- **docker-compose.yml**: Defines a single Nginx web server container.
- **Screenshot**: (To be added) showing the default Nginx web page running at http://localhost:8080.

### Steps
1. Run `docker-compose up -d` to start the Nginx container.
2. Open your browser and go to [http://localhost:8080](http://localhost:8080) to verify the web server is running.
3. Take a screenshot of the default Nginx page and save it as `nginx_screenshot.png` (or similar).

## Part 2: Continuous Integration (CI)

### Deliverables
- **app.py**: Simple Python Flask web application.
- **requirements.txt**: Python dependencies for the app.
- **.github/workflows/main.yml**: GitHub Actions CI pipeline (to be added).
- **Screenshot**: (To be added) showing a successful CI pipeline run.

### Steps
1. (Optional) Run the app locally:
   ```sh
   pip install -r requirements.txt
   python app.py
   ```
   Visit [http://localhost:5000](http://localhost:5000) to see 'Hello, World!'.
2. Commit and push your code to your GitHub repository: https://github.com/stef-writes/basicCICD.git
3. The CI pipeline will be set up in the next step.

## Part 3: Continuous Delivery (CD)

### Deliverables
- **Updated .github/workflows/main.yml**: Now includes a Deploy stage after tests pass.
- **Explanation**: The Deploy stage is currently a placeholder that simulates deployment. In a real scenario, this is where you would add commands to copy files to a server, trigger a Docker deployment, or use a cloud provider's CLI.
- **Screenshot**: (To be added) showing the Deploy stage running successfully in GitHub Actions.

### How deployment is automated
After the build and test stages pass, the Deploy stage runs automatically. This is where you would automate the deployment of your application to your infrastructure (e.g., using Docker, SSH, or a cloud provider). For demonstration, the workflow currently just echoes deployment steps.

---

Further deliverables and instructions for CI/CD will be added as we progress. 
🧰 Jenkins Docker Setup

A simple Docker Compose configuration to deploy Jenkins, the popular open-source automation server. This setup includes the Jenkins setup wizard enabled by default to help you quickly configure Jenkins on first startup.
🚀 What is Jenkins and Why Use It?

Jenkins is a powerful automation tool widely used for continuous integration and continuous delivery (CI/CD). It automates building, testing, and deploying software projects, enabling development teams to deliver code changes faster and with higher quality.

By using Jenkins, you can:

Automate repetitive tasks like compiling code, running tests, and deploying applications.
Integrate with hundreds of plugins to extend functionality.
Orchestrate complex workflows and pipelines.
Support distributed builds across multiple machines (agents).
Improve software development efficiency and reliability.

🔧 Jenkins Container Details

Runs the official Jenkins Docker image as a container.
Runs with root privileges for full access to the environment.
Exposes important ports:

8080: Web UI for managing Jenkins.
50000: Port for Jenkins agent connections (used to run builds on separate nodes).

Persists all Jenkins data, jobs, plugins, and configurations in a Docker volume called jenkins_home.

The Jenkins setup wizard runs on first launch to guide you through creating the initial admin user, installing plugins, and basic setup.

⚙️ Usage

To get started, run:

docker-compose up -d

Then open your browser and visit:

    Jenkins UI: http://localhost:8080

The setup wizard will launch automatically the first time you access Jenkins, making it easy to configure your instance step-by-step.

💾 Data Persistence

All Jenkins data is stored in the jenkins_home Docker volume. This ensures your jobs, settings, and plugins persist even if you stop or recreate the container.
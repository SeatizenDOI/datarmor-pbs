# Datarmor PBS Scripts

Each folder includes a **README** file explaining how its contents work.

When using a **PBS script**, **always make a copy** before modifying it for a new session, and **keep all output files**.

Maintaining copies and outputs helps you **track changes and ensure reproducibility** of your computations.


The code can be used in two different ways:

* **Local environment:**
  Install a local development environment with **Conda** to run the code directly.

* **Singularity image (from a Docker image):**
  
  Build a **Singularity** image from the provided Docker image.
  
  **Why Singularity instead of Docker?**
  
  Datarmor is an HPC system where users do **not have root privileges**.
  
  Docker requires root access and allows writing inside the running container, which is restricted on Datarmor — only specific Docker images are permitted.
  
  In contrast, **Singularity** runs without root privileges: you **cannot write inside the container**, so you must **bind or link all directories** where you intend to write data.




If you need help, open an issue and i will try to help you.
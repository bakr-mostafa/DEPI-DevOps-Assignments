# Git Workflow: Branching, Collaboration, and Pull Requests

In this assignment, I walked through the steps to set up SSH authentication, create a new feature branch, push it to the remote repository, and then submit a pull request for review. 
## Steps Followed for the Assignment

### 1. **Generate an SSH Key**
To begin, I generated a new SSH key on my local machine to enable secure, password-free communication with GitHub.

- I ran the following command in the terminal to create the SSH key:

  ```bash
  ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

- Used the email associated with my GitHub account as the label.
- Accepted the default file location (`~/.ssh/id_rsa`) for the key.
- Set an optional passphrase for additional security.

---

### **2. Add the SSH Key to GitHub**

- I added the SSH public key to my GitHub account so that I could authenticate securely when pushing to and pulling from repositories.

  ```bash
  cat ~/.ssh/id_rsa.pub

- copied the output (the SSH public key) and added it to my GitHub account:
- went to GitHub > Settings > SSH and GPG keys.
- Added SSH key to complete the process.

---

### **3. Clone the Repository**

- I cloned the DEPI-DevOps-Assignments repository from GitHub to my local machine.

- From the repository on GitHub, I copied the SSH URL:
        git@github.com:bakr-mostafa/DEPI-DevOps-Assignments.git

- Then, I ran the following command in my terminal to clone it:
  
   ```bash
  git clone git@github.com:bakr-mostafa/DEPI-DevOps-Assignments.git

---

### 4. Create a New Branch

I created a new feature branch called feature_a to work on my changes.

    I used the following command to create and switch to the new branch:

    git checkout -b feature_a

### 5. Make Changes to the Files

After creating the branch, I made changes to the HTML file (as part of the feature_a task).

### 6. Stage and Commit Changes

After making the changes, I staged and committed them to the feature_a branch.

    I staged the changes using the following command:

git add .

Then, I created a commit with the following message:

    git commit -m "Updated index.html for feature_a""

7. Push the Branch to the Remote Repository

With my changes committed locally, I pushed the feature_a branch to GitHub.

    I used the following command to push the branch:

    git push origin feature_a

### 8. Create a Pull Request

Once the branch was pushed, I created a pull request (PR) to merge my changes into the main branch.

    I navigated to the Pull Requests tab in the repository on GitHub.
    Clicked New Pull Request and selected main as the base branch and feature_a as the compare branch.
    I added a title and description explaining the changes I made.
    I also added a reviewer to approve the PR before merging.
    Finally, I clicked Create Pull Request.
    
---

### In this assignment, I followed the typical Git workflow to:

    Set up SSH authentication for secure communication with GitHub.
    Clone the repository to my local machine.
    Create a new feature branch and make changes.
    Commit and push the changes to the remote repository.
    Create a pull request and submit it for review.

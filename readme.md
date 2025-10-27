Team Profile Cards Collaboration Challenge

Welcome to the Team Profile Cards Collaboration Challenge!
This repository exercise helps a team of 7 developers practice Git and GitHub collaboration workflows while customizing a shared team page.

🎯 Objective

Each team member will customize their own profile card on a shared team page using proper Git branching and pull request workflows.

👥 Team Roles & Assignments
User	Role	Branch Name	Card Class
User 1	Frontend Developer	feature/user-1-card	.user-1
User 2	Backend Developer	feature/user-2-card	.user-2
User 3	UI/UX Designer	feature/user-3-card	.user-3
User 4	Full Stack Developer	feature/user-4-card	.user-4
User 5	DevOps Engineer	feature/user-5-card	.user-5
User 6	Data Scientist	feature/user-6-card	.user-6
User 7	Project Manager	feature/user-7-card	.user-7
🚀 Getting Started
Prerequisites

Git installed

GitHub account

Basic HTML/CSS knowledge

Code editor (VS Code recommended)

Initial Setup

Fork the repository

Go to the main repository on GitHub.

Click Fork to create your personal copy.

Clone your fork

git clone https://github.com/YOUR_USERNAME/team-profile-cards.git
cd team-profile-cards


Add upstream remote

git remote add upstream https://github.com/ORIGINAL_OWNER/team-profile-cards.git


Verify remotes

git remote -v


You should see both origin (your fork) and upstream (original repo).

🛠 Your Task: Customize Your Card
Step 1: Create Your Feature Branch

⚠️ Always create a new branch for your work!

# Switch to main branch first
git checkout main

# Pull latest changes
git pull upstream main

# Create and switch to your feature branch
git checkout -b feature/user-X-card
# Replace X with your user number (1-7)

Step 2: Customize Your HTML Content

Find your card in the HTML file (look for comments like <!-- User X Card -->) and update:

Name: Replace "User X" with your actual name

Role: Customize your role title

Bio: 2–3 sentence professional bio

Skills: Update with your actual technical skills

Social Links: Replace # with your profile URLs

Avatar: Replace the initial with your first letter or add an image

Example (User 1):

<div class="card user-1">
    <div class="card-header">
        <div class="card-avatar">
            <!-- Change from <span>U1</span> to your initial or image -->
            <span>A</span>
        </div>
    </div>
    <div class="card-body">
        <h2 class="card-name">Alex Johnson</h2>
        <p class="card-role">Frontend Specialist</p>
        <p class="card-bio">Passionate about creating responsive web applications with modern JavaScript frameworks. Love hiking and coffee.</p>
        <div class="card-skills">
            <span class="skill-tag">React</span>
            <span class="skill-tag">TypeScript</span>
            <span class="skill-tag">CSS</span>
        </div>
        <div class="card-social">
            <a href="https://linkedin.com/in/alexjohnson" class="social-icon">in</a>
            <a href="https://github.com/alexjohnson" class="social-icon">gh</a>
            <a href="https://twitter.com/alexjohnson" class="social-icon">tw</a>
        </div>
    </div>
</div>

Step 3: Style Your Card

Find your CSS section (look for .user-X classes) and add custom styles. Options:

Background colors/gradients

Border styles/colors

Custom animations

Hover effects

Typography changes

Shadows

Example CSS (User 1):

/* User 1 Card Styles */
.user-1 {
    border: 2px solid #6a11cb;
    transform: rotate(-1deg);
}

.user-1 .card-header {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.user-1:hover {
    transform: rotate(0deg) scale(1.02);
    box-shadow: 0 10px 30px rgba(106, 17, 203, 0.3);
}

.user-1 .skill-tag {
    background-color: #667eea;
    color: white;
}

Step 4: Test Your Changes

Open index.html in your browser

Verify responsiveness and that your card looks right

Ensure you didn’t modify other users’ cards

Step 5: Commit Your Changes
# Stage all changes
git add .

# Commit with descriptive message
git commit -m "feat: add personalized card for User X with custom styling"

# Push to your fork
git push origin feature/user-X-card

📤 Creating Your Pull Request

Go to your fork on GitHub.

You should see a banner suggesting creating a PR for your pushed branch → Click Compare & pull request.

Set:

base: main (original repo)

compare: feature/user-X-card

Title: Add User X Profile Card

In the description mention:

What you changed

Any custom styling you added

Tag team members for review

Click Create pull request.

Note: Do not merge your own PR. Wait for review.

📋 Collaboration Rules & Guidelines
✅ DO:

Only modify YOUR assigned card section

Create a new branch for your work

Write descriptive commit messages

Test before committing

Review teammates’ PRs

Keep cards responsive and accessible

Sync with upstream before starting new work

❌ DON'T:

Modify other users' cards

Change base CSS styles (above user sections)

Work directly on main

Push to the upstream repository directly

Merge your own pull requests

🔄 Syncing with Upstream

To get the latest changes from the original repo:

# Switch to main branch
git checkout main

# Fetch and merge upstream changes
git fetch upstream
git merge upstream/main

# Push to your fork
git push origin main

🆘 Troubleshooting Common Issues
Merge Conflicts
# Pull latest changes
git pull upstream main

# Resolve conflicts in your editor
# Mark as resolved
git add .

# Continue merge
git commit -m "Resolve merge conflicts"

Branch Issues

If you accidentally worked on main:

git checkout -b feature/user-X-card
git add .
git commit -m "Your message"
git push origin feature/user-X-card

# Delete local branch (if needed):
git branch -d branch-name

# Delete remote branch:
git push origin --delete branch-name

🎨 Creative Challenges (Optional)

Try one of these to go beyond the basics:

Animation Challenge: Add a unique CSS animation to your card

Accessibility Challenge: Ensure your card meets WCAG guidelines

Responsive Challenge: Make the card look great on mobile

Theme Challenge: Coordinate with another member for complementary styles

📊 Success Metrics

The challenge is successful when:

All 7 team members have customized cards

Each change was made via a separate feature branch

All changes were merged via pull requests

Every PR received at least one review

Final page displays correctly with all cards

No merge conflicts disrupted the workflow

🏆 What You'll Learn

Git fundamentals: branching, committing, pushing

GitHub workflow: forking, PRs, code review

Collaboration: working concurrently on the same project

Conflict resolution: handling merge conflicts

Code review: giving and receiving constructive feedback

🤝 Code Review Guidelines

When reviewing teammates’ PRs:

Check for errors: Does the code work? Any broken styles?

Respect boundaries: Did they only modify their assigned section?

Offer suggestions: e.g., “Consider this color/effect…”

Be constructive: “This looks great! What about adding…”

Approve promptly for non-blocking issues

📞 Need Help?

Git Documentation: Git Handbook

GitHub Help: Understanding GitHub Flow

Ask your team via PR comments or team chat

🚀 Quick Command Reference
# Clone repository
git clone https://github.com/YOUR_USERNAME/team-profile-cards.git

# Create new branch
git checkout -b feature/user-X-card

# Check current branch
git branch

# Stage changes
git add .

# Commit changes
git commit -m "Descriptive message"

# Push to your fork
git push origin feature/user-X-card

# Get latest changes
git pull upstream main

# Check status
git status

# View commit history
git log --oneline

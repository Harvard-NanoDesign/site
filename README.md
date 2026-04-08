# Welcome to the Nano-Design Group Website Source!

## Quick Start
- Install Ruby, Bundle, and Jekyll
- `bundle install`
- `bundle exec jekyll serve` in this directory to see changes locally at `http://localhost:4000`

## How to Update Content

### 1. People & Profiles
To add yourself or update your bio:
- Navigate to `_people/`.
- Create a new Markdown file (e.g., `your-name.md`).
- Use the following Front Matter:
  ```markdown
  ---
  layout: bio
  name: Your Full Name
  role: Your Role (e.g., PhD Candidate)
  image: /assets/images/your_headshot.jpg
  ---
  Your bio content goes here...
  ```

### 2. Research Projects
To add a new project:
- Navigate to `_projects/`.
- Create a new Markdown file.
- **For an Umbrella (Thrust):** set `is_umbrella: true`.
- **For a Sub-project:** Add the name of the umbrella project to `parent_projects`.
- Example Front Matter:
  ```markdown
  ---
  layout: project
  title: Project Title
  status: Active
  parent_projects:
    - Overarching Thrust Name
  people:
    - Your Name
  ---
  Project description goes here...
  ```

### 3. Publications
*(Note: If you have a dedicated system like a BibTeX file or a `_publications` collection, update this section accordingly)*
- Navigate to `_publications/`.
- Add your paper details as a new Markdown file with the appropriate metadata.

### 4. Assets (Images/PDFs)
- Place all profile pictures in `assets/images/`.
- Ensure filenames match what you write in your Markdown file's `image:` field.

## Advanced Customization
The look and feel of the site is controlled by **SCSS Variables**.
- To change colors or fonts, edit `_sass/_variables.scss`. No other CSS files should be touched for basic re-skinning.

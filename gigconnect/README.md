# Final Project
Bare repo for you to begin your final project

## Website URL
The live site for this project is deployed at: {https://gigconnect-rgfqsyxfl-gus-projects-7874b3fd.vercel.app/planner}
## Installation and Running
 1. git clone https://github.com/cscie12/final-project-gsun2698.git
   - cd final-project-gsun2698
   - cd. gig-connect
2. npm install
3. npm run build
4. npm run preview
  - The project is built using Astro -> Tailwind CSS for styling
## How requirements are met
1. Pages built through Build Process
    - The site has multiple pages generated through Astro
        - / - Home Page
        - /index - Artists listing page
        - /artist[slug] - Individual artist detail page
        - /about - About page for the project
        - /planner - Event Planner Interface
2. Data-Driven Generation
    - Artists and their attributes are stored in artists.json. Along with the venues data which is stored in venues.json. Pages like artist listings and detail pages are generated dynamically based on this data
3. Interactive Features / Web App Concepts
    - Planner functionality: add/remove artists to shortlist, assign to stages and timeslots
    - LocalStorage persistance to retain state between sessions
    - Modal popups for selecting stage times.
4. New Functionality
    - This project includes a complete event planning interface, which was not done in previous assignments. The ability to organize artists into stages with times is unique to this project
5. Use of GitHub
    - Code versioned and hosted on GitHub
6. Automated Deployment
    - The site is deployed using Vercel for automatic hosting
7. "Go Deeper" Aspect
    - The project explores client-side interactivity with a static build framework (Astro), including dynamic data handling, conditional UI updates, and local storage synchronization.

## 5-Planes approach

### Strategy
- GigConnect provides a web interface for event planners to explore, shortlist, and assign artists to stages and times. It is designed for usability, speed, and clarity.

### Scope
- Users can browse artists by category.
- View individual artist details.
- Shortlist artists for planning.
- Assign artists to stages and times.
- Remove artists from stages or planner.
- Persistant storage of planner data.

### Structure
- Pages: index.astro, artists/index.astro, artists/[slug].astro, planner.astro, about.astro
- Components: ArtistCard.Astro, shared layout BaseLayout.astro, Footer.Astro, nav.astro
- Data: data/artists.json && data/venues.json
- Style: Tailwind CSS with gradient, dark and modern styling
- Scripts: Client-side Javascript for planner and interactive UI

### Skeleton
- Navigation bar with responsive hamburger menu
- Home Page with hero section and description
- Artists page grouped into curated sections
- Artist detail page with bio, tour dates, and management info
- Planner page with
    - Shortlist grid
    - Stage boards
    - Assign/remove artists
    - Modal for selecting performance times

### Surface
- Modern aesthetic using gradients, blurred images, and shadows
- Fully responsive design across devices
- Ineractive buttons with dynamic updates (Add to Planner / Remove / Assigned to Stage)
- Planner and stages update in real-time without page reloads
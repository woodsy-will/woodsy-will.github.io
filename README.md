# William Steinley - GIS & Forestry Portfolio Website

**Live Site:** https://woodsy-will.github.io

## Project Overview

This is a professional portfolio website showcasing GIS expertise, software development skills, and geospatial projects. The site features a forestry and GIS-inspired design with earth tones and nature-based color schemes.

### Key Features
- ✅ Professional Resume Section (Experience & Education)
- - ✅ GIS Projects Showcase (PostgreSQL-GIS, PICNIC-PURSUIT, Forestry Web Scraper)
  - - ✅ Development Tools & Products (6+ tools/products)
    - - ✅ Technical Skills (categorized by expertise area)
      - - ✅ Contact Information Section
        - - ✅ Fully Responsive Design
          - - ✅ Custom CSS with Forest/GIS Theme
            - - ✅ GitHub Pages Deployment
             
              - ---

              ## File Structure

              ```
              woodsy-will.github.io/
              ├── index.html          # Main HTML file with all content
              ├── styles.css          # Complete styling with forest/GIS theme
              └── README.md           # This documentation file
              ```

              **Total Files:** 3 (HTML + CSS + Documentation)

              ---

              ## Quick Start for Future Development

              ### To Make Changes:

              1. **Edit Content (HTML):**
              2.    - Go to: https://github.com/woodsy-will/woodsy-will.github.io/blob/main/index.html
                    -    - Click the pencil icon to edit
                         -    - Make changes and commit
                          
                              - 2. **Edit Styling (CSS):**
                                3.    - Go to: https://github.com/woodsy-will/woodsy-will.github.io/blob/main/styles.css
                                      -    - Click the pencil icon to edit
                                           -    - Modify colors, fonts, or layouts
                                                -    - Commit changes
                                                 
                                                     - 3. **View Live Site:**
                                                       4.    - https://woodsy-will.github.io (updates in 1-2 minutes after commit)
                                                         
                                                             - 4. **Hard Refresh to See Changes:**
                                                               5.    - Press `Ctrl+Shift+R` (Windows/Linux) or `Cmd+Shift+R` (Mac)
                                                                 
                                                                     - ---

                                                                 ## CSS Customization Guide

                                                               ### Color Variables (All in `:root` at top of styles.css)

                                                               ```css
                                                               :root {
                                                                   /* PRIMARY COLORS - Edit these to change the entire theme */
                                                                   --primary-green: #2d5016;        /* Header & footer background */
                                                                   --secondary-green: #3d7f2f;      /* Navigation bar color */
                                                                   --accent-green: #5a9f3f;         /* Card borders & highlights */
                                                                   --light-green: #a8d08d;          /* Hover states & accents */

                                                                   /* SUPPORTING COLORS */
                                                                   --water-blue: #4a90b8;           /* Project cards & accents */
                                                                   --forest-brown: #6b4423;         /* Dark accents */

                                                                   /* NEUTRALS */
                                                                   --dark-text: #1a1a1a;            /* Text color */
                                                                   --light-bg: #f5f5f0;             /* Page background */
                                                                   --white: #ffffff;                /* Card backgrounds */
                                                               }
                                                               ```

                                                               ### How to Change Colors

                                                               **Example 1: Change to Mountain Theme**
                                                               ```css
                                                               --primary-green: #1a2e1a;
                                                               --secondary-green: #2d5a2d;
                                                               --accent-green: #4a7c4e;
                                                               --water-blue: #5b8fb5;
                                                               ```

                                                               **Example 2: Change to Desert Theme**
                                                               ```css
                                                               --primary-green: #6b4423;
                                                               --secondary-green: #8b6239;
                                                               --accent-green: #a0824d;
                                                               --water-blue: #c4a747;
                                                               ```

                                                               **Example 3: Change to Ocean Theme**
                                                               ```css
                                                               --primary-green: #1a3a52;
                                                               --secondary-green: #2d5a7f;
                                                               --accent-green: #4a90b8;
                                                               --water-blue: #87ceeb;
                                                               ```

                                                               ### Common Customizations

                                                               **1. Change Font**
                                                               Find: `body { font-family: ...}`
                                                               ```css
                                                               /* Modern option */
                                                               font-family: 'Arial', sans-serif;

                                                               /* Classic option */
                                                               font-family: 'Georgia', serif;

                                                               /* Google Font option (add to HTML <head>):
                                                               <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
                                                               font-family: 'Roboto', sans-serif;
                                                               ```

                                                               **2. Increase Spacing**
                                                               Find: `:root { --spacing-unit: 1rem; }`
                                                               Change to: `1.5rem` for more spacious feel

                                                               **3. Change Border Radius (Roundness)**
                                                               Find: `:root { --border-radius: 8px; }`
                                                               Change to: `15px` for rounder, `3px` for sharper

                                                               **4. Modify Hover Effects**
                                                               Find: `.gis-project-card:hover { transform: translateY(-8px) scale(1.02); }`
                                                               Change `-8px` to `-12px` for more dramatic lift

                                                               **5. Adjust Text Sizes**
                                                               Find: `header h1 { font-size: 3.5rem; }`
                                                               Change to: `4rem` for larger, `3rem` for smaller

                                                               ---

                                                               ## Content Structure & HTML Classes

                                                               ### Resume Section
                                                               ```html
                                                               <section id="resume">
                                                                   <div class="resume-section">
                                                                       <div class="experience-item">
                                                                           <div class="position">Job Title</div>
                                                                           <div class="company">Company Name</div>
                                                                       </div>
                                                                   </div>
                                                               </section>
                                                               ```

                                                               ### GIS Projects Section
                                                               ```html
                                                               <section id="gis-projects">
                                                                   <div class="gis-projects-grid">
                                                                       <div class="gis-project-card">
                                                                           <h3>Project Name</h3>
                                                                           <p>Description</p>
                                                                           <div class="project-tech">
                                                                               <span class="tech-badge">Technology</span>
                                                                           </div>
                                                                       </div>
                                                                   </div>
                                                               </section>
                                                               ```

                                                               ### Development Tools Section
                                                               ```html
                                                               <section id="tools">
                                                                   <div class="tools-products-grid">
                                                                       <div class="tool-card">
                                                                           <span class="tool-icon">🔧</span>
                                                                           <h3>Tool Name</h3>
                                                                           <p>Description</p>
                                                                           <span class="tool-type">Type</span>
                                                                       </div>
                                                                   </div>
                                                               </section>
                                                               ```

                                                               ### Skills Section
                                                               ```html
                                                               <section id="skills">
                                                                   <div class="skills-grid">
                                                                       <div class="skill-category">
                                                                           <h3>Category</h3>
                                                                           <div class="skill-tags">
                                                                               <span class="skill-tag">Skill</span>
                                                                           </div>
                                                                       </div>
                                                                   </div>
                                                               </section>
                                                               ```

                                                               ---

                                                               ## How to Update Content

                                                               ### 1. Add a New GIS Project

                                                               Edit `index.html`, find the GIS Projects section, and add:

                                                               ```html
                                                               <div class="gis-project-card">
                                                                   <h3>New Project Name</h3>
                                                                   <p>Brief description of the project and what it demonstrates.</p>
                                                                   <div class="project-tech">
                                                                       <span class="tech-badge">Technology1</span>
                                                                       <span class="tech-badge">Technology2</span>
                                                                   </div>
                                                                   <a href="https://github.com/..." class="gis-link" target="_blank">View on GitHub →</a>
                                                               </div>
                                                               ```

                                                               ### 2. Add a New Skill

                                                               Find the Skills section, locate your skill category, and add:

                                                               ```html
                                                               <span class="skill-tag">New Skill</span>
                                                               ```

                                                               ### 3. Update Your Resume

                                                               Find the Resume section and modify:
                                                               - Job titles and company names
                                                               - - Dates and descriptions
                                                                 - - Education details
                                                                  
                                                                   - ### 4. Add a New Development Tool
                                                                  
                                                                   - Find the Development Tools section and add:
                                                                  
                                                                   - ```html
                                                                     <div class="tool-card">
                                                                         <span class="tool-icon">🛠️</span>
                                                                         <h3>Tool Name</h3>
                                                                         <p>Description of what the tool does.</p>
                                                                         <span class="tool-type">Category</span>
                                                                     </div>
                                                                     ```

                                                                     ---

                                                                     ## CSS Classes Reference

                                                                     | Class | Purpose | Location |
                                                                     |-------|---------|----------|
                                                                     | `.container` | Constrain content width | Wraps main content |
                                                                     | `.resume-section` | Grid layout for resume | Resume section |
                                                                     | `.experience-item` | Individual job entry | Resume experience |
                                                                     | `.gis-projects-grid` | 3-column grid layout | GIS Projects |
                                                                     | `.gis-project-card` | Project card styling | Individual projects |
                                                                     | `.tools-products-grid` | 3-column grid layout | Development tools |
                                                                     | `.tool-card` | Tool card styling | Individual tools |
                                                                     | `.skills-grid` | Responsive skill grid | Skills section |
                                                                     | `.skill-tag` | Individual skill badge | Skills |
                                                                     | `.tech-badge` | Technology badge | Project cards |
                                                                     | `.contact-links` | Contact button styling | Contact section |

                                                                     ---

                                                                     ## Responsive Design

                                                                     The site is fully responsive with breakpoints at:
                                                                     - **Desktop:** 1200px (full width)
                                                                     - - **Tablet:** 768px and below
                                                                       - - **Mobile:** 480px and below
                                                                        
                                                                         - The CSS automatically adjusts:
                                                                         - - Font sizes
                                                                           - - Grid layouts (switches to single column on mobile)
                                                                             - - Navigation (stays sticky)
                                                                               - - Spacing and padding
                                                                                
                                                                                 - ---

                                                                                 ## Navigation Structure

                                                                                 The site uses anchor links for smooth scrolling:

                                                                                 ```
                                                                                 Header (Home)
                                                                                 ├── Resume (#resume)
                                                                                 ├── GIS Projects (#gis-projects)
                                                                                 ├── Development Tools (#tools)
                                                                                 ├── Skills (#skills)
                                                                                 └── Contact (#contact)
                                                                                 ```

                                                                                 Each nav link smoothly scrolls to the corresponding section.

                                                                                 ---

                                                                                 ## Browser Compatibility

                                                                                 - ✅ Chrome/Edge (latest)
                                                                                 - - ✅ Firefox (latest)
                                                                                   - - ✅ Safari (latest)
                                                                                     - - ✅ Mobile browsers (iOS Safari, Chrome Mobile)
                                                                                      
                                                                                       - Uses modern CSS features (CSS Grid, Flexbox, CSS Variables).
                                                                                      
                                                                                       - ---

                                                                                       ## Deployment & GitHub Pages

                                                                                       **Current Setup:**
                                                                                       - Repository: `woodsy-will/woodsy-will.github.io`
                                                                                       - - Branch: `main`
                                                                                         - - Deployment: Automatic (GitHub Pages)
                                                                                           - - Status: Live at https://woodsy-will.github.io
                                                                                             - - HTTPS: ✅ Enabled
                                                                                              
                                                                                               - **To Deploy Changes:**
                                                                                               - 1. Edit files in GitHub web interface or locally
                                                                                                 2. 2. Commit to `main` branch
                                                                                                    3. 3. GitHub Pages automatically rebuilds (1-2 minutes)
                                                                                                       4. 4. Hard refresh browser: `Ctrl+Shift+R`
                                                                                                         
                                                                                                          5. ---
                                                                                                         
                                                                                                          6. ## Color Palette Reference
                                                                                                         
                                                                                                          7. ### Current Forestry/GIS Theme
                                                                                                          8. - **Primary Green:** `#2d5016` (Deep forest)
                                                                                                             - - **Secondary Green:** `#3d7f2f` (Medium forest)
                                                                                                               - - **Accent Green:** `#5a9f3f` (Bright green)
                                                                                                                 - - **Water Blue:** `#4a90b8` (Topographic water)
                                                                                                                   - - **Brown Accents:** `#6b4423` (Bark/earth)
                                                                                                                     - - **Light Background:** `#f5f5f0` (Off-white)
                                                                                                                      
                                                                                                                       - ### Color Psychology
                                                                                                                       - - **Greens:** Nature, growth, GIS/forestry connection
                                                                                                                         - - **Blues:** Water features, GIS data layers
                                                                                                                           - - **Browns:** Earth, forestry, stability
                                                                                                                            
                                                                                                                             - ---
                                                                                                                             
                                                                                                                             ## Future Enhancement Ideas
                                                                                                                             
                                                                                                                             ### Content Additions
                                                                                                                             - [ ] Add portfolio images/screenshots of projects
                                                                                                                             - [ ] - [ ] Include PDF resume download link
                                                                                                                             - [ ] - [ ] Add blog/articles section
                                                                                                                             - [ ] - [ ] Create case studies for major projects
                                                                                                                             - [ ] - [ ] Add testimonials/recommendations
                                                                                                                            
                                                                                                                             - [ ] ### Technical Enhancements
                                                                                                                             - [ ] - [ ] Add dark mode toggle
                                                                                                                             - [ ] - [ ] Implement smooth scroll animations
                                                                                                                             - [ ] - [ ] Add image gallery/lightbox
                                                                                                                             - [ ] - [ ] Create filtering for projects by technology
                                                                                                                             - [ ] - [ ] Add search functionality
                                                                                                                             - [ ] - [ ] Implement contact form
                                                                                                                            
                                                                                                                             - [ ] ### Design Improvements
                                                                                                                             - [ ] - [ ] Add custom fonts via Google Fonts
                                                                                                                             - [ ] - [ ] Implement hero section with background image
                                                                                                                             - [ ] - [ ] Add animated background elements
                                                                                                                             - [ ] - [ ] Create custom icons instead of emoji
                                                                                                                             - [ ] - [ ] Implement parallax scrolling
                                                                                                                            
                                                                                                                             - [ ] ### Functionality
                                                                                                                             - [ ] - [ ] GitHub API integration to display live projects
                                                                                                                             - [ ] - [ ] Analytics tracking (Google Analytics)
                                                                                                                             - [ ] - [ ] Email subscription form
                                                                                                                             - [ ] - [ ] Social media integration
                                                                                                                            
                                                                                                                             - [ ] ---
                                                                                                                            
                                                                                                                             - [ ] ## Common Issues & Solutions
                                                                                                                            
                                                                                                                             - [ ] ### **Changes Not Appearing?**
                                                                                                                             - [ ] - Hard refresh: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)
                                                                                                                             - [ ] - Wait 2-3 minutes for GitHub Pages to rebuild
                                                                                                                             - [ ] - Check that you committed the changes
                                                                                                                            
                                                                                                                             - [ ] ### **Colors Look Wrong?**
                                                                                                                             - [ ] - Make sure you're using hex color codes: `#2d5016`
                                                                                                                             - [ ] - CSS variables must be in `:root { }`
                                                                                                                             - [ ] - Check that closing `}` is present in `:root`
                                                                                                                            
                                                                                                                             - [ ] ### **Grid Not Aligning?**
                                                                                                                             - [ ] - Check `display: grid;` or `display: flex;` is set
                                                                                                                             - [ ] - Verify `gap:` property is correct
                                                                                                                             - [ ] - Ensure `grid-template-columns:` is valid
                                                                                                                            
                                                                                                                             - [ ] ### **Links Not Working?**
                                                                                                                             - [ ] - Verify href attributes are correct: `href="#section-id"`
                                                                                                                             - [ ] - Check that section IDs match nav link hrefs
                                                                                                                             - [ ] - External links need `target="_blank"`
                                                                                                                            
                                                                                                                             - [ ] ---
                                                                                                                            
                                                                                                                             - [ ] ## Technologies Used
                                                                                                                            
                                                                                                                             - [ ] - **HTML5:** Semantic markup
                                                                                                                             - [ ] - **CSS3:** Grid, Flexbox, CSS Variables, Animations
                                                                                                                             - [ ] - **GitHub Pages:** Static site hosting
                                                                                                                             - [ ] - **Responsive Design:** Mobile-first approach
                                                                                                                            
                                                                                                                             - [ ] ---
                                                                                                                            
                                                                                                                             - [ ] ## File Size Information
                                                                                                                            
                                                                                                                             - [ ] - `index.html`: ~15 KB
                                                                                                                             - [ ] - `styles.css`: ~25 KB
                                                                                                                             - [ ] - Total: ~40 KB (very lightweight)
                                                                                                                            
                                                                                                                             - [ ] **Page Load Speed:** Excellent (no external dependencies)
                                                                                                                            
                                                                                                                             - [ ] ---
                                                                                                                            
                                                                                                                             - [ ] ## Quick Reference: Edit URLs
                                                                                                                            
                                                                                                                             - [ ] | Task | URL |
                                                                                                                             - [ ] |------|-----|
                                                                                                                             - [ ] | Edit HTML | https://github.com/woodsy-will/woodsy-will.github.io/edit/main/index.html |
                                                                                                                             - [ ] | Edit CSS | https://github.com/woodsy-will/woodsy-will.github.io/edit/main/styles.css |
                                                                                                                             - [ ] | View Live | https://woodsy-will.github.io |
                                                                                                                             - [ ] | View Files | https://github.com/woodsy-will/woodsy-will.github.io |
                                                                                                                            
                                                                                                                             - [ ] ---
                                                                                                                            
                                                                                                                             - [ ] ## Project Status
                                                                                                                            
                                                                                                                             - [ ] **Version:** 1.0 (Complete)
                                                                                                                             - [ ] **Last Updated:** March 2026
                                                                                                                             - [ ] **Status:** ✅ Live and Production Ready
                                                                                                                            
                                                                                                                             - [ ] ---
                                                                                                                            
                                                                                                                             - [ ] ## How to Use This Documentation in Future Chats
                                                                                                                            
                                                                                                                             - [ ] 1. Copy this entire README
                                                                                                                             - [ ] 2. Share it with Claude in a new chat
                                                                                                                             - [ ] 3. Say: "Here's my portfolio project context. I want to [make changes]"
                                                                                                                             - [ ] 4. Include any specific CSS color codes or sections you've customized
                                                                                                                             - [ ] 5. Provide screenshots if needed
                                                                                                                            
                                                                                                                             - [ ] This will give the new chat complete context about your project structure and customization options.
                                                                                                                            
                                                                                                                             - [ ] ---
                                                                                                                            
                                                                                                                             - [ ] ## Support & Next Steps
                                                                                                                            
                                                                                                                             - [ ] - To make CSS changes: Edit the color variables at the top of `styles.css`
                                                                                                                             - [ ] - To add content: Edit the HTML sections in `index.html`
                                                                                                                             - [ ] - To troubleshoot: Check the "Common Issues & Solutions" section above
                                                                                                                             - [ ] - To explore new features: See "Future Enhancement Ideas"
                                                                                                                            
                                                                                                                             - [ ] **Happy Building! 🚀**

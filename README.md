## Week 5-6: Advanced CSS Layouts 🎨

### In this week you will learn: 🏫

- Advanced CSS layout techniques
   - Flexbox
   - Grid
   - Responsive Design
   - CSS Frameworks (recommended Bootstrap instead of tailwind)

### Resources🔗

- [Flexbox Guide (CSS-Tricks)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Grid Guide (MDN Web Docs)](https://developer.mozilla.org/en-US/docs/Web/CSS/grid)
- [Responsive Web Design (w3schools.com)](https://www.w3schools.com/css/css_rwd_intro.asp)
- [Learn CSS In Arabic 2021](https://www.youtube.com/playlist?list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe)
- [Useful Channel for CSS](https://www.youtube.com/@KevinPowell/playlists)
- [Bootstrap Documentation](https://getbootstrap.com/docs/5.0/getting-started/introduction/) (optional)
- [Bootstrap Video](https://www.youtube.com/watch?v=GByMUIyfJhk&list=PLYyqC4bNbCIdES52srHE6xTiIgvgMkBWu&index=30&ab_channel=%D8%A3%D9%83%D8%A7%D8%AF%D9%8A%D9%85%D9%8A%D8%A9%D8%AA%D8%B1%D9%85%D9%8A%D8%B2) (optional)

---
**Why Consider Using Bootstrap?**

Bootstrap is a popular CSS framework that provides pre-built, responsive design components and styles. It can significantly simplify the process of designing and styling your web pages. Here's why Bootstrap may be a good choice:

- **Ready-Made Components**: Bootstrap offers a library of ready-to-use UI components, such as navigation bars, modals, and forms. This means you can quickly add common elements to your page without having to write custom CSS.

- **Responsive by Default**: Bootstrap is designed with mobile-first responsiveness in mind. It automatically adapts your webpage's layout to different screen sizes, saving you time and effort in creating a responsive design from scratch.

- **Consistent Design**: Bootstrap provides a consistent and visually appealing design across different browsers and devices. This ensures a polished and professional look for your portfolio.

- **Documentation and Community Support**: Bootstrap has extensive documentation and a large community of developers. This means you can easily find resources, tutorials, and help when working with Bootstrap.


---

### Your Task 📝

Create a Responsive Web Page using CSS Layouts
Apply CSS layout techniques to your previous personal portfolio page. Implement the following features:

1. **Flexbox Layout**: Use Flexbox to create a flexible and responsive layout for sections of your webpage, you can use it to organize buttons on your page.

2. **Grid Layout**: Implement a grid-based layout to organize and display images.

3. **Responsive Design**: Ensure that your webpage looks good and functions well on two screen sizes.

4. **Optional: CSS Framework (e.g., Bootstrap)**: You may create your whole personal portfolio using Bootstrap.

**Note**: You have the option to either complete the first three parts of the task (Flexbox, Grid, and Responsive Design) or create a whole new web page based on Bootstrap.

**Example**:

```css
/* Flexbox container */
.container {
   display: flex;
   justify-content: space-between;
   align-items: center;
}

/* Grid layout for project showcase */
.project-grid {
   display: grid;
   grid-template-columns: repeat(3, 1fr);
   gap: 20px;
}

/* Responsive Design for smaller screens (e.g., mobile devices) */
@media screen and (max-width: 768px) {
   .container {
      flex-direction: column;
      align-items: flex-start;
   }

   .container > div {
      margin-bottom: 10px;
   }

   .project-grid {
      grid-template-columns: repeat(2, 1fr);
   }
}

/* Responsive Design for larger screens (e.g., tablets and desktops) */
@media screen and (min-width: 769px) {
   .container {
      justify-content: space-evenly;
   }

   .container > div {
      margin: 0;
   }

   .project-grid {
      grid-template-columns: repeat(3, 1fr);
   }
}

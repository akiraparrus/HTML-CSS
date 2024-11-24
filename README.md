# HTML-CSS
# Broadway Design Project

This project is a responsive landing page for a fictional design firm, **Broadway Design**. It demonstrates CSS layout and positioning techniques, focusing on improving the structure and visual appeal of the webpage.

## Features

- **Sticky Navigation Bar**: The `<header>` stays fixed at the top of the screen as users scroll.
- **Horizontal Navigation Menu**: List items in the `<nav>` are displayed side by side.
- **Flexible Layout**: Supporting sections (Design, Develop, Deploy) are aligned horizontally with defined dimensions.
- **Proper Stacking with `z-index`**: Ensures no overlapping issues between the header and main content.
- **Responsive Design**: Modern layout that adapts to different screen sizes.

## Technologies Used

- HTML5
- CSS3

## Key Enhancements

1. **Header Positioning**:
   - Used `position: fixed` to make the header stick to the top of the viewport.
   - Adjusted the width of the header to span its parent container.

2. **Navigation Menu**:
   - Set `<li>` elements inside `<nav>` to `display: inline` for a horizontal layout.
   - Defined a consistent width of 80px for each navigation item.

3. **Content Flow**:
   - Adjusted the `<main>` element to avoid overlap with the sticky header by using offsets.
   - Applied `z-index` to bring the header above other elements.

4. **Supporting Sections**:
   - Styled supporting elements (Design, Develop, Deploy) using `display: inline-block` for horizontal alignment.
   - Set their dimensions to 200px by 200px.

## How to View the Project

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/Broadway-Design.git

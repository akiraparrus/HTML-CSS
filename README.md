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

   html, body {
  margin: 0;
  padding: 0;
}

header {
  background-color: #333333;
  position: fixed;
  width: 500px;
}

nav {
  margin: 0;
  padding: 20px 0;
}

nav li {
  color: #fff;
  font-family: 'Raleway', sans-serif;
  font-weight: 600;
  font-size: 12px;
  display: inline-block;
  width: 80px;
}

main {
  text-align: center;
  position: relative;
  z-index: 1;
  top: 80px;
}

main h1 {
  color: #333;
  font-family: 'Raleway', sans-serif;
  font-weight: 600;
  font-size: 70px;
  margin-top: 0px;
  padding-top: 80px;
  margin-bottom: 80px;
  text-transform: uppercase;
}

footer {
  background-color: #333;
  color: #fff;
  padding: 30px 0;
}

footer p {
  font-family: 'Raleway', sans-serif;
  text-transform: uppercase;
  font-size: 11px;
}

.container {
  max-width: 940px;
  margin: 0 auto;
  padding: 0 10px;
  text-align: center;
}

.jumbotron {
  height: 800px;
  background-image: url("https://content.codecademy.com/projects/broadway/bg.jpg");
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}

.btn-main {
  background-color: #333;
  color: #fff;
  font-family: 'Raleway', sans-serif;
  font-weight: 600;
  font-size: 18px;
  letter-spacing: 1.3px;
  padding: 16px 40px;
  text-decoration: none;
  text-transform: uppercase;
}

.btn-default {
  font-family: 'Raleway', sans-serif;
  font-weight: 600;
  font-size: 10px;
  letter-spacing: 1.3px;
  padding: 10px 20px;
  text-decoration: none;
  text-transform: uppercase;  
  margin-bottom: 20px;      
}

.supporting {
  padding-top: 80px;
  padding-bottom: 100px;
}

.supporting .col {
  font-family: 'Raleway', sans-serif;
  text-align: center;
  display: inline-block;
  height: 200px;
  width: 200px;
}

.supporting img {
  height: 32px;
}

.supporting h2 {
  font-weight: 600;
  font-size: 23px;
  text-transform: uppercase;
}

.supporting p {
  font-weight: 400;
  font-size: 14px;
  line-height: 20px;
  padding: 0 20px;
  margin-bottom: 20px;
}

.supporting a {
  background-color: white;
  color: #333333;
  font-family: 'Raleway', sans-serif;
  font-weight: 600;
  font-size: 12px;
  letter-spacing: 1.3px;
  text-decoration: none;
  text-transform: uppercase;
  padding: 10px;
  margin-bottom: 10px;
  border: 2px solid #333333; 
}

@media (max-width: 500px) {
  main h1 {
    font-size: 50px;
    padding: 0 40px;
  }

  .supporting .col {
    width: 100%;
  }
  footer {
  position: fixed;
  bottom: 0;
  width: 100%;
}
<!DOCTYPE html>
<html>
  
  <head>
    <link href='https://fonts.googleapis.com/css?family=Raleway:400, 600' rel='stylesheet' type='text/css'>
    <link href='style.css' rel='stylesheet' type='text/css'/>
  </head>

  <body>
    
    <header>
        <nav>
          <ul>
            <li> About </li> <li> Work </li> <li> Team </li> <li> Contact </li>
          </ul>
        </nav>
    </header>

    <main>
      <div class="jumbotron">
        <div class="container">  
          <h1>We are Broadway</h1>
          <a href="#" class="btn-main"> Get Started </a>
        </div>
      </div>
    </main>

    <section class="supporting">
      <div class="container">
        
        <div class="col">
          <img src="https://content.codecademy.com/projects/broadway/design.svg">
          <h2>Design</h2>
          <p>Make your projects look great and interact beautifully.</p>
          <a href="#"> Learn More</a><br>
        </div>
        
        <div class="col">
          <img src="https://content.codecademy.com/projects/broadway/develop.svg">
          <h2>Develop</h2>
          <p>Use modern tools to turn your design into a web site</p>
          <a href="#"> Learn More</a><br>
        </div>
        
        <div class="col">
          <img src="https://content.codecademy.com/projects/broadway/deploy.svg">
          <h2>Deploy</h2>
          <p>Use modern tools to turn your design into a web site</p>
          <a href="#"> Learn More</a><br>
        </div>
        
      </div>
    </section>

    <footer>
      <div class="container">
        <p>&copy; Broadway 2017</p>
      </div>
    </footer>
    
  </body>
</html>

# Abiyag.github.io
HW #2:
# Reflection

# 1. Difference between flex-direction: row and flex-direction: column.
flex-direction: row places flex items next to each other horizontally from left to right. This is the default layout for a flex container.
flex-direction: column stacks the items vertically from top to bottom. 

# 2. Importance of relative units in responsive design
Relative units like %, vh, and rem adjust based on the screen size or parent element. This helps layouts resize properly on different devices like phones, tablets, and laptops. Fixed pixels stay the same size, which can make elements too large or too small on different screens.

## 3. AI Attribution
I used AI to help troubleshoot my CSS layout and responsiveness. One prompt I used was: "How do I make my project cards display in a 3-column grid and collapse to one column on mobile?"*

The AI suggested the following CSS:

```
.project-grid{
display:grid;
grid-template-columns: repeat(3,1fr);
gap:20px;
}
```

I modified the layout by adding a media query so that the grid changes to a single column on smaller screens:

```
@media (max-width:768px){
.project-grid{
grid-template-columns:1fr;
}
}
```

This adjustment allowed my projects section to be responsive and display properly on mobile devices.






1. Describe the path an HTTP Request takes from a browser to your GitHub Pages site.
    - When I type my website URL into the browser, the browser asks DNS to find the IP address of the site. Then it sends an HTTP request through my internet provider to GitHub’s servers. GitHub’s server finds my HTML and CSS files and sends them back to my browser. The browser then displays the website on my screen.

2. We discussed Docker Containers in class. Explain how a Docker Container differs from the
environment provided by GitHub Pages.
    - A Docker container is a full environment that can run applications with its own system. GitHub Pages only hosts static files like HTML and CSS. Docker can run programs, but GitHub Pages cannot run backend code.

3. AI Attribution: If you used GenAI (ChatGPT, Claude, etc.) to help write code, you must
include the prompt you used and explain one logic error the AI made that you had to fix
manually.

    - All I used AI for is asking for a step-by-step breakdown of what to do. Here is the prompt: "so my teacher wants us to create our own git page. tell me what i need to do step my step by reading the instruction files i uploaded. be very precise and clear"
    - I used google to searc up styling and html syntaxes whenever I needed.  
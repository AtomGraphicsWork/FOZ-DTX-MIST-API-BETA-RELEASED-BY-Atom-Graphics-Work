# MIST Framework

MIST (Modular Interactive UI Framework) is a JavaScript framework designed for building powerful and secure web applications with a focus on performance and flexibility. MIST offers a unique virtualization feature, providing enhanced speed and security by preventing third-party renderers from accessing the content directly.

## Features

- **Virtual Background:** MIST virtualizes its components, ensuring consistent rendering and behavior across different platforms and environments.
- **High Performance:** With its modular architecture and optimized rendering, MIST delivers fast and responsive web applications.
- **Security:** By blocking third-party web views through its virtual world nature, MIST enhances security and prevents unauthorized access to the application content.
- **Customizable Widgets:** MIST provides a range of widgets and UI components for building modern and interactive user interfaces.

## Getting Started

To get started with MIST, follow these steps:

1. Download Include the MIST framework in your HTML file:

   ```html
   <!-- Place the downloaded project files int the root directory of the project -->
   <link rel="stylesheet" href="mist.min.css">
   <script src="mist.min.js"></script>
   
   ``` 

2. Follow the documentation


# Documentation

## Using JavaScript for designing the UI

We will use JavaScript as primary language for using <b>MIST</b> because it provides various functions and beggner friendly syntax for learning <b>MIST</b>.

## Window

<b>MIST</b> provides a full fledged Independent <b>Window Manager</b> which is responsible for making the fully functional <code>windows</code> and for making the <code>windows</code> we need to actually tell <b>MIST</b> to create <code>windows</code> and for this <b>MIST</b> provides us 2 classes <code>MIST_Window</code> and <code>MIST_Mirror_Window</code>. These classes are responsible to tell <b>MIST</b> that we want to actually create <code>window</code>.

### MIST_Window (Class)

<code>MIST_Window</code> class takes 3 arguments for getting the information about <code>window</code> to create on your app, Those 3 arguments are <code>title, width, height</code>. <code>title</code> will asssign the title for your window and <code>width,height</code> will assign the width and height for your window.

<b>Example</b>

```javascript
// Defining an inheritance of MIST_Window class for making window
const my_Window = new MIST_Window("my quite Window", 300, 200); // This will create a window with title my quite Window and width of 300 pixels and height of 200 pixels
```

### Properties

Ok congratulations if you has created your first <code>Window with</code> <b>MIST</b>, Now you will feel prety good but you must know these <code>properties</code> of the <code>window</code> you have just created othervise it's nothing for you. So let's dive into these properties , So currently <b>MIST</b> has <code>setContent(), setFont(), setBackground(), setTextColor(), getHtmlId()<code>.

### setContent(htmlContent) (Method)

<code>setContent()</code> injects the <b>HTML</b> inside the <code>window</code> and this is so much important as without content you can't really do anything with <code>window</code>.

<b>Example</b>

```javascript
// Defining an inheritance of MIST_Window class for making window
const my_Window = new MIST_Window("my quite Window", 300, 200); // This will create a window with title my quite Window and width of 300 pixels and height of 200 pixels

// Adding the content in the window
my_Window.setContent("<h2>Hi there</h2><p>This is the content inside the window</p>");
```

### setFont(fontName) (Method)

<code>setFont()</code> sets the <b>FONT</b> inside the <code>window</code> and this is so much important for customising the <code>window</code>. This method is so powerfull because this can add <code>css</code> fonts as well as <code>MIST FONTS</code> also, <b>MIST</b> Actually ships a lot of fonts with the package here's the list of the available <code>FONTS</code> which are shipped with current versions <code>Raleway, Exo, Oswald, Writing, Ubuntu_Mono, Ubuntu, Ubuntu_C, RobotoCondensed, RobotoCondensed_Intalic, Outdoor, Metropolis, good_times, GlacialIndifference, Coolvetica, AxelBrush</code>. You can find these fonts inside <code>mist.min.css</code> file in the root directory of package also you can use these with css also.

<b>Example</b>

```javascript
// Defining an inheritance of MIST_Window class for making window
const my_Window = new MIST_Window("my quite Window", 300, 200); // This will create a window with title my quite Window and width of 300 pixels and height of 200 pixels

// Adding the content in the window
my_Window.setFont("Exo");
```

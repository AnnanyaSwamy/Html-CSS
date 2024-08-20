# Meta Tags

| **Tag** | **Description** | **Example** |
| --- | --- | --- |
| `<meta name="description"/>` | Provides a brief description of the web page. | `<meta name="description" content="A brief description of your page">` |
| `<meta name="title"/>` | Specifies the title of the web page. | `<meta name="title" content="Your Page Title">` |
| `<meta name="author"/>` | Specifies the author of the web page. | `<meta name="author" content="Author Name">` |
| `<meta name="language"/>` | Specifies the language of the web page. | `<meta name="language" content="english">` |
| `<meta name="robots"/>` | Tells search engines how to crawl or index a certain page. | `<meta name="robots" content="index,follow">` |
| `<meta name="google"/>` | Tells Google not to show the sitelinks search box for your page when showing search results. | `<meta name="google" content="nositelinkssearchbox">` |
| `<meta name="googlebot"/>` | Tells Google not to provide automatic translation for your page if the user uses a different language. | `<meta name="googlebot" content="notranslate">` |
| `<meta name="revised"/>` | Specifies the last modified date and time of changes on the page. | `<meta name="revised" content="Sunday, July 18th, 2010, 5:15 pm">` |
| `<meta name="rating"/>` | Specifies the expected audience for your page. | `<meta name="rating" content="safe for kids">` |
| `<meta name="copyright"/>` | Specifies the copyright for the page. | `<meta name="copyright" content="Copyright 2022">` |
| `<meta charset="UTF-8"/>` | Specifies the character encoding used for the page. | `<meta charset="UTF-8">` |
| `<meta http-equiv="content-type"/>` | Specifies the format of the document returned by the server. | `<meta http-equiv="content-type" content="text/html">` |
| `<meta http-equiv="default-style"/>` | Specifies the format of the styling document. | `<meta http-equiv="default-style" content="yourstyle.css">` |
| `<meta http-equiv="refresh"/>` | Specifies the duration before the page is considered stale (refresh interval). | `<meta http-equiv="refresh" content="30">` |
| `<meta http-equiv="Content-language"/>` | Specifies the language of the page. | `<meta http-equiv="Content-language" content="en-US">` |
| `<meta http-equiv="Cache-Control"/>` | Instructs the browser how to cache your page. | `<meta http-equiv="Cache-Control" content="no-cache">` |
| `<meta name="format-detection"/>` | Indicates that telephone numbers should appear as clickable hypertext links for making calls. | `<meta name="format-detection" content="telephone=yes">` |
| `<meta name="HandheldFriendly"/>` | Specifies that the page can be properly viewed on mobile devices. | `<meta name="HandheldFriendly" content="true">` |
| `<meta name="viewport"/>` | Specifies the area of the window in which web content can be seen, crucial for responsive design. | `<meta name="viewport" content="width=device-width, initial-scale=1.0">` |
| `<meta http-equiv="refresh"/>` | Specifies the duration of the page before it’s considered stale. | `<meta http-equiv="refresh" content="30">` |
- I is important to build repositories of code templates and knowledge you build overtime
- Script elements to link js files are added at the end of the body
- link tag for css at the end of the head element
- Common Template:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bare Bones Layout</title>
    <meta name="description" content="A brief desscription">
    <meta name="author" content="Your site name">
    <link rel="stylesheet" href="">
</head>
<body>
    <header></header>
    <nav></nav>
    <main></main>
    <footer></footer>
    <script></script>
</body>
</html>
```

- Common layouts:
1. NavBar
2. Carousel
3. Blog Layout
4. Dashboard Layout

## Meta tags help webpages create previews of other web pages

- Different from traditional seo meta tags they are related to search engine opt
- Open Graph Protocol: Metadata Rules for describing websites-Established by facebook to give users a preview of the link theyre about to click
- these are also inside head element but instead of name attribute they use property attribute instead of name attitude property=”og:type” etc etc.
- image, type and title are compulsory
- more than 1 header element can exist in an html doc
- Here's a table summarizing the information about the Open Graph Protocol:

| **Property** | **Description** | **Example** |
| --- | --- | --- |
| `og:title` | Defines the title of the page, which will appear in the social media preview. | `<meta property="og:title" content="Blog Post Title">` |
| `og:type` | Defines the type of content (e.g., website, video, music, article). | `<meta property="og:type" content="article">` |
| `og:url` | Defines the permanent web address (URL) of the page to be used in the preview. | `<meta property="og:url" content="<https://example.com/blog-post>">` |
| `og:image` | Defines the URL of an image that must display when the page is shared. | `<meta property="og:image" content="<https://example.com/image.jpg>">` |
| `og:description` | Provides a description of the webpage, often displayed beneath the title in the preview. | `<meta property="og:description" content="This is a brief description of the content.">` |
| `og:locale` | Describes the language and territory of the webpage's content (e.g., en_US for English/United States). | `<meta property="og:locale" content="en_US">` |
| `og:site_name` | Describes the name of the overall website that the webpage belongs to. | `<meta property="og:site_name" content="Example Website">` |

### Required Properties

1. **Title (`og:title`)**: Defines the title of the page that will appear in the preview.
2. **Type (`og:type`)**: Defines the type of content (e.g., website, video, music, article).
3. **URL (`og:url`)**: Defines the permanent web address that the social network must use for the specific page.
4. **Image (`og:image`)**: Defines a URL to an image that must display when the website is shared.

### Optional Properties

1. **Description (`og:description`)**: Provides a description of the webpage.
2. **Locale (`og:locale`)**: Describes the language and territory of the webpage's content.
3. **Site Name (`og:site_name`)**: Describes the name of the overall website that the webpage belongs to.

- **Pre-OGP Issues**:
    - Before the Open Graph Protocol (OGP), social networks and search engines struggled to accurately interpret the title, description, and images for shared content.
    - This often resulted in poorly scaled or random images in link previews.
- **OGP Adoption**:
    - Facebook introduced OGP to give users more control over how their content is displayed on social media.
    - Other social media platforms, including Meta-owned companies, adopted similar protocols with different prefixes.
- **Need for Social Media Cards**:
    - Social media cards are essential for capturing user attention, especially in the era of internet marketing.
    - They should summarize the content of a webpage and can be tailored to specific pages or the entire website.
- **Importance of `type` OGP Tag**:
    - The `type` tag is crucial for describing the link’s content (e.g., book, article, movie).
    - It helps provide detailed metadata, which can make a stronger impression on social media users.
- **Social Media Cards and SEO**:
    - Social media cards enhance SEO by providing web crawlers with metadata that helps rank websites.
    - They also help track website traffic and can include auxiliary tags like video for better engagement.
- **Best Practices**:
    - Developers should stick to required tags but can use additional tags for specific needs.
    - Meta offers resources for developers to optimize social media cards.
- **Conclusion**:
    - Effective social media cards are vital for informing users and driving traffic to websites.
    - The effort spent on adding social media tags is worthwhile for better online visibility.

# Form Validation

- Ensures data is valid and conforms to defined rules
- types: Client Side Validation (JavaScript),  Server Side Validation (More Secure, prevents malicious users from tampering with your websites code and prevent invalid submissions of dat to your server, backend validates data before processing it).
- Required attribute: compulsory value
- Here’s a table summarizing the different HTML input types along with beginner-friendly examples:

| **Input Type** | **Description** | **Example Code** | **Example Use Case** |
| --- | --- | --- | --- |
| **Button** | Clickable button, often used in forms to trigger a script. | `<input type="button" value="Click me" onclick="msg()" />` | A button that displays an alert when clicked. |
| **Checkbox** | Allows the user to select/deselect one or more options. | `<input type="checkbox" id="dog" name="dog" value="Dog"> <label for="dog">I like dogs</label>` | Checkboxes for selecting favorite pets (e.g., dogs, cats). |
| **Radio** | Allows the user to select one option from a group. | `<input type="radio" id="light" name="theme" value="Light"> <label for="light">Light</label>` | Radio buttons for selecting a theme (e.g., Light, Dark). |
| **Submit** | Submits all form values to a specified URL or server. | `<form action="myserver.com" method="POST"> <input type="submit" value="Submit" /></form>` | A form submission button. |
| **Text** | Single-line text input field. | `<label for="fname">First name:</label> <input type="text" id="fname" name="fname">` | Input field for a user's first name. |
| **Password** | Text input field where characters are obscured. | `<label for="pwd">Password:</label> <input type="password" id="pwd" name="pwd">` | Password input field. |
| **Date** | Input field for selecting a date. | `<label for="dob">Date of birth:</label> <input type="date" id="dob" name="dob">` | Input field for selecting a date of birth. |
| **Datetime-local** | Input field for selecting both date and time. | `<label for="birthdaytime">Birthday (date and time):</label> <input type="datetime-local" id="birthdaytime" name="birthdaytime">` | Input for selecting a date and time for an event. |
| **Email** | Input field specifically for email addresses with built-in validation. | `<label for="email">Enter your email:</label> <input type="email" id="email" name="email">` | Input for collecting an email address. |
| **File** | Allows the user to select and upload a file. | `<label for="myfile">Select a file:</label> <input type="file" id="myfile" name="myfile">` | File upload input for attaching a document. |
| **Hidden** | Stores data without displaying it on the webpage. | `<input type="hidden" id="custId" name="custId" value="3487">` | Hidden field for passing user ID to the server. |
| **Image** | Displays an image that functions as a submit button. | `<input type="image" src="submit_img.png" alt="Submit" width="48" height="48">` | Image-based submit button. |
| **Number** | Input field for numbers with optional restrictions like min/max values. | `<input type="number" id="quantity" name="quantity" min="1" max="5">` | Input for selecting a quantity between 1 and 5. |
| **Range** | Displays a slider for selecting a number within a range. | `<label for="volume">Volume:</label> <input type="range" id="volume" name="volume" min="0" max="10">` | Slider for adjusting volume level. |
| **Reset** | Resets all form fields to their default values. | `<input type="reset">` | Reset button for clearing a form. |
| **Search** | Input field for entering a search query, often styled differently by browsers. | `<label for="gsearch">Search in Google:</label> <input type="search" id="gsearch" name="gsearch">` | Search box for querying Google. |
| **Time** | Input field for selecting a time (hours and minutes). | `<label for="appt">Select a time:</label> <input type="time" id="appt" name="appt">` | Time input for scheduling an appointment. |
| **Tel** | Input field for telephone numbers with optional validation. | `<label for="phone">Enter your phone number:</label> <input type="tel" id="phone" name="phone" pattern="[+]{1}[0-9]{11,14}">` | Phone number input with validation for format. |
| **Url** | Input field for URLs with built-in validation. | `<label for="homepage">Add your homepage:</label> <input type="url" id="homepage" name="homepage">` | URL input field for entering a website address. |
| **Week** | Input field for selecting a specific week and year. | `<label for="week">Select a week:</label> <input type="week" id="week" name="week">` | Input for selecting a specific week of the year. |
| **Month** | Input field for selecting a month and year. | `<label for="month">Select a month:</label> <input type="month" id="month" name="month">` | Input for selecting a month and year (e.g., for billing cycle). |

This table provides a quick reference for choosing the appropriate HTML input type based on your use case, along with simple examples for each.

- POST improves data security of the forms
- name attribute for input element acts as the key for the value submitted to the server
- the label element is associated with the corresponding input field by using the same value for attribute for in label that was used for the id in the input tag
- Pseudo Class Selectors in CSS select elements based on their state
- The fieldset element defines a group for the radio buttons
- The name in input matches with the id of fieldset

```
            <fieldset id="size">
                <input type="radio"  value="2" name="size">
            </fieldset>
```

| **Attribute** | **Description** | **Example** |
| --- | --- | --- |
| **Required** | Ensures the user cannot leave the input field empty. Useful for any input type (e.g., text, password, radio). | `<input type="text" id="firstName" name="firstName" required>` |
| **Maxlength** | Limits the maximum number of characters a user can enter in a text field. | `<input type="text" id="description" name="description" maxlength="50">` |
| **Minlength** | Sets the minimum number of characters required for a text input field. | `<input type="password" id="password" name="password" minlength="8">` |
| **Min/Max** | Defines the minimum and maximum values allowed for numeric, range, or date inputs. | `<input type="number" id="quantity" name="quantity" min="1" max="10">`<br>`<input type="range" id="volume" name="volume" min="1" max="100">` |
| **Multiple** | Allows the user to select or input multiple values in a single field, applicable for email and file types. | `<input type="file" id="gallery" name="gallery" multiple>` |
| **Pattern** | Validates the input based on a specific regular expression pattern. Works with text, date, search, URL, tel, email, and password fields. | `<input type="tel" id="phone" name="phone" pattern="^(?:0 |

# Calendar, Range, Data List : Type values for input

- Date, week and month are valid input types, Year is not.

# Sending Data to server

- data can be sent as a part of http request
- using http get and post method specified using the method attribute of form element
- Get: when submitted the login data is sent as a part of the request url: i.e. user data appended at the end of the url in the navigation bar, server gets the data and extracts the data from the url
    - Problems
        - The url length is limited upto around 2000 char depending upon what browser youre using
        - The url length is limited by some web servers
        - Security Threats: data stored in history
- Post: when submitted the form data is entered into the http request, it will send an http post request with the info in the body of the post req
    - More Secure than get but data can still be read by a third party listening to http req
- To secure this completely https is used to secure the data
- Form submissions are a crucial part of the internet. Almost every website uses forms, whether you're buying items online or ordering food for delivery. For example, when you click the login button on a website, it sends your username and password to a web server to log you into your account.
- To add a form to your webpage, you use the `<form>` tag:

```html
<form>
</form>

```

However, how the form is submitted depends on two key attributes: **action** and **method**.

- The **action** attribute specifies the web address (URL) where the form data will be sent. This address points to the server-side code that will process the request.

```html
<form action="/login">
</form>

```

- The **action** can be a full URL (like `https://meta.com`), an absolute path (like `/login`), or a relative path (like `login`).

### Absolute Path:

- An absolute path starts with a forward slash (`/`) and is combined with the base address of the current website.
- For instance, if the absolute path is `/login`, and the base address is `https://meta.com`, the form will be submitted to `https://meta.com/login`.
- Even if the current page is `https://meta.com/company-info/`, the submission address will still be `https://meta.com/login`.

### Relative Path:

- A relative path doesn't start with a forward slash and is combined with the current web page's address.
- For example, if the current page is `https://meta.com/company-info/`, and the relative path is `login`, the form will be submitted to `https://meta.com/company-info/login`.

This distinction is important for directing form submissions to the correct location on your server.

- Default method is get when not specified

# Inconsistency between the way forms are displayed on different browser

- solved using css

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Input</title>
    <style>
        input[type="text"],
        input[type="email"] {
            font-size: 14px;
            width: 200px;
            height: 30px;
            border: 1px solid #ccc;
            padding: 5px;
        }
    </style>
</head>
<body>

<form>
    <input type="text" placeholder="Name">
    <input type="email" placeholder="Email">
</form>

</body>
</html>

```

# Glossary: HTML form elements

| **Element** | **Description** | **Example Code** |
| --- | --- | --- |
| `<input>` | Used to create interactive controls, such as buttons and text fields, to accept input from the user. The `type` attribute defines the input type (e.g., `text`, `password`, `email`, etc.). | `html <form action="my_action_page"> <label for="uname">Username:</label><br> <input type="text" id="uname" name="username"><br> <label for="pwd">Password:</label><br> <input type="password" id="pwd" name="pwd"><br><br> </form>` |
| `<label>` | Defines a label for an element. The `for` attribute associates the label with a specific element by matching its `id` attribute. | `html <label for="uname">Username:</label> <input type="text" id="uname" name="username">` |
| `<select>` | Defines a drop-down list of options. Common attributes include `form`, `name`, `multiple`, `required`, and `size`. Options are defined using the `<option>` element inside `<select>`. | `html <label for="course">Choose a course:</label><br> <select id="course" name="courselist"> <option value="html">HTML Introduction</option> <option value="css">Styling with CSS</option> <option value="js">JavaScript</option> <option value="react">React Basics</option> </select>` |
| `<textarea>` | Defines a multi-line input field for longer textual data. Common attributes include `cols`, `form`, `maxlength`, `minlength`, `readonly`, and `rows`. | `html <textarea name="response" rows="10" cols="30" maxlength="200"></textarea>` |
| `<button>` | Defines a clickable button. The `onclick` attribute specifies behavior when the button is clicked. | `html <button type="button" onclick="alert('You just clicked!')">Click Me!</button>` |
| `<fieldset>` | Used to group related input elements in a form. For example, grouping elements related to personal information and educational qualifications separately. | `html <fieldset> <legend>Personal Info</legend> <label for="fname">First name:</label><br> <input type="text" id="fname" name="fname" value="John"><br> <label for="lname">Last name:</label><br> <input type="text" id="lname" name="lname" value="Doe"><br> </fieldset>` |
| `<legend>` | Defines a caption for the `<fieldset>` element. | `html <legend>Personal Info</legend>` |
| `<datalist>` | Specifies a list of predefined options for an input element. Unlike `<select>`, the user can still provide input other than the listed options. | `html <label for="flowers">Favourite flower:</label><br> <input list="flowers" name="flowers"> <datalist id="flowers"> <option value="Rose"> <option value="Lily"> <option value="Tulip"> <option value="Daffodil"> <option value="Orchid"> </datalist>` |
| `<output>` | Represents the result of a calculation or the outcome of a user action. | `html <output name="result"></output>` |
| `<option>` | Defines an option in a drop-down list. To define a pre-selected option, use the `selected` attribute. | `html <option value="html">HTML Introduction</option> <option value="css">Styling with CSS</option> <option value="js">JavaScript</option> <option value="react">React Basics</option>` |
| `<optgroup>` | Defines a group of related options in a drop-down list. The `label` attribute names the group. | `html <optgroup label="Frontend"> <option value="html">HTML Introduction</option> <option value="css">Styling with CSS</option> <option value="js">JavaScript</option> </optgroup>` |

This table provides a quick reference to various HTML form elements along with code snippets that illustrate their usage.

# Audio And Video Tags

- **HTML Video and Audio Tags**:
    - **Purpose**: Embeds media on a webpage.
    - **Supported File Types**:
        - **Video**: MP4, WebM, OGG
        - **Audio**: MP3, WAV, OGG
- **Using the `<video>` Tag**:
    - **Basic Structure**:
        
        ```html
        <video>
          <source src="dance.mp4" type="video/mp4">
        </video>
        
        ```
        
    - **Attributes**:
        - `src`: Specifies the address of the video file (e.g., `dance.mp4`).
        - `type`: Specifies the file type (e.g., `video/mp4` for MP4 files).
        - **Customizing the Video Player**:
            - `width`: Sets the width of the player.
            - `height`: Sets the height of the player.
            - `controls`: Enables player controls like pause and volume buttons.
        - **Multiple Sources**: You can provide multiple `<source>` elements. The browser will use the first supported format.
- **Using the `<audio>` Tag**:
    - **Basic Structure**:
        
        ```html
        <audio>
          <source src="music.mp3" type="audio/mpeg">
        </audio>
        
        ```
        
    - **Attributes**:
        - `src`: Specifies the address of the audio file (e.g., `music.mp3`).
        - `type`: Specifies the file type (e.g., `audio/mpeg` for MP3 files).
        - **Customizing the Audio Player**:
            - `controls`: Enables player controls like pause and volume buttons.
- **Fallback and Compatibility**:
    - If a file type isn’t supported, the browser will attempt to use the next specified source.
    - Always specify sources in a preferred order to ensure compatibility.
- **Further Customization**:
    - Additional attributes are available for more customization, which will be covered in future content.

This summary should help you understand how to use and customize video and audio elements on your webpage.

# Iframe SandBox

Here's a concise cheat sheet for the `<iframe>` element with a focus on its attributes and their usage:

### `<iframe>` Cheat Sheet

- **`allow`**: Specifies features or permissions available to the frame.
    - Example:
        
        ```html
        <iframe src="<https://example.com/>" allow="camera; microphone"></iframe>
        
        ```
        
    - Permissions:
        - `fullscreen`: Enables fullscreen mode.
        - `geolocation`: Accesses the user’s location.
        - Multiple permissions are separated by semicolons.
- **`name`**: Defines a name for the `<iframe>`.
    - Example:
        
        ```html
        <iframe name="My Frame" width="400" height="300"></iframe>
        
        ```
        
- **`height`**: Sets the height of the frame in CSS pixels. Default is 150 pixels.
    - Example:
        
        ```html
        <iframe src="example.html" height="400"></iframe>
        
        ```
        
- **`width`**: Sets the width of the frame in CSS pixels. Default is 300 pixels.
    - Example:
        
        ```html
        <iframe src="example.html" width="600"></iframe>
        
        ```
        
- **`referrerpolicy`**: Determines which referrer information is sent when loading the frame resource.
    - Values:
        - `no-referrer`: No referrer header sent.
        - `origin`: Referrer limited to the origin.
        - `strict-origin`: Referrer sent only with same protocol security level.
    - Example:
        
        ```html
        <iframe src="example.html" referrerpolicy="origin"></iframe>
        
        ```
        
- **`sandbox`**: Applies extra restrictions for security; specific permissions can be lifted with permission tokens.
    - Permission Tokens:
        - `allow-downloads`: Allows downloads.
        - `allow-forms`: Allows form submission.
        - `allow-modals`: Allows opening modal windows.
        - `allow-orientation-lock`: Allows screen orientation lock.
        - `allow-popups`: Allows popups.
        - `allow-presentation`: Allows presentation sessions.
        - `allow-scripts`: Allows scripts to run.
    - Example:
        
        ```html
        <iframe src="my_iframe_sandbox.html" sandbox="allow-forms allow-scripts"></iframe>
        
        ```
        
- **`src`**: URL of the page to embed. `about:blank` embeds an empty page.
    - Example:
        
        ```html
        <iframe src="example.html"></iframe>
        
        ```
        
- **`srcdoc`**: Specifies inline HTML to embed in the `<iframe>`, overriding `src`.
    - Example:
        
        ```html
        <iframe src="my_iframe_src.html" srcdoc="<p>My inline html</p>"></iframe>
        
        ```
        
- **`loading`**: Specifies when the iframe should be loaded. Options are `eager` (immediately) or `lazy` (when displayed).
    - Example:
        
        ```html
        <iframe src="my_iframe_src.html" loading="lazy"></iframe>
        
        ```
        
- **`title`**: Adds a description for accessibility purposes.
    - Example:
        
        ```html
        <iframe src="history.html" title="An embedded document about the history of my family"></iframe>
        
        ```
        

This cheat sheet provides a quick reference for using and customizing `<iframe>` elements in HTML.

# CSS

- display property specifiesrty spcifies the type of box you want to use for your html element
- display: flex, grid, block, inline
- Flexbox is 1D whereas grid is 2D
- Flexbox: flexible box mode, adds resposnsiveness

# Flex Box

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ac72945-7719-4461-a74f-b6f343ba6e50/e6cbc178-b4bb-46c8-becd-f435314d1eba/Untitled.png)

Here’s a simplified overview of Flexbox:

- **Flexbox Overview**:
    - **Single-Dimensional Layout**: Aligns items along either a row (horizontal) or column (vertical).
    - **Default Alignment**: Horizontal (row).
- **Axes**:
    - **Main Axis**:
        - Default is horizontal when flex-direction is set to row.
        - Can be vertical if flex-direction is set to column.
    - **Cross Axis**:
        - Perpendicular to the main axis.
        - Default is vertical when flex-direction is row.
        - Becomes horizontal if flex-direction is column.
- **Item Placement**:
    - Items start from the top-left corner.
    - Fill the main axis first.
    - Continue to the next row or column when the current one is filled.
- **Flex Direction**:
    - **Row (default)**: Main axis is horizontal.
        
        ```css
        .container {
          display: flex;
          flex-direction: row;
        }
        
        ```
        
    - **Column**: Main axis is vertical.
        
        ```css
        .container {
          display: flex;
          flex-direction: column;
        }
        
        ```
        
- **Properties**:
    - **Alignment**: Control alignment and spacing of items.
    - **Direction**: Define the direction of the main axis (row or column).

Flexbox properties help you control the alignment, spacing, and styling of flex container and items effectively.

# Align items

Here are code snippets demonstrating how to use each of the main alignment properties in Flexbox:

### 1. `justify-content`

Aligns flex items along the main axis (horizontal by default).

- **Values**:
    - `flex-start` (default): Align items at the start of the main axis.
    - `flex-end`: Align items at the end of the main axis.
    - `center`: Align items in the center of the main axis.
    - `space-between`: Distribute items with space between them.
    - `space-around`: Distribute items with space around them.
    - `space-evenly`: Distribute items with equal space between them.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>justify-content Example</title>
    <style>
        .container {
            display: flex;
            height: 100px;
            border: 2px solid #000;
        }
        .item {
            width: 50px;
            height: 50px;
            background-color: lightblue;
            margin: 5px;
        }
        .center {
            justify-content: center; /* Align items in the center */
        }
        .space-between {
            justify-content: space-between; /* Distribute items with space between them */
        }
    </style>
</head>
<body>
    <div class="container center">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
    </div>
    <div class="container space-between">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
    </div>
</body>
</html>

```

### 2. `align-items`

Aligns flex items along the cross axis (vertical by default).

- **Values**:
    - `stretch` (default): Stretch items to fill the container.
    - `flex-start`: Align items at the start of the cross axis.
    - `flex-end`: Align items at the end of the cross axis.
    - `center`: Align items in the center of the cross axis.
    - `baseline`: Align items along their baseline.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>align-items Example</title>
    <style>
        .container {
            display: flex;
            height: 200px;
            border: 2px solid #000;
        }
        .item {
            width: 50px;
            height: 50px;
            background-color: lightgreen;
            margin: 5px;
        }
        .center {
            align-items: center; /* Align items in the center of the cross axis */
        }
        .flex-start {
            align-items: flex-start; /* Align items at the start of the cross axis */
        }
    </style>
</head>
<body>
    <div class="container center">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
    </div>
    <div class="container flex-start">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
    </div>
</body>
</html>

```

### 3. `align-self`

Aligns a single flex item along the cross axis, overriding `align-items`.

- **Values**:
    - `auto` (default): Inherits alignment from `align-items`.
    - `flex-start`: Align item at the start of the cross axis.
    - `flex-end`: Align item at the end of the cross axis.
    - `center`: Align item in the center of the cross axis.
    - `baseline`: Align item along its baseline.
    - `stretch`: Stretch item to fill the container.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>align-self Example</title>
    <style>
        .container {
            display: flex;
            height: 200px;
            border: 2px solid #000;
            align-items: flex-end; /* Default alignment for all items */
        }
        .item {
            width: 50px;
            height: 50px;
            background-color: lightcoral;
            margin: 5px;
        }
        .align-center {
            align-self: center; /* Override alignment for this item */
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item"></div>
        <div class="item align-center"></div>
        <div class="item"></div>
    </div>
</body>
</html>

```

### 4. `align-content`

Aligns flex lines within the flex container when there is extra space on the cross axis.

- **Values**:
    - `stretch` (default): Stretch lines to fill the container.
    - `flex-start`: Align lines at the start of the cross axis.
    - `flex-end`: Align lines at the end of the cross axis.
    - `center`: Align lines in the center of the cross axis.
    - `space-between`: Distribute lines with space between them.
    - `space-around`: Distribute lines with space around them.
    - `space-evenly`: Distribute lines with equal space between them.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>align-content Example</title>
    <style>
        .container {
            display: flex;
            flex-wrap: wrap;
            height: 400px;
            border: 2px solid #000;
        }
        .item {
            width: 100px;
            height: 100px;
            background-color: lightgoldenrodyellow;
            margin: 5px;
        }
        .space-between {
            align-content: space-between; /* Distribute lines with space between them */
        }
        .center {
            align-content: center; /* Align lines in the center of the cross axis */
        }
    </style>
</head>
<body>
    <div class="container space-between">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
    </div>
    <div class="container center">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
    </div>
</body>
</html>

```

These snippets should help you understand and apply the different alignment properties in Flexbox.

# FlexBox

Here’s a structured breakdown of Flexbox concepts and properties along with code snippets:

### Understanding Flexbox

- **Flexbox Container**: A flexible box layout system in CSS.
- **Single-Dimensional**: Aligns items along a single axis (row or column).
- **Default Axis**: Row alignment (horizontal axis as the main axis).

### Main and Cross Axis:

- **Main Axis**: Horizontal axis by default (controlled by `flex-direction`).
- **Cross Axis**: Vertical axis (perpendicular to the main axis).

### Flexbox Properties

1. **Basic Setup**:
    - **HTML**:
        
        ```html
        <body>
          <div class="flex-container">
            <div class="box box1">One..</div>
            <div class="box box2">Two..</div>
            <div class="box box3">Three..</div>
            <div class="box box4">Four..</div>
            <div class="box box5">Five..</div>
            <div class="box box6">Six..</div>
            <div class="box box7">Seven..</div>
          </div>
        </body>
        
        ```
        
    - **CSS**:
        
        ```css
        .box {
            background-color: aquamarine;
            border-radius: 5px;
            margin: 2px;
            padding: 10px;
        }
        
        ```
        
2. **Turning Container into Flexbox**:
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
        }
        
        ```
        
    - **Output**: Items align from left to right in a row.
3. **Align Items Along Main Axis** (`justify-content`):
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
            justify-content: center; /* Center items horizontally */
        }
        
        ```
        
    - **Output**: Items centered horizontally.
4. **Wrapping Items** (`flex-wrap`):
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap; /* Allows items to wrap to the next line */
        }
        
        ```
        
    - **Output**: Items wrap onto multiple lines.
5. **Changing Main Axis Direction** (`flex-direction`):
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
            flex-direction: column; /* Align items vertically */
            justify-content: center;
            flex-wrap: wrap;
        }
        
        ```
        
    - **Output**: Items align vertically in columns.
6. **Align Items on Cross Axis** (`align-items`):
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
            justify-content: center;
            flex-direction: column;
            flex-wrap: wrap;
            align-items: flex-end; /* Align items to the end (bottom) */
        }
        
        ```
        
    - **Output**: Items aligned to the bottom of the container.
7. **Align Specific Item** (`align-self`):
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
            justify-content: center;
            flex-direction: column;
            flex-wrap: wrap;
            align-items: flex-end;
        }
        .box3 {
            background-color: blanchedalmond;
            align-self: center; /* Align this item to the center on cross axis */
        }
        
        ```
        
    - **Output**: `box3` is centered while others are aligned to the bottom.
8. **Spacing Between Items** (`gap`):
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
            justify-content: center;
            flex-direction: column;
            flex-wrap: wrap;
            align-items: flex-end;
            gap: 10px; /* Space between items */
        }
        
        ```
        
    - **Output**: Increased spacing between items.
9. **Flex Growth, Shrink, and Basis** (`flex` shorthand):
    - **CSS**:
        
        ```css
        .flex-container {
            display: flex;
            flex-direction: row;
            justify-content: center;
        }
        .box3 {
            background-color: blanchedalmond;
            flex: 1 1 auto; /* Flex-grow: 1, Flex-shrink: 1, Flex-basis: auto */
        }
        
        ```
        
    - **Output**: `box3` takes up available space in the container.

### Key Takeaways:

- **`align-items`**: Aligns items within a single line on the cross axis.
- **`align-content`**: Aligns flex lines within the container, controlling the spacing between lines.

### Flexbox Diagram

Here’s a visual reference for the flexbox properties:

- **Flex Container**: Defines the flex container.
- **Main Axis**: Horizontal or vertical based on `flex-direction`.
- **Cross Axis**: Perpendicular to the main axis.
- **Flex Items**: Items inside the container affected by properties like `align-items`, `justify-content`, etc.

This breakdown and visualization should help you understand the flexibility and alignment properties within Flexbox.

# CSS Units of Measurement

CSS units of measurement help define the size and spacing of elements on a web page. They can be categorized into **Absolute Units** and **Relative Units**, each serving different purposes based on the context and requirements of the web design.

---

### Absolute Units

Absolute units have a fixed size and do not change based on other elements or viewport size. They are often used for print styles or when a fixed size is necessary.

| Unit | Name | Comparison |
| --- | --- | --- |
| `Q` | Quarter-millimeters | 1Q = 1/40th of 1cm |
| `mm` | Millimeters | 1mm = 1/10th of 1cm |
| `cm` | Centimeters | 1cm = 37.8px = 25.2/64in |
| `in` | Inches | 1in = 2.54cm = 96px |
| `pc` | Picas | 1pc = 1/6th of 1in |
| `pt` | Points | 1pt = 1/72nd of 1in |
| `px` | Pixels | 1px = 1/96th of 1in |

**Commonly Used Absolute Units:**

- **Pixels (`px`)**: Most frequently used for screen sizes.
- **Centimeters (`cm`)**: Used when specific physical measurements are needed.

---

### Relative Units

Relative units are based on the size of other elements or the viewport. They provide more flexibility and adapt to different screen sizes and resolutions.

| Unit | Description | Relativity |
| --- | --- | --- |
| `em` | Font size of the parent element | Scales with the font size of the parent element |
| `ex` | Height of the font's "x" character | Related to the font's x-height |
| `ch` | Width of the "0" character | Useful for aligning text |
| `rem` | Font size of the root element (`<html>`) | Scales with the root font size |
| `lh` | Line height of the parent element | Based on the line height of the parent |
| `rlh` | Line height of the root element | Based on the line height of the root |
| `vw` | 1% of the viewport width | Relative to the width of the viewport |
| `vh` | 1% of the viewport height | Relative to the height of the viewport |
| `vmin` | 1% of the smaller dimension of the viewport | Minimum of viewport width or height |
| `vmax` | 1% of the larger dimension of the viewport | Maximum of viewport width or height |
| `%` | Percentage of the parent element's size | Relative to the size of the parent element |

**Commonly Used Relative Units:**

- **Percentage (`%`)**: Used for widths, heights, and other dimensions relative to the parent.
- **Viewport Width (`vw`)** and **Viewport Height (`vh`)**: Useful for responsive designs.
- **`em`** and **`rem`**: Primarily used for font sizes and spacing in relation to font sizes.

---

### Example Code Snippets

**Using Absolute Units:**

```css
.fixed-size {
    width: 200px;   /* Fixed width in pixels */
    height: 10cm;   /* Fixed height in centimeters */
}

```

**Using Relative Units:**

```css
.relative-size {
    font-size: 2em;    /* Font size relative to the parent element's font size */
    width: 50vw;       /* Width relative to the viewport width */
    height: 50vh;      /* Height relative to the viewport height */
    margin: 5%;        /* Margin relative to the parent element's size */
}

```

---

### Choosing the Right Unit

- **Absolute Units**: Best for fixed dimensions or print design.
- **Relative Units**: Ideal for responsive designs and adapting to different screen sizes.

Understanding when and how to use these units effectively will help you create flexible, responsive web designs that work well across various devices and screen sizes.

# Creating Bar Charts with Flexbox

Using Flexbox to create bar charts is a great way to visualize data using CSS. Flexbox provides a flexible layout model that allows for responsive and dynamic data representations. Here’s a step-by-step guide on how to create vertical and horizontal bar charts using Flexbox:

### 1. **HTML Structure**

Start by setting up the basic HTML structure for your bar chart. For this example, let's assume you're creating a chart for a restaurant survey.

**`flex-charts.html`:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Bar Charts</title>
    <link rel="stylesheet" href="flex-charts.css">
</head>
<body>
    <div class="row">
        <div class="label">Preferred Dishes</div>
        <div class="container">
            <div class="dish item-pasta">
                <span class="percentage">35%</span>
            </div>
            <div class="dish item-pizza">
                <span class="percentage">50%</span>
            </div>
            <div class="dish item-burrito">
                <span class="percentage">15%</span>
            </div>
        </div>
    </div>
    <div class="columns">
        <div class="container">
            <div class="bar bar-male">
                <span class="percentage">60%</span>
            </div>
            <div class="bar bar-female">
                <span class="percentage">40%</span>
            </div>
        </div>
    </div>
</body>
</html>

```

### 2. **CSS Styling**

Add CSS to style the bar charts using Flexbox.

**`flex-charts.css`:**

```css
/* General styles */
body {
    font-family: Arial, sans-serif;
}

/* Row container for horizontal bar chart */
.row {
    display: flex;
    align-items: stretch;
    margin-bottom: 20px;
}

.row .label {
    flex: 0 0 200px; /* Fixed width for label */
    padding: 10px;
    font-weight: bold;
}

.row .container {
    display: flex;
    justify-content: flex-start; /* Align items to the start */
    flex: 1;
}

.dish {
    flex: 1;
    margin: 0 5px;
    position: relative;
}

.dish .percentage {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: #fff;
}

/* Specific colors for dishes */
.item-pasta {
    background-color: #ff6f61;
    flex-basis: 35%;
}

.item-pizza {
    background-color: #ffca28;
    flex-basis: 50%;
}

.item-burrito {
    background-color: #4caf50;
    flex-basis: 15%;
}

/* Columns container for vertical bar chart */
.columns {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.columns .container {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.bar {
    width: 100px;
    margin: 5px;
    position: relative;
    text-align: center;
}

.bar .percentage {
    position: absolute;
    bottom: 10px;
    width: 100%;
}

/* Specific colors for bars */
.bar-male {
    background-color: #2196f3;
    height: 60%;
}

.bar-female {
    background-color: #e91e63;
    height: 40%;
}

```

### 3. **Explanation of CSS Properties**

- **`.row`**: Creates a flex container for horizontal bars. `align-items: stretch` ensures that the bars stretch to the same height as the container.
- **`.dish`**: Represents each bar in the horizontal chart. `flex-basis` sets the width of each bar relative to the total container width.
- **`.columns`**: Creates a flex container for vertical bars. `flex-direction: column` stacks bars vertically.
- **`.bar`**: Represents each bar in the vertical chart. `height` specifies the height relative to the container.

### 4. **Visual Output**

- The **horizontal bar chart** shows the percentage for each dish with different colors.
- The **vertical bar chart** displays percentages for male and female with different heights.

### Conclusion

Flexbox is a powerful tool for creating bar charts and other data visualizations with CSS. By using Flexbox properties like `flex-grow`, `flex-shrink`, and `flex-basis`, you can dynamically adjust the size and layout of elements to represent data effectively. Experimenting with different Flexbox properties will help you master data visualization using CSS.

# Grid

### Overview of CSS Grid Layouts

CSS Grid layouts are essential for creating well-structured and responsive web page designs. Grids divide a page into rows and columns, making it easier to organize content. This guide will walk you through setting up and customizing a grid layout using CSS.

### 1. **Setting Up the HTML Document**

Create an HTML file called `index.html` with the following content:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Grid Layout Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <div class="box">A</div>
        <div class="box">B</div>
        <div class="box">C</div>
        <div class="box">D</div>
        <div class="box">E</div>
    </div>
</body>
</html>

```

### 2. **Basic Grid Setup in CSS**

Create a CSS file called `styles.css` and define the initial grid properties:

```css
/* Container is a grid */
.container {
    display: grid; /* Set the container to use grid layout */
    grid-template-columns: 100px 100px 100px; /* Define three columns of 100px each */
    grid-template-rows: 100px 100px; /* Define two rows of 100px each */
    gap: 10px; /* Set a 10px gap between grid items */
    background-color: red; /* Set background color for better visualization */
}

/* Style for individual grid items */
.box {
    background-color: lightblue; /* Background color for each grid item */
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%; /* Ensure the item height fills the grid cell */
    font-size: 20px;
}

```

### 3. **Using Fraction Units**

You can use fractional units to define grid sizes:

```css
/* Updated container with fractional units */
.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr; /* Define three columns with equal width using fractions */
    grid-template-rows: 2fr 1fr; /* Define two rows with proportional height */
    gap: 10px; /* Gap between grid items */
    background-color: red; /* Background color for visualization */
}

```

### 4. **Grid Auto Rows**

Adjust the rows' size automatically:

```css
/* Use auto-sizing for rows */
.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr; /* Three columns */
    grid-auto-rows: 100px; /* Automatically set row height to 100px */
    gap: 10px;
    background-color: red;
}

```

### 5. **Using `repeat()` Function**

The `repeat()` function simplifies repetitive code:

```css
/* Use repeat function to define grid columns */
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* Repeat 1fr column definition three times */
    grid-template-rows: repeat(2, 100px); /* Repeat 100px row definition twice */
    gap: 10px;
    background-color: red;
}

```

### 6. **Using `minmax()` Function**

Set minimum and maximum values for grid sizes:

```css
/* Use minmax function to define flexible grid sizes */
.container {
    display: grid;
    grid-template-columns: repeat(3, minmax(100px, 1fr)); /* Columns with min 100px, max 1fr */
    grid-template-rows: repeat(2, minmax(150px, auto)); /* Rows with min 150px, auto for maximum */
    gap: 10px;
    background-color: red;
}

```

### 7. **Grid Frameworks**

Common grid frameworks include the 12-column and 16-column grids:

- **12-Column Grid**: Often used for flexible layouts.
- **16-Column Grid**: Provides more precise control.

Example for a 12-column grid:

```css
/* Define a 12-column grid */
.container {
    display: grid;
    grid-template-columns: repeat(12, 1fr); /* 12 columns with equal width */
    gap: 10px;
    background-color: red;
}

```

### Summary

- **CSS Grid Layouts**: Divide your page into rows and columns, providing a structured layout.
- **Fraction Units (`fr`)**: Allows flexible column and row sizing.
- **`repeat()` Function**: Reduces redundancy by repeating grid definitions.
- **`minmax()` Function**: Sets minimum and maximum sizes for grid items.
- **Grid Frameworks**: Use predefined column structures like 12 or 16 columns for consistent layouts.

Understanding and using CSS Grid effectively can greatly enhance your ability to design complex and responsive web layouts.

# Grid Flexbox Cheatsheet

### **CSS Grid**

**Syntax for Creating a Grid:**

```css
selector {
    display: grid; /* or inline-grid */
}

```

**Grid Shorthand Properties:**

- **grid-template-rows:** Defines the number of rows and their sizes.
    
    ```css
    grid-template-rows: none; /* Can be specified as measurement units, % units, or repeat() */
    
    ```
    
- **grid-template-columns:** Defines the number of columns and their sizes.
    
    ```css
    grid-template-columns: none; /* Can be specified as measurement units, % units, or repeat() */
    
    ```
    
- **grid-template-areas:** Defines named areas in the grid.
    
    ```css
    grid-template-areas: none; /* Can be defined using area names and grid lines */
    
    ```
    
- **grid-auto-rows:** Default size for rows not explicitly set.
    
    ```css
    grid-auto-rows: auto; /* Can be set to specific measurement units */
    
    ```
    
- **grid-auto-columns:** Default size for columns not explicitly set.
    
    ```css
    grid-auto-columns: auto; /* Can be set to specific measurement units */
    
    ```
    
- **grid-auto-flow:** Determines placement of items in the grid.
    
    ```css
    grid-auto-flow: row; /* Alternatives: column | dense */
    
    ```
    
- **column-gap:** Sets the gap between columns.
    
    ```css
    column-gap: normal; /* Can be set to specific measurement units */
    
    ```
    
- **row-gap:** Sets the gap between rows.
    
    ```css
    row-gap: normal; /* Can be set to specific measurement units */
    
    ```
    

**Grid Properties for Container:**

- **grid-template-columns:** Defines column sizes and names.
    
    ```css
    grid-template-columns: measurement units | % units | repeat(); /* Example: repeat(3, 1fr) */
    
    ```
    
- **grid-template-rows:** Defines row sizes and names.
    
    ```css
    grid-template-rows: measurement units | % units | repeat(); /* Example: repeat(2, 100px) */
    
    ```
    
- **grid-auto-columns:** Default column size for implicit grid columns.
    
    ```css
    grid-auto-columns: measurement units; /* Example: 100px */
    
    ```
    
- **grid-auto-rows:** Default row size for implicit grid rows.
    
    ```css
    grid-auto-rows: measurement units; /* Example: 100px */
    
    ```
    
- **grid-template:** Shorthand to define grid areas.
    
    ```css
    grid-template: "header header" auto /* Example with row heights: "main right" 75vh */
    
    ```
    

**Gap Properties:**

- **grid-gap:** Sets both row and column gaps.
    
    ```css
    grid-gap: measurement units; /* Example: 10px */
    
    ```
    
- **grid-column-gap:** Sets the gap between columns.
    
    ```css
    grid-column-gap: measurement units; /* Example: 10px */
    
    ```
    
- **grid-row-gap:** Sets the gap between rows.
    
    ```css
    grid-row-gap: measurement units; /* Example: 10px */
    
    ```
    

**Alignment Properties:**

- **justify-items:** Aligns items along the inline axis.
    
    ```css
    justify-items: start | center | end | stretch;
    
    ```
    
- **align-items:** Aligns items along the block axis.
    
    ```css
    align-items: start | center | end | stretch;
    
    ```
    
- **place-items:** Shorthand for `justify-items` and `align-items`.
    
    ```css
    place-items: start | stretch;
    
    ```
    

**Justification Properties:**

- **justify-content:** Aligns grid content along the main axis.
    
    ```css
    justify-content: start | center | end | stretch | space-between | space-evenly | space-around;
    
    ```
    
- **align-content:** Aligns grid content along the cross axis.
    
    ```css
    align-content: start | center | end | stretch | space-between | space-evenly | space-around;
    
    ```
    
- **place-content:** Shorthand for `justify-content` and `align-content`.
    
    ```css
    place-content: center | start;
    
    ```
    

**Positioning Properties:**

- **grid-auto-flow:** Controls automatic placement.
    
    ```css
    grid-auto-flow: row | column | dense;
    
    ```
    
- **grid-auto-columns:** Sets default size for columns created implicitly.
    
    ```css
    grid-auto-columns: measurement units; /* Example: 100px */
    
    ```
    
- **grid-auto-rows:** Sets default size for rows created implicitly.
    
    ```css
    grid-auto-rows: measurement units; /* Example: 100px */
    
    ```
    

**Grid Properties for Items (Children):**

- **grid-column:** Specifies the start and end positions for columns.
    
    ```css
    grid-column: column-start / column-end; /* Example: 1 / 3 */
    
    ```
    
- **grid-column-start:** Defines the starting column position.
    
    ```css
    grid-column-start: column-number | line-name; /* Example: 1 */
    
    ```
    
- **grid-column-end:** Defines the ending column position.
    
    ```css
    grid-column-end: column-number | line-name; /* Example: 3 */
    
    ```
    
- **grid-row:** Specifies the start and end positions for rows.
    
    ```css
    grid-row: row-start / row-end; /* Example: 1 / 2 */
    
    ```
    
- **grid-row-start:** Defines the starting row position.
    
    ```css
    grid-row-start: row-number | line-name; /* Example: 1 */
    
    ```
    
- **grid-row-end:** Defines the ending row position.
    
    ```css
    grid-row-end: row-number | line-name; /* Example: 2 */
    
    ```
    

**Justification and Alignment Properties for Items:**

- **justify-self:** Aligns an item within its grid area along the inline axis.
    
    ```css
    justify-self: start | center | end | stretch;
    
    ```
    
- **align-self:** Aligns an item within its grid area along the block axis.
    
    ```css
    align-self: start | center | end | stretch;
    
    ```
    
- **place-self:** Shorthand for `justify-self` and `align-self`.
    
    ```css
    place-self: start | stretch;
    
    ```
    

---

### **Flexbox**

**Syntax for Creating a Flexbox:**

```css
selector {
    display: flex; /* or inline-flex */
}

```

**Properties for Flexbox Container:**

- **flex-direction:** Defines the direction of flex items.
    
    ```css
    flex-direction: row | row-reverse | column | column-reverse;
    
    ```
    
- **flex-wrap:** Defines whether flex items should wrap.
    
    ```css
    flex-wrap: wrap | nowrap;
    
    ```
    
- **align-items:** Aligns flex items along the cross axis.
    
    ```css
    align-items: flex-start | flex-end | center | stretch;
    
    ```
    
- **justify-content:** Aligns flex items along the main axis.
    
    ```css
    justify-content: flex-start | flex-end | center | space-between | space-evenly | space-around;
    
    ```
    

**Properties for Flexbox Items (Children):**

- **flex-grow:** Defines the ability for a flex item to grow.
    
    ```css
    flex-grow: number; /* Example: 1 */
    
    ```
    
- **flex-shrink:** Defines the ability for a flex item to shrink.
    
    ```css
    flex-shrink: number; /* Example: 1 */
    
    ```
    
- **flex-basis:** Defines the initial size of a flex item.
    
    ```css
    flex-basis: auto | measurement unit; /* Example: 100px */
    
    ```
    
- **order:** Defines the order of flex items.
    
    ```css
    order: number; /* Example: 2 */
    
    ```
    
- **align-self:** Aligns a flex item within its flex container.
    
    ```css
    align-self: start | center | end | stretch;
    
    ```
    

By understanding and applying these properties, you can create complex and responsive layouts using CSS Grid and Flexbox.unit

# CSS Grid Template Areas

**Grid Template Areas** provide a way to name specific sections of a grid layout, making it easier to assign and manage those areas in your CSS. This technique helps in creating more readable and maintainable stylesheets by allowing you to use descriptive names for your grid areas.

### **How to Use Grid Template Areas**

**1. Define the Grid:**

Use the `display` property to define the element as a grid container.

```css
selector {
    display: grid; /* or inline-grid */
}

```

**2. Set Grid Dimensions:**

Define the height and width of the grid container if necessary.

```css
selector {
    height: 200px; /* Example height */
}

```

**3. Define Grid Template Areas:**

Assign names to different sections of your grid using the `grid-template-areas` property. These names will correspond to the areas you want to create.

```css
selector {
    grid-template-areas:
        "header header"
        "nav main"
        "footer footer";
}

```

**4. Define Row and Column Sizes:**

Specify the size of rows and columns using `grid-template-rows` and `grid-template-columns`.

```css
selector {
    grid-template-rows: 50px auto 30px; /* Example for three rows */
    grid-template-columns: 1fr 3fr; /* Example for two columns */
}

```

**5. Apply Styles to Named Areas:**

Use the names defined in `grid-template-areas` to style the specific grid areas.

```css
header {
    grid-area: header;
    background: lightblue;
}

nav {
    grid-area: nav;
    background: lightcoral;
}

main {
    grid-area: main;
    background: lightgreen;
}

footer {
    grid-area: footer;
    background: lightgoldenrodyellow;
}

```

### **Example**

**HTML Code:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid Template Areas Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>Header</header>
    <nav>Navigation</nav>
    <main>Main content</main>
    <footer>Footer</footer>
</body>
</html>

```

**CSS Code:**

```css
body {
    display: grid;
    grid-template-areas:
        "header header"
        "nav main"
        "footer footer";
    grid-template-rows: 50px auto 30px;
    grid-template-columns: 1fr 3fr;
    height: 100vh; /* Full viewport height */
}

header {
    grid-area: header;
    background: lightblue;
}

nav {
    grid-area: nav;
    background: lightcoral;
}

main {
    grid-area: main;
    background: lightgreen;
}

footer {
    grid-area: footer;
    background: lightgoldenrodyellow;
}

```

**Output:**

The layout will consist of:

- A **header** spanning two columns at the top.
- A **navigation** area in the first column.
- A **main content** area in the second column.
- A **footer** spanning two columns at the bottom.

**Changing Grid Template Areas:**

You can adjust the size of grid areas by modifying the `grid-template-areas` property. For example:

```css
body {
    grid-template-areas:
        "header header header"
        "nav main main"
        "footer footer footer";
}

```

This will make the `header` and `footer` span three columns, while `nav` and `main` will adjust according to the new layout.

### **Advantages**

- **Clarity:** Naming grid areas makes it easier to understand and manage complex layouts.
- **Maintainability:** Updates to the layout are easier to manage by modifying the names and sizes directly.
- **Flexibility:** Allows for a clear and flexible way to position and size elements within the grid.

By using grid template areas, you can create complex layouts with a clear and organized structure, making your CSS more readable and maintainable.

# Advanced CSS Selectors

### **1. Attribute Selectors**

**Overview:**
Attribute selectors allow you to select HTML elements based on their attributes and attribute values. This provides a way to target elements more precisely without adding additional classes or IDs.

**Syntax Variations:**

- **[attribute]**: Selects elements with the specified attribute, regardless of its value.
    
    ```css
    a[href] {
        color: blue;
    }
    
    ```
    
    Selects all `<a>` elements with an `href` attribute.
    
- **[attribute="value"]**: Selects elements with the specified attribute and exact value.
    
    ```css
    a[href="<https://example.com>"] {
        color: green;
    }
    
    ```
    
    Selects `<a>` elements with an `href` attribute exactly equal to "[https://example.com](https://example.com/)".
    
- **[attribute~="value"]**: Selects elements with an attribute containing a space-separated list of values, one of which is the specified value.
    
    ```css
    [class~="highlight"] {
        background-color: yellow;
    }
    
    ```
    
    Selects elements with a `class` attribute that includes the word "highlight".
    
- **[attribute|="value"]**: Selects elements with an attribute value that starts with the specified value followed by a hyphen.
    
    ```css
    [lang|="en"] {
        font-style: italic;
    }
    
    ```
    
    Selects elements with a `lang` attribute value that starts with "en", such as "en", "en-US", etc.
    
- **[attribute^="value"]**: Selects elements with an attribute value that starts with the specified value.
    
    ```css
    [href^="https://"] {
        color: red;
    }
    
    ```
    
    Selects `<a>` elements with an `href` attribute value starting with "https://".
    
- **[attribute$="value"]**: Selects elements with an attribute value that ends with the specified value.
    
    ```css
    [href$=".pdf"] {
        color: purple;
    }
    
    ```
    
    Selects `<a>` elements with an `href` attribute value ending in ".pdf".
    
- *[attribute="value"]*: Selects elements with an attribute value containing the specified value.
    
    ```css
    [href*="example"] {
        color: orange;
    }
    
    ```
    
    Selects `<a>` elements with an `href` attribute containing "example".
    

### **2. `nth-of-type` and `nth-child` Selectors**

**Overview:**
These selectors are used to select elements based on their position within a parent element.

- **`:nth-of-type(n)`**: Selects the nth child of its type within the parent.
    
    ```css
    ul li:nth-of-type(2) {
        color: aqua;
    }
    
    ```
    
    Selects the second `<li>` in each `<ul>`.
    
- **`:nth-child(n)`**: Selects the nth child of its parent, regardless of type.
    
    ```css
    ul li:nth-child(2) {
        color: pink;
    }
    
    ```
    
    Selects the second child of each `<ul>`, which could be any type of element, not just `<li>`.
    

**Formulae:**

- `n`: Selects every nth element.
- `2n`: Selects every second element (2, 4, 6, ...).
- `2n+1`: Selects every odd element (1, 3, 5, ...).
- `3n+2`: Selects every third element starting from the second (2, 5, 8, ...).

### **3. Star Selector**

**Overview:**
The star selector (`*`) selects all elements within the page.

```css
* {
    box-sizing: border-box;
}

```

This can be useful for applying a reset or applying a style globally across all elements.

### **4. Group Selectors**

**Overview:**
Group selectors allow you to apply the same styles to multiple elements by separating them with commas.

```css
h1, h2, h3, p {
    font-family: Arial, sans-serif;
}

```

This applies the same font-family to `<h1>`, `<h2>`, `<h3>`, and `<p>` elements.

### **Practice and Application**

Understanding and using these advanced selectors effectively can help you create more dynamic and flexible stylesheets. Practice using these selectors to target and style specific elements in your HTML documents based on their attributes, position, or grouping.

# Understanding CSS Specificity

CSS specificity determines which CSS rule is applied by calculating a "score" based on the selectors in your stylesheets. When multiple rules could apply to an element, specificity helps the browser choose the most appropriate rule. Here’s a detailed breakdown:

### **Specificity Hierarchy**

1. **Inline Styles**
    - **Syntax:** `style="property: value;"` directly in the HTML tag.
    - **Specificity Score:** 1000
    - **Example:** `<p style="color: red;">Text</p>`
    - **Explanation:** Inline styles have the highest specificity and will override any other styles.
2. **IDs**
    - **Syntax:** `#id`
    - **Specificity Score:** 100
    - **Example:** `#header { color: blue; }`
    - **Explanation:** ID selectors have higher specificity compared to classes and element selectors.
3. **Classes, Attributes, and Pseudo-classes**
    - **Syntax:** `.class`, `[attribute]`, `:hover`, `:nth-child()`
    - **Specificity Score:** 10
    - **Example:** `.button { color: green; }`, `input[type="text"] { color: orange; }`, `a:hover { color: pink; }`
    - **Explanation:** These selectors target elements based on their classes, attributes, or states.
4. **Elements and Pseudo-elements**
    - **Syntax:** `element`, `::before`, `::after`
    - **Specificity Score:** 1
    - **Example:** `p { color: black; }`, `::first-line { font-weight: bold; }`
    - **Explanation:** These selectors have the lowest specificity and are usually overridden by more specific selectors.

### **Calculating Specificity Scores**

The specificity is calculated based on the following format: `a b c d`, where:

- **a**: Number of inline styles (1000)
- **b**: Number of ID selectors (100)
- **c**: Number of class selectors, attributes, and pseudo-classes (10)
- **d**: Number of element selectors and pseudo-elements (1)

**Examples:**

1. **`#hello {}`**
    - **Specificity:** 0100 (1 ID, 0 classes/attributes/pseudo-classes, 0 elements/pseudo-elements)
2. **`div {}`**
    - **Specificity:** 0001 (0 IDs, 0 classes/attributes/pseudo-classes, 1 element)
3. **`div p.foo {}`**
    - **Specificity:** 0012 (0 IDs, 1 class, 1 element for `div`, 1 element for `p`)

**Example Calculation:**

1. **`p {}`**
    - **Specificity:** 0001 (1 element)
2. **`div p {}`**
    - **Specificity:** 0002 (2 elements: `div` and `p`)
3. **`div p.foo {}`**
    - **Specificity:** 0012 (1 class, 2 elements)

In the above examples, `div p.foo {}` has the highest specificity and will be applied over `p {}` and `div p {}`.

**Additional Guidelines:**

- **Selectors with equal specificity:** The rule that appears last in the CSS file takes precedence.
- **Universal selectors (``)** have zero specificity.
- **Specificity Calculators:** Tools are available to help you calculate and visualize specificity scores.

### Conclusion

CSS specificity is crucial for resolving conflicts in styling and ensuring that the correct rules are applied to elements. Understanding the hierarchy and calculation of specificity helps in writing more efficient and predictable CSS.

# Combination Selectors in CSS

Combination selectors in CSS allow you to target elements based on their relationships to other elements, giving you more control over your styling. Here’s a breakdown of the four main types:

### **1. Descendant Selectors**

- **Definition:** Selects elements that are descendants (i.e., children, grandchildren, etc.) of a specified element.
- **Syntax:** `ancestor descendant`
- **Example:**
    
    ```html
    <div id="blog">
      <h1>Title</h1>
      <p>Paragraph</p>
    </div>
    
    ```
    
    ```css
    #blog h1 {
      color: blue;
    }
    
    ```
    
    **Explanation:** All `h1` elements within the `div` with ID `blog` will be styled blue. This includes all levels of descendants.
    

### **2. Child Selectors**

- **Definition:** Selects elements that are direct children of a specified element.
- **Syntax:** `parent > child`
- **Example:**
    
    ```html
    <div id="blog">
      <h1>Title</h1>
      <div>
        <h1>Another Title</h1>
      </div>
    </div>
    
    ```
    
    ```css
    #blog > h1 {
      color: blue;
    }
    
    ```
    
    **Explanation:** Only the `h1` elements that are direct children of the `div` with ID `blog` will be styled blue. In this case, only the first `h1` will be styled blue.
    

### **3. General Sibling Selectors**

- **Definition:** Selects all elements that are siblings of a specified element, following it.
- **Syntax:** `reference ~ sibling`
- **Example:**
    
    ```html
    <h1>Title</h1>
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
    
    ```
    
    ```css
    h1 ~ p {
      color: blue;
    }
    
    ```
    
    **Explanation:** All `p` elements that follow an `h1` element are styled blue. The first `p` will not be styled if it does not come after the `h1`.
    

### **4. Adjacent Sibling Selectors**

- **Definition:** Selects the immediate next sibling of a specified element.
- **Syntax:** `reference + adjacent`
- **Example:**
    
    ```html
    <img src="image1.jpg" />
    <p>Caption 1</p>
    <p>Paragraph</p>
    <img src="image2.jpg" />
    <p>Caption 2</p>
    
    ```
    
    ```css
    img + p {
      font-style: italic;
    }
    
    ```
    
    **Explanation:** Only the `p` elements immediately following an `img` element are styled italic. The second `p` does not get affected if it's not immediately after an `img`.
    

### Practical Examples

### **General Sibling Selector Example:**

```html
<p>Basic Info About Little Lemon</p>
<div>About</div>
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

```

```css
div ~ ul {
  background-color: orange;
  box-shadow: 1px 1px 3px gray;
}

```

**Explanation:** All `ul` elements following a `div` will have an orange background and box shadow.

### **Adjacent Sibling Selector Example:**

```html
<img src="photo.jpg" />
<p>Description 1</p>
<img src="photo2.jpg" />
<p>Description 2</p>

```

```css
img + p {
  font-size: 0.9em;
  text-align: center;
}

```

**Explanation:** Only the `p` elements immediately after an `img` are styled as captions with smaller font size and centered text.

### Conclusion

Combination selectors allow you to be more specific in targeting elements based on their relationships in the HTML structure. This helps in applying styles more efficiently and avoiding conflicts. Understanding and using these selectors effectively will enhance your ability to design well-structured and styled web pages.

# Understanding Pseudo-Class Selectors in CSS

Pseudo-class selectors in CSS are powerful tools for styling elements based on their state or position. They enhance interactivity and allow for more nuanced styling without complex JavaScript. Here’s a detailed look at different types of pseudo-classes and their practical applications:

### **1. User Action States**

These pseudo-classes respond to user interactions with elements.

- **`:hover`**
    - **Definition:** Applies styles when the user hovers over an element.
    - **Syntax:** `selector:hover { property: value; }`
    - **Example:**
        
        ```html
        <a href="#">Hover over me</a>
        
        ```
        
        ```css
        a:hover {
          color: red;
        }
        
        ```
        
    
    **Explanation:** The link color changes to red when the cursor is over it.
    
- **`:active`**
    - **Definition:** Applies styles while the user is pressing and holding the mouse button on an element.
    - **Syntax:** `selector:active { property: value; }`
    - **Example:**
        
        ```html
        <button>Click me</button>
        
        ```
        
        ```css
        button:active {
          background-color: blue;
        }
        
        ```
        
    
    **Explanation:** The button background turns blue while it’s being clicked.
    
- **`:focus`**
    - **Definition:** Applies styles to an element when it gains focus, usually from user interaction like tabbing through form fields.
    - **Syntax:** `selector:focus { property: value; }`
    - **Example:**
        
        ```html
        <input type="text" placeholder="Type here">
        
        ```
        
        ```css
        input:focus {
          border-color: green;
        }
        
        ```
        
    
    **Explanation:** The input field border turns green when focused.
    

### **2. Form States**

Pseudo-classes used to style form elements based on their state.

- **`:disabled`**
    - **Definition:** Applies styles to disabled elements.
    - **Syntax:** `selector:disabled { property: value; }`
    - **Example:**
        
        ```html
        <button disabled>Disabled Button</button>
        
        ```
        
        ```css
        button:disabled {
          background-color: gray;
        }
        
        ```
        
    
    **Explanation:** Disabled buttons have a gray background.
    
- **`:enabled`**
    - **Definition:** Applies styles to enabled elements.
    - **Syntax:** `selector:enabled { property: value; }`
    - **Example:**
        
        ```html
        <button>Enabled Button</button>
        
        ```
        
        ```css
        button:enabled {
          background-color: blue;
        }
        
        ```
        
    
    **Explanation:** Enabled buttons have a blue background.
    
- **`:checked`**
    - **Definition:** Applies styles to checked checkboxes or radio buttons.
    - **Syntax:** `selector:checked { property: value; }`
    - **Example:**
        
        ```html
        <input type="checkbox" checked>
        
        ```
        
        ```css
        input:checked {
          background-color: yellow;
        }
        
        ```
        
    
    **Explanation:** Checked checkboxes have a yellow background.
    
- **`:valid` and `:invalid`**
    - **Definition:** Applies styles based on the validity of form inputs.
    - **Syntax:**
        
        ```css
        input:valid { property: value; }
        input:invalid { property: value; }
        
        ```
        
    - **Example:**
        
        ```html
        <input type="email" required>
        
        ```
        
        ```css
        input:valid {
          border-color: green;
        }
        input:invalid {
          border-color: red;
        }
        
        ```
        
    
    **Explanation:** Valid email inputs have a green border, and invalid ones have a red border.
    

### **3. Position-Based States**

These pseudo-classes target elements based on their position within a group.

- **`:first-of-type`**
    - **Definition:** Applies styles to the first element of its type within a parent.
    - **Syntax:** `selector:first-of-type { property: value; }`
    - **Example:**
        
        ```html
        <ul>
          <li>Item 1</li>
          <li>Item 2</li>
        </ul>
        
        ```
        
        ```css
        li:first-of-type {
          font-weight: bold;
        }
        
        ```
        
    
    **Explanation:** The first `li` in each `ul` will be bold.
    
- **`:last-of-type`**
    - **Definition:** Applies styles to the last element of its type within a parent.
    - **Syntax:** `selector:last-of-type { property: value; }`
    - **Example:**
        
        ```html
        <ul>
          <li>Item 1</li>
          <li>Item 2</li>
        </ul>
        
        ```
        
        ```css
        li:last-of-type {
          font-style: italic;
        }
        
        ```
        
    
    **Explanation:** The last `li` in each `ul` will be italicized.
    
- **`:nth-of-type(n)`**
    - **Definition:** Applies styles to elements based on their position within a group, where `n` can be a number, keyword, or formula.
    - **Syntax:** `selector:nth-of-type(n) { property: value; }`
    - **Example:**
        
        ```html
        <ul>
          <li>Item 1</li>
          <li>Item 2</li>
          <li>Item 3</li>
        </ul>
        
        ```
        
        ```css
        li:nth-of-type(2) {
          color: red;
        }
        
        ```
        
    
    **Explanation:** The second `li` in each `ul` will be red.
    
- **`:nth-last-of-type(n)`**
    - **Definition:** Similar to `:nth-of-type`, but counts from the end.
    - **Syntax:** `selector:nth-last-of-type(n) { property: value; }`
    
    **Example:**
    
    ```html
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
    
    ```
    
    ```css
    li:nth-last-of-type(2) {
      color: green;
    }
    
    ```
    
    **Explanation:** The second `li` from the end will be green.
    

### Conclusion

Pseudo-class selectors are essential for creating interactive and well-styled web pages. They allow you to apply styles based on user interactions, form states, and element positions, making your CSS more dynamic and efficient. Experiment with these selectors to enhance the user experience on your web pages.

# CSS Text Effects Cheat Sheet

### **Basic Text Properties**

| **Property** | **Values** | **Description** |
| --- | --- | --- |
| **Text-transform** | none, uppercase, lowercase, capitalize, full-width | Modifies the case of the text (e.g., all caps, all lowercase) |
| **Font-style** | normal, italic, oblique | Controls the style of the text (e.g., italics) |
| **Font-weight** | normal, weight, lighter, bolder, 100-900 | Defines the thickness of the text (e.g., bold) |
| **Text-decoration** | none, underline, overline, line-through | Adds decorations to text (e.g., underline) |

### **Additional Text Effects**

| **Property** | **Values** | **Description** |
| --- | --- | --- |
| **Text-align** | left, right, center, justify | Horizontal alignment of text |
| **Text-align-last** | auto, left, right, center, justify | Alignment of the last line when text is justified |
| **Text-combine-upright** | none, all, single | Combines multiple characters into a single upright character (useful in languages like Mandarin) |
| **Text-decoration-color** | color values | Sets the color of the text decoration |
| **Text-decoration-line** | none, underline, overline, line-through | Specifies the type of line decoration |
| **Text-decoration-style** | solid, double, dotted, dashed, wavy | Defines the style of the text decoration line |
| **Text-decoration-thickness** | auto, from-font, or length (e.g., 2px) | Specifies the thickness of the decoration line |
| **Text-emphasis** | none, filled, hollow, or color/style | Shorthand for text emphasis properties (e.g., color, style) |
| **Text-indent** | length (e.g., 2em), percentage | Indentation of the first line of text |
| **Text-justify** | auto, inter-word, inter-ideograph, distribute | Specifies justification method when text-align is "justify" |
| **Text-orientation** | mixed, upright, sideways | Orientation of text in a line (e.g., vertical, horizontal) |
| **Text-shadow** | offset-x offset-y blur-radius color | Adds shadow to text (e.g., 2px 2px 4px gray) |
| **Text-underline-position** | auto, under, left, right, center | Position of underline (used with text-decoration) |

### **Text Overflow and Wrapping**

| **Property** | **Values** | **Description** |
| --- | --- | --- |
| **Text-overflow** | clip, ellipsis | Determines how text overflow is handled (e.g., show ellipsis) |
| **Word-wrap** | normal, anywhere, break-word | Defines how words should wrap within their container (alias for overflow-wrap) |
| **Word-break** | normal, break-all, keep-all, break-word | Defines how long words are broken (e.g., allow breaks in words) |
| **Writing-mode** | horizontal-tb, vertical-lr, vertical-rl | Sets the direction of text (e.g., horizontal or vertical) |

This cheat sheet covers the core properties and their values that you can use to create a variety of text effects on your web pages. You can combine these properties with other CSS rules to achieve the desired visual style and behavior for your text elements.

# Here's a concise cheat sheet for CSS keyframes:

### **@keyframes Rule**

**Purpose:** Defines the animation sequence by specifying how properties should change over time.

**Syntax:**

```css
@keyframes animation-name {
  from { /* Initial state */ }
  to { /* Final state */ }
}

```

**OR**

```css
@keyframes animation-name {
  0% { /* Initial state */ }
  50% { /* Intermediate state */ }
  100% { /* Final state */ }
}

```

**Example:**

```css
@keyframes example {
  0% { background-color: red; }
  100% { background-color: blue; }
}

```

### **Animation Property**

**Purpose:** Applies the animation defined in the `@keyframes` rule to an element.

**Syntax:**

```css
element {
  animation: animation-name duration timing-function delay iteration-count direction fill-mode play-state;
}

```

**Shorthand Properties:**

- `animation-name` (Required): Name of the `@keyframes` animation.
- `animation-duration` (Required): Duration of the animation.
- `animation-timing-function`: Timing function (e.g., `ease`, `linear`).
- `animation-delay`: Delay before the animation starts.
- `animation-iteration-count`: Number of times the animation should repeat (`infinite` for endless).
- `animation-direction`: Direction of the animation (`normal`, `reverse`, `alternate`).
- `animation-fill-mode`: Determines how styles are applied before and after the animation (`none`, `forwards`, `backwards`, `both`).
- `animation-play-state`: Controls whether the animation is running or paused (`running`, `paused`).

**Example:**

```css
.box {
  animation: example 3s ease-in-out 1s infinite alternate;
}

```

### **Detailed Example:**

**HTML:**

```html
<body>
  <div class="box"></div>
</body>

```

**CSS:**

```css
@keyframes myanimation {
  0% { width: 50px; }
  50% { background-color: aquamarine; height: 20px; }
  100% { width: 100px; }
}

.box {
  width: 50px;
  height: 50px;
  background-color: lightcoral;
  animation: myanimation 3s infinite;
}

```

**Explanation:**

- `@keyframes myanimation` defines an animation that changes the width of an element from 50px to 100px, with an intermediate step changing the background color and height.
- `.box` applies the animation, which runs for 3 seconds and repeats infinitely.

This cheat sheet should help you understand and apply CSS animations using `@keyframes` and the `animation` property effectively.

# Here's a comprehensive cheat sheet for CSS animations and effects:

### **Transform Property**

**Syntax:**

```css
transform: transform-function values;

```

**Examples:**

- **None:** Resets any transformation.
    
    ```css
    .sample-class {
        transform: none;
    }
    
    ```
    
- **Matrix:** Defines a 2D transformation matrix.
    
    ```css
    .sample-class {
        transform: matrix(1.0, 2.0, 3.0, 4.0, 5.0, 6.0);
    }
    
    ```
    
- **Rotate:** Rotates an element.
    
    ```css
    .sample-class {
        transform: rotate(60deg);
    }
    
    ```
    
- **Rotate3d:** Rotates an element in 3D space.
    
    ```css
    .sample-class {
        transform: rotate3d(3, 2, 1, 100deg);
    }
    
    ```
    
- **Translate:** Moves an element from its current position.
    
    ```css
    .sample-class {
        transform: translate(10px, 20px);
    }
    
    ```
    
- **Translate3d:** Moves an element in 3D space.
    
    ```css
    .sample-class {
        transform: translate3d(10px, 20px, 30px);
    }
    
    ```
    
- **Scale:** Resizes an element.
    
    ```css
    .sample-class {
        transform: scale(1.5);
    }
    
    ```
    
- **Scale3d:** Resizes an element in 3D space.
    
    ```css
    .sample-class {
        transform: scale3d(2, 1, 0.5);
    }
    
    ```
    
- **Skew:** Skews an element.
    
    ```css
    .sample-class {
        transform: skew(20deg, 10deg);
    }
    
    ```
    

**Global Values:**

```css
.sample-class {
    transform: inherit;
    transform: initial;
    transform: revert;
    transform: revert-layer;
    transform: unset;
}

```

**Multiple Transforms:**

```css
.sample-class {
    transform: rotate(45deg) scale(1.5) translate(45px);
}

```

**Transform Origin:**

```css
.sample-class {
    transform-origin: 10px 10px;
    transform-origin: right bottom;
}

```

---

### **Transition Property**

**Syntax:**

```css
transition: property duration timing-function delay;

```

**Example:**

```css
.sample-class {
    transition: margin-left 2s ease-in-out 0.5s;
}

```

**Sub-properties:**

- **transition-property**
- **transition-duration**
- **transition-timing-function**
- **transition-delay**

---

### **Animations and @keyframes**

**Animation Property:**

**Syntax:**

```css
animation: name duration timing-function delay iteration-count direction fill-mode play-state;

```

**Example:**

```css
.sample-class {
    animation: animation-name 2s ease 0.5s 4 normal none running;
}

```

**Sub-properties:**

- `animation-name`
- `animation-duration`
- `animation-timing-function`
- `animation-delay`
- `animation-iteration-count`
- `animation-direction`
- `animation-fill-mode`
- `animation-play-state`

**@keyframes Rule:**

**Syntax:**

```css
@keyframes animation-name {
    from { property: value; }
    to { property: value; }
}

```

**Example:**

```css
@keyframes animation-name {
    from { bottom: 0px; }
    to { bottom: 100px; }
}

```

**Alternative Syntax:**

```css
@keyframes animation-name {
    0%, 100% { background-color: blue; }
    50% { background-color: green; }
}

```

**Multiple Animations:**

```css
#some-class {
    animation: animation-a 2s linear infinite alternate,
               animation-b 3s ease infinite alternate;
}

```

This cheat sheet should help you quickly reference key properties and examples for CSS animations and transformations.

# **CSS Preprocessors: Overview and Examples**

CSS preprocessors like SASS, SCSS, and Stylus extend CSS capabilities, providing advanced features like variables, nesting, mixins, and functions to streamline and enhance CSS development. Here’s a detailed look at these preprocessors:

---

### **1. SASS (Syntactically Awesome Style Sheets)**

SASS is a popular preprocessor that offers two syntaxes:

### **SCSS (Sassy CSS)**

- **Syntax:** SCSS is a more CSS-like syntax where you use curly braces and semicolons.
- **Example:**
    
    ```scss
    $font-stack: Arial;
    $primary-color: lightblue;
    
    body {
      font: 100% $font-stack;
      color: $primary-color;
    }
    
    ```
    

### **Indented Syntax (SASS)**

- **Syntax:** Uses indentation instead of curly braces and semicolons.
- **Example:**
    
    ```sass
    $font-stack: Arial
    $primary-color: lightblue
    
    body
      font: 100% $font-stack
      color: $primary-color
    
    ```
    

**Key Features:**

- **Variables:** Define reusable values.
- **Nesting:** Nest selectors to mirror HTML structure.
- **Mixins:** Reusable blocks of code.
    
    ```scss
    @mixin some-rules {
      color: lightblue;
      font-size: 25px;
      font-weight: bold;
    }
    
    div {
      @include some-rules;
    }
    
    ```
    
- **Directives:**
    - `@import`: Import styles from other files.
    - `@extend`: Inherit styles from another selector.

---

### **2. Stylus**

Stylus offers a flexible syntax where you can omit colons, braces, and semicolons if desired.

**Example:**

```
body
  font 100% Arial
  color lightblue

```

**Key Features:**

- **Flexible Syntax:** Allows omitting or including syntax characters.
- **Functions:** Define reusable functions.
    
    ```
    add(a, b)
      a + b
    
    div
      margin add(10px, 20px)
    
    ```
    

**Functions:** Useful for calculations and dynamic values.

---

### **3. LESS (Leaner Style Sheets)**

LESS is another popular preprocessor similar to SASS but with its own syntax and features.

**Key Features:**

- **Variables:** Store values for reuse.
    
    ```less
    @font-stack: Arial;
    @primary-color: lightblue;
    
    body {
      font: 100% @font-stack;
      color: @primary-color;
    }
    
    ```
    
- **Mixins:** Reusable styles.
    
    ```less
    .some-rules {
      color: lightblue;
      font-size: 25px;
      font-weight: bold;
    }
    
    div {
      .some-rules;
    }
    
    ```
    
- **Nesting:** Similar to SCSS for nesting selectors.

---

### **4. PostCSS**

PostCSS is a tool that can be used as a preprocessor with plugins for various CSS enhancements, including variables, nesting, and more.

**Key Features:**

- **Modular:** Use plugins to extend functionality.
- **Autoprefixer:** Automatically adds vendor prefixes.
- **Custom Properties:** Allows using CSS variables.

---

### **Conclusion**

CSS preprocessors significantly enhance the development workflow by providing advanced features not available in standard CSS. They help in writing cleaner, more maintainable, and reusable code. Depending on your project requirements and personal preferences, you can choose between SASS/SCSS, Stylus, LESS, or PostCSS to leverage these powerful tools.

# Notes on Creating Themes

### **Color Schemes Overview**

- **Color Scheme Definition**: The combination of colors used in the design of a website. It sets the tone and enhances the visual appeal of the site.
- **Importance**: Colors are crucial in setting the tone and mood of a website.

### **Color Theory Basics**

- **Primary Colors**: Red, Yellow, Blue
- **Secondary Colors**: Orange, Purple, Green (formed by combining two primary colors)
- **Tertiary Colors**: Six colors formed from mixing primary and secondary colors
- **Color Wheel**: A circular diagram of colors that serves as the foundation for color schemes.

### **Common Color Schemes**

1. **Monochromatic**
    - Uses variations of a single color.
    - Creates a harmonious and cohesive look.
2. **Analogous**
    - Uses colors that are next to each other on the color wheel.
    - Creates a serene and comfortable design.
3. **Complementary**
    - Uses colors that are opposite each other on the color wheel.
    - Creates high contrast and vibrant designs.
4. **Split Complementary**
    - Uses one base color and the two colors adjacent to its complementary color.
    - Provides high contrast with less tension than complementary schemes.
5. **Triadic**
    - Uses three colors that are evenly spaced around the color wheel.
    - Creates a balanced and vibrant color scheme.
6. **Square**
    - Uses four colors evenly spaced around the color wheel.
    - Offers a rich and diverse color palette.
7. **Rectangle (Tetradic)**
    - Uses four colors arranged in two complementary pairs.
    - Provides a balanced and varied color scheme.

### **Choosing and Using Color Schemes**

- **Purpose**: Enhances website appeal and user experience.
- **Considerations**:
    - **Type of Website**: Some schemes are more suitable depending on the website's purpose (e.g., complementary colors for charts and bars).
    - **Number of Colors**: Based on the design requirements and complexity.
    - **Target Audience**: Consider user demographics and preferences.
    - **Topic and Domain**: E.g., medical websites often use white backgrounds.
    - **Achromatic Themes**: Black and white schemes can also be effective with strong design.

### **Factors for Effective Themes and Colors**

- **User Experience**: Balance information and design to avoid cognitive overload.
    - **Cognitive Overload**: Too much information or activity can overwhelm users.
- **Psychological Impact**: Nature-inspired colors are generally more pleasant.
- **Visual Hierarchy**: Use color themes to guide users and create a clear navigation path.
- **Experimentation**: Keep multiple color combinations on hand for experimentation and inspiration.

### **Final Tips**

- **Trial and Error**: Choosing the right colors involves experimentation.
- **Inspiration**: Draw inspiration from well-designed websites.
- **Color Theory**: A critical component of user experience and web design. Don’t hesitate to try different schemes to find what works best.

By considering these aspects, you can create a visually appealing and user-friendly website that effectively communicates its message and enhances the overall user experience.

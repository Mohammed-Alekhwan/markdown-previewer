# Markdown Previewer

This project is a Markdown previewer built using React. Markdown is a lightweight markup language with plain-text formatting syntax, often used to format readme files, comments, and messages. The Markdown previewer allows users to input Markdown syntax into a text area, and it dynamically generates a preview of the formatted content in real-time.

## Components and Functionality

### 1. Markdown Input
- Users can input Markdown syntax into a textarea.
- The textarea is part of the `editor` div.

### 2. Markdown Preview
- As the user types Markdown syntax into the textarea, the preview section (`preview` div) displays the formatted HTML version of the Markdown content.
- The preview is updated in real-time using React's state management.

### 3. Markdown Conversion
- When the user inputs Markdown syntax, it is converted to HTML using the `marked` library. This library parses Markdown and converts it into HTML.
- The HTML output is sanitized using `DOMPurify` to prevent XSS (Cross-Site Scripting) attacks by removing any potentially harmful content.

### 4. State Management
- The component utilizes React's state hooks (`useState`) to manage the Markdown input (`markdown`) and the HTML output (`html`).

### 5. Effect Hook
- The `useEffect` hook is used to update the HTML output (`html`) whenever the Markdown input (`markdown`) changes. This ensures that the preview is always synchronized with the input.

### 6. Styling
- The project includes CSS for styling the editor and preview sections.
- Media queries are used to adjust the width of the editor and preview sections for different screen sizes.

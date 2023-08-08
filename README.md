# Notes-App
This is a simple web application that allows users to add, delete and edit notes. 
1. **HTML Structure**:
   - The project starts with an HTML structure that includes a button to add new notes and placeholders for displaying the individual notes.
   - External resources like Font Awesome for icons and a JavaScript library called "marked" for rendering Markdown are linked.
2. **CSS Styling**:
   - CSS styles are applied to achieve a clean and visually appealing design for the app. This includes font imports(google poppins), setting box-sizing and outline styles for all elements, and specific styling for buttons, notes, and textarea
3. **JavaScript Logic**:
   - The JavaScript code adds interactivity to the app and makes it functional.
   - It begins by fetching any existing notes from local storage and rendering them on the page when the page loads.
4. **Event Listeners**:
   - An event listener is added to the "Add note" button. When clicked, this button triggers the `addNewNote` function.
  
     
5. **addNewNote Function**:
   - This function is responsible for creating a new note element with appropriate structure for editing and viewing.
   - It includes buttons for editing and deleting, a main content area for displaying rendered Markdown content, and a textarea for editing the note's content.
   - Event listeners are attached to the edit and delete buttons to toggle visibility and handle the note's removal.
6. **Toggle Edit Mode**:
   - The edit button's event listener toggles between displaying the main content and the editing textarea when clicked. This allows users to easily switch between 
     viewing and editing modes.
7. **Live Preview**:
   - The `textArea` event listener captures input events (typing) in the textarea.
   - As the user types, the content is rendered using the "marked" library and displayed in the main content area. This provides a live preview of how the note will appear as Markdown is being typed
8. **Updating Local Storage**:
   - Whenever content is edited or notes are deleted, the `updateLS` function is called.
   - This function collects the content from all textareas and stores it in local storage as JSON data.
   - This ensures that the notes' content persists even after the user closes the browser or refreshes the page.
    



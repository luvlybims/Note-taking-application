```javascript
/** 
 * Class to implement a note taking application
 * @constructor {string} author note author
 * @constructor {Array.<string>} notes list of notes to be processed
 */
class NotesApplication
{ 
    constructor(author) 
    {
        this.author = author; 
        this.notes = []; 
    }

/**
 * Takes the note content as parameter and returns an array including the
 * note content
 * @param {string} adds note content to notes array
 * @return {Array.<string>} returns notes array including note content
create(note_content) 
    {
        this.notes.push(note_content); 
    }
    listNotes(); /**lists out each of the notes*/
    get(note_id); /**takes a note_id which refers to the index of the note in the notes list and returns the content of that note as a string*/
    search(search_text); /**take a search string, search_text and returns all the notes with that text within it*/
    delete(note_id); /**deletes the note at the index note_id of the notes list*/
    edit(note_id, new_content); /**replaces the content in the note at note_id with new_content.*/
}
```
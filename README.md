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
 * @param {string} note_content adds note content to notes array
 * @return {Array.<string>} returns notes array including note content
 * /
create(note_content) 
    {
        this.notes.push(note_content);
        return notes[]; 
    }

/**
 * lists out each of the notes in the notes list in the specified format. 
 * @return {string} returns the respective index of each of the item in the *array, the note content and the author 
 */
listNotes()
    {
        (for note_id === 0; note_id <== notes.length - 1; note_id++)
        {
           return "Note ID: [" +note_id+ "]" +"\n[" +this.notenote[note_id]+ "]\n\nBy Author [" +this.author+ "]";           
        }        
    }
     
    get(note_id); 
    search(search_text); 
    delete(note_id); 
    edit(note_id, new_content); 
}
```
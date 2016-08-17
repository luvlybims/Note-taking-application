```javascript
/** 
 * Class to implement a note taking application
 * @constructor {string} author note author
 * @constructor {Array.<string>} notes list of notes to be processed
 * @param {string} author parameter passed into constructor
 */
class NotesApplication
{ 
    constructor(author) 
    {
        if(typeof author === 'string')
        {
            this.author = author; 
            this.notes = []; 
        }
        else
        {
            throw new Error('error');   
        }
    }

/**
 * Takes the note content as parameter and returns an array including the
 * note content
 * @param {string} note_content adds note content to notes array
 */
create(note_content) 
    {
        if (typeof  note_content === 'string')
        {
        this.notes.push(note_content);
           
        }
        else
        {
           throw new Error('error');
        }
    }

/**
 * lists out each of the notes in the notes list in the specified format. 
 * @return {string} returns the respective index of each of the item in the *array, the note content and the author 
 */
listNotes()
    {
        for (let note_id = 0; note_id <= this.notes.length - 1; note_id++)
        {
           console.log(`Note ID: [${note_id}]\n${this.notes[note_id]}\n\nBy Author [${this.author}]`);           
        }        
    }
    
/**
 * takes the index of the note in the notes list and returns the content of that note as a string.
 * @param {number} note_id index of the note 
 * @return {string} returns the content of the note
 */ 
get(note_id)
    {   
        if (typeof  note_id === 'number')
        {
            for (let note_id = 0; note_id <= this.notes.length - 1; note_id++)
            {
                return this.notes[note_id];
            }
        }
        else
        {
           throw new Error('error');
        }
        
    } 
    search(search_text); 
    delete(note_id); 
    edit(note_id, new_content); 
}
```
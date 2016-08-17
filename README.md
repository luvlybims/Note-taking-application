```javascript
class NotesApplication
{ 
    constructor(author) /**Takes in parameter author as the author of the note*/

    {
        this.author = author; /**saves in an instance variable*/
        this.notes = []; /**saves in an instance property*/
    }
    create(note_content) /**takes the note content as the parameter and adds  it to the notes array*/
    {
        this.notes.push(note_content); /**adds the note content to the notes array*/
    }
    listNotes(); /**lists out each of the notes*/
    get(note_id); /**takes a note_id which refers to the index of the note in the notes list and returns the content of that note as a string*/
    search(search_text); /**take a search string, search_text and returns all the notes with that text within it*/
    delete(note_id); /**deletes the note at the index note_id of the notes list*/
    edit(note_id, new_content); /**replaces the content in the note at note_id with new_content.*/
}
```

## PROJECT TITLE:

 Note Taker

## PROBLEM DESCRIPTION:

### (in a Business Context)

For users that need to keep track of a lot of information, it's easy to forget or be unable to recall something important. Being able to take persistent notes allows users to have written information available when needed.

## SOLUTION:

Create an application to write, save, and delete notes. Application will use Express backend, save and retrieve notes from  JSON file.

## USER STORY:

AS A user, I want to be able to write and save notes
I WANT to be able to delete notes I've written before
SO THAT I can organize my thoughts and keep track of tasks I need to complete

## APPLICATION DESCRIPTION and OPERATION

Given an application frontend, a backend was built and and the two connected.

The following HTML routes are used:

  GET notes returns the notes.html file.                              

  GET  / returns the index.html file.                                        

  Notes are stored in a json file on the backend and the fs module is used to read and write to this file.

  GET /api/notes reads the db.json file and return all saved notes as JSON.                                                              

  POST /api/notes receives a new note to save on the request.body, add it to the `db.json` file, and then return the new note to the client when the save icon is clicked.

  DELETE /api/notes/:id receives a query parameter containing the id of a note to delete when the trash icon is clicked. The note is deleted from the list and from the db.json file.


## LICENSE

MIT License

Copyright (c) 2020 David Brown

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


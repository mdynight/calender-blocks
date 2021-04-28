# Calender Blocks (Temporary Title) [Prototype]

## What is it?
A user can add a note with a date and a block (card) will be displayed to represent it. As the blocks populate the interface they are arranged in chronological order. A user should be able to delete a block.
        
## Process

### Database Design
#### Table Design
| Primary Key | Field 2 |
| --- | --- |
| Date | Content |
#### DDL
    SQL goes here
### Query Design (DML)
| Query # | Query 1 | Query 2 | Query 3 |
| --- | --- | --- | --- |
| Job | Select all records (to be displayed) | Insert a record (Date & Cotent) | Delete a record (Date) |
| SQL | | | |
### Markup (HTML5)
    <!-- Display -->
    <ul>
        <li>
            <span class='date'>27/4</span>
            <span class='content'>Do the thing</span>
        </li>
    </ul>
    
    
    <!-- Form -->
    <div id='block-area'>    
        <form method="post" action="includes/insert.php">
            <input type="date" id='new-block-date'
            <input type="text" id='new-block-content' name='new-block-content'>
            <input type="submit" name="submit" value="Add Block">
        </form>
    </div>    
    
### Scripting (PHP)
* Script to run Query 1
* Script to loop li creation based on number of records retrieved in Query 1
* Script to send Query 2 with form content
* Script to send Query 3 with specific record key
### Styling (CSS6)
* Flex the li
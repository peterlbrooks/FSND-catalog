Catalog App


In general:

- The catalog is diplayed at the home page: localhost://8000
- From this page a user can login via facebook or google, or be a public user
- Logged in users can create, add, and delete items. Public users can not udpate
- All instructions are from the app home directory


To start:
- Per instructions it is assumed you have python and vagrant installed

1. Copy the entire folder and subfolder structure from github to your computer
2. From the app home directory:
    - Start up vagrant: vagrant up
    - Start the app: python application.py
        - Click on "allow" if any network requests appear
3. You are up and running!
4. Start the app by entering in your browswer: localhost://8000
5. The main page should appear


Database

A database withe categories is included. If you wish to recreate the database from scratch:

1. Erase the existing database: delete catalog.db
2. Create the DB: python models.py
3. Initialize the DB: python models-create-categories.py


Catalog Page

- Default view is catalog categories on left, and the 10 last updated items on the left
- Catalog categories are predefined in the DB, no editting allowed
- Click on a category to see the list of items for that category
- Click on the title word "Category" to see the list of the last 10 updated items
- Log in if you want item edit / delete capabilty. Google and Facebook logins are included


Items
- To add an item, click on the category in which you wish to add an item. The list of current items will appear as well as an "New Item" link next to the Item List title (top right)
- To view an item, click on the item name (rigth coloum of the main screen)
- Editting and deleting an item is done from buttons on the view item screen


JSON
- There are two JSON outputs
    - List of catalog categories from a link on the lower right of the main catalog screen
    - Item detail from a link on the lower right of a show item screen
    - From a JSON screen, to continue press your browser back button



# Collection Tracker
v1.1.2  
  
Are you an avid collector? You like to jam loot in a stash and just let it collect dust as the memory of it fades?  
  
Imagine this horrible scenario:  
You're out on the field. You have some important stuff on you. Almost encumbered.  
You fight a group of enemies and find some incredible looking equipment. Then you start to wonder.  
- Do I already have this at home?
- I should just take it in case I need it for my collection.
- Damn I'm too encumbered. Nevermind let's just walk home nice and slow.

Then you get home open up your trusty/dusty stash and realize that all the items you painstakingly carried for your collection are already present.  
Well no more!  

With this mod you can right click any weapon/armor and either log it into your collection or remove from it.  
When you're out on the field and unsure if you have an item you can just take out your PDA.  
**Guide -> Notes -> Equipment Inventory.**  
Here you see all of your collection items that you've taken an inventory for previously.

# Installation
Priority should be higher than the priority of `287- G.A.M.M.A. Massive Text Overhaul Project - SageDaHerb and Dr.Pr1nkos`

# Features
- Saving game saves your registered inventory entries.
- Selling an item (yes it's impossible to sell a weapon/BLACK MARKET) will automatically delete the entry for you.
- Dropping an item will mark the entry for deletion. If you don't pick it up and leave the map the entry will automatically be deleted for you.
- Putting stuff in a stash. If you taken inventory of it then it will be safe even on map changes etc.
- You can right click stuff even if it's in your stashes and it will get registered into the collection.
- Disassembling an item will automatically delete the entry for you after a map change.
- Duplicate item types: You can choose to overwrite the already existing inventory entry with the new item.
- Adding/Removing scope from weapon won't unregister your collection inventory entry.
- Hovering over an item will can tell you the following:
  - Is this exact item registered?
  - Is this type of item registered?
  - Item not registered?
 
![image](https://github.com/user-attachments/assets/5448e6b2-7b41-470d-965c-947916672c16)


This needs more space to explain all aspects:  
**Batch inventory registering**: If a stash is open a new option will appear on items `batch inventory`.  
When you press it the **Collection Tracker** will register every item in the stash automatically.  

If the **Collection Tracker** encounters multiple items of same type (same BRN-180 for example). It will register the one that's in the best condition overall.  
Now this condition calculation is the following: Sum of parts condition + Median of parts condition.  
This way if there're 2 similar condition items: 
- [1%, 1%, 1%, 1%, 100%]    - Sum is: 105  Median = 1  Final sum: 106
- [10%, 25%, 5%, 40%, 17%]  - sum is: 97   Median = 17 Final sum: 114  
The one with the better distribution of parts condition will be registered.

- **MCM options**:
  - **Slim entries**: The inventory entries won't contain the parts and conditions of the object.
  - **Display general item condition**: General item condition will be shown next to the item's name (except firearms)
  - **Delete all inventory entries for the currently loaded save**: Deletes all saved entry data (for current save only).
  - **Update data structure**: Performs an update on the data of the PDA inventory entries.

# Planned features
- An image for the PDA notes part.


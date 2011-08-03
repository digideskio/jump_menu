Install...
Normal procedure:
1) Place in modules/contrib/jump_menu
2) Enable at admin/build/modules or via drush.

Menus...
This modules runs from: any exsisting menu, from any parent item, to any depth.
Create the menu you want manually, via nodes, Taxonomy Menu, Auto Menu, etc.

Placing...
Here is the function definition to output the drop-down menu:
jump_menu($menuName, $menuItemID, $depth = 0, $choose = 'Select destination');

I'd recommend an example like this:
<?php
if(module_exists('jump_menu')) {
  echo jump_menu('primary-links', '8970');
}
?>
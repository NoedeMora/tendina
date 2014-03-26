Tendina
=======

A super easy-to-use jQuery plugin to build rapidly dropdown side menus.

![Tendina reveals!](/demo/tendina.gif "Tendina reveals")

[Demo CodePen](http://codepen.io/iprignano/full/tjoua)

Usage
===

To use Tendina, you just need to have some basic markup for your menu. That means you'll have some nested unordered lists, like this:

```html
<ul class="dropdown">
  <li>
    <a href="#">Menu 1</a>
    <ul>
      <li><a href="#">Submenu 1</a></li>
    </ul>
  </li>
  <li>
    <a href="#">Menu 2</a>
    <ul>
      <li><a href="#">Submenu 2</a></li>
      <li><a href="#">Submenu 2</a></li>
      <li><a href="#">Submenu 2</a>
        <ul>
          <li>Subsubmenu 2</li>
          <li>Subsubmenu 2</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>
    <a href="#">Menu 3</a>
    <ul>
      <li><a href="#">Submenu 3</a></li>
      <li><a href="#">Submenu 3</a></li>
    </ul>
  </li>
</ul>
```

Next step is to have jQuery and Tendina in your page:

```html
<script src="http://code.jquery.com/jquery-1.11.0.min.js"></script>
<script src="tendina.js"></script>
```

Finally, you can simply call the function on your list to transform it in a snappy side menu:

```javascript
$('.dropdown').tendina()
```

The plugin supports three-level deep nesting (`ul > li > ul > li > ul > li`). *Bring on the categories!*

Tendina will hide your nested submenus and manage all interactions with a nice slideUp/Down effect. You can even call Tendina on dinamically added elements (nice to have when building a menu from a JSON tree)!

Additionally, Tendina will add a "selected" class to the currently open menu, so you can customize its looks as you want!

License
===

Tendina is released under the MIT License.
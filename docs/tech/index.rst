*****
Index
*****

The index page, while not entirely important, might work differently then you may think it does. 

Mutat.io uses an iframe to load the central page, whether that would be for unit conversion, file conversion, or so on. 
This method allows the website to only load the converter itself when switching pages, while also cutting down on overall size. 

The page itself is also meant to be lightweight, loading only the FontAwesome and Google Fonts apis. 
It also loads the side navigation script and stylesheet. 
*This may change to be included in the HTML file itself whether than on separate files.*

Adding a new page
-----------------

Adding a page is simple - All you need to do is add an anchor tag in ``#sidenav``. Then you set the onclick property to the ``loadPage()`` function, like so:

.. code:: html

   <div id="sidenav" class="sidenav" style="display:none;">
     ...
	 <a onclick="loadPage('/page.html')">New page!</a>
	 ...
   </div>

You can also add an href property to add click functionality (cursor changes when hovering over it, different colors for hovering/clicking, etc.)

If you're adding a FontAwesome icon to the page title, make sure to make it full width by adding the ``fa-fw`` class to it.
# prueba-Backbone

More information: https://www.youtube.com/watch?v=pQE5OGGo6KE

Install first node.js to begin

Steps 

1.when de repo is cloned it contain a  file with:
app.js
datos.json
index.html
package.json

2. In the Terminal go to the file is located and run: npm install
This will create the folder node_modules with the dependencies that are in package.json

3.  Run the application: node app.js

4. Go to url http://localhost:4000/

5. create client-side files:
css
img
js->vendor
    backbone-> models, collections, views, routers
    init.js

6. Into the file vendor add the dependencies that backbone require download:

jquery(Help to manipulate the DOM) https://jquery.com/download/

undersore.js(provides a whole mess of useful functional programming helpers without extending any built-in objects):
http://underscorejs.org/

backbone(framework): http://backbonejs.org/backbone-min.js

7. Add there files to bottom body in the index.html
8. Download boostrap: move the files css to the project files css
9. move file fonts into file public
10. And finally move files js into vendor
11. Add there files to index.html
12.Add into the file models a file libro.js
13. call in index.html
14. add in file libro.js var Libro = Backbone.Model.extend();
15. in the console of html copy:
   > var primerLibro = new Libro ({titulo: 'la odisea', autor: 'ana', categoria: 'literatura'});
    and the method toJSON bring it:
   > primerLibro.toJSON();
16.there are two methods to bring dates:
   > primerLibro.get('titulo'); -> the method GET returns the value of an attribute
   > primerLibro.set('autor', 'desconocido'); -> method SET It changes the value of an attribute or adding new attributes to a model
  to see:  > primerLibro._previousAttributes.autor
The method initialize, es call when a new instad is created(see initialize in libro.js)
en console see: > var segundoLibro = new Libro();
The method defaults (see default in libro.js)
en console see: > var tercerLibro = new Libro({title: "lazarillo a muerto"});
                > tercerLibro.toJSON();

What is it?
-----------

This is a simple extension to manipulate the browser navigation.
Is not very convenient work with backbone routing url using strings. We also have routing!

This library extends the prototype of backbone routing with one method - `to()`

### Example

	```
	var Main = Backbone.Router.extend({

	    routes: {
        	"":"index",
        	"category/:id/:page": "category"
	    }

	   //...

	});

	var routing = new Main();
	Backbone.history.start({pushState: true});

	routing.to('index');		// navigate to url "/"
	routing.to('category', {
	    'id':1,
	    'page':1
	});				// navigate to url "/category/1/1"
	```


	```


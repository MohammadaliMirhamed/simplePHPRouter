# Simple PHP Router

Hey! This is a simple class that can handel the whole url routing for your project.

It utilizes RegExp and PHPs anonymous functions to create a lightweight and fast routing system.

Take a look in the index.php file. As you can see the ```Route::add()``` method is used to add new routes to your project.
The first argument takes the path segment. You can also use RegExp in there to parse out variables. 
All matches will be pushed to the handler method. The handler is the second argument of the add function.

Example:
```
Route::add('/user/(.*)/edit',function($id){
	//Do something
	echo 'Edit user with id '.$id.'<br/>';
});
```

## Testing
* Clone or download this repo
* Cd into the repo folder and run:
* ```php -S 0.0.0.0:8080```
* Than open your Webbrowser and navigate to http://localhost:8080

## Something does not work?
* Dont forget to set the basepath in your index.php and .htaccess file.
* Enable mod_rewrite in your apache settings

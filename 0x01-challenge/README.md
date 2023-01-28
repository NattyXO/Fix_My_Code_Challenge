
# Fix my code

Fix my code is a new type of project, where we’ll jump into an existing code base and fix it!

Sometime you will know the language, sometime not.

Please download the repository 0x01-Fix_My_Code_Challenge and use it as initial files for all solutions.

You should not recode everything, just fix it!


## Documentation
### [File: status_server/]
I provided a code that creates a Flask web server that runs on http://0.0.0.0:5000/ and has a route for the status of the API at http://0.0.0.0:5000/api/v1/status.

However, it seems that I am running the command python -m api.v1.app instead of running the app.py file directly, which is causing the "Not found" error to be returned. I should run the command python app.py instead, which will execute the script and start the server on the specified host and port.

Additionally, I have to check the blueprint routes, to make sure that the blueprint is registered with the app, and the path to the blueprint is correct. This will ensure that the blueprint is properly integrated with the app and my routes will work as expected.
### [File: square.py]
I provided a code that creates a class called square that calculates the area and perimeter of a square. However, there is an issue with my implementation.

In the area_of_my_square method, I am calculating the area of a square by multiplying the width by itself, but in the PerimeterOfMySquare method, I am calculating the perimeter by multiplying the width by 2 and the height by 2. This is incorrect because in a square the width and height are the same, so I should multiply the width by 4 to correctly calculate the perimeter.

Also, in the str method, I am returning the width and height, but in the square only width is the same as height, so I should return only width to be correct.

I will make these changes to my code and let you know if I need any further help.

### [File: user.py]
I am trying to create a class called 'User' that has an email property. I am using decorators (@property and @email.setter) to define getter and setter methods for the email property. However, I am using the same name 'email' for both the property and the setter method, which is causing a recursion and an infinite loop. To fix this, I need to use different names for the property and setter method.
### [File: blog]
Based on the code provided, it appears that I am not defining any routes for my blog posts in my Rails application. Without any routes defined, the application will not know how to handle requests for specific URLs, resulting in the "Not found" error that users are experiencing.

To fix this issue, I will need to define routes for my blog posts in the config/routes.rb file of my application. For example, I could define a route that maps the root URL of my application to a controller action that retrieves and displays a list of blog posts.

This would map the root URL of my application (e.g. "http://your-app.com") to the index action of the Posts controller. Then I will need to create this controller and action, along with a view template to render the list of posts.

For the second part of my question, I can add a new field called "online" to the Post model to store the online status of the post and then I can use a boolean data type for this field.
Then I can add a check in my index action that filters out the post which are not online and then I can use this field in my views to show or hide some blog posts from the listing.
I can also add a checkbox in my edit form to allow user to change the online status of the post. This will allow me to control which posts are visible on the website.

### [File: react-blog]

This is a server-side JavaScript file for an application that I am building using the Express framework, React, and various other modules such as react-router, iso, and express-session. I am setting up various middlewares for handling sessions, cookies, and parsing request bodies, as well as defining routes for handling requests to specific URLs. I am also using React to render the application and handle client-side routing. However, it appears that there is an issue with the website's pagination and the website is broken. I am also exporting a configuration object that sets up the port, base URL, and other settings for the application. I need to investigate and fix the issue with the pagination to ensure that the website is functioning properly.
## 🚀 About Me
I'm a full stack developer...


## Usage/Examples

```Ruby
Rails.application.routes.draw do
  root to: 'posts#index'
end

```
```python
#!/usr/bin/python3
"""
Web server 
"""
from flask import Flask, jsonify

app = Flask(__name__)

@app.route('/api/v1/status', methods=['GET'], strict_slashes=False)
def status():
    """ Status of the web server
    """
    return jsonify({"status": "OK"})

if __name__ == "__main__":
    # python app.py 
    app.run(host="0.0.0.0", port=5000)

```


## Authors

- [@NattyXO](https://github.com/NattyXO)


## Badges

[Linkedin](https://www.linkedin.com/in/natnael-bizuneh-zenebe/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)


## Support

For support, email nattyxo2018@gmail.com or join our Slack channel.


## Review for yesterday:

Q: If you have dependent-destroy on a through association, does it also destroy the row in the join table?
A: It probably does.

## Lecture

Q: What would 'new_plant_url' look like?
A: Look at your routes! If this is RESTful, it'd be something like 'localhost:3000/plants/new'

Q: Why can forms only make post and get requests?
A: Historical reasons

Q: What other input types are there?
A: Luke rattles off a few of the most popular...

Q: What's up with that helper url taking in an argument?
A: The existence of the url helper methods are due to the fact that we are using resources (RESTful routes). You may pass in the plant or the plant's id and Rails will interpret it.
***typo on button_to slide***

Q: What is the anatomy of an HTML tag?
A: <tagname flag attribute="">inner HTML</tagname> on whiteboard...A lot of these things get used as CSS selectors

Q: What's up with the shortcut for rendering a partial?
A: The name of the instance variable and the name of the corresponding partial must match in order to utilize that shortcut.

Q: Do you still have access to instance variables inside of a partial?
A: We prefer to use local variables, because instance variables will return nil (and not throw a helpful error)

Q: Why are we rendering instead of redirecting? What's the difference?
A: The difference is if we render, we're directly sending them back to the view. If we redirect, they must make another request. The main goal of redirect is to keep the url in sync
***hot fix on #destroy***

Q: Can you make a custom helper url?
A: Use alias :as

Q: Header sizes?
A: Just for lower-level vs. higher-level headers. You'll be able to control the size and appearance in CSS. Screen-readers interpret the significance of those headers.

Q: Where does it put linebreaks?
A: HTML ignores white space. We use break or paragraph tags to break lines.

Q: What anchor tag is being returned by link_to?
A: Right click, inspect, and see that it is an <a> tag.

Q: Date formatting?
A: Don't worry too much about it...

Q: What does a section tag do?
A: It's a container, which will allow you to group multiple pieces of HTML together, to apply styling rules

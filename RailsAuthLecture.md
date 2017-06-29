# Authentication

## Models

### User
  ::find_by_credentials(username, password)
    - will be used in Session#create
  #password=(password)
    - declare @password instance variable
    - don't forget to put an attr_reader on it
    - generate and save password_digest
  #is_password?(password)
    - be familiar with BCrypt
    - called from within ::find_by_credentials to validate user
  #ensure_session_token
    - callback validation
    - lazy assignment
  #reset_session_token!
    - remember to return the new session_token!

## Controllers

- N.B. Views can use information from the corresponding Controller action's instance variables

### User
  #new
    - renders sign up form
  #create
    ApplicationController#login(user)

### Session
  #new
    - renders sign-in form (very similar to sign up)
  #create
    ApplicationController#login(user)
  #destroy
    ApplicationController#logout

### Application
  #login(user)
    - set the session[:session_token] to equal the user's session_token
    - be sure to refresh the user's session_token for added security
  #logout
    - change the user's session_token
    - set the session[:session_token] to nil
  #logged_in?
    - helper_method
    - can be used inside of views
  #current_user
    - helper_method
    - can be used inside of views
    - make it an instance variable!

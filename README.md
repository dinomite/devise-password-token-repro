Reproduction of https://github.com/plataformatec/devise/issues/4397#issuecomment-274038522.

The development sqlite DB is in Git, just run Rails in development mode.

Here is a [reset password link](http://localhost:3000/users/password/edit?reset_password_token=---fq9wEMk3-nHYg9R98)

Try to reset the password for 'foo@example.com', note that the reset-password form has no fields,
and doesn't submit anything.  Despite this, Devise doesn't complain, though it also doesn't change
the password—you should still be able to login with 'foo@example.com' with the password 'foobar'.

This repo is based upon from https://github.com/RailsApps/rails-devise

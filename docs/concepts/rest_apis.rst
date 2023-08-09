edx-platform REST API Concepts
##############################

APIs in the edx-platform fall into one of two categories.  **Personal APIs**
that only let you manipluate resources related to your user (the single user
associated with the OAuth2 Application) or **Machine-to-machine APIs** that
allow you to manipulate other users and system resources so long as the user
associated with the OAuth2 application has the permissions to do so.

The best way to interact with the APIs is to get a JWT Token associated with a
user and then pass that to the server as a part of the request header.

You can get a JWT one of two ways, one is to exchange the username and password
for a user to get their JWT, and the other is to get a JWT associated with an
OAuth2 Application (the application is associated with your user)that allow you
to manipulate other users and system resources so long as the user associated
with the OAuth2 application has the permissions to do so.

The best way to interact with the APIs is to get a JWT Token associated with a
user and then pass that to the server as a part of the request header.

You can get a JWT one of two ways, one is to exchange the username and password
for a user to get their JWT, and the other is to get a JWT associated with an
OAuth2 Application (the application is associated with your user).

JWTs by default expire every hour so when they expire you'll have to get a new
one before you can call the API again.

.. seealso::

   * :doc:`/how-tos/use_the_api`
